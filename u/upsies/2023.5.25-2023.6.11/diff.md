# Comparing `tmp/upsies-2023.5.25.tar.gz` & `tmp/upsies-2023.6.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upsies-2023.5.25.tar", last modified: Thu May 25 13:47:13 2023, max compression
+gzip compressed data, was "upsies-2023.6.11.tar", last modified: Sun Jun 11 11:33:55 2023, max compression
```

## Comparing `upsies-2023.5.25.tar` & `upsies-2023.6.11.tar`

### file list

```diff
@@ -1,154 +1,259 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.493727 upsies-2023.5.25/
--rw-------   0 ich       (1000) ich       (1000)    35149 2021-06-11 16:56:53.000000 upsies-2023.5.25/LICENSE
--rw-------   0 ich       (1000) ich       (1000)     2367 2023-05-25 13:47:13.493727 upsies-2023.5.25/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     1815 2023-04-25 13:55:04.000000 upsies-2023.5.25/README.rst
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.473728 upsies-2023.5.25/bb/
--rw-------   0 ich       (1000) ich       (1000)      115 2023-04-25 13:54:40.000000 upsies-2023.5.25/bb/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3145 2023-04-25 13:54:40.000000 upsies-2023.5.25/bb/config.py
--rw-------   0 ich       (1000) ich       (1000)    51071 2023-04-25 13:54:40.000000 upsies-2023.5.25/bb/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     8450 2023-04-25 13:54:40.000000 upsies-2023.5.25/bb/tracker.py
--rw-------   0 ich       (1000) ich       (1000)       38 2023-05-25 13:47:13.493727 upsies-2023.5.25/setup.cfg
--rw-------   0 ich       (1000) ich       (1000)     1664 2023-05-25 13:46:48.000000 upsies-2023.5.25/setup.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.477728 upsies-2023.5.25/upsies/
--rw-------   0 ich       (1000) ich       (1000)     1181 2023-05-25 13:46:48.000000 upsies-2023.5.25/upsies/__init__.py
--rw-------   0 ich       (1000) ich       (1000)       73 2022-03-13 08:26:06.000000 upsies-2023.5.25/upsies/__main__.py
--rw-------   0 ich       (1000) ich       (1000)     1399 2023-03-19 11:08:21.000000 upsies-2023.5.25/upsies/constants.py
--rw-------   0 ich       (1000) ich       (1000)     2058 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/defaults.py
--rw-------   0 ich       (1000) ich       (1000)     6188 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/errors.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.477728 upsies-2023.5.25/upsies/jobs/
--rw-------   0 ich       (1000) ich       (1000)      215 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    27889 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/base.py
--rw-------   0 ich       (1000) ich       (1000)     2165 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/custom.py
--rw-------   0 ich       (1000) ich       (1000)    21011 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/dialog.py
--rw-------   0 ich       (1000) ich       (1000)     3707 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/imghost.py
--rw-------   0 ich       (1000) ich       (1000)     4807 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/mediainfo.py
--rw-------   0 ich       (1000) ich       (1000)     7596 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/poster.py
--rw-------   0 ich       (1000) ich       (1000)     8642 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/scene.py
--rw-------   0 ich       (1000) ich       (1000)    17965 2023-05-25 13:46:48.000000 upsies-2023.5.25/upsies/jobs/screenshots.py
--rw-------   0 ich       (1000) ich       (1000)     2770 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/set.py
--rw-------   0 ich       (1000) ich       (1000)     7977 2023-04-25 14:32:10.000000 upsies-2023.5.25/upsies/jobs/submit.py
--rw-------   0 ich       (1000) ich       (1000)    13209 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/jobs/torrent.py
--rw-------   0 ich       (1000) ich       (1000)    13899 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/webdb.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.477728 upsies-2023.5.25/upsies/trackers/
--rw-------   0 ich       (1000) ich       (1000)     1385 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.477728 upsies-2023.5.25/upsies/trackers/base/
--rw-------   0 ich       (1000) ich       (1000)      149 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/base/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3222 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/trackers/base/_howto.py
--rw-------   0 ich       (1000) ich       (1000)     3102 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/trackers/base/config.py
--rw-------   0 ich       (1000) ich       (1000)    33425 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/trackers/base/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     5985 2023-04-25 14:57:27.000000 upsies-2023.5.25/upsies/trackers/base/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.481727 upsies-2023.5.25/upsies/trackers/bhd/
--rw-------   0 ich       (1000) ich       (1000)      119 2023-04-28 07:24:11.000000 upsies-2023.5.25/upsies/trackers/bhd/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3643 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/bhd/config.py
--rw-------   0 ich       (1000) ich       (1000)    15623 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/bhd/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     6243 2023-04-25 14:57:27.000000 upsies-2023.5.25/upsies/trackers/bhd/tracker.py
--rw-------   0 ich       (1000) ich       (1000)     3647 2023-04-25 14:57:27.000000 upsies-2023.5.25/upsies/trackers/dummy.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.481727 upsies-2023.5.25/upsies/trackers/mtv/
--rw-------   0 ich       (1000) ich       (1000)      119 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/mtv/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     2306 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/mtv/config.py
--rw-------   0 ich       (1000) ich       (1000)     9488 2023-04-25 14:57:27.000000 upsies-2023.5.25/upsies/trackers/mtv/jobs.py
--rw-------   0 ich       (1000) ich       (1000)    12862 2023-04-25 14:57:27.000000 upsies-2023.5.25/upsies/trackers/mtv/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.481727 upsies-2023.5.25/upsies/trackers/nbl/
--rw-------   0 ich       (1000) ich       (1000)      119 2023-04-28 07:24:11.000000 upsies-2023.5.25/upsies/trackers/nbl/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     1059 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/nbl/config.py
--rw-------   0 ich       (1000) ich       (1000)     1855 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/nbl/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     3969 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/nbl/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.481727 upsies-2023.5.25/upsies/trackers/ptp/
--rw-------   0 ich       (1000) ich       (1000)      119 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/ptp/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     2146 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/ptp/config.py
--rw-------   0 ich       (1000) ich       (1000)    27925 2023-05-25 09:30:06.000000 upsies-2023.5.25/upsies/trackers/ptp/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     2001 2023-04-25 14:57:27.000000 upsies-2023.5.25/upsies/trackers/ptp/metadata.py
--rw-------   0 ich       (1000) ich       (1000)    15920 2023-04-28 13:48:23.000000 upsies-2023.5.25/upsies/trackers/ptp/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.481727 upsies-2023.5.25/upsies/uis/
--rw-------   0 ich       (1000) ich       (1000)       24 2021-06-11 16:55:41.000000 upsies-2023.5.25/upsies/uis/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.481727 upsies-2023.5.25/upsies/uis/tui/
--rw-------   0 ich       (1000) ich       (1000)       55 2022-03-13 08:25:17.000000 upsies-2023.5.25/upsies/uis/tui/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.485727 upsies-2023.5.25/upsies/uis/tui/commands/
--rw-------   0 ich       (1000) ich       (1000)     1319 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    15230 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/base.py
--rw-------   0 ich       (1000) ich       (1000)     1942 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/mediainfo.py
--rw-------   0 ich       (1000) ich       (1000)     3500 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/poster.py
--rw-------   0 ich       (1000) ich       (1000)     2513 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/release_name.py
--rw-------   0 ich       (1000) ich       (1000)     2710 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/scene.py
--rw-------   0 ich       (1000) ich       (1000)     4546 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/uis/tui/commands/screenshots.py
--rw-------   0 ich       (1000) ich       (1000)     5152 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/set.py
--rw-------   0 ich       (1000) ich       (1000)     8269 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/uis/tui/commands/submit.py
--rw-------   0 ich       (1000) ich       (1000)     8308 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/uis/tui/commands/torrent.py
--rw-------   0 ich       (1000) ich       (1000)     2034 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/upload_images.py
--rw-------   0 ich       (1000) ich       (1000)     1799 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/webdb.py
--rw-------   0 ich       (1000) ich       (1000)     3061 2022-03-13 08:27:19.000000 upsies-2023.5.25/upsies/uis/tui/headless.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.485727 upsies-2023.5.25/upsies/uis/tui/jobwidgets/
--rw-------   0 ich       (1000) ich       (1000)      947 2021-06-11 16:56:53.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6992 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/base.py
--rw-------   0 ich       (1000) ich       (1000)      252 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/config.py
--rw-------   0 ich       (1000) ich       (1000)      202 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/custom.py
--rw-------   0 ich       (1000) ich       (1000)     1902 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/dialog.py
--rw-------   0 ich       (1000) ich       (1000)      767 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/imghost.py
--rw-------   0 ich       (1000) ich       (1000)      205 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/mediainfo.py
--rw-------   0 ich       (1000) ich       (1000)     1105 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/poster.py
--rw-------   0 ich       (1000) ich       (1000)     4143 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/scene.py
--rw-------   0 ich       (1000) ich       (1000)     1649 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/screenshots.py
--rw-------   0 ich       (1000) ich       (1000)      686 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/submit.py
--rw-------   0 ich       (1000) ich       (1000)     8671 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/torrent.py
--rw-------   0 ich       (1000) ich       (1000)     9727 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/webdb.py
--rw-------   0 ich       (1000) ich       (1000)     2865 2023-05-22 08:06:05.000000 upsies-2023.5.25/upsies/uis/tui/main.py
--rw-------   0 ich       (1000) ich       (1000)     1345 2022-10-25 10:31:19.000000 upsies-2023.5.25/upsies/uis/tui/style.py
--rw-------   0 ich       (1000) ich       (1000)     9795 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/tui.py
--rw-------   0 ich       (1000) ich       (1000)      626 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/utils.py
--rw-------   0 ich       (1000) ich       (1000)    13814 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/widgets.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.489727 upsies-2023.5.25/upsies/utils/
--rw-------   0 ich       (1000) ich       (1000)    13326 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/utils/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     5658 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/utils/argtypes.py
--rw-------   0 ich       (1000) ich       (1000)      302 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/browser.py
--rw-------   0 ich       (1000) ich       (1000)     2794 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/utils/btclient.py
--rw-------   0 ich       (1000) ich       (1000)    15025 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/configfiles.py
--rw-------   0 ich       (1000) ich       (1000)     1825 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/country.py
--rw-------   0 ich       (1000) ich       (1000)     7285 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/daemon.py
--rw-------   0 ich       (1000) ich       (1000)    17717 2023-04-28 13:48:23.000000 upsies-2023.5.25/upsies/utils/fs.py
--rw-------   0 ich       (1000) ich       (1000)     2353 2023-05-25 13:46:48.000000 upsies-2023.5.25/upsies/utils/html.py
--rw-------   0 ich       (1000) ich       (1000)    23553 2023-04-28 13:48:23.000000 upsies-2023.5.25/upsies/utils/http.py
--rw-------   0 ich       (1000) ich       (1000)    10178 2023-05-25 13:46:48.000000 upsies-2023.5.25/upsies/utils/image.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.489727 upsies-2023.5.25/upsies/utils/imghosts/
--rw-------   0 ich       (1000) ich       (1000)     1391 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/imghosts/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     7453 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/imghosts/base.py
--rw-------   0 ich       (1000) ich       (1000)     1147 2021-06-11 16:56:53.000000 upsies-2023.5.25/upsies/utils/imghosts/common.py
--rw-------   0 ich       (1000) ich       (1000)     1011 2021-10-31 14:15:29.000000 upsies-2023.5.25/upsies/utils/imghosts/dummy.py
--rw-------   0 ich       (1000) ich       (1000)     1997 2021-11-27 15:46:37.000000 upsies-2023.5.25/upsies/utils/imghosts/freeimage.py
--rw-------   0 ich       (1000) ich       (1000)     2517 2021-11-26 16:53:37.000000 upsies-2023.5.25/upsies/utils/imghosts/imgbb.py
--rw-------   0 ich       (1000) ich       (1000)      912 2021-10-19 13:17:48.000000 upsies-2023.5.25/upsies/utils/imghosts/imgbox.py
--rw-------   0 ich       (1000) ich       (1000)     3154 2023-04-23 11:00:43.000000 upsies-2023.5.25/upsies/utils/imghosts/ptpimg.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.489727 upsies-2023.5.25/upsies/utils/predbs/
--rw-------   0 ich       (1000) ich       (1000)     1364 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     9573 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/base.py
--rw-------   0 ich       (1000) ich       (1000)     4128 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/common.py
--rw-------   0 ich       (1000) ich       (1000)     2276 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/corruptnet.py
--rw-------   0 ich       (1000) ich       (1000)    20069 2023-05-19 14:42:15.000000 upsies-2023.5.25/upsies/utils/predbs/multi.py
--rw-------   0 ich       (1000) ich       (1000)     2174 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/predbclub.py
--rw-------   0 ich       (1000) ich       (1000)     2333 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/predbde.py
--rw-------   0 ich       (1000) ich       (1000)     2167 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/predbovh.py
--rw-------   0 ich       (1000) ich       (1000)     5207 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/query.py
--rw-------   0 ich       (1000) ich       (1000)     3434 2023-05-22 08:05:50.000000 upsies-2023.5.25/upsies/utils/predbs/srrdb.py
--rw-------   0 ich       (1000) ich       (1000)    55868 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/release.py
--rw-------   0 ich       (1000) ich       (1000)     3931 2023-02-19 13:31:01.000000 upsies-2023.5.25/upsies/utils/signal.py
--rw-------   0 ich       (1000) ich       (1000)     3922 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/string.py
--rw-------   0 ich       (1000) ich       (1000)     1908 2023-03-31 14:19:32.000000 upsies-2023.5.25/upsies/utils/subproc.py
--rw-------   0 ich       (1000) ich       (1000)     7760 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/subtitle.py
--rw-------   0 ich       (1000) ich       (1000)     2034 2021-09-23 10:04:01.000000 upsies-2023.5.25/upsies/utils/timestamp.py
--rw-------   0 ich       (1000) ich       (1000)    19249 2023-04-25 14:57:27.000000 upsies-2023.5.25/upsies/utils/torrent.py
--rw-------   0 ich       (1000) ich       (1000)    11165 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/types.py
--rw-------   0 ich       (1000) ich       (1000)     2927 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/update.py
--rw-------   0 ich       (1000) ich       (1000)    35045 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/video.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.493727 upsies-2023.5.25/upsies/utils/webdbs/
--rw-------   0 ich       (1000) ich       (1000)     1140 2023-01-16 18:31:24.000000 upsies-2023.5.25/upsies/utils/webdbs/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     8898 2023-04-28 13:26:45.000000 upsies-2023.5.25/upsies/utils/webdbs/base.py
--rw-------   0 ich       (1000) ich       (1000)    12546 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/webdbs/common.py
--rw-------   0 ich       (1000) ich       (1000)    17839 2023-04-28 13:48:23.000000 upsies-2023.5.25/upsies/utils/webdbs/imdb.py
--rw-------   0 ich       (1000) ich       (1000)    12105 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/webdbs/tmdb.py
--rw-------   0 ich       (1000) ich       (1000)     9757 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/webdbs/tvmaze.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.477728 upsies-2023.5.25/upsies.egg-info/
--rw-------   0 ich       (1000) ich       (1000)     2367 2023-05-25 13:47:13.000000 upsies-2023.5.25/upsies.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     3702 2023-05-25 13:47:13.000000 upsies-2023.5.25/upsies.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2023-05-25 13:47:13.000000 upsies-2023.5.25/upsies.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       47 2023-05-25 13:47:13.000000 upsies-2023.5.25/upsies.egg-info/entry_points.txt
--rw-------   0 ich       (1000) ich       (1000)      237 2023-05-25 13:47:13.000000 upsies-2023.5.25/upsies.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)       10 2023-05-25 13:47:13.000000 upsies-2023.5.25/upsies.egg-info/top_level.txt
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.966841 upsies-2023.6.11/
+-rw-------   0 ich       (1000) ich       (1000)    35149 2021-06-11 16:56:53.000000 upsies-2023.6.11/LICENSE
+-rw-------   0 ich       (1000) ich       (1000)     2637 2023-06-11 11:33:55.966841 upsies-2023.6.11/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     1815 2023-04-25 13:55:04.000000 upsies-2023.6.11/README.rst
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.754842 upsies-2023.6.11/docs/
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.754842 upsies-2023.6.11/docs/_ext/
+-rw-------   0 ich       (1000) ich       (1000)     2805 2021-10-10 10:59:55.000000 upsies-2023.6.11/docs/_ext/cli_reference.py
+-rw-------   0 ich       (1000) ich       (1000)      571 2023-04-25 13:55:04.000000 upsies-2023.6.11/docs/conf.py
+-rw-------   0 ich       (1000) ich       (1000)     1772 2023-06-11 11:33:26.000000 upsies-2023.6.11/pyproject.toml
+-rw-------   0 ich       (1000) ich       (1000)       38 2023-06-11 11:33:55.966841 upsies-2023.6.11/setup.cfg
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.758842 upsies-2023.6.11/tests/
+-rw-------   0 ich       (1000) ich       (1000)     1598 2023-05-26 17:05:24.000000 upsies-2023.6.11/tests/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)     3565 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/errors_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.778842 upsies-2023.6.11/tests/jobs_test/
+-rw-------   0 ich       (1000) ich       (1000)     3036 2023-05-26 16:44:13.000000 upsies-2023.6.11/tests/jobs_test/add_torrent_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    18181 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/choice_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4769 2023-01-16 18:34:35.000000 upsies-2023.6.11/tests/jobs_test/copy_torrent_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    18147 2023-05-26 16:44:13.000000 upsies-2023.6.11/tests/jobs_test/create_torrent_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4787 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/custom_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4769 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/imghost_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    36618 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/job_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)    30782 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/mediainfo_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    15638 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/poster_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     7757 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/queue_job_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)    18248 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/scene_check_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3547 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/scene_search_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    35363 2023-05-25 13:46:48.000000 upsies-2023.6.11/tests/jobs_test/screenshots_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5619 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/set_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    12625 2023-05-25 09:31:21.000000 upsies-2023.6.11/tests/jobs_test/submit_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    14134 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/text_field_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    27694 2023-05-26 17:03:17.000000 upsies-2023.6.11/tests/jobs_test/webdb_search_job_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.782842 upsies-2023.6.11/tests/trackers_test/
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.782842 upsies-2023.6.11/tests/trackers_test/base/
+-rw-------   0 ich       (1000) ich       (1000)     3420 2023-05-25 09:31:21.000000 upsies-2023.6.11/tests/trackers_test/base/tracker_base_howto_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6319 2023-04-25 14:57:27.000000 upsies-2023.6.11/tests/trackers_test/base/tracker_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6206 2023-05-25 09:31:21.000000 upsies-2023.6.11/tests/trackers_test/base/tracker_config_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)    69602 2023-05-25 09:31:21.000000 upsies-2023.6.11/tests/trackers_test/base/tracker_jobs_base_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.790842 upsies-2023.6.11/tests/trackers_test/bhd/
+-rw-------   0 ich       (1000) ich       (1000)     5905 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/bhd/bhd_tracker_config_test.py
+-rw-------   0 ich       (1000) ich       (1000)    28649 2023-05-25 09:31:21.000000 upsies-2023.6.11/tests/trackers_test/bhd/bhd_tracker_jobs_test.py
+-rw-------   0 ich       (1000) ich       (1000)    11005 2023-04-25 14:57:27.000000 upsies-2023.6.11/tests/trackers_test/bhd/bhd_tracker_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1347 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/conftest.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.798842 upsies-2023.6.11/tests/trackers_test/mtv/
+-rw-------   0 ich       (1000) ich       (1000)     4438 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/mtv/mtv_tracker_config_test.py
+-rw-------   0 ich       (1000) ich       (1000)    31545 2023-06-06 17:48:16.000000 upsies-2023.6.11/tests/trackers_test/mtv/mtv_tracker_jobs_test.py
+-rw-------   0 ich       (1000) ich       (1000)    31622 2023-04-25 14:57:27.000000 upsies-2023.6.11/tests/trackers_test/mtv/mtv_tracker_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.802842 upsies-2023.6.11/tests/trackers_test/nbl/
+-rw-------   0 ich       (1000) ich       (1000)     1577 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/nbl/nbl_tracker_config_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4726 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/nbl/nbl_tracker_jobs_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6113 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/nbl/nbl_tracker_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.806842 upsies-2023.6.11/tests/trackers_test/ptp/
+-rw-------   0 ich       (1000) ich       (1000)     4113 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/ptp/ptp_tracker_config_test.py
+-rw-------   0 ich       (1000) ich       (1000)    31683 2023-05-25 09:31:21.000000 upsies-2023.6.11/tests/trackers_test/ptp/ptp_tracker_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1916 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/trackers_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.750842 upsies-2023.6.11/tests/uis_test/
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.810842 upsies-2023.6.11/tests/uis_test/tui_test/
+-rw-------   0 ich       (1000) ich       (1000)    21480 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/uis_test/tui_test/tui_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1425 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/uis_test/tui_test/tui_utils_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4429 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/uis_test/tui_test/tui_widgets_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.846841 upsies-2023.6.11/tests/utils_test/
+-rw-------   0 ich       (1000) ich       (1000)     9433 2023-05-25 09:31:21.000000 upsies-2023.6.11/tests/utils_test/argtypes_test.py
+-rw-------   0 ich       (1000) ich       (1000)     9133 2023-05-26 16:44:13.000000 upsies-2023.6.11/tests/utils_test/btclient_test.py
+-rw-------   0 ich       (1000) ich       (1000)    35526 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/configfiles_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1266 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/country_test.py
+-rw-------   0 ich       (1000) ich       (1000)     9048 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/daemon_test.py
+-rw-------   0 ich       (1000) ich       (1000)    31470 2023-06-11 08:46:28.000000 upsies-2023.6.11/tests/utils_test/fs_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3723 2023-04-28 07:24:11.000000 upsies-2023.6.11/tests/utils_test/html_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.854842 upsies-2023.6.11/tests/utils_test/http_test/
+-rw-------   0 ich       (1000) ich       (1000)     1474 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/http_test/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)    54514 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/http_test/http_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1233 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/http_test/http_tls_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1750 2023-05-25 13:46:48.000000 upsies-2023.6.11/tests/utils_test/image_optimize_test.py
+-rw-------   0 ich       (1000) ich       (1000)     7391 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/image_resize_test.py
+-rw-------   0 ich       (1000) ich       (1000)    12900 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/image_screenshot_test.py
+-rw-------   0 ich       (1000) ich       (1000)      425 2021-07-26 09:11:09.000000 upsies-2023.6.11/tests/utils_test/image_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.854842 upsies-2023.6.11/tests/utils_test/imghosts_test/
+-rw-------   0 ich       (1000) ich       (1000)     3390 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/imghosts_test/freeimage_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3690 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/imghosts_test/imgbb_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1932 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/imghosts_test/imgbox_test.py
+-rw-------   0 ich       (1000) ich       (1000)    14346 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/imghosts_test/imghost_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3055 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/imghosts_test/imghost_common_test.py
+-rw-------   0 ich       (1000) ich       (1000)     2791 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/imghosts_test/imghost_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6927 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/imghosts_test/ptpimg_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.866841 upsies-2023.6.11/tests/utils_test/predbs_test/
+-rw-------   0 ich       (1000) ich       (1000)     1173 2023-05-29 17:37:37.000000 upsies-2023.6.11/tests/utils_test/predbs_test/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)     6369 2023-05-29 17:37:37.000000 upsies-2023.6.11/tests/utils_test/predbs_test/corruptnet_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5723 2023-05-29 17:37:37.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbclub_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6719 2023-06-11 11:33:26.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbde_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5710 2023-05-29 17:37:37.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbovh_test.py
+-rw-------   0 ich       (1000) ich       (1000)     8255 2023-06-06 17:48:16.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbs_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)     8539 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbs_common_test.py
+-rw-------   0 ich       (1000) ich       (1000)    49224 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbs_integration_test.py
+-rw-------   0 ich       (1000) ich       (1000)    22846 2023-06-05 13:33:01.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbs_multi_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1900 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbs_test.py
+-rw-------   0 ich       (1000) ich       (1000)    22438 2023-05-31 14:49:34.000000 upsies-2023.6.11/tests/utils_test/predbs_test/srrdb_test.py
+-rw-------   0 ich       (1000) ich       (1000)     9604 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/release_episodes_test.py
+-rw-------   0 ich       (1000) ich       (1000)    31672 2023-06-01 13:28:44.000000 upsies-2023.6.11/tests/utils_test/release_info_test.py
+-rw-------   0 ich       (1000) ich       (1000)    64364 2023-06-06 17:48:16.000000 upsies-2023.6.11/tests/utils_test/release_name_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5455 2021-09-30 12:51:20.000000 upsies-2023.6.11/tests/utils_test/signal_test.py
+-rw-------   0 ich       (1000) ich       (1000)     9667 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/string_test.py
+-rw-------   0 ich       (1000) ich       (1000)     2695 2023-03-13 14:34:58.000000 upsies-2023.6.11/tests/utils_test/subproc_test.py
+-rw-------   0 ich       (1000) ich       (1000)    11884 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/subtitle_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3156 2021-06-11 16:56:53.000000 upsies-2023.6.11/tests/utils_test/timestamp_test.py
+-rw-------   0 ich       (1000) ich       (1000)    30246 2023-05-26 16:44:13.000000 upsies-2023.6.11/tests/utils_test/torrent_test.py
+-rw-------   0 ich       (1000) ich       (1000)    14894 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/types_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5089 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/update_test.py
+-rw-------   0 ich       (1000) ich       (1000)    13913 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/utils_test.py
+-rw-------   0 ich       (1000) ich       (1000)    72586 2023-06-01 13:28:44.000000 upsies-2023.6.11/tests/utils_test/video_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.874841 upsies-2023.6.11/tests/utils_test/webdbs_test/
+-rw-------   0 ich       (1000) ich       (1000)     1423 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/webdbs_test/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)    37489 2023-04-28 13:26:51.000000 upsies-2023.6.11/tests/utils_test/webdbs_test/imdb_test.py
+-rw-------   0 ich       (1000) ich       (1000)    20288 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/webdbs_test/tmdb_test.py
+-rw-------   0 ich       (1000) ich       (1000)    25066 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/webdbs_test/tvmaze_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4812 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/webdbs_test/webdbs_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)    19231 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/webdbs_test/webdbs_common_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1903 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/webdbs_test/webdbs_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.878841 upsies-2023.6.11/upsies/
+-rw-------   0 ich       (1000) ich       (1000)     1117 2023-06-11 11:33:26.000000 upsies-2023.6.11/upsies/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)       73 2022-03-13 08:26:06.000000 upsies-2023.6.11/upsies/__main__.py
+-rw-------   0 ich       (1000) ich       (1000)     1399 2023-03-19 11:08:21.000000 upsies-2023.6.11/upsies/constants.py
+-rw-------   0 ich       (1000) ich       (1000)     2058 2023-05-26 09:17:09.000000 upsies-2023.6.11/upsies/defaults.py
+-rw-------   0 ich       (1000) ich       (1000)     6274 2023-05-26 16:44:13.000000 upsies-2023.6.11/upsies/errors.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.886841 upsies-2023.6.11/upsies/jobs/
+-rw-------   0 ich       (1000) ich       (1000)      215 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/jobs/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    27889 2023-06-05 13:24:27.000000 upsies-2023.6.11/upsies/jobs/base.py
+-rw-------   0 ich       (1000) ich       (1000)     2165 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/jobs/custom.py
+-rw-------   0 ich       (1000) ich       (1000)    21011 2023-06-01 14:38:39.000000 upsies-2023.6.11/upsies/jobs/dialog.py
+-rw-------   0 ich       (1000) ich       (1000)     3707 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/jobs/imghost.py
+-rw-------   0 ich       (1000) ich       (1000)     4807 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/jobs/mediainfo.py
+-rw-------   0 ich       (1000) ich       (1000)     7596 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/jobs/poster.py
+-rw-------   0 ich       (1000) ich       (1000)     8681 2023-06-05 13:24:22.000000 upsies-2023.6.11/upsies/jobs/scene.py
+-rw-------   0 ich       (1000) ich       (1000)    17965 2023-05-25 13:46:48.000000 upsies-2023.6.11/upsies/jobs/screenshots.py
+-rw-------   0 ich       (1000) ich       (1000)     2770 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/jobs/set.py
+-rw-------   0 ich       (1000) ich       (1000)     7977 2023-06-05 13:23:49.000000 upsies-2023.6.11/upsies/jobs/submit.py
+-rw-------   0 ich       (1000) ich       (1000)    13075 2023-05-26 16:44:13.000000 upsies-2023.6.11/upsies/jobs/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)    13899 2023-06-01 14:34:49.000000 upsies-2023.6.11/upsies/jobs/webdb.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.886841 upsies-2023.6.11/upsies/trackers/
+-rw-------   0 ich       (1000) ich       (1000)     1385 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.894841 upsies-2023.6.11/upsies/trackers/base/
+-rw-------   0 ich       (1000) ich       (1000)      149 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/base/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3222 2023-05-25 09:31:21.000000 upsies-2023.6.11/upsies/trackers/base/_howto.py
+-rw-------   0 ich       (1000) ich       (1000)     3102 2023-05-25 09:31:21.000000 upsies-2023.6.11/upsies/trackers/base/config.py
+-rw-------   0 ich       (1000) ich       (1000)    33425 2023-05-25 09:31:21.000000 upsies-2023.6.11/upsies/trackers/base/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     5985 2023-04-25 14:57:27.000000 upsies-2023.6.11/upsies/trackers/base/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.898841 upsies-2023.6.11/upsies/trackers/bhd/
+-rw-------   0 ich       (1000) ich       (1000)      119 2023-04-28 07:24:11.000000 upsies-2023.6.11/upsies/trackers/bhd/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3643 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/bhd/config.py
+-rw-------   0 ich       (1000) ich       (1000)    15623 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/bhd/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     6243 2023-04-25 14:57:27.000000 upsies-2023.6.11/upsies/trackers/bhd/tracker.py
+-rw-------   0 ich       (1000) ich       (1000)     3647 2023-05-26 15:12:26.000000 upsies-2023.6.11/upsies/trackers/dummy.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.902841 upsies-2023.6.11/upsies/trackers/mtv/
+-rw-------   0 ich       (1000) ich       (1000)      119 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/mtv/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     2306 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/mtv/config.py
+-rw-------   0 ich       (1000) ich       (1000)    10049 2023-06-06 17:48:16.000000 upsies-2023.6.11/upsies/trackers/mtv/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)    12862 2023-04-25 14:57:27.000000 upsies-2023.6.11/upsies/trackers/mtv/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.906841 upsies-2023.6.11/upsies/trackers/nbl/
+-rw-------   0 ich       (1000) ich       (1000)      119 2023-04-28 07:24:11.000000 upsies-2023.6.11/upsies/trackers/nbl/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     1059 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/nbl/config.py
+-rw-------   0 ich       (1000) ich       (1000)     1855 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/nbl/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     3969 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/nbl/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.914841 upsies-2023.6.11/upsies/trackers/ptp/
+-rw-------   0 ich       (1000) ich       (1000)      119 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/ptp/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     2146 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/ptp/config.py
+-rw-------   0 ich       (1000) ich       (1000)    27925 2023-05-25 09:30:06.000000 upsies-2023.6.11/upsies/trackers/ptp/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     2001 2023-04-25 14:57:27.000000 upsies-2023.6.11/upsies/trackers/ptp/metadata.py
+-rw-------   0 ich       (1000) ich       (1000)    15920 2023-04-28 13:48:23.000000 upsies-2023.6.11/upsies/trackers/ptp/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.914841 upsies-2023.6.11/upsies/uis/
+-rw-------   0 ich       (1000) ich       (1000)       24 2021-06-11 16:55:41.000000 upsies-2023.6.11/upsies/uis/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.922841 upsies-2023.6.11/upsies/uis/tui/
+-rw-------   0 ich       (1000) ich       (1000)       55 2022-03-13 08:25:17.000000 upsies-2023.6.11/upsies/uis/tui/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.926841 upsies-2023.6.11/upsies/uis/tui/commands/
+-rw-------   0 ich       (1000) ich       (1000)     1319 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    15239 2023-06-07 15:27:08.000000 upsies-2023.6.11/upsies/uis/tui/commands/base.py
+-rw-------   0 ich       (1000) ich       (1000)     1942 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/mediainfo.py
+-rw-------   0 ich       (1000) ich       (1000)     3500 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/poster.py
+-rw-------   0 ich       (1000) ich       (1000)     2513 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/release_name.py
+-rw-------   0 ich       (1000) ich       (1000)     2710 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/scene.py
+-rw-------   0 ich       (1000) ich       (1000)     4546 2023-05-25 09:31:21.000000 upsies-2023.6.11/upsies/uis/tui/commands/screenshots.py
+-rw-------   0 ich       (1000) ich       (1000)     5152 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/set.py
+-rw-------   0 ich       (1000) ich       (1000)     8323 2023-05-26 16:44:13.000000 upsies-2023.6.11/upsies/uis/tui/commands/submit.py
+-rw-------   0 ich       (1000) ich       (1000)     8424 2023-05-26 16:44:13.000000 upsies-2023.6.11/upsies/uis/tui/commands/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)     2034 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/upload_images.py
+-rw-------   0 ich       (1000) ich       (1000)     1799 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/webdb.py
+-rw-------   0 ich       (1000) ich       (1000)     3061 2022-03-13 08:27:19.000000 upsies-2023.6.11/upsies/uis/tui/headless.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.930841 upsies-2023.6.11/upsies/uis/tui/jobwidgets/
+-rw-------   0 ich       (1000) ich       (1000)      947 2021-06-11 16:56:53.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6992 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/base.py
+-rw-------   0 ich       (1000) ich       (1000)      252 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/config.py
+-rw-------   0 ich       (1000) ich       (1000)      202 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/custom.py
+-rw-------   0 ich       (1000) ich       (1000)     1902 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/dialog.py
+-rw-------   0 ich       (1000) ich       (1000)      767 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/imghost.py
+-rw-------   0 ich       (1000) ich       (1000)      205 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/mediainfo.py
+-rw-------   0 ich       (1000) ich       (1000)     1105 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/poster.py
+-rw-------   0 ich       (1000) ich       (1000)     4143 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/scene.py
+-rw-------   0 ich       (1000) ich       (1000)     1649 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/screenshots.py
+-rw-------   0 ich       (1000) ich       (1000)      686 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/submit.py
+-rw-------   0 ich       (1000) ich       (1000)     8671 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)     9727 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/webdb.py
+-rw-------   0 ich       (1000) ich       (1000)     2865 2023-06-07 15:14:22.000000 upsies-2023.6.11/upsies/uis/tui/main.py
+-rw-------   0 ich       (1000) ich       (1000)     1345 2022-10-25 10:31:19.000000 upsies-2023.6.11/upsies/uis/tui/style.py
+-rw-------   0 ich       (1000) ich       (1000)     9795 2023-06-05 13:36:26.000000 upsies-2023.6.11/upsies/uis/tui/tui.py
+-rw-------   0 ich       (1000) ich       (1000)      626 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/utils.py
+-rw-------   0 ich       (1000) ich       (1000)    13814 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/widgets.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.950841 upsies-2023.6.11/upsies/utils/
+-rw-------   0 ich       (1000) ich       (1000)    13326 2023-06-05 13:36:24.000000 upsies-2023.6.11/upsies/utils/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     5658 2023-05-25 09:31:21.000000 upsies-2023.6.11/upsies/utils/argtypes.py
+-rw-------   0 ich       (1000) ich       (1000)      302 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/browser.py
+-rw-------   0 ich       (1000) ich       (1000)     4303 2023-05-26 16:44:13.000000 upsies-2023.6.11/upsies/utils/btclient.py
+-rw-------   0 ich       (1000) ich       (1000)    15025 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/configfiles.py
+-rw-------   0 ich       (1000) ich       (1000)     1825 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/country.py
+-rw-------   0 ich       (1000) ich       (1000)     7285 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/daemon.py
+-rw-------   0 ich       (1000) ich       (1000)    17924 2023-06-11 11:33:26.000000 upsies-2023.6.11/upsies/utils/fs.py
+-rw-------   0 ich       (1000) ich       (1000)     2353 2023-05-25 13:46:48.000000 upsies-2023.6.11/upsies/utils/html.py
+-rw-------   0 ich       (1000) ich       (1000)    23553 2023-05-26 16:34:04.000000 upsies-2023.6.11/upsies/utils/http.py
+-rw-------   0 ich       (1000) ich       (1000)    10178 2023-05-25 13:46:48.000000 upsies-2023.6.11/upsies/utils/image.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.954841 upsies-2023.6.11/upsies/utils/imghosts/
+-rw-------   0 ich       (1000) ich       (1000)     1391 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/imghosts/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     7453 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/imghosts/base.py
+-rw-------   0 ich       (1000) ich       (1000)     1147 2021-06-11 16:56:53.000000 upsies-2023.6.11/upsies/utils/imghosts/common.py
+-rw-------   0 ich       (1000) ich       (1000)     1011 2021-10-31 14:15:29.000000 upsies-2023.6.11/upsies/utils/imghosts/dummy.py
+-rw-------   0 ich       (1000) ich       (1000)     1997 2021-11-27 15:46:37.000000 upsies-2023.6.11/upsies/utils/imghosts/freeimage.py
+-rw-------   0 ich       (1000) ich       (1000)     2517 2021-11-26 16:53:37.000000 upsies-2023.6.11/upsies/utils/imghosts/imgbb.py
+-rw-------   0 ich       (1000) ich       (1000)      912 2021-10-19 13:17:48.000000 upsies-2023.6.11/upsies/utils/imghosts/imgbox.py
+-rw-------   0 ich       (1000) ich       (1000)     3154 2023-04-23 11:00:43.000000 upsies-2023.6.11/upsies/utils/imghosts/ptpimg.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.958841 upsies-2023.6.11/upsies/utils/predbs/
+-rw-------   0 ich       (1000) ich       (1000)     1364 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/predbs/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     9619 2023-06-06 17:48:16.000000 upsies-2023.6.11/upsies/utils/predbs/base.py
+-rw-------   0 ich       (1000) ich       (1000)     4128 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/predbs/common.py
+-rw-------   0 ich       (1000) ich       (1000)     2278 2023-05-29 17:37:37.000000 upsies-2023.6.11/upsies/utils/predbs/corruptnet.py
+-rw-------   0 ich       (1000) ich       (1000)    20881 2023-06-05 13:43:50.000000 upsies-2023.6.11/upsies/utils/predbs/multi.py
+-rw-------   0 ich       (1000) ich       (1000)     2176 2023-05-29 17:37:37.000000 upsies-2023.6.11/upsies/utils/predbs/predbclub.py
+-rw-------   0 ich       (1000) ich       (1000)     2414 2023-06-11 11:33:26.000000 upsies-2023.6.11/upsies/utils/predbs/predbde.py
+-rw-------   0 ich       (1000) ich       (1000)     2169 2023-05-29 17:37:37.000000 upsies-2023.6.11/upsies/utils/predbs/predbovh.py
+-rw-------   0 ich       (1000) ich       (1000)     5425 2023-05-29 17:37:37.000000 upsies-2023.6.11/upsies/utils/predbs/query.py
+-rw-------   0 ich       (1000) ich       (1000)     6654 2023-05-31 14:49:34.000000 upsies-2023.6.11/upsies/utils/predbs/srrdb.py
+-rw-------   0 ich       (1000) ich       (1000)    56212 2023-06-01 13:28:44.000000 upsies-2023.6.11/upsies/utils/release.py
+-rw-------   0 ich       (1000) ich       (1000)     3931 2023-02-19 13:31:01.000000 upsies-2023.6.11/upsies/utils/signal.py
+-rw-------   0 ich       (1000) ich       (1000)     3922 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/string.py
+-rw-------   0 ich       (1000) ich       (1000)     1908 2023-03-31 14:19:32.000000 upsies-2023.6.11/upsies/utils/subproc.py
+-rw-------   0 ich       (1000) ich       (1000)     7760 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/subtitle.py
+-rw-------   0 ich       (1000) ich       (1000)     2034 2021-09-23 10:04:01.000000 upsies-2023.6.11/upsies/utils/timestamp.py
+-rw-------   0 ich       (1000) ich       (1000)    19315 2023-05-26 16:44:13.000000 upsies-2023.6.11/upsies/utils/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)    11165 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/types.py
+-rw-------   0 ich       (1000) ich       (1000)     2927 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/update.py
+-rw-------   0 ich       (1000) ich       (1000)    35111 2023-06-01 13:28:44.000000 upsies-2023.6.11/upsies/utils/video.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.962841 upsies-2023.6.11/upsies/utils/webdbs/
+-rw-------   0 ich       (1000) ich       (1000)     1140 2023-01-16 18:31:24.000000 upsies-2023.6.11/upsies/utils/webdbs/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     8898 2023-04-28 13:26:45.000000 upsies-2023.6.11/upsies/utils/webdbs/base.py
+-rw-------   0 ich       (1000) ich       (1000)    12546 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/webdbs/common.py
+-rw-------   0 ich       (1000) ich       (1000)    17839 2023-04-28 13:48:23.000000 upsies-2023.6.11/upsies/utils/webdbs/imdb.py
+-rw-------   0 ich       (1000) ich       (1000)    12105 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/webdbs/tmdb.py
+-rw-------   0 ich       (1000) ich       (1000)     9757 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/webdbs/tvmaze.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.878841 upsies-2023.6.11/upsies.egg-info/
+-rw-------   0 ich       (1000) ich       (1000)     2637 2023-06-11 11:33:55.000000 upsies-2023.6.11/upsies.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     7413 2023-06-11 11:33:55.000000 upsies-2023.6.11/upsies.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2023-06-11 11:33:55.000000 upsies-2023.6.11/upsies.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)       47 2023-06-11 11:33:55.000000 upsies-2023.6.11/upsies.egg-info/entry_points.txt
+-rw-------   0 ich       (1000) ich       (1000)      320 2023-06-11 11:33:55.000000 upsies-2023.6.11/upsies.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)       65 2023-06-11 11:33:55.000000 upsies-2023.6.11/upsies.egg-info/top_level.txt
```

### Comparing `upsies-2023.5.25/LICENSE` & `upsies-2023.6.11/LICENSE`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/PKG-INFO` & `upsies-2023.6.11/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: upsies
-Version: 2023.5.25
+Version: 2023.6.11
 Summary: Media metadata aggregator
-Home-page: https://upsies.readthedocs.io
-Author: plotski
-Author-email: plotski@example.org
+Author-email: plotski <plotski@example.org>
+License: GPL-3.0-or-later
+Project-URL: Repository, https://codeberg.org/plotski/upsies
+Project-URL: Documentation, https://upsies.readthedocs.io
+Project-URL: Bug Tracker, https://codeberg.org/plotski/upsies/issues
+Project-URL: Changelog, https://codeberg.org/plotski/upsies/raw/branch/master/NEWS
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: dev
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/pyversions/upsies
            :target: https://www.python.org/
 .. image:: https://img.shields.io/pypi/l/upsies
            :target: https://www.gnu.org/licenses/gpl-3.0.en.html
 .. image:: https://img.shields.io/pypi/v/upsies
```

### Comparing `upsies-2023.5.25/README.rst` & `upsies-2023.6.11/README.rst`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/bb/jobs.py` & `upsies-2023.6.11/upsies/utils/release.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1303 +1,1642 @@
 """
-Concrete :class:`~.base.TrackerJobsBase` subclass for bB
+Release name parsing and formatting
+
+:class:`ReleaseInfo` parses a string into a dictionary-like object with a
+specific set of keys, e.g. "title", "resolution", "source", etc.
+
+:class:`ReleaseName` wraps :class:`ReleaseInfo` to do the same, but in addition
+it tries to read media data from the file system to get information. It also
+adds a :class:`~.ReleaseName.format` method to turn everything back into a
+string.
 """
 
 import asyncio
+import collections
+import copy
+import functools
 import os
 import re
+import time
 
+import natsort
 import unidecode
 
-from ... import __homepage__, __project_name__, __version__, errors, jobs
-from ...utils import cached_property, fs, http, image, release, string, video
-from ..base import TrackerJobsBase
+from .. import constants, errors, utils
+from . import LazyModule, fs, video
+from .types import ReleaseType
 
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
+# Disable debugging messages from rebulk
+logging.getLogger('rebulk').setLevel(logging.WARNING)
 
-class BbTrackerJobs(TrackerJobsBase):
-    @cached_property
-    def release_name(self):
-        """:class:`~.release.ReleaseName` instance"""
-        return release.ReleaseName(self.content_path)
+_guessit = LazyModule(module='guessit.api', name='_guessit', namespace=globals())
 
-    @property
-    def release_type(self):
-        """:class:`~.types.ReleaseType` enum"""
-        return self.release_type_job.choice
 
-    @property
-    def is_movie_release(self):
-        return self.release_type is release.ReleaseType.movie
+DELIM = r'[ \.-]'
+"""
+Regular expression that matches a single delimiter between release name
+parts, usually ``"."`` or ``" "``
+"""
 
-    @property
-    def is_season_release(self):
-        return self.release_type is release.ReleaseType.season
 
-    @property
-    def is_episode_release(self):
-        return self.release_type is release.ReleaseType.episode
+class _translated_property:
+    """
+    Property that is automatically translated on lookup
+
+    The translation is based on a mapping on the parent instance. It must be
+    available as ``_translate``. It maps regular expressions to replacement
+    strings. All regular expressions are applied in order.
+    """
+
+    def __init__(self, fget=None, fset=None, fdel=None, doc=None):
+        self.name = fget.__name__
+        self.fget = fget
+        self.fset = fset
+        self.fdel = fdel
+        if doc is None and fget is not None:
+            doc = fget.__doc__
+        self.__doc__ = doc
+
+    def __get__(self, obj, objtype=None):
+        if obj is None:
+            return self
+        else:
+            value = self.fget(obj)
+            return self._apply_translation(value, obj._translate)
+
+    def _apply_translation(self, value, tables):
+        def translate(string):
+            table = tables.get(self.name, {})
+            for regex, replacement in table.items():
+                string = regex.sub(replacement, string)
+            return string
+
+        if isinstance(value, str):
+            value = translate(value)
+        elif isinstance(value, collections.abc.Iterable):
+            value[:] = [translate(v) for v in value]
+
+        return value
+
+    def __set__(self, obj, value):
+        if self.fset is None:
+            raise AttributeError("Can't set attribute")
+        self.fset(obj, value)
+
+    def __delete__(self, obj):
+        raise AttributeError("Can't delete attribute")
+
+    def getter(self, fget):
+        return type(self)(fget, self.fset, self.fdel, self.__doc__)
+
+    def setter(self, fset):
+        return type(self)(self.fget, fset, self.fdel, self.__doc__)
+
+
+class ReleaseName(collections.abc.Mapping):
+    """
+    Standardized release name
+
+    :param str path: Path to release file or directory
+
+        If :attr:`path` exists, it is used to read video and audio metadata,
+        e.g. to detect the codecs, resolution, etc.
+
+    :param str name: Path or other string to pass to :class:`ReleaseInfo`
+        (defaults to `path`)
+
+    :param dict translate: Map names of properties that return a string
+        (e.g. ``audio_format``) to maps of regular expressions to replacement
+        strings. The replacement strings may contain backreferences to groups in
+        their regular expression.
+
+        Example:
+
+        >>> {
+        >>>     'audio_format': {
+        >>>         re.compile(r'^DDP$'): r'DD+',
+        >>>     },
+        >>>     'video_format': {
+        >>>         re.compile(r'^x26([45])$'): r'H.26\1',
+        >>>     },
+        >>> }
+
+    :param str separator: Separator between release name parts (usually " " or
+        ".") or `None` to use the default
+
+    Example:
+
+    >>> rn = ReleaseName("path/to/The.Foo.1984.1080p.Blu-ray.X264-ASDF")
+    >>> rn.source
+    'BluRay'
+    >>> rn.format()
+    'The Foo 1984 1080p BluRay DTS x264-ASDF'
+    >>> "{title} ({year}) [{group}]".format(**rn)
+    'The Foo (1984) [ASDF]'
+    >>> rn.set_name('The Foo 1985 1080p BluRay DTS x264-AsdF')
+    >>> "{title} ({year}) [{group}]".format(**rn)
+    'The Foo (1985) [AsdF]'
+    """
+
+    def __init__(self, path, name=None, translate=None, separator=None):
+        self._path = str(path)
+        self._name = name
+        self.separator = separator
+        self._info = ReleaseInfo(str(name) if name is not None else self._path)
+        self._translate = translate or {}
+
+    @property
+    def release_info(self):
+        """Internal :class:`~.ReleaseInfo` instance"""
+        return self._info
+
+    def set_release_info(self, path):
+        """
+        Update internal :class:`ReleaseInfo` instance
+
+        :param path: Argument for :class:`ReleaseInfo` (path or any other
+            string)
+        """
+        self._info = ReleaseInfo(str(path))
+
+    def __repr__(self):
+        posargs = [self._path]
+        kwargs = {}
+        if self._name is not None:
+            kwargs['name'] = self._name
+        if self._translate:
+            kwargs['translate'] = self._translate
+        args = ', '.join(repr(arg) for arg in posargs)
+        if kwargs:
+            args += ', ' + ', '.join(f'{k}={v!r}' for k, v in kwargs.items())
+        return f'{type(self).__name__}({args})'
+
+    def __str__(self):
+        return self.format()
+
+    def __len__(self):
+        return len(tuple(iter(self)))
+
+    def __iter__(self):
+        # Non-private properties are dictionary keys
+        cls = type(self)
+        return iter(attr for attr in dir(self)
+                    if (not attr.startswith('_')
+                        and isinstance(getattr(cls, attr), (property, _translated_property))))
+
+    def __getitem__(self, name):
+        if not isinstance(name, str):
+            raise TypeError(f'Not a string: {name!r}')
+        elif isinstance(getattr(type(self), name, None), (property, _translated_property)):
+            return getattr(self, name)
+        else:
+            raise KeyError(name)
 
     @property
-    def is_series_release(self):
-        return self.release_type in (release.ReleaseType.season,
-                                     release.ReleaseType.episode)
+    def path(self):
+        """:class:`str` version of the `path` instantiation argument"""
+        return self._path
 
     @property
-    def season(self):
-        """Season number or `None`"""
-        match = re.search(r'S0*(\d+)', self.release_name.episodes)
-        if match:
-            return int(match.group(1))
+    def separator(self):
+        """
+        Separator between release name parts (usually " " or ".") or `None` to use
+        the default
+        """
+        return self._separator
+
+    @separator.setter
+    def separator(self, separator):
+        self._separator = str(separator) if separator is not None else ' '
 
     @property
-    def episode(self):
-        """Episode number or `None`"""
-        match = re.search(r'E0*(\d+)', self.release_name.episodes)
-        if match:
-            return int(match.group(1))
+    def type(self):
+        """
+        :class:`~.types.ReleaseType` enum or one of its value names
+
+        See also :meth:`fetch_info`.
+        """
+        return self._info.get('type', ReleaseType.unknown)
 
-    # Web DBs
+    @type.setter
+    def type(self, value):
+        if not value:
+            self._info['type'] = ReleaseType.unknown
+        else:
+            self._info['type'] = ReleaseType(value)
 
-    async def get_imdb_id(self):
-        """Return IMDb ID by any means possible, default to `None`"""
-        if self.imdb_job.is_enabled:
-            await self.imdb_job.wait()
-            if self.imdb_job.output:
-                return self.imdb_job.output[0]
-        else:
-            tvmaze_id = await self.get_tvmaze_id()
-            if tvmaze_id:
-                return await self.tvmaze.imdb_id(tvmaze_id)
-
-    async def get_tvmaze_id(self):
-        """Return TVmaze ID by any means possible, default to `None`"""
-        if self.tvmaze_job.is_enabled:
-            await self.tvmaze_job.wait()
-            if self.tvmaze_job.output:
-                return self.tvmaze_job.output[0]
+    @_translated_property
+    def title(self):
+        """
+        Original name of movie or series or "UNKNOWN_TITLE"
 
-    async def try_webdbs(self, webdbs, method, default=None):
+        See also :meth:`fetch_info`.
         """
-        Try to run `method` on each item in `webdbs` and return the first truthy
-        return value
+        return self._info.get('title') or 'UNKNOWN_TITLE'
 
-        :params webdbs: Sequence of :class:`~.webdbs.base.WebDbApiBase`
-            instances
-        :params str method: Name of a method of any item in `webdbs`
-
-        Before calling `method`, an attempt is made to get the DB's ID by
-        calling the ``get_<webdb.name>_id`` method. If that fails, the next DB
-        is tried. If an ID is returned, it is passed to `method`.
-
-        :return: The first truthy return value of `method`
-        """
-        for webdb in webdbs:
-            id_getter = getattr(self, f'get_{webdb.name}_id')
-            id = await id_getter()
-            if id:
-                result_getter = getattr(webdb, method)
-                result = await result_getter(id)
-                if result:
-                    return result
-        try:
-            # Default to return value from final webdb, e.g. empty string, empty
-            # list, etc (these wouldn't be returned above, they are falsy)
-            return result
-        except NameError:
-            # Return default if we couldn't get an ID for any webdb
-            return default
-
-    # Jobs
-
-    @cached_property
-    def jobs_before_upload(self):
-        # Turn generic jobs from parent class into conditional jobs.
-        all_release_types = (release.ReleaseType.movie, release.ReleaseType.series, release.ReleaseType.episode)
-        generic_job_attributes = ('mediainfo_job', 'scene_check_job', 'create_torrent_job',
-                                  'screenshots_job', 'upload_screenshots_job',
-                                  'add_torrent_job', 'copy_torrent_job')
-        for job_attr in generic_job_attributes:
-            job = getattr(self, job_attr)
-            if job is not None:
-                job.condition = self.make_job_condition(job_attr, *all_release_types)
-
-        # Return all possible jobs and disable/enable them via JobBase's
-        # "condition" argument.
-        return (
-            # Generic jobs
-            self.release_type_job,
-            self.mediainfo_job,
-            self.create_torrent_job,
-            self.screenshots_job,
-            self.upload_screenshots_job,
-            self.scene_check_job,
-
-            # Movie jobs
-            self.imdb_job,
-            self.movie_title_job,
-            self.movie_year_job,
-            self.movie_resolution_job,
-            self.movie_source_job,
-            self.movie_audio_codec_job,
-            self.movie_video_codec_job,
-            self.movie_container_job,
-            self.movie_release_info_job,
-            self.movie_poster_job,
-            self.movie_tags_job,
-            self.movie_description_job,
-
-            # Series jobs
-            self.tvmaze_job,
-            self.series_title_job,
-            self.series_poster_job,
-            self.series_tags_job,
-            self.series_description_job,
-        )
+    @title.setter
+    def title(self, value):
+        self._info['title'] = str(value)
 
-    def make_job_condition(self, job_attr, *release_types):
+    @_translated_property
+    def title_aka(self):
         """
-        Return :attr:`~.base.JobBase.condition` for jobs
+        Alternative name of movie or series or empty string
 
-        :param str job_attr: Name of the job attribute this condition is for
+        For non-English original titles, this should be the English title. If
+        :attr:`title` is identical, this is an empty string.
+
+        See also :meth:`fetch_info`.
         """
-        def condition():
-            if self.release_type in release_types:
-                # Job is appropriate for release type
-                isolated_jobs = self.isolated_jobs
-                if not isolated_jobs:
-                    # No jobs where singled out via CLI arguments or other
-                    # means; all appropriate jobs are enabled
-                    return True
-                elif job_attr in isolated_jobs:
-                    # This particular job was singled out by the user;
-                    # all other jobs are disabled
-                    return True
-            return False
+        aka = self._info.get('aka') or ''
+        if aka and aka != self.title:
+            return aka
+        else:
+            return ''
 
-        return condition
+    @title_aka.setter
+    def title_aka(self, value):
+        self._info['aka'] = str(value)
+
+    @_translated_property
+    def title_with_aka(self):
+        """Combination of :attr:`title` and :attr:`title_aka`"""
+        if self.title_aka:
+            return f'{self.title} AKA {self.title_aka}'
+        else:
+            return self.title
+
+    @_translated_property
+    def title_with_aka_and_year(self):
+        """
+        Combination of :attr:`title_with_aka` with :attr:`country` and :attr:`year`
+        if appropriate
+
+        If :attr:`date` is specified, it is appended to :attr:`title_with_aka`.
+        Otherwise, if :attr:`year_required` is `True`, :attr:`year` is appended.
+
+        If :attr:`country_required` is `True`, :attr:`country` is appended.
+        """
+        title = [self.title_with_aka]
+
+        if self.date:
+            title.append(self.date)
+        elif self.year_required:
+            title.append(self.year)
+
+        if self.country_required:
+            title.append(self.country)
+
+        return ' '.join(title)
+
+    @_translated_property
+    def year(self):
+        """
+        Release year or "UNKNOWN_YEAR" if :attr:`year_required` is set, empty string
+        otherwise
+
+        See also :meth:`fetch_info`.
+        """
+        if self.year_required:
+            return self._info.get('year') or 'UNKNOWN_YEAR'
+        else:
+            return self._info.get('year') or ''
+
+    @year.setter
+    def year(self, value):
+        if not isinstance(value, (str, int)) and value is not None:
+            raise TypeError(f'Not a number: {value!r}')
+        elif not value:
+            self._info['year'] = ''
+        else:
+            year = str(value)
+            current_year = int(time.strftime('%Y')) + 2
+            if len(year) != 4 or not year.isdecimal() or not 1880 <= int(year) <= current_year:
+                raise ValueError(f'Invalid year: {value}')
+            self._info['year'] = year
 
     @property
-    def isolated_jobs(self):
+    def year_required(self):
         """
-        Sequence of attribute names (e.g. "movie_poster_job") that were singled out
-        by the user, e.g. with a CLI argument
+        Whether :attr:`title_with_aka_and_year` includes :attr:`year`
+
+        See also :meth:`fetch_info`.
         """
-        if self.is_movie_release:
-            if self.options.get('only_description', False):
-                return ('imdb_job', 'movie_description_job')
-            elif self.options.get('only_poster', False):
-                return ('imdb_job', 'movie_poster_job')
-            elif self.options.get('only_release_info', False):
-                return ('movie_release_info_job',)
-            elif self.options.get('only_tags', False):
-                return ('imdb_job', 'movie_tags_job')
-            elif self.options.get('only_title', False):
-                return ('imdb_job', 'movie_title_job')
-
-        elif self.is_series_release:
-            if self.options.get('only_description', False):
-                return ('tvmaze_job', 'mediainfo_job', 'screenshots_job',
-                        'upload_screenshots_job', 'series_description_job')
-            elif self.options.get('only_poster', False):
-                return ('tvmaze_job', 'series_poster_job')
-            elif self.options.get('only_title', False) or self.options.get('only_release_info', False):
-                # Series title and release_info are combined
-                return ('tvmaze_job', 'series_title_job')
-            elif self.options.get('only_tags', False):
-                return ('tvmaze_job', 'series_tags_job')
-
-        return ()
-
-    @cached_property
-    def release_type_job(self):
-        return jobs.dialog.ChoiceJob(
-            name=self.get_job_name('release-type'),
-            label='Release Type',
-            choices=(
-                ('Movie', release.ReleaseType.movie),
-                ('Season', release.ReleaseType.season),
-                ('Episode', release.ReleaseType.episode),
-            ),
-            focused=self.release_name.type,
-            callbacks={
-                'output': self.handle_release_type_selected,
-            },
-            **self.common_job_args,
-        )
+        default = self.type is ReleaseType.movie
+        return getattr(self, '_year_required', default)
 
-    def handle_release_type_selected(self, _):
-        if self.release_type_job.choice:
-            self.imdb_job.query.type = self.release_type_job.choice
-
-    # Movie jobs
-
-    @cached_property
-    def imdb_job(self):
-        """:class:`~.jobs.webdb.WebDbSearchJob` instance"""
-        imdb_job = super().imdb_job
-        imdb_job.condition = self.make_job_condition('imdb_job', release.ReleaseType.movie)
-        imdb_job.no_id_ok = True
-        return imdb_job
-
-    @cached_property
-    def movie_title_job(self):
-        self.imdb_job.signal.register('finished', self.fill_in_movie_title)
-        return jobs.dialog.TextFieldJob(
-            name=self.get_job_name('movie-title'),
-            label='Title',
-            condition=self.make_job_condition('movie_title_job', release.ReleaseType.movie),
-            validator=self.movie_title_validator,
-            **self.common_job_args,
-        )
+    @year_required.setter
+    def year_required(self, value):
+        self._year_required = bool(value)
 
-    def movie_title_validator(self, text):
-        text = text.strip()
-        if not text:
-            raise ValueError('Failed to autodetect title')
-
-    def fill_in_movie_title(self, job_):
-        task = self.movie_title_job.fetch_text(
-            coro=self.get_movie_title(),
-            default_text=self.release_name.title_with_aka,
-            finish_on_success=False,
-        )
-        self.movie_title_job.add_task(task)
+    @_translated_property
+    def country(self):
+        """
+        Release country or "UNKNOWN_COUNTRY" if :attr:`country_required` is set,
+        empty string otherwise
 
-    @cached_property
-    def movie_year_job(self):
-        self.imdb_job.signal.register('finished', self.fill_in_movie_year)
-        return jobs.dialog.TextFieldJob(
-            name=self.get_job_name('movie-year'),
-            label='Year',
-            condition=self.make_job_condition('movie_year_job', release.ReleaseType.movie),
-            validator=self.movie_year_validator,
-            **self.common_job_args,
-        )
+        See also :meth:`fetch_info`.
+        """
+        country = self._info.get('country')
+        if self.country_required:
+            return country or 'UNKNOWN_COUNTRY'
+        else:
+            return country or ''
 
-    def movie_year_validator(self, text):
-        # Raise ValueError if not a valid year
-        self.release_name.year = text
-        # release_name.year is now "UNKNOWN_YEAR" if year is required but not known
-        if self.release_name.year == 'UNKNOWN_YEAR':
-            raise ValueError('Failed to autodetect year')
-
-    def fill_in_movie_year(self, job_):
-        task = self.movie_year_job.fetch_text(
-            coro=self.get_movie_year(),
-            default_text=self.release_name.year,
-            finish_on_success=True,
-        )
-        self.movie_year_job.add_task(task)
+    @country.setter
+    def country(self, value):
+        if not value:
+            self._info['country'] = ''
+        else:
+            self._info['country'] = str(value)
 
-    @cached_property
-    def movie_resolution_job(self):
-        return self.make_choice_job(
-            name=self.get_job_name('movie-resolution'),
-            label='Resolution',
-            condition=self.make_job_condition('movie_resolution_job', release.ReleaseType.movie),
-            autodetected=self.release_info_resolution,
-            autofinish=True,
-            options=(
-                {'label': '4320p', 'value': '2160p', 'regex': re.compile(r'4320p')},
-                {'label': '2160p', 'value': '2160p', 'regex': re.compile(r'2160p')},
-                {'label': '1080p', 'value': '1080p', 'regex': re.compile(r'1080p')},
-                {'label': '1080i', 'value': '1080i', 'regex': re.compile(r'1080i')},
-                {'label': '720p', 'value': '720p', 'regex': re.compile(r'720p')},
-                {'label': '720i', 'value': '720i', 'regex': re.compile(r'720i')},
-                {'label': '576p', 'value': '480p', 'regex': re.compile(r'576p')},
-                {'label': '576i', 'value': '480i', 'regex': re.compile(r'576i')},
-                {'label': '540p', 'value': '480p', 'regex': re.compile(r'540p')},
-                {'label': '540i', 'value': '480i', 'regex': re.compile(r'540i')},
-                {'label': '480p', 'value': '480p', 'regex': re.compile(r'480p')},
-                {'label': '480i', 'value': '480i', 'regex': re.compile(r'480i')},
-                {'label': 'SD', 'value': 'SD', 'regex': re.compile(r'SD')},
-            ),
-        )
+    @property
+    def country_required(self):
+        """
+        Whether :attr:`title_with_aka_and_year` includes :attr:`country`
 
-    @cached_property
-    def movie_source_job(self):
-        return self.make_choice_job(
-            name=self.get_job_name('movie-source'),
-            label='Source',
-            condition=self.make_job_condition('movie_source_job', release.ReleaseType.movie),
-            autodetected=self.release_name.source,
-            autofinish=True,
-            options=(
-                {'label': 'BluRay', 'value': 'BluRay', 'regex': re.compile('BluRay')},  # [Hybrid] BluRay [Remux]
-                {'label': 'DVD5', 'value': 'DVD5', 'regex': re.compile('^DVD5$')},
-                {'label': 'DVD9', 'value': 'DVD9', 'regex': re.compile('^DVD9$')},
-                {'label': 'DVDRip', 'value': 'DVDRip', 'regex': re.compile('^DVDRip$')},
-                {'label': 'HD-DVD', 'value': 'HD-DVD', 'regex': re.compile('^HD-DVD$')},
-                {'label': 'HDTV', 'value': 'HDTV', 'regex': re.compile('^HDTV$')},
-                {'label': 'WEB-DL', 'value': 'WEB-DL', 'regex': re.compile('^WEB-DL$')},
-                {'label': 'WEBRip', 'value': 'WebRip', 'regex': re.compile('^WEBRip$')},
-                # I don't know if guessit supports these
-                {'label': 'BluRay 3D', 'value': 'BluRay 3D'},
-                {'label': 'BluRay RC', 'value': 'BluRay RC'},
-                {'label': 'CAM', 'value': 'CAM'},
-                {'label': 'DVDSCR', 'value': 'DVDSCR'},
-                {'label': 'HDRip', 'value': 'HDRip'},
-                {'label': 'PDTV', 'value': 'PDTV'},
-                {'label': 'R5', 'value': 'R5'},
-                {'label': 'SDTV', 'value': 'SDTV'},
-                {'label': 'TC', 'value': 'TC'},
-                {'label': 'TeleSync', 'value': 'TeleSync'},
-                {'label': 'VHSRip', 'value': 'VHSRip'},
-                {'label': 'VODRip', 'value': 'VODRip'},
-            ),
-        )
+        See also :meth:`fetch_info`.
+        """
+        return getattr(self, '_country_required', False)
 
-    @cached_property
-    def movie_audio_codec_job(self):
-        return self.make_choice_job(
-            name=self.get_job_name('movie-audio-codec'),
-            label='Audio Codec',
-            condition=self.make_job_condition('movie_audio_codec_job', release.ReleaseType.movie),
-            autodetected=self.release_info_audio_format,
-            autofinish=True,
-            options=(
-                {'label': 'AAC', 'value': 'AAC', 'regex': re.compile(r'^AAC$')},
-                {'label': 'AC-3', 'value': 'AC-3', 'regex': re.compile(r'^(?:E-|)AC-3$')},   # AC-3, E-AC-3
-                {'label': 'DTS', 'value': 'DTS', 'regex': re.compile(r'^DTS(?!-HD)')},       # DTS, DTS-ES
-                {'label': 'DTS-HD', 'value': 'DTS-HD', 'regex': re.compile(r'^DTS-HD\b')},   # DTS-HD, DTS-HD MA
-                {'label': 'DTS:X', 'value': 'DTS:X', 'regex': re.compile(r'^DTS:X$')},
-                {'label': 'Dolby Atmos', 'value': 'Dolby Atmos', 'regex': re.compile(r'Atmos')},
-                {'label': 'FLAC', 'value': 'FLAC', 'regex': re.compile(r'^FLAC$')},
-                {'label': 'MP3', 'value': 'MP3', 'regex': re.compile(r'^MP3$')},
-                # {'label': 'PCM', 'value': 'PCM', 'regex': re.compile(r'^$')},
-                {'label': 'TrueHD', 'value': 'True-HD', 'regex': re.compile(r'TrueHD')},
-                {'label': 'Vorbis', 'value': 'Vorbis', 'regex': re.compile(r'^Vorbis$')},
-            ),
-        )
+    @country_required.setter
+    def country_required(self, value):
+        self._country_required = bool(value)
 
-    @cached_property
-    def movie_video_codec_job(self):
-        return self.make_choice_job(
-            name=self.get_job_name('movie-video-codec'),
-            label='Video Codec',
-            condition=self.make_job_condition('movie_video_codec_job', release.ReleaseType.movie),
-            autodetected=self.release_name.video_format,
-            autofinish=True,
-            options=(
-                {'label': 'x264', 'value': 'x264', 'regex': re.compile(r'x264')},
-                {'label': 'x265', 'value': 'x265', 'regex': re.compile(r'x265')},
-                {'label': 'XviD', 'value': 'XVid', 'regex': re.compile(r'(?i:XviD)')},
-                # {'label': 'MPEG-2', 'value': 'MPEG-2', 'regex': re.compile(r'')},
-                # {'label': 'WMV-HD', 'value': 'WMV-HD', 'regex': re.compile(r'')},
-                # {'label': 'DivX', 'value': 'DivX', 'regex': re.compile(r'')},
-                {'label': 'H.264', 'value': 'H.264', 'regex': re.compile(r'H.264')},
-                {'label': 'H.265', 'value': 'H.265', 'regex': re.compile(r'H.265')},
-                # {'label': 'VC-1', 'value': 'VC-1', 'regex': re.compile(r'')},
-            ),
-        )
+    @_translated_property
+    def episodes(self):
+        """
+        Season and episodes in "S01E02"-style format or "UNKNOWN_SEASON" for season
+        packs, "UNKNOWN_EPISODE" for episodes, empty string for other types
 
-    @cached_property
-    def movie_container_job(self):
-        # Get file extension from largest file
-        files = sorted(fs.file_list(self.content_path), key=fs.file_size)
-        autodetected_extension = fs.file_extension(files[-1])
-        return self.make_choice_job(
-            name=self.get_job_name('movie-container'),
-            label='Container',
-            condition=self.make_job_condition('movie_container_job', release.ReleaseType.movie),
-            autodetected=autodetected_extension,
-            autofinish=True,
-            options=(
-                {'label': 'AVI', 'value': 'AVI', 'regex': re.compile(r'^(?i:avi)$')},
-                {'label': 'MKV', 'value': 'MKV', 'regex': re.compile('^(?i:mkv)$')},
-                {'label': 'MP4', 'value': 'MP4', 'regex': re.compile(r'^(?i:mp4)$')},
-                {'label': 'TS', 'value': 'TS', 'regex': re.compile(r'^(?i:ts)$')},
-                {'label': 'VOB', 'value': 'VOB', 'regex': re.compile(r'^(?i:vob)$')},
-                {'label': 'WMV', 'value': 'WMV', 'regex': re.compile(r'^(?i:wmv)$')},
-                {'label': 'm2ts', 'value': 'm2ts', 'regex': re.compile(r'^(?i:m2ts|mts)$')},
-            ),
-        )
+        This property can be set to one or more season numbers (:class:`str`,
+        :class:`int` or sequence of those), a "S01E02"-style string (see
+        :meth:`Episodes.from_string`) or any falsy value.
+        """
+        if self.type is ReleaseType.season:
+            return str(self._info.get('episodes') or 'UNKNOWN_SEASON')
+        elif self.type is ReleaseType.episode:
+            episodes = self._info.get('episodes', Episodes())
+            if not any(season for season in episodes.values()):
+                return 'UNKNOWN_EPISODE'
+            else:
+                return str(episodes)
+        elif self.type is ReleaseType.unknown:
+            return str(self._info.get('episodes') or '')
+        else:
+            return ''
 
-    @cached_property
-    def movie_release_info_job(self):
-        return jobs.dialog.TextFieldJob(
-            name=self.get_job_name('movie-release-info'),
-            label='Release Info',
-            condition=self.make_job_condition('movie_release_info_job', release.ReleaseType.movie),
-            text=self.get_movie_release_info(),
-            **self.common_job_args,
-        )
+    @episodes.setter
+    def episodes(self, value):
+        if isinstance(value, str) and Episodes.has_episodes_info(value):
+            self._info['episodes'] = Episodes.from_string(value)
+        elif not isinstance(value, str) and isinstance(value, collections.abc.Mapping):
+            self._info['episodes'] = Episodes(value)
+        elif not isinstance(value, str) and isinstance(value, collections.abc.Iterable):
+            self._info['episodes'] = Episodes({v: () for v in value})
+        elif value:
+            self._info['episodes'] = Episodes({value: ()})
+        else:
+            self._info['episodes'] = Episodes()
 
-    @cached_property
-    def movie_poster_job(self):
-        """Re-upload poster from IMDb to :attr:`~.TrackerJobsBase.image_host`"""
-        return jobs.custom.CustomJob(
-            name=self.get_job_name('movie-poster'),
-            label='Poster',
-            condition=self.make_job_condition('movie_poster_job', release.ReleaseType.movie),
-            worker=self.movie_get_poster_url,
-            catch=(errors.RequestError,),
-            **self.common_job_args,
-        )
+    @property
+    def episodes_dict(self):
+        """Episodes as :class:`Episodes` object"""
+        return self._info.get('episodes') or Episodes()
 
-    async def movie_get_poster_url(self, poster_job):
-        return await self.get_resized_poster_url(poster_job, self.get_movie_poster_url)
+    @property
+    def only_season(self):
+        """
+        Season if there is only one season in :attr:`episodes_dict`, `None`
+        otherwise
+        """
+        seasons = tuple(self.episodes_dict)
+        return seasons[0] if len(seasons) == 1 else None
 
-    @cached_property
-    def movie_tags_job(self):
-        self.imdb_job.signal.register('finished', self.fill_in_movie_tags)
-        return jobs.dialog.TextFieldJob(
-            name=self.get_job_name('movie-tags'),
-            label='Tags',
-            condition=self.make_job_condition('movie_tags_job', release.ReleaseType.movie),
-            validator=self.movie_tags_validator,
-            normalizer=self.normalize_tags,
-            **self.common_job_args,
-        )
+    @_translated_property
+    def episode_title(self):
+        """Episode title if :attr:`type` is "episode" or empty string"""
+        if self.type is ReleaseType.episode:
+            return self._info.get('episode_title') or ''
+        else:
+            return ''
 
-    def movie_tags_validator(self, text):
-        text = text.strip()
-        if not text:
-            raise ValueError('Failed to generate tags (use --tags)')
-
-    def fill_in_movie_tags(self, job_):
-        task = self.movie_tags_job.fetch_text(
-            coro=self.get_tags(),
-            finish_on_success=True,
-        )
-        self.movie_tags_job.add_task(task)
+    @episode_title.setter
+    def episode_title(self, value):
+        self._info['episode_title'] = str(value)
 
-    @cached_property
-    def movie_description_job(self):
-        self.imdb_job.signal.register('finished', self.fill_in_movie_description)
-        return jobs.dialog.TextFieldJob(
-            name=self.get_job_name('movie-description'),
-            label='Description',
-            condition=self.make_job_condition('movie_description_job', release.ReleaseType.movie),
-            validator=self.movie_description_validator,
-            **self.common_job_args,
-        )
+    @_translated_property
+    def date(self):
+        """
+        Date (YYYY-MM-DD)
 
-    def movie_description_validator(self, text):
-        text = text.strip()
-        if not text:
-            raise ValueError('Failed to generate description (use --description)')
-
-    def fill_in_movie_description(self, job_):
-        task = self.movie_description_job.fetch_text(
-            coro=self.get_description(),
-            finish_on_success=True,
-        )
-        self.movie_description_job.add_task(task)
+        Sometimes single episodes are not released as part of a season but with
+        an air date to identify them.
 
-    # Series jobs
+        For episodes, this should be the air date or an empty string.
 
-    @cached_property
-    def tvmaze_job(self):
-        """:class:`~.jobs.webdb.WebDbSearchJob` instance"""
-        tvmaze_job = super().tvmaze_job
-        tvmaze_job.condition = self.make_job_condition(
-            'tvmaze_job',
-            release.ReleaseType.season,
-            release.ReleaseType.episode,
-        )
-        tvmaze_job.no_id_ok = True
-        return tvmaze_job
+        For anything that isn't an episode, this is always an empty string.
+        """
+        if self.type is ReleaseType.episode:
+            return self._info.get('date') or ''
+        else:
+            return ''
 
-    @cached_property
-    def series_title_job(self):
-        self.tvmaze_job.signal.register('finished', self.fill_in_series_title)
-        return jobs.dialog.TextFieldJob(
-            name=self.get_job_name('series-title'),
-            label='Title',
-            condition=self.make_job_condition('series_title_job', release.ReleaseType.season, release.ReleaseType.episode),
-            validator=self.series_title_validator,
-            **self.common_job_args,
-        )
+    @date.setter
+    def date(self, value):
+        self._info['date'] = str(value)
+
+    @_translated_property
+    def service(self):
+        """Streaming service abbreviation (e.g. "AMZN", "NF") or empty string"""
+        return self._info.get('service') or ''
+
+    @service.setter
+    def service(self, value):
+        self._info['service'] = str(value)
 
-    def series_title_validator(self, text):
-        text = text.strip()
-        if not text:
-            raise ValueError('Failed to generate title')
-        unknown = ', '.join(u.lower() for u in re.findall(r'UNKNOWN_([A-Z_]+)', text))
-        if unknown:
-            raise ValueError(f'Failed to autodetect: {unknown}')
-
-    def fill_in_series_title(self, job_):
-        task = self.series_title_job.fetch_text(
-            coro=self.get_series_title_and_release_info(),
-            default_text=self.release_name.title_with_aka_and_year,
-            finish_on_success=False,
-        )
-        self.series_title_job.add_task(task)
+    @_translated_property
+    def edition(self):
+        """
+        List of "Director's Cut", "Uncut", "Unrated", etc
 
-    @cached_property
-    def series_poster_job(self):
-        """Re-upload poster from TVmaze to :attr:`~.TrackerJobsBase.image_host`"""
-        return jobs.custom.CustomJob(
-            name=self.get_job_name('series-poster'),
-            label='Poster',
-            condition=self.make_job_condition('series_poster_job', release.ReleaseType.season, release.ReleaseType.episode),
-            worker=self.series_get_poster_url,
-            catch=(errors.RequestError,),
-            **self.common_job_args,
-        )
+        :raise ContentError: if :attr:`path` exists but contains unexpected data
+        """
+        if 'edition' not in self._info:
+            self._info['edition'] = []
 
-    async def series_get_poster_url(self, poster_job):
-        return await self.get_resized_poster_url(poster_job, self.get_series_poster_url)
+        # Dual Audio
+        while 'Dual Audio' in self._info['edition']:
+            self._info['edition'].remove('Dual Audio')
+        if self.has_dual_audio:
+            self._info['edition'].append('Dual Audio')
+
+        return self._info['edition']
+
+    @edition.setter
+    def edition(self, value):
+        self._info['edition'] = [str(v) for v in value]
+
+    @_translated_property
+    def source(self):
+        '''Original source (e.g. "BluRay", "WEB-DL") or "UNKNOWN_SOURCE"'''
+        source = None
+
+        # DVD
+        video_ts_path = utils.fs.find_name('VIDEO_TS', self._path, validator=os.path.isdir)
+        if video_ts_path:
+            # Include VIDEO_TS siblings (e.g. "cover")
+            release_size = utils.fs.path_size(os.path.dirname(video_ts_path))
+            _log.debug('VIDEO_TS size: %r: %r', video_ts_path, release_size)
+            if release_size <= 4_700_000_000:
+                source = 'DVD5'
+            else:
+                source = 'DVD9'
 
-    @cached_property
-    def series_tags_job(self):
-        self.tvmaze_job.signal.register('finished', self.fill_in_series_tags)
-        return jobs.dialog.TextFieldJob(
-            name=self.get_job_name('series-tags'),
-            label='Tags',
-            condition=self.make_job_condition('series_tags_job', release.ReleaseType.season, release.ReleaseType.episode),
-            validator=self.series_tags_validator,
-            normalizer=self.normalize_tags,
-            **self.common_job_args,
-        )
+        if source is None:
+            # Blu-ray
+            bdmv_path = utils.fs.find_name('BDMV', self._path, validator=os.path.isdir)
+            if bdmv_path:
+                # Include BDMV siblings (e.g. "CERTIFICATE", and "ANY!")
+                release_size = utils.fs.path_size(os.path.dirname(bdmv_path))
+                _log.debug('Blu-ray size: %r: %r', bdmv_path, release_size)
+                if release_size <= 25e9:
+                    source = 'BD25'
+                elif release_size <= 50e9:
+                    source = 'BD50'
+                elif release_size <= 66e9:
+                    source = 'BD66'
+                else:
+                    source = 'BD100'
 
-    def series_tags_validator(self, text):
-        text = text.strip()
-        if not text:
-            raise ValueError('Failed to generate tags (use --tags)')
-
-    def fill_in_series_tags(self, job_):
-        task = self.series_tags_job.fetch_text(
-            coro=self.get_tags(),
-            finish_on_success=True,
-        )
-        self.series_tags_job.add_task(task)
+        if source is None:
+            source = self._info.get('source') or 'UNKNOWN_SOURCE'
 
-    @cached_property
-    def series_description_job(self):
-        self.tvmaze_job.signal.register('finished', self.fill_in_series_description)
-        return jobs.dialog.TextFieldJob(
-            name=self.get_job_name('series-description'),
-            label='Description',
-            condition=self.make_job_condition('series_description_job', release.ReleaseType.season, release.ReleaseType.episode),
-            validator=self.series_description_validator,
-            **self.common_job_args,
-        )
+        return source
 
-    def series_description_validator(self, text):
-        text = text.strip()
-        if not text:
-            raise ValueError('Failed to generate description (use --description)')
-
-    def fill_in_series_description(self, job_):
-        task = self.series_description_job.fetch_text(
-            coro=self.get_description(),
-            finish_on_success=True,
-        )
-        self.series_description_job.add_task(task)
+    @source.setter
+    def source(self, value):
+        self._info['source'] = str(value)
 
-    # Release Info
+    @_translated_property
+    def resolution(self):
+        """
+        Resolution (e.g. "1080p") or "UNKNOWN_RESOLUTION"
 
-    @property
-    def release_info_subtitles(self):
-        subtitle_tracks = video.tracks(self.content_path, default={}).get('Text', ())
-        if subtitle_tracks:
-            subtitle_languages = [track.get('Language') for track in subtitle_tracks]
-            if 'en' in subtitle_languages:
-                return 'w. Subtitles'
+        :raise ContentError: if :attr:`path` exists but contains unexpected data
+        """
+        res = video.resolution(self._path, default=None)
+        if res is None:
+            res = self._info.get('resolution') or 'UNKNOWN_RESOLUTION'
+        return res
+
+    @resolution.setter
+    def resolution(self, value):
+        self._info['resolution'] = str(value)
 
-    @property
-    def release_info_commentary(self):
-        if self.release_name.has_commentary:
-            return 'w. Commentary'
+    @_translated_property
+    def audio_format(self):
+        """
+        Audio format (e.g. "FLAC") or empty string (no audio track)
 
-    @property
-    def release_info_source(self):
-        if self.release_name.source == 'WEBRip':
-            return 'WebRip'
+        :raise ContentError: if :attr:`path` exists but contains unexpected data
+        """
+        af = video.audio_format(self._path, default=None)
+        if af is None:
+            af = self._info.get('audio_codec') or ''
+        return af
+
+    @audio_format.setter
+    def audio_format(self, value):
+        self._info['audio_codec'] = str(value)
+
+    @_translated_property
+    def audio_channels(self):
+        """
+        Audio channels (e.g. "5.1") or empty string (no audio track)
+
+        :raise ContentError: if :attr:`path` exists but contains unexpected data
+        """
+        ac = video.audio_channels(self._path, default=None)
+        if ac is None:
+            ac = self._info.get('audio_channels') or ''
+        return ac
+
+    @audio_channels.setter
+    def audio_channels(self, value):
+        self._info['audio_channels'] = str(value)
+
+    @_translated_property
+    def hdr_format(self):
+        """
+        HDR format name (e.g. "Dolby Vision" or "HDR10") or empty string
+
+        If not set explicitly and :attr:`path` exists, this value is
+        autodetected if possible, otherwise default to whatever
+        :class:`ReleaseInfo` detected in the release name.
+
+        Setting this value back to `None` turns on autodetection as described
+        above.
+
+        :raise ContentError: if :attr:`path` exists but contains unexpected data
+        """
+        # Use manually set value unless it is None
+        if getattr(self, '_hdr_format', None) is not None:
+            return self._hdr_format
+
+        # Autodetect from existing files
+        if os.path.exists(self._path):
+            hdr_format = video.hdr_format(self._path, default=None)
+            if hdr_format:
+                self._hdr_format = hdr_format
+                return self._hdr_format
+
+        # Autodetect from release name
+        guessed_hdr = self._info.get('hdr_format', '')
+        if guessed_hdr:
+            return guessed_hdr
+
+        # No HDR detected
+        return ''
+
+    @hdr_format.setter
+    def hdr_format(self, value):
+        if value is None:
+            # Turn on autodetection
+            self._hdr_format = None
+        elif value == '':
+            # No HDR
+            self._hdr_format = ''
+        elif value in video.hdr_formats:
+            self._hdr_format = value
         else:
-            return string.remove_suffix(self.release_name.source, 'Remux').strip()
+            raise ValueError(f'Unknown HDR format: {value!r}')
 
-    @property
-    def release_info_remux(self):
-        if 'Remux' in self.release_name.source:
-            return 'REMUX'
+    @_translated_property
+    def video_format(self):
+        """
+        Video format (or encoder in case of x264/x265/XviD) or "UNKNOWN_VIDEO_FORMAT"
+
+        :raise ContentError: if :attr:`path` exists but contains unexpected data
+        """
+        vf = video.video_format(self._path, default=None)
+        if vf is None:
+            vf = self._info.get('video_codec') or 'UNKNOWN_VIDEO_FORMAT'
+        return vf
+
+    @video_format.setter
+    def video_format(self, value):
+        self._info['video_codec'] = str(value)
+
+    @_translated_property
+    def group(self):
+        '''Name of release group or "NOGROUP"'''
+        return self._info.get('group') or 'NOGROUP'
+
+    @group.setter
+    def group(self, value):
+        self._info['group'] = str(value)
 
     @property
-    def release_info_resolution(self):
-        # Move/TV Rule 3.6.1 - Encodes with a stored resolution less than 700px
-        #                      AND a height less than 460px should be labelled
-        #                      "SD"
-        width = video.width(self.content_path, default=0)
-        height = video.height(self.content_path, default=0)
-        if 1 < width < 700 and 1 < height < 460:
-            return 'SD'
-
-        # Movie Rule 3.6.2 - 576p PAL encodes with a stored resolution of at
-        #                    least 700px wide and/or 560px tall should be
-        #                    labelled "480p" with "576p PAL" noted in the
-        #                    Release Info field
-        # We also apply this to series releases by using this property in
-        # get_series_title_and_release_info().
-        resolution = self.release_name.resolution
-        frame_rate = video.frame_rate(self.content_path, default=0)
-        if resolution == '576p' and frame_rate == 25:
-            return '576p PAL'
+    def has_commentary(self):
+        """
+        Whether this release has a commentary audio track
 
-        return self.release_name.resolution
+        If not set explicitly and `:attr:`path`` exists, this value is
+        autodetected by looking for "commentary" case-insensitively in any audio
+        track title.
 
-    @property
-    def release_info_576p_PAL(self):
-        """Return "576p PAL" if release is 576p and PAL or `None`"""
-        if self.release_info_resolution == '576p PAL':
-            return '576p PAL'
+        If not set explicitly and :attr:`path` does not exists, default to
+        detection by :class:`ReleaseInfo`.
 
-    @property
-    def release_info_proper(self):
-        if 'Proper' in self.release_name.edition:
-            return 'PROPER'
+        Setting this value back to `None` turns on autodetection as described
+        above.
 
-    @property
-    def release_info_repack(self):
-        if 'Repack' in self.release_name.edition:
-            return 'REPACK'
+        :raise ContentError: if :attr:`path` exists but contains unexpected data
+        """
+        # Use manually set value unless it is None
+        if getattr(self, '_has_commentary', None) is not None:
+            return self._has_commentary
+
+        # Find "Commentary" in audio track titles
+        elif os.path.exists(self._path):
+            self._has_commentary = bool(video.has_commentary(self._path))
+            return self._has_commentary
 
-    @property
-    def release_info_hdr_format(self):
-        hdr_format = video.hdr_format(self.content_path, default=None)
-        if hdr_format:
-            return hdr_format
+        # Default to ReleaseInfo['has_commentary']
+        else:
+            return self._info.get('has_commentary')
 
-    @property
-    def release_info_10bit(self):
-        if video.bit_depth(self.content_path, default=None) == 10:
-            return '10-bit'
+    @has_commentary.setter
+    def has_commentary(self, value):
+        if value is None:
+            self._has_commentary = None
+        else:
+            self._has_commentary = bool(value)
 
     @property
-    def release_info_dual_audio(self):
-        if video.has_dual_audio(self.content_path, default=False):
-            return 'Dual Audio'
+    def has_dual_audio(self):
+        """
+        Whether this release has an English and a non-English audio track
 
-    @property
-    def release_info_audio_format(self):
-        audio_format = self.release_name.audio_format
-        # "E-AC-3 Atmos" and "TrueHD Atmos" -> "Atmos"
-        if 'Atmos' in audio_format:
-            return 'Atmos'
-        return audio_format
+        If not set explicitly and :attr:`path` exists, this value is
+        autodetected if possible, otherwise default to whatever
+        :class:`ReleaseInfo` detected in the release name.
 
-    @property
-    def release_info_uncensored(self):
-        if 'Uncensored' in self.release_name.edition:
-            return 'Uncensored'
+        Setting this value back to `None` turns on autodetection as described
+        above.
 
-    @property
-    def release_info_uncut(self):
-        if 'Uncut' in self.release_name.edition:
-            return 'Uncut'
+        :raise ContentError: if :attr:`path` exists but contains unexpected data
+        """
+        # Use manually set value unless it is None
+        if getattr(self, '_has_dual_audio', None) is not None:
+            return self._has_dual_audio
+
+        # Autodetect dual audio
+        elif os.path.exists(self._path):
+            self._has_dual_audio = bool(video.has_dual_audio(self._path))
+            return self._has_dual_audio
 
-    @property
-    def release_info_unrated(self):
-        if 'Unrated' in self.release_name.edition:
-            return 'Unrated'
+        # Default to ReleaseInfo['edition']
+        else:
+            return 'Dual Audio' in self._info.get('edition', ())
 
-    @property
-    def release_info_remastered(self):
-        if '4k Remastered' in self.release_name.edition:
-            return '4k Remaster'
-        elif '4k Restored' in self.release_name.edition:
-            return '4k Restored'
-        elif 'Remastered' in self.release_name.edition:
-            return 'Remastered'
-        elif 'Restored' in self.release_name.edition:
-            return 'Restored'
+    @has_dual_audio.setter
+    def has_dual_audio(self, value):
+        if value is None:
+            self._has_dual_audio = None
+        else:
+            self._has_dual_audio = bool(value)
 
-    @property
-    def release_info_directors_cut(self):
-        if "Director's Cut" in self.release_name.edition:
-            return "Director's Cut"
+    _needed_attrs = {
+        ReleaseType.movie: ('title', 'year', 'resolution', 'source', 'video_format'),
+        ReleaseType.season: ('title', 'episodes', 'resolution', 'source', 'video_format'),
+        ReleaseType.episode: ('title', 'episodes', 'resolution', 'source', 'video_format'),
+    }
 
-    @property
-    def release_info_theatrical_cut(self):
-        if 'Theatrical Cut' in self.release_name.edition:
-            return 'Theatrical Cut'
+    @functools.cached_property
+    def dvd_encoding(self):
+        """"PAL", "NTSC" or `None`"""
+        if self.source in ('DVD', 'DVD5', 'DVD9', 'DVDRip'):
+            frame_rate = utils.video.frame_rate(self._path, default=0)
+            if frame_rate:
+                if frame_rate <= 25:
+                    return 'PAL'
+                elif frame_rate <= 30:
+                    return 'NTSC'
 
     @property
-    def release_info_imax(self):
-        if 'IMAX' in self.release_name.edition:
-            return 'IMAX'
+    def is_complete(self):
+        """
+        Whether all needed information is known and the string returned by
+        :meth:`format` will not contain "UNKNOWN_*"
 
-    @property
-    def release_info_extended_edition(self):
-        if 'Extended Cut' in self.release_name.edition:
-            return 'Extended Edition'
+        This always returns `False` if :attr:`type` is
+        :attr:`~.ReleaseType.unknown`.
+        """
+        if self.type is ReleaseType.unknown:
+            return False
+        for attr in self._needed_attrs[self.type]:
+            if self[attr].startswith('UNKNOWN_'):
+                return False
+        return True
 
-    @property
-    def release_info_anniversary_edition(self):
-        for name in fs.file_and_parent(self.content_path):
-            match = re.search(rf'(?i:{release.DELIM}(?:(\d+)th{release.DELIM}|)Anniversary{release.DELIM})', name)
-            if match:
-                if match.group(1):
-                    return f'{match.group(1)}th Anniversary Edition'
+    async def fetch_info(self, *, webdb, webdb_id, callback=None):
+        """
+        Fill in information web database
+
+        :param webdb: :class:`~.webdbs.base.WebDbApiBase` instance (see
+            :class:`~.webdbs.webdb`)
+        :param str webdb_id: Valid ID for `webdb`
+        :param callable callback: Function to call after info was fetched; gets
+            the instance (`self`) as a keyword argument
+
+        Attempt to set these attributes if they are supported by `webdb`:
+
+          - :attr:`title`
+          - :attr:`title_aka`
+          - :attr:`type`
+          - :attr:`year`
+          - :attr:`year_required` (IMDb only)
+          - :attr:`country`
+          - :attr:`country_required` (IMDb only)
+
+        :return: The method's instance (`self`) for convenience
+        """
+        await asyncio.gather(
+            self._update_attributes(webdb, webdb_id),
+            self._update_type(webdb, webdb_id),
+            self._update_country(webdb, webdb_id),
+            self._update_year_country_required(webdb, webdb_id),
+        )
+        _log.debug('Release name updated with %s info: %s', webdb.label, self)
+        if callback is not None:
+            callback(self)
+        return self
+
+    async def _update_attributes(self, webdb, webdb_id):
+        info = await webdb.gather(
+            webdb_id,
+            'title_english',
+            'title_original',
+            'year',
+        )
+        for attr, key in (
+            ('title', 'title_original'),
+            ('title_aka', 'title_english'),
+            ('year', 'year'),
+        ):
+            # Only overload non-empty values
+            if info[key]:
+                setattr(self, attr, info[key])
+
+    async def _update_type(self, webdb, webdb_id):
+        # Use type from database if possible. ReleaseInfo can misdetect (e.g. if
+        # mini-series doesn't contain "S01"). But if ReleaseInfo detected an
+        # episode (e.g. "S04E03"), it's unlikely to be wrong.
+        webdb_type = await webdb.type(webdb_id)
+        if webdb_type and self.type is not ReleaseType.episode:
+            self.type = webdb_type
+
+    async def _update_country(self, webdb, webdb_id):
+        try:
+            countries = await webdb.countries(webdb_id)
+        except NotImplementedError:
+            pass
+        else:
+            if countries:
+                self.country = utils.country.tld(countries[0]).upper()
+
+    async def _update_year_country_required(self, webdb, webdb_id):
+        if self.type in (ReleaseType.season, ReleaseType.episode):
+            # Find out if there are any TV show name duplicates. If so, require
+            # year and/or country code in release name to pin it down.
+
+            @functools.lru_cache(maxsize=None)
+            def normalize_title(title):
+                return unidecode.unidecode(title.casefold())
+
+            # Find result with the same title, removing any "smart" matches
+            query = utils.webdbs.Query(title=self.title, type=ReleaseType.series)
+            results = [
+                {
+                    'title': normalize_title(result.title),
+                    'year': result.year,
+                    'countries': await result.countries(),
+                }
+                for result in await webdb.search(query)
+                if normalize_title(self.title) == normalize_title(result.title)
+            ]
+
+            # Assemble relevant info
+            info = {
+                'title': normalize_title(self.title),
+                'year': await webdb.year(webdb_id),
+                'countries': await webdb.countries(webdb_id),
+            }
+
+            def has_duplicates(*attributes):
+                combinations = [
+                    combine(result, attributes)
+                    for result in results
+                ]
+                relevant_info = {attr: info[attr] for attr in attributes}
+                return combinations.count(relevant_info) >= 2
+
+            def combine(result, attributes):
+                combined = {}
+                for attr in attributes:
+                    if result.get(attr):
+                        combined[attr] = result[attr]
+                return combined
+
+            if has_duplicates('title'):
+                if not has_duplicates('title', 'year'):
+                    self.year_required = True
+                elif not has_duplicates('title', 'countries'):
+                    self.country_required = True
                 else:
-                    return 'Anniversary Edition'
+                    self.year_required = True
+                    self.country_required = True
 
-    @property
-    def release_info_criterion_edition(self):
-        if 'Criterion Collection' in self.release_name.edition:
-            return 'Criterion Edition'
+    def format(self, separator=None):
+        """
+        Assemble all parts into string
 
-    @property
-    def release_info_special_edition(self):
-        if 'Special Edition' in self.release_name.edition:
-            return 'Special Edition'
+        :param separator: Separator to use instead of space
 
-    @property
-    def release_info_limited_edition(self):
-        if 'Limited' in self.release_name.edition:
-            return 'Limited'
+            The typical use case would be ``.``.
+        """
+        parts = [self.title_with_aka_and_year]
 
-    @property
-    def release_info_2in1(self):
-        if '2in1' in self.release_name.edition:
-            return '2in1'
-
-    # Metadata generators
-
-    async def get_movie_title(self):
-        imdb_id = await self.get_imdb_id()
-        if imdb_id:
-            await self.release_name.fetch_info(imdb_id=imdb_id)
-            return self.release_name.title_with_aka
-
-    async def get_movie_year(self):
-        imdb_id = await self.get_imdb_id()
-        if imdb_id:
-            await self.release_name.fetch_info(imdb_id=imdb_id)
-            return self.release_name.year
-
-    async def get_series_title_and_release_info(self):
-        imdb_id = await self.get_imdb_id()
-        if imdb_id:
-            await self.release_name.fetch_info(imdb_id=imdb_id)
-
-        title = [self.release_name.title_with_aka]
-        if self.release_name.year_required:
-            title.append(f'({self.release_name.year})')
-
-        # "Season x"
-        if self.is_season_release:
-            title.append(f'- Season {self.season or "UNKNOWN_SEASON"}')
-
-        # "SxxEyy"
-        elif self.is_episode_release:
-            title.append(str(self.release_name.episodes))
-
-        info = [
-            # [Source / VideoCodec / AudioCodec / Container / Resolution]
-            self.release_info_source,
-            self.release_name.video_format,
-            self.release_info_audio_format,
-            fs.file_extension(video.first_video(self.content_path)).upper(),
-            self.release_info_resolution,
-
-            # Scene tags
-            self.release_info_proper,
-            self.release_info_repack,
-
-            # Special formats
-            self.release_info_remux,
-            self.release_info_10bit,
-            self.release_info_hdr_format,
-
-            # Editions
-            self.release_info_uncensored,
-            self.release_info_uncut,
-            self.release_info_unrated,
-            self.release_info_remastered,
-            self.release_info_directors_cut,
-            self.release_info_theatrical_cut,
-            self.release_info_imax,
-            self.release_info_extended_edition,
-            self.release_info_anniversary_edition,
-            self.release_info_criterion_edition,
-            self.release_info_special_edition,
-            self.release_info_limited_edition,
-            self.release_info_2in1,
-
-            # Features
-            self.release_info_dual_audio,
-            self.release_info_commentary,
-            self.release_info_subtitles,
-        ]
-        info_string = ' / '.join(i for i in info if i)
-        return ' '.join(title) + f' [{info_string}]'
-
-    async def get_resized_poster_url(self, poster_job, poster_url_getter):
-        poster_path = await self.get_poster_file(poster_job, poster_url_getter)
-        if not poster_path:
-            self.error('Provide a poster file or URL with the --poster option.')
+        if self.type in (ReleaseType.season, ReleaseType.episode) and not self.date:
+            parts.append(str(self.episodes))
+
+        if self.edition:
+            parts.append(' '.join(self.edition))
+
+        if self.dvd_encoding:
+            parts.append(self.dvd_encoding)
         else:
-            # Resize poster
+            parts.append(self.resolution)
+
+        if self.service:
+            parts.append(self.service)
+
+        parts.append(self.source)
+
+        if self.audio_format:
+            parts.append(self.audio_format)
+
+        if self.audio_channels:
+            parts.append(self.audio_channels)
+
+        if self.hdr_format:
+            parts.append(self.hdr_format)
+
+        parts.append(self.video_format)
+
+        joined = ' '.join(parts) + f'-{self.group}'
+
+        # Separator (usually " " or ".")
+        sep = separator if separator is not None else self.separator
+        if sep != ' ':
+            joined = joined.replace(' ', sep)
+
+        if sep == '.':
+            # Replace "&" with "and" before "&" gets removed
+            joined = re.sub(r'&', 'and', joined)
+            # Remove non-word characters like (e.g.: ,:) with some exceptions
+            joined = re.sub(r'[^ \w\.-]', '', joined)
+            # Deduplicate "."
+            joined = re.sub(r'\.+', '.', joined)
+
+        return joined
+
+
+class ReleaseInfo(collections.abc.MutableMapping):
+    """
+    Parse information from release name or path
+
+    .. note::
+
+       Consider using :class:`~.ReleaseName` instead to get more accurate info
+       from the data of existing files.
+
+    :param str release: Release name or path to release content
+
+    :param bool strict: Whether to raise :class:`~.errors.ContentError` if
+        `release` looks bad, e.g. an abbreviated scene release file name like
+        "tf-foof.mkv"
+
+    If `release` looks like an abbreviated scene file name (e.g.
+    "abd-mother.mkv"), the parent directory's name is used if possible.
+
+    Gathered information is provided as a dictionary with the following keys:
+
+      - ``type`` (:class:`~.types.ReleaseType` enum)
+      - ``title``
+      - ``aka`` (Also Known As; anything after "AKA" in the title)
+      - ``country``
+      - ``year``
+      - ``episodes`` (:class:`~.Episodes` instance)
+      - ``episode_title``
+      - ``date``
+      - ``edition`` (:class:`list` of "Extended", "Uncut", etc)
+      - ``resolution``
+      - ``service`` (Streaming service abbreviation)
+      - ``source`` ("BluRay", "WEB-DL", etc)
+      - ``audio_codec`` (Audio codec abbreviation)
+      - ``audio_channels`` (e.g. "2.0" or "7.1")
+      - ``hdr_format``
+      - ``video_codec``
+      - ``group``
+      - ``has_commentary`` (:class:`bool` or `None` to autodetect)
+
+    Unless documented otherwise above, all values are strings. Unknown values
+    are empty strings.
+    """
+
+    def __init__(self, path, strict=False):
+        if strict:
             try:
-                resized_poster_path = image.resize(
-                    image_file=poster_path,
-                    target_directory=poster_job.home_directory,
-                    width=300,
-                )
-            except errors.ImageResizeError as e:
-                self.error(f'Poster resizing failed: {e}')
-            else:
-                _log.debug('Poster resized: %r', resized_poster_path)
-                # Upload poster to self.image_host
-                poster_job.info = f'Uploading poster to {self.image_host.name}'
-                try:
-                    return await self.image_host.upload(resized_poster_path)
-                except errors.RequestError as e:
-                    self.error(f'Poster upload failed: {e}')
-                finally:
-                    poster_job.info = ''
-
-    async def get_poster_file(self, poster_job, poster_url_getter):
-        if self.options.get('poster'):
-            # Get custom poster from user (e.g. CLI argument)
-            if re.search(r'^[a-z]+://', self.options['poster']):
-                # Poster argument is URL
-                poster_url = self.options['poster']
-            else:
-                # Poster is file path
-                return self.options['poster']
+                utils.predbs.assert_not_abbreviated_filename(str(path))
+            except errors.SceneAbbreviatedFilenameError as e:
+                raise errors.ContentError(e)
+        self._path = str(path)
+        self._abspath = os.path.abspath(self._path)
+        self._dict = {}
+
+    def __contains__(self, name):
+        return hasattr(self, f'_get_{name}')
+
+    def __getitem__(self, name):
+        if name not in self:
+            raise KeyError(name)
         else:
-            # Get poster URL from webdb
-            poster_url = await poster_url_getter()
+            value = self._dict.get(name, None)
+            if value is None:
+                value = self[name] = getattr(self, f'_get_{name}')()
+            return value
+
+    def __setitem__(self, name, value):
+        if not hasattr(self, f'_get_{name}'):
+            raise KeyError(name)
+        elif hasattr(self, f'_set_{name}'):
+            self._dict[name] = getattr(self, f'_set_{name}')(value)
+        else:
+            self._dict[name] = value
 
-        if not poster_url:
-            self.error('Failed to find poster URL (use --poster)')
+    def __delitem__(self, name):
+        if not hasattr(self, f'_get_{name}'):
+            raise KeyError(name)
+        elif name in self._dict:
+            del self._dict[name]
+
+    def __iter__(self):
+        return iter(name[5:] for name in dir(type(self))
+                    if name.startswith('_get_'))
+
+    def __len__(self):
+        return len(tuple(name[5:] for name in dir(type(self))
+                         if name.startswith('_get_')))
+
+    def __repr__(self):
+        return f'{type(self).__name__}({self._path!r})'
+
+    def copy(self):
+        """Return instance copy"""
+        cp = type(self)(self._path)
+        cp._dict = copy.deepcopy(self._dict)
+        return cp
+
+    @property
+    def path(self):
+        """`path` argument as :class:`str`"""
+        return self._path
+
+    @functools.cached_property
+    def _guess(self):
+        path = self._abspath
+
+        # _log.debug('Running guessit on %r with %r', path, constants.GUESSIT_OPTIONS)
+        guess = dict(_guessit.default_api.guessit(path, options=constants.GUESSIT_OPTIONS))
+        # _log.debug('Original guess: %r', guess)
+
+        # We try to do our own episode parsing to preserve order and support
+        # multiple seasons and episodes
+        for name in fs.file_and_parent(path):
+            if Episodes.has_episodes_info(name):
+                guess['episodes'] = Episodes.from_string(name)
+                break
         else:
-            # Download poster
-            poster_job.info = f'Downloading poster: {poster_url}'
-            poster_path = os.path.join(poster_job.home_directory, 'poster.bb.jpg')
-            try:
-                await http.download(poster_url, poster_path)
-            except errors.RequestError as e:
-                self.error(f'Poster download failed: {e}')
+            # Guessit can parse multiple seasons/episodes to some degree
+            seasons = _as_list(guess.get('season'))
+            episodes = _as_list(guess.get('episode'))
+            string = []
+            if seasons:
+                string.append(f'S{seasons[0]:02d}')
+            for e in episodes:
+                string.append(f'E{e:02d}')
+            guess['episodes'] = Episodes.from_string(''.join(string))
+
+        # If we got an abbreviated file name (e.g. "group-titles01e02.mkv"),
+        # guessit can't handle it. Try to find episode information in it.
+        if guess['episodes']:
+            episodes_string = str(guess['episodes'])
+            if (
+                'S' in episodes_string
+                and 'E' not in episodes_string
+                and utils.predbs.is_abbreviated_filename(path)
+            ):
+                filename = fs.basename(path)
+                match = re.search(r'((?i:[SE]\d+)+)', filename)
+                if match:
+                    episodes = Episodes.from_string(match.group(1))
+                    guess['episodes'].update(episodes)
+                    _log.debug('Found episodes in abbreviated file name: %r: %r', filename, guess['episodes'])
+
+        return guess
+
+    @property
+    def _guessit_options(self):
+        return _guessit.default_api.advanced_config
+
+    def _get_type(self):
+        if self['date']:
+            # We interpret a date as an air date, which should mean it's an
+            # episode.
+            return ReleaseType.episode
+
+        elif self['episodes']:
+            # guessit doesn't differentiate between episodes and season packs.
+            # Does any season specify an episode?
+            if any(episodes for episodes in self['episodes'].values()):
+                return ReleaseType.episode
+            # No single episode means it's one or more season packs.
             else:
-                return poster_path
+                return ReleaseType.season
+        else:
+            return ReleaseType.movie
 
-    async def get_movie_poster_url(self):
-        imdb_id = await self.get_imdb_id()
-        if imdb_id:
-            poster_url = await self.imdb.poster_url(imdb_id)
-            _log.debug('Poster URL for %r: %r', imdb_id, poster_url)
-            return poster_url
-
-    async def get_series_poster_url(self):
-        tvmaze_id = await self.get_tvmaze_id()
-        if tvmaze_id:
-            poster_url = await self.tvmaze.poster_url(tvmaze_id, season=self.season)
-            _log.debug('Poster URL for %r: %r', tvmaze_id, poster_url)
-            return poster_url
-
-    def get_movie_release_info(self):
-        info = (
-            # Scene tags
-            self.release_info_proper,
-            self.release_info_repack,
-
-            # Special formats
-            self.release_info_remux,
-            self.release_info_576p_PAL,
-            self.release_info_10bit,
-            self.release_info_hdr_format,
-
-            # Editions
-            self.release_info_uncensored,
-            self.release_info_uncut,
-            self.release_info_unrated,
-            self.release_info_remastered,
-            self.release_info_directors_cut,
-            self.release_info_theatrical_cut,
-            self.release_info_imax,
-            self.release_info_extended_edition,
-            self.release_info_anniversary_edition,
-            self.release_info_criterion_edition,
-            self.release_info_special_edition,
-            self.release_info_limited_edition,
-            self.release_info_2in1,
-
-            # Features
-            self.release_info_dual_audio,
-            self.release_info_commentary,
-            self.release_info_subtitles,
-        )
-        return ' / '.join(i for i in info if i)
+    _title_split_regex = re.compile(
+        r'[ \.](?:'
+        r'\d{4}|'  # Year
+        r'(?i:[SE]\d+)+|'  # Sxx or SxxExx
+        r'((?i:Season|Episode)[ \.]*\d+[ \.]*)+|'
+        r')[ \.]'
+    )
 
-    async def get_tags(self):
-        if self.options.get('tags', ()):
-            # Get custom tags from user (e.g. CLI argument)
-            tags_list = self.options['tags'].split(',')
+    @functools.cached_property
+    def release_name_params(self):
+        """
+        Release name without title and year or season/episode info
 
+        This allows us to find stuff in the release name that guessit doesn't
+        support without accidentally finding it in the title.
+        """
+        path_no_ext = fs.strip_extension(self._abspath, only=constants.VIDEO_FILE_EXTENSIONS)
+
+        # Look for year/season/episode info in file and parent directory name
+        for name in fs.file_and_parent(path_no_ext):
+            match = self._title_split_regex.search(name)
+            if match:
+                return self._title_split_regex.split(name, maxsplit=1)[-1]
+
+        # Default to the file/parent that contains either " " or "." (without
+        # the "." from the extension)
+        for name in fs.file_and_parent(path_no_ext):
+            if ' ' in name or '.' in name:
+                return name
+
+        # Default to file name
+        return fs.basename(path_no_ext)
+
+    _title_aka_regex = re.compile(rf'{DELIM}AKA{DELIM}')
+
+    @functools.cached_property
+    def _title_parts(self):
+        # guessit splits AKA at " - ", so we re-join it
+        title_parts = [_as_string(self._guess.get('title', ''))]
+        if self._guess.get('alternative_title'):
+            title_parts.extend(_as_list(self._guess.get('alternative_title')))
+        title = ' - '.join(title_parts)
+        title_parts = self._title_aka_regex.split(title, maxsplit=1)
+
+        # guessit recognizes mixed seasons and episodes (e.g. "S02E10S03E05") as
+        # part of the title.
+        def remove_episodes(string):
+            return Episodes.regex.sub('', string)
+
+        if len(title_parts) > 1:
+            return {'title': remove_episodes(title_parts[0]),
+                    'aka': remove_episodes(title_parts[1])}
         else:
-            # Get custom tags from webdb
+            return {'title': remove_episodes(title_parts[0]),
+                    'aka': ''}
 
-            # For movies, TVmaze ID is None and tvmaze is ignored.
-            # For series, IMDb might have information TVmaze is missing.
-            webdbs = (self.tvmaze, self.imdb)
+    def _get_title(self):
+        return self._title_parts['title']
 
-            # Gather tags
-            tags_list = list(await self.try_webdbs(webdbs, 'genres', default=()))
-            if self.is_movie_release:
-                tags_list.extend(await self.try_webdbs(webdbs, 'directors', default=()))
-            elif self.is_series_release:
-                tags_list.extend(await self.try_webdbs(webdbs, 'creators', default=()))
-            tags_list.extend(await self.try_webdbs(webdbs, 'cast', default=()))
+    def _get_aka(self):
+        return self._title_parts['aka']
 
-        return self.normalize_tags(tags_list)
+    def _get_year(self):
+        return _as_string(self._guess.get('year') or '')
 
-    _tags_translation = {
-        re.compile('^sci.?fi$'): 'science.fiction',
+    _country_translation = {
+        'UK': re.compile(r'^GB$'),
     }
 
-    def normalize_tags(self, tags):
-        if isinstance(tags, str):
-            tags = tags.split(',')
-
-        allowed_characters = (
-            string.group('ascii_lowercase')
-            + string.group('digits')
-            + '.'
-        )
+    def _get_country(self):
+        country = utils.country.tld(
+            _as_string(self._guess.get('country') or '')
+        ).upper()
+        for country_, regex in self._country_translation.items():
+            if regex.search(country):
+                country = country_
+        return country
+
+    def _get_episodes(self):
+        if 'episodes' not in self._guess:
+            self._guess['episodes'] = Episodes()
+        return self._guess['episodes']
+
+    def _set_episodes(self, value):
+        # Keep Episodes() object ID. Ensure `value` is not the object in
+        # self._guess['episodes'] so we can clear() without losing items in
+        # `value`.
+        value = dict(value)
+        episodes = self._get_episodes()
+        episodes.clear()
+        episodes.update(value)
+
+    def _get_episode_title(self):
+        return _as_string(self._guess.get('episode_title', ''))
+
+    _edition_translation = {
+        "Collector's Edition": re.compile(r'Collector'),
+        'Criterion Collection': re.compile(r'Criterion'),
+        'Deluxe Edition': re.compile(r'Deluxe'),
+        'Extended Cut': re.compile(r'Extended'),
+        'Special Edition': re.compile(r'Special'),
+        'Theatrical Cut': re.compile(r'Theatrical'),
+        'Ultimate Cut': re.compile(r'Ultimate'),
+    }
+    _proper_repack_regex = re.compile(rf'(?:{DELIM}|^)((?i:proper|repack\d*))(?:{DELIM}|$)')
+    _remastered_regex = re.compile(rf'(?:{DELIM}|^)((?i:4k{DELIM}+|)(?i:remaster(?:ed|)|restored))(?:{DELIM}|$)')
 
-        # Replace spaces, non-ASCII characters, etc
-        normalized = []
-        for tag in tags:
-            tag = (
-                str(tag)
-                .strip()
-                .lower()
-                .replace(' ', '.')
-                .replace('-', '.')
-                .replace("'", '')
-            )
-            tag = re.sub(r'\.+', '.', tag)  # Dedup "."
-            tag = unidecode.unidecode(tag)  # Translate exotic characters to ASCII
-            tag = ''.join(c for c in tag    # Remove remaining non-ASCII characters
-                          if c in allowed_characters)
-            for regex, replacement in self._tags_translation.items():
-                if regex.search(tag):
-                    tag = replacement
-                    break
-            tag = tag.strip(',.')           # Remove leading/trailing tag/space separators
-            normalized.append(tag)
+    def _get_date(self):
+        return _as_string(self._guess.get('date', ''))
 
-        def join_tags(tags):
-            return ','.join(str(tag) for tag in tags if tag)
+    def _get_edition(self):
+        edition = _as_list(self._guess.get('edition'))
+        for edition_fixed, regex in self._edition_translation.items():
+            for i in range(len(edition)):
+                if regex.search(edition[i]):
+                    edition[i] = edition_fixed
 
-        # Maximum length of concatenated tags is 200 characters
-        tags_string = join_tags(normalized)
-        while len(tags_string) > 200:
-            del normalized[-1]
-            tags_string = join_tags(normalized)
+        # Revision (guessit doesn't distinguish between REPACK, PROPER, etc)
+        match = self._proper_repack_regex.search(self.release_name_params)
+        if match:
+            edition.append(match.group(1).upper())
 
-        return tags_string
+        # Various
+        guessit_other = _as_list(self._guess.get('other'))
+        if 'Open Matte' in guessit_other:
+            edition.append('Open Matte')
+        if 'Original Aspect Ratio' in guessit_other:
+            edition.append('OAR')
+        if 'Dual Audio' in guessit_other:
+            edition.append('Dual Audio')
+        if '2in1' in guessit_other:
+            edition.append('2in1')
+
+        def is_4k_source():
+            # guessit only detects remastered, not if it's from 4k
+            match = self._remastered_regex.search(self.release_name_params)
+            if match:
+                remastered_string = match.group(1)
+                return '4k' in remastered_string.lower()
 
-    async def get_description(self):
-        parts = []
+        if 'Remastered' in edition and is_4k_source():
+            edition[edition.index('Remastered')] = '4k Remastered'
+        elif 'Restored' in edition and is_4k_source():
+            edition[edition.index('Restored')] = '4k Restored'
+
+        return edition
+
+    def _get_resolution(self):
+        return _as_string(self._guess.get('screen_size', ''))
+
+    _streaming_service_regex = re.compile(rf'{DELIM}([A-Z]+){DELIM}(?i:WEB-?(?:DL|Rip))(?:{DELIM}|$)')
+    _streaming_service_translation = {
+        re.compile(r'(?i:IT)'): 'iT',
+        re.compile(r'(?i:4OD)'): 'ALL4',   # 4oD is old name of Channel 4's VOD service
+        # Not a streaming service
+        re.compile(r'OAR'): '',  # Original Aspect Ratio
+    }
 
-        if self.options.get('description', ''):
-            # Custom description
-            if os.path.exists(self.options['description']):
-                try:
-                    with open(self.options['description'], mode='r', encoding='utf-8') as f:
-                        parts.append(f.read())
-                except OSError as e:
-                    msg = e.strerror if e.strerror else str(e)
-                    self.error(f'Failed to read {self.options["description"]}: {msg}')
-                    return ''
-            else:
-                parts.append(self.options['description'])
+    def _get_service(self):
+        def translate(service):
+            for regex, abbrev in self._streaming_service_translation.items():
+                if regex.search(service):
+                    return abbrev
+            return service
+
+        service = _as_string(self._guess.get('streaming_service', ''))
+        if service:
+            # guessit translates abbreviations to full names (NF -> Netflix),
+            # but we want abbreviations. Use the same dictionary as guessit.
+            translation = self._guessit_options['streaming_service']
+            for full_name, aliases in translation.items():
+                if service.casefold().strip() == full_name.casefold().strip():
+                    # `aliases` is either a string or a list of strings and
+                    # other objects.
+                    if isinstance(aliases, str):
+                        return translate(aliases)
+                    else:
+                        # Find shortest string
+                        aliases = (a for a in aliases if isinstance(a, str))
+                        return translate(sorted(aliases, key=len)[0])
 
-        else:
-            async def extend_parts(*coros, sep='', fmt='{text}'):
-                info_table = await asyncio.gather(*coros)
-                text = sep.join(
-                    str(item) for item in info_table
-                    if item is not None
-                )
-                if text:
-                    parts.append(fmt.format(text=text))
-
-            # Summary
-            await extend_parts(self.format_description_summary())
-
-            # Table-like quote block with details
-            await extend_parts(
-                self.format_description_webdbs(),
-                self.format_description_year(),
-                self.format_description_status(),
-                self.format_description_countries(),
-                self.format_description_runtime(),
-                self.format_description_directors(),
-                self.format_description_creators(),
-                self.format_description_cast(),
-                sep='\n',
-                fmt='[quote]{text}[/quote]',
-            )
-
-            # Season and episode description also contains screenshots and
-            # mediainfo
-            if self.is_series_release:
-                await extend_parts(
-                    self.format_description_series_screenshots(),
-                    self.format_description_series_mediainfo(),
-                )
-
-        return ''.join(parts).strip()
-
-    async def format_description_summary(self):
-        summary = await self.try_webdbs((self.tvmaze, self.imdb), 'summary', default='')
-        if summary:
-            summary = '[quote]' + summary
-            if self.is_episode_release and self.season and self.episode:
-                ep_summary = await self.format_description_episode_summary()
-                if ep_summary:
-                    summary += f'\n\n{ep_summary}'
-            summary += '[/quote]'
-            return summary
-
-    async def format_description_episode_summary(self):
-        tvmaze_id = await self.get_tvmaze_id()
-        if tvmaze_id:
-            try:
-                episode = await self.tvmaze.episode(
-                    id=tvmaze_id,
-                    season=self.season,
-                    episode=self.episode,
-                )
-            except errors.RequestError:
-                pass
-            else:
-                summary = (
-                    f'[url={episode["url"]}]{episode["title"]}[/url]',
-                    ' - ',
-                    f'Season {episode["season"]}, Episode {episode["episode"]}',
-                    f' - [size=2]{episode["date"]}[/size]' if episode.get('date') else '',
-                    f'\n\n[spoiler]\n{episode["summary"]}[/spoiler]' if episode.get('summary') else '',
-                )
-                return ''.join(summary)
+        # Default to manual detection
+        match = self._streaming_service_regex.search(self.release_name_params)
+        if match:
+            return translate(match.group(1))
 
-    async def format_description_webdbs(self):
-        parts = []
+        return ''
 
-        async def append_line(webdb, id):
-            url = await webdb.url(id)
-            line = [f'[b]{webdb.label}[/b]: [url={url}]{id}[/url]']
-            rating = await webdb.rating(id)
-            if rating:
-                rating_stars = ''.join((
-                    '[color=#ffff00]',
-                    string.star_rating(rating, max_rating=webdb.rating_max),
-                    '[/color]',
-                ))
-                line.append(f'{rating}/{int(webdb.rating_max)} {rating_stars}')
-            parts.append(' | '.join(line))
-
-        imdb_id = await self.get_imdb_id()
-        if imdb_id:
-            await append_line(self.imdb, imdb_id)
-
-        tvmaze_id = await self.get_tvmaze_id()
-        if tvmaze_id:
-            await append_line(self.tvmaze, tvmaze_id)
+    _source_translation = {
+        re.compile(r'(?i:ultra hd blu-?ray)') : 'UHD BluRay',
+        re.compile(r'(?i:blu-?ray)')          : 'BluRay',
+        re.compile(r'(?i:dvd-?rip)')          : 'DVDRip',
+        re.compile(r'(?i:tv-?rip)')           : 'TVRip',
+        re.compile(r'(?i:web-?dl)')           : 'WEB-DL',
+        re.compile(r'(?i:web-?rip)')          : 'WEBRip',
+        re.compile(r'(?i:web)')               : 'WEB-DL',
+    }
+    _web_source_regex = re.compile(rf'{DELIM}(WEB-?(?:DL|Rip))(?:{DELIM}|$)', flags=re.IGNORECASE)
 
-        return '\n'.join(parts)
+    def _get_source(self):
+        source = self._guess.get('source', '')
 
-    async def format_description_year(self):
-        year = None
-        try:
-            if self.is_movie_release:
-                imdb_id = await self.get_imdb_id()
-                if imdb_id:
-                    year = await self.imdb.year(imdb_id)
-
-            elif self.is_series_release:
-                tvmaze_id = await self.get_tvmaze_id()
-                if tvmaze_id:
-                    if self.season:
-                        episode = await self.tvmaze.episode(id=tvmaze_id, season=self.season, episode=1)
-                        if episode.get('date'):
-                            year = episode['date'].split('-')[0]
-                    if not year:
-                        year = await self.tvmaze.year(tvmaze_id)
-        except errors.RequestError:
-            pass
-        else:
-            if year:
-                return f'[b]Year[/b]: {year}'
+        # guessit parses multiple source (e.g. ["WEB", "Blu-ray"]) if it can
+        # find them. This is an issue if an episode title contains a "source",
+        # e.g. "TC" -> "Telecine".
+        if not isinstance(source, str):
+            source = source[0]
+
+        if source.lower() == 'web':
+            # guessit doesn't distinguish between WEB-DL and WEBRip. Get the
+            # source from the path.
+            match = self._web_source_regex.search(self.release_name_params)
+            if match:
+                source = match.group(1)
 
-    async def format_description_status(self):
-        tvmaze_id = await self.get_tvmaze_id()
-        if tvmaze_id:
-            status = await self.tvmaze.status(tvmaze_id)
-            if status == 'Ended':
-                return f'[b]Status[/b]: {status}'
-
-    async def format_description_countries(self):
-        countries = await self.try_webdbs((self.tvmaze, self.imdb), 'countries', default=())
-        if countries:
-            return (f'[b]Countr{"ies" if len(countries) > 1 else "y"}[/b]: '
-                    + ', '.join(countries))
-
-    async def format_description_runtime(self):
-        def format_runtime(minutes):
-            if minutes > 60:
-                hours = minutes // 60
-                minutes = minutes - ((minutes // 60) * 60)
-                if minutes:
-                    return f'{hours}h{minutes}m'
-                else:
-                    return f'{hours}h'
+        elif 'Rip' in self._guess.get('other', ()):
+            source = f'{source}Rip'
+
+        elif 'DVD9' in self.release_name_params:
+            source = 'DVD9'
+        elif 'DVD5' in self.release_name_params:
+            source = 'DVD5'
+
+        if source:
+            # Fix spelling
+            for regex,source_fixed in self._source_translation.items():
+                if regex.search(source):
+                    source = source_fixed
+                    break
+
+        # Detect Remux and Hybrid
+        other = self._guess.get('other', ())
+        if 'Remux' in other and 'WEB' not in source and 'Rip' not in source:
+            source += ' Remux'
+        if 'Hybrid' in other:
+            source = 'Hybrid ' + source
+
+        return source
+
+    _audio_codec_translation = {
+        re.compile(r'^AC-?3')             : 'DD',
+        re.compile(r'Dolby Digital$')     : 'DD',
+        re.compile(r'^E-?AC-?3')          : 'DDP',
+        re.compile(r'Dolby Digital Plus') : 'DDP',
+        re.compile(r'TrueHD')             : 'TrueHD',
+        re.compile(r'Dolby Atmos')        : 'Atmos',
+        re.compile(r'Master Audio')       : 'MA',
+        re.compile(r'High Resolution')    : 'HR',
+        re.compile(r'Extended Surround')  : 'ES',
+        re.compile(r'High Efficiency')    : 'HE',
+        re.compile(r'Low Complexity')     : 'LC',
+        re.compile(r'High Quality')       : 'HQ',
+    }
+
+    def _get_audio_codec(self):
+        audio_codec = _as_string(self._guess.get('audio_codec'))
+        if not audio_codec:
+            return ''
+        else:
+            if isinstance(audio_codec, str):
+                infos = [audio_codec]
             else:
-                return f'{minutes}m'
+                infos = audio_codec
 
-        runtimes = await self.try_webdbs((self.imdb, self.tvmaze), 'runtimes', default=())
-        if len(runtimes) == 1:
-            runtime = tuple(runtimes.values())[0]
-            return f'[b]Runtime[/b]: {format_runtime(runtime)}'
-        elif len(runtimes) > 1:
             parts = []
-            for cut, minutes in runtimes.items():
-                part = f'{format_runtime(minutes)}'
-                if cut != 'default':
-                    part += f' ({cut})'
-                parts.append(part)
-            return f'[b]Runtimes[/b]: {", ".join(parts)}'
-
-    @staticmethod
-    def _format_person(person):
-        if hasattr(person, 'url') and person.url:
-            return f'[url={person.url}]{person}[/url]'
-        else:
-            return str(person)
-
-    async def format_description_directors(self):
-        directors = await self.try_webdbs((self.imdb, self.tvmaze), 'directors', default=())
-        if directors:
-            directors_links = [self._format_person(director) for director in directors]
-            return (f'[b]Director{"s" if len(directors) > 1 else ""}[/b]: '
-                    + ', '.join(directors_links))
-
-    async def format_description_creators(self):
-        creators = await self.try_webdbs((self.tvmaze, self.imdb), 'creators', default=())
-        if creators:
-            creators_links = [self._format_person(creator) for creator in creators]
-            return (f'[b]Creator{"s" if len(creators) > 1 else ""}[/b]: '
-                    + ', '.join(creators_links))
-
-    async def format_description_cast(self):
-        actors = await self.try_webdbs((self.tvmaze, self.imdb), 'cast')
-        if actors:
-            actors_links = [self._format_person(actor) for actor in actors]
-            return ('[b]Cast[/b]: ' + ', '.join(actors_links))
-
-    async def format_description_series_screenshots(self):
-        await self.upload_screenshots_job.wait()
-        screenshot_urls = self.get_job_output(self.upload_screenshots_job)
-        screenshots_bbcode_parts = [
-            f'[img={url}]'
-            for url in screenshot_urls
-        ]
-        screenshots_bbcode = '\n\n'.join(screenshots_bbcode_parts)
-        if screenshots_bbcode:
-            return (
-                '[quote]\n'
-                f'[align=center]{screenshots_bbcode}[/align]\n'
-                '[/quote]'
-            )
-
-    async def format_description_series_mediainfo(self):
-        await self.mediainfo_job.wait()
-        mediainfo = self.get_job_output(self.mediainfo_job, slice=0)
-        if mediainfo:
-            return f'[mediainfo]{mediainfo}[/mediainfo]'
+            for info in infos:
+                for regex,abbrev in self._audio_codec_translation.items():
+                    if regex.search(info):
+                        parts.append(abbrev)
+                        continue
+
+            # Join translations, default to what guessit detected
+            audio_codec = ' '.join(parts or infos)
+
+            # Final adjustments
+            audio_codec = re.sub(r'DDP? TrueHD', 'TrueHD', audio_codec)
+            audio_codec = re.sub(r'DDP? Atmos', 'Atmos', audio_codec)
+
+            return audio_codec
+
+    _audio_channels_regex = re.compile(rf'{DELIM}(\d\.\d){DELIM}')
+
+    def _get_audio_channels(self):
+        audio_channels = _as_string(self._guess.get('audio_channels', ''))
+        if not audio_channels:
+            match = self._audio_channels_regex.search(self.release_name_params)
+            if match:
+                return match.group(1)
+        return audio_channels
 
-    # Web form data
+    _hdr_translation = {
+        re.compile(rf'(?:{DELIM}|^)(?i:DV|DoVi|Dolby{DELIM}Vision)(?:{DELIM}|$)'): 'DV',
+        re.compile(rf'(?:{DELIM}|^)(?i:HDR10\+)(?:{DELIM}|$)'): 'HDR10+',
+        re.compile(rf'(?:{DELIM}|^)(?i:HDR10)(?!:\+)(?:{DELIM}|$)'): 'HDR10',
+        re.compile(rf'(?:{DELIM}|^)(?i:HDR)(?!:10\+)(?:{DELIM}|$)'): 'HDR',
+    }
 
-    @property
-    def submission_ok(self):
+    def _get_hdr_format(self):
+        for regex, hdr_format in self._hdr_translation.items():
+            if regex.search(self.release_name_params):
+                return hdr_format
+        return ''
+
+    _x264_regex = re.compile(rf'(?:{DELIM}|^)(?i:x264)(?:{DELIM}|$)')
+    _x265_regex = re.compile(rf'(?:{DELIM}|^)(?i:x265)(?:{DELIM}|$)')
+
+    def _get_video_codec(self):
+        video_codec = _as_string(self._guess.get('video_codec', ''))
+        if video_codec == 'H.264':
+            if self._x264_regex.search(self.release_name_params):
+                return 'x264'
+
+        elif video_codec == 'H.265':
+            if self._x265_regex.search(self.release_name_params):
+                return 'x265'
+
+        return video_codec
+
+    def _get_group(self):
+        return _as_string(self._guess.get('release_group', ''))
+
+    _has_commentary_regex = re.compile(rf'{DELIM}(?i:plus{DELIM}+comm|commentary){DELIM}')
+
+    def _get_has_commentary(self):
+        if self._guess.get('has_commentary', None) is None:
+            self._guess['has_commentary'] = \
+                bool(self._has_commentary_regex.search(self.release_name_params))
+        return self._guess['has_commentary']
+
+    def _set_has_commentary(self, value):
+        if value is None:
+            self._guess['has_commentary'] = None
+        else:
+            self._guess['has_commentary'] = bool(value)
+
+
+class Episodes(dict):
+    """
+    :class:`dict` subclass that maps season numbers to lists of episode numbers
+
+    All keys and values are :class:`str` objects. All episodes from a season are
+    indicated by an empty sequence. For episodes from any sason, the key is an
+    empty string.
+
+    This class accepts the same arguments as :class:`dict`.
+
+    To provide seasons as keyword arguments, you need to prefix "S" to each
+    keyword. This is because numbers can't be keyword arguments, but it also
+    looks nicer.
+
+    >>> e = Episodes({"1": ["1", "2", "3"], "2": []})
+    >>> e.update(S01=[3, "4"], S3=range(2, 4), s05=[], S=[10, "E11", 12])
+    >>> e
+    >>> Episodes({'1': ['1', '2', '3', '4'], '2': [], '3': ['2', '3'], '5': [], '': ['10', '11', '12']})
+    """
+
+    regex = re.compile(rf'(?:{DELIM}|^)((?i:[SE]\d+)+)(?:{DELIM}|$)')
+    """Regular expression that matches "S01E02"-like episode information"""
+
+    @classmethod
+    def has_episodes_info(cls, string):
+        """Whether `string` contains "S01E02"-like episode information"""
+        return bool(cls.regex.search(string))
+
+    _is_episodes_info_regex = re.compile(r'^(?i:[SE]\d+)+$')
+
+    @classmethod
+    def is_episodes_info(cls, string):
+        """Whether `string` is "S01E02"-like episode information and nothing else"""
+        return bool(cls._is_episodes_info_regex.search(string))
+
+    @classmethod
+    def from_string(cls, value):
         """
-        `False` if :attr:`isolated_jobs` is truthy, parent implementation
-        otherwise
+        Create instance from release name or string that contains "Sxx" and "Exx"
+
+        Examples:
+
+            >>> Episodes.from_string('foo.E01 bar')
+            {'': ('1',)}
+            >>> Episodes.from_string('foo E01E2.bar')
+            {'': ('1', '2')}
+            >>> Episodes.from_string('foo.bar.E01E2S03')
+            {'': ('1', '2'), '3': ()}
+            >>> Episodes.from_string('E01E2S03E04E05.baz')
+            {'': ('1', '2'), '3': ('4', '5')}
+            >>> Episodes.from_string('S09E08S03E06S9E1')
+            {'9': ('1', '8',), '3': ('6',)}
+            >>> Episodes.from_string('E01S03E06.bar.E02')
+            {'': ('1', '2',), '3': ('6',)}
         """
-        if self.isolated_jobs:
-            return False
-        else:
-            return super().submission_ok
+        def extract_number(string):
+            n = ''.join(c for c in string if c in '0123456789').lstrip('0')
+            return '0' if n == '' else n
+
+        def split_episodes(string):
+            return {extract_number(e) for e in string.split('E') if e.strip()}
+
+        # Extract episode information to get "S..E.." string without any other
+        # characters. The original value might have delimiters,
+        # e.g. "...S09E14-E15...", and we want "S09E14E15".
+        episodes_string = ''.join(re.findall(
+            (
+                r'(?i:[^SE\d]*|^)'
+                r'((?i:[SE]\d+)+)'
+                r'(?i:[^SE\d]+|$)'
+            ),
+            str(value).upper(),
+        ))
 
-    @property
-    def torrent_filepath(self):
-        return self.get_job_output(self.create_torrent_job, slice=0)
+        seasons = collections.defaultdict(lambda: set())
+        for part in (k for k in episodes_string.split('S') if k):
+            season = re.sub(r'E.*$', '', part)
+            season = str(int(season)) if season else ''
+            episodes = re.sub(r'^\d+', '', part)
+            episodes = split_episodes(episodes) if episodes else ()
+            seasons[season].update(episodes)
+
+        args = {season: tuple(natsort.natsorted(episodes))
+                for season, episodes in natsort.natsorted(seasons.items())}
+        return cls(args)
 
-    @property
-    def post_data(self):
-        if self.is_movie_release:
-            post_data = {
-                'submit': 'true',
-                'type': 'Movies',
-                'title': self.get_job_output(self.movie_title_job, slice=0),
-                'year': self.get_job_output(self.movie_year_job, slice=0),
-                'source': self.get_job_attribute(self.movie_source_job, 'choice'),
-                'videoformat': self.get_job_attribute(self.movie_video_codec_job, 'choice'),
-                'audioformat': self.get_job_attribute(self.movie_audio_codec_job, 'choice'),
-                'container': self.get_job_attribute(self.movie_container_job, 'choice'),
-                'resolution': self.get_job_attribute(self.movie_resolution_job, 'choice'),
-                'remaster_title': self.get_job_output(self.movie_release_info_job, slice=0),
-                'tags': self.get_job_output(self.movie_tags_job, slice=0),
-                'desc': self.post_data_description,
-                'release_desc': self.get_job_output(self.mediainfo_job, slice=0),
-                'image': self.get_job_output(self.movie_poster_job, slice=0),
-            }
-            post_data.update(self.post_data_screenshot_urls)
-            if self.get_job_attribute(self.scene_check_job, 'is_scene_release'):
-                post_data['scene'] = '1'
-            return post_data
-
-        elif self.is_series_release:
-            post_data = {
-                'submit': 'true',
-                'type': 'Anime' if self.options['anime'] else 'TV',
-                'title': self.get_job_output(self.series_title_job, slice=0),
-                'tags': self.get_job_output(self.series_tags_job, slice=0),
-                'desc': self.post_data_description,
-                'image': self.get_job_output(self.series_poster_job, slice=0),
-            }
-            if self.get_job_attribute(self.scene_check_job, 'is_scene_release'):
-                post_data['scene'] = '1'
-            return post_data
+    @classmethod
+    def from_sequence(cls, sequence):
+        """
+        Combine episode information from multiple strings
 
-        else:
-            raise RuntimeError(f'Weird release type: {self.release_type!r}')
+        Examples:
 
-    @property
-    def post_data_screenshot_urls(self):
-        urls = self.get_job_output(self.upload_screenshots_job)
-        return {f'screenshot{i}': url for i, url in enumerate(urls, start=1)}
+            >>> Episodes.from_sequence(['foo.S01E01.bar', 'hello'])
+            {'1': ('1',)}
+            >>> Episodes.from_sequence(['foo.S01E01.bar', 'bar.S01E02.baz'])
+            {'1': ('1', '2')}
+        """
+        episodes = Episodes()
+        for string in sequence:
+            eps = cls.from_string(string)
+            for season in eps:
+                if season in episodes:
+                    episodes[season] += eps[season]
+                else:
+                    episodes[season] = eps[season]
+        return episodes
 
-    @property
-    def post_data_description(self):
-        parts = []
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        self._set(*args, **kwargs)
 
-        if self.is_movie_release:
-            # Screenshots and mediainfo are submitted separately
-            parts.append(self.get_job_output(self.movie_description_job, slice=0))
-
-        elif self.is_series_release:
-            parts.append(self.get_job_output(self.series_description_job, slice=0))
-
-        # Append self promotion below. A closing [/quote] tag automatically
-        # renders a newline. Otherwise, we must add a newline character.
-        if parts and not parts[-1].endswith(('[/quote]', '\n')):
-            parts.append('\n')
-        parts.append(self.promotion)
+    def update(self, *args, clear=False, **kwargs):
+        """
+        Set specific episodes from specific seasons, remove all other episodes and
+        seasons
+
+        :params bool clear: Whether to remove all seasons and episodes first
+        """
+        if clear:
+            self.clear()
+        self._set(*args, **kwargs)
+
+    def _set(self, *args, **kwargs):
+        # Validate all values before applying any changes
+        validated = {}
+        update = dict(*args, **kwargs)
+        for season, episodes in update.items():
+            season = self._normalize_season(season)
+            if not isinstance(episodes, collections.abc.Iterable) or isinstance(episodes, str):
+                episodes = [self._normalize_episode(episodes)]
+            else:
+                episodes = [self._normalize_episode(e) for e in episodes]
+
+            if season in validated:
+                validated[season].extend(episodes)
+            else:
+                validated[season] = episodes
+
+        # Set validated values
+        for season, episodes in validated.items():
+            if season in self:
+                self[season].extend(episodes)
+            else:
+                self[season] = episodes
+
+            # Remove duplicates
+            self[season][:] = set(self[season])
 
+            # Sort naturally
+            self[season].sort(key=natsort.natsort_key)
+
+    def _normalize_season(self, value):
+        return self._normalize(value, name='season', prefix='S', empty_string_ok=True)
+
+    def _normalize_episode(self, value):
+        return self._normalize(value, name='episode', prefix='E', empty_string_ok=False)
+
+    def _normalize(self, value, name, prefix=None, empty_string_ok=False):
+        if isinstance(value, int):
+            if value >= 0:
+                return str(value)
+
+        elif isinstance(value, str):
+            if value == '' and empty_string_ok:
+                return str(value)
+
+            if value.isdigit():
+                return str(int(value))
+
+            if prefix and len(value) >= len(prefix):
+                prefix_ = value[:len(prefix)].casefold()
+                if prefix_ == prefix.casefold():
+                    actual_value = value[len(prefix):]
+                    return self._normalize(
+                        actual_value,
+                        name=name,
+                        prefix=None,
+                        empty_string_ok=empty_string_ok,
+                    )
+
+        raise TypeError(f'Invalid {name}: {value!r}')
+
+    def remove_specific_episodes(self):
+        """Remove episodes from each season, leaving only complete seasons"""
+        for season in tuple(self):
+            if season:
+                self[season] = ()
+            else:
+                del self[season]
+
+    def __repr__(self):
+        return f'{type(self).__name__}({dict(self)!r})'
+
+    def __str__(self):
+        parts = []
+        for season, episodes in sorted(self.items()):
+            if season:
+                parts.append(f'S{season:0>2}')
+            for episode in episodes:
+                parts.append(f'E{episode:0>2}')
         return ''.join(parts)
 
-    promotion = (
-        '[align=right][size=1]Shared with '
-        f'[url={__homepage__}]{__project_name__} {__version__}[/url]'
-        '[/size][/align]'
-    )
+
+def _as_list(value):
+    if not value:
+        return []
+    elif isinstance(value, str):
+        return [value]
+    elif isinstance(value, list):
+        return list(value)
+    else:
+        return [value]
+
+def _as_string(value):
+    if not value:
+        return ''
+    elif isinstance(value, str):
+        return value
+    elif isinstance(value, list):
+        return ' '.join(value)
+    else:
+        return str(value)
```

### Comparing `upsies-2023.5.25/bb/tracker.py` & `upsies-2023.6.11/upsies/uis/tui/jobwidgets/torrent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,215 +1,228 @@
-"""
-Concrete :class:`~.base.TrackerBase` subclass for bB
-"""
-
-import asyncio
-import re
-import urllib
-
-from ... import __project_name__, errors
-from ...utils import html, http
-from ..base import TrackerBase
-from .config import BbTrackerConfig
-from .jobs import BbTrackerJobs
+import functools
+
+from prompt_toolkit.filters import Condition
+from prompt_toolkit.layout.containers import ConditionalContainer, HorizontalAlign, HSplit, VSplit, Window, WindowAlign
+from prompt_toolkit.layout.controls import FormattedTextControl
+from prompt_toolkit.layout.dimension import Dimension
+
+from ....utils import fs, torrent
+from .. import widgets
+from . import JobWidgetBase
 
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
 
-class BbTracker(TrackerBase):
-    name = 'bb'
-    label = 'bB'
-
-    TrackerConfig = BbTrackerConfig
-    TrackerJobs = BbTrackerJobs
-
-    _url_path = {
-        'login': '/login.php',
-        'logout': '/logout.php',
-        'upload': '/upload.php',
-        'torrent': '/torrents.php',
-    }
-
-    _max_login_attempts = 30
-    _login_retry_delay = 1
-    _login_retry_delay_max = 3
-
-    async def login(self):
-        if not self.is_logged_in:
-            if not self.options.get('username'):
-                raise errors.RequestError('Login failed: No username configured')
-            elif not self.options.get('password'):
-                raise errors.RequestError('Login failed: No password configured')
-
-            login_url = urllib.parse.urljoin(
-                self.options['base_url'],
-                self._url_path['login'],
-            )
+class CreateTorrentJobWidget(JobWidgetBase):
+    def setup(self):
+        self._progress = widgets.ProgressBar()
+        self._file_tree = FormattedTextControl()
+        self._throughput = FormattedTextControl()
+        self._throughput_unit = ''
+        self._percent_done = FormattedTextControl()
+        self._seconds_elapsed = FormattedTextControl()
+        self._seconds_remaining = FormattedTextControl()
+        self._seconds_total = FormattedTextControl()
+        self._time_started = FormattedTextControl()
+        self._time_finished = FormattedTextControl()
+        self._current_file_name = ''
+
+        status_column1 = HSplit(
+            children=[
+                self.make_readout(' Started:', '_time_started', width=8),
+                self.make_readout('Finished:', '_time_finished', width=8),
+            ],
+        )
+        status_column2 = HSplit(
+            children=[
+                self.make_readout('  Elapsed:', '_seconds_elapsed', width=8),
+                self.make_readout('Remaining:', '_seconds_remaining', width=8),
+                self.make_readout('    Total:', '_seconds_total', width=8),
+            ],
+        )
+        status_column3 = HSplit(
+            children=[
+                self.make_readout(
+                    lambda: '%'.ljust(len(self._throughput_unit)),
+                    '_percent_done',
+                    width=6,
+                    value_align='right',
+                    label_side='right',
+                ),
+                self.make_readout(
+                    lambda: self._throughput_unit.ljust(len(self._throughput_unit)),
+                    '_throughput',
+                    width=6,
+                    value_align='right',
+                    label_side='right',
+                ),
+            ],
+        )
+        status = VSplit(children=[status_column1, status_column2, status_column3], padding=3)
 
-            doc = html.parse('')
-            while await self._work_around_login_bug(doc):
-                _log.debug('%s: Logging in as %r', self.name, self.options['username'])
-                response = await http.post(
-                    url=login_url,
-                    user_agent=True,
-                    data={
-                        'username': self.options['username'],
-                        'password': self.options['password'],
-                        'login': 'Log In!',
-                    },
-                )
-                doc = html.parse(response)
-                self._raise_login_error(doc)
-
-            self._store_auth_token(doc)
-
-    def _raise_login_error(self, doc):
-        error_tag = doc.find('font', color='red')
-        if error_tag:
-            raise errors.RequestError(f'Login failed: {error_tag.string.strip()}')
-        elif doc.find('form', id='loginform'):
-            html.dump(doc, 'login.html')
-            raise errors.RequestError('Login failed: No error message found. See login.html.')
-
-    async def _work_around_login_bug(self, doc):
-        # Login sometimes fails and redirects to main page without logging in
-        if not self._get_auth_token(doc):
-            if not hasattr(self, '_login_attempts'):
-                self._login_attempts = -1
-            self._login_attempts += 1
-
-            if self._login_attempts < self._max_login_attempts:
-                if self._login_attempts:
-                    self._login_retry_delay = min(self._login_retry_delay * 1.2,
-                                                  self._login_retry_delay_max)
-                assert type(self)._login_retry_delay == 1
-                if self._login_attempts > 1:
-                    _log.debug(f'Encountered login bug; retrying in {round(self._login_retry_delay)}s')
-                    await asyncio.sleep(round(self._login_retry_delay))
-                return True
-            else:
-                _log.debug(f'Encountered login bug; giving up after {self._login_attempts} attempts')
-                raise errors.RequestError('Login failed: Giving up after encountering '
-                                          f'login bug {self._login_attempts} times')
-        return False
-
-    _auth_token_regex = re.compile(r'logout\.php\?.*\bauth=([0-9a-fA-F]+)')
-
-    @classmethod
-    def _get_auth_token(cls, doc):
-        logout_link_tag = doc.find('a', href=cls._auth_token_regex)
-        if logout_link_tag:
-            logout_link_href = logout_link_tag['href']
-            if logout_link_href:
-                match = cls._auth_token_regex.search(logout_link_href)
-                if match:
-                    return match.group(1)
-
-    def _store_auth_token(self, doc):
-        auth_token = self._get_auth_token(doc)
-        if not auth_token:
-            raise RuntimeError('Failed to find authentication token')
-        else:
-            self._auth_token = auth_token
+        self._activity_indicator = widgets.ActivityIndicator(
+            style='class:info',
+        )
+        self.job.signal.register('finished', lambda _: self._activity_indicator.disable())
 
-    @property
-    def is_logged_in(self):
-        return bool(getattr(self, '_auth_token', False))
-
-    async def logout(self):
-        if self.is_logged_in:
-            _log.debug('%s: Logging out', self.name)
-            logout_url = urllib.parse.urljoin(
-                self.options['base_url'],
-                self._url_path['logout'],
-            )
-            params = {'auth': self._auth_token}
-            delattr(self, '_auth_token')
-            await http.get(url=logout_url, params=params, user_agent=True)
-
-    async def get_announce_url(self):
-        if self.options.get('announce_url'):
-            return self.options['announce_url']
-        else:
-            url = urllib.parse.urljoin(
-                self.options['base_url'],
-                self._url_path['upload'],
+        self._runtime_widget = HSplit(
+            children=[
+                ConditionalContainer(
+                    filter=Condition(lambda: self._progress.percent > 0),
+                    content=HSplit([
+                        # Estimated times, progress per second, etc
+                        status,
+                        # Progress bar
+                        self._progress,
+                    ]),
+                ),
+                VSplit([
+                    # Moving character to indicate activity
+                    ConditionalContainer(
+                        filter=Condition(lambda: self._activity_indicator.active),
+                        content=VSplit([
+                            self._activity_indicator,
+                            widgets.hspacer,
+                        ]),
+                    ),
+                    # "Hashing", "Searching", "Press ... to skip hashing", etc.
+                    Window(
+                        FormattedTextControl(self._get_current_activity),
+                        # Make sure that the activity is always displayed in
+                        # full and the current file name is trimmed to make it fit
+                        width=Dimension(weight=10),
+                        dont_extend_width=True,
+                    ),
+                    widgets.hspacer,
+                    # Current file name (torrent or content file)
+                    ConditionalContainer(
+                        filter=Condition(lambda: self._current_file_name),
+                        content=Window(
+                            FormattedTextControl(lambda: self._current_file_name),
+                            style='class:info.readout',
+                        ),
+                    ),
+                ]),
+                ConditionalContainer(
+                    filter=Condition(lambda: bool(self._file_tree.text)),
+                    content=Window(self._file_tree),
+                ),
+            ],
+            style='class:info',
+            width=Dimension(min=55, max=150),
+        )
+
+        @self.keybindings_global.add(
+            'c-t', 'h',
+            filter=Condition(lambda: self.job.activity in ('searching', 'verifying')),
+        )
+        def _(event):
+            self.job.cancel_search()
+
+        self.job.signal.register('file_tree', self.handle_file_tree)
+        self.job.signal.register('progress_update', self.handle_progress_update)
+        self.job.signal.register('finished', lambda _: self.invalidate())
+
+    def make_readout(self, label, attribute, value_align='left', width=None, label_side='left'):
+        readout_widget = Window(
+            getattr(self, attribute),
+            dont_extend_width=True,
+            dont_extend_height=True,
+            style='class:info.readout',
+            width=width,
+            align=getattr(WindowAlign, value_align.upper()),
+        )
+        label_widget = Window(FormattedTextControl(label), dont_extend_width=True)
+
+        if label_side == 'left':
+            children = [label_widget, readout_widget]
+        elif label_side == 'right':
+            children = [readout_widget, label_widget]
+
+        return VSplit(
+            children=children,
+            padding=1,
+            align=HorizontalAlign.CENTER,
+        )
+
+    def handle_file_tree(self, file_tree):
+        self._file_tree.text = fs.format_file_tree(file_tree)
+
+    def handle_progress_update(self, info):
+        self._progress.percent = info.percent_done
+        self._percent_done.text = f'{info.percent_done:.2f}'
+
+        self._time_started.text = info.time_started.strftime('%H:%M:%S')
+        self._time_finished.text = info.time_finished.strftime('%H:%M:%S')
+
+        def timedelta_string(delta):
+            hours, rest = divmod(delta.total_seconds(), 3600)
+            minutes, seconds = divmod(rest, 60)
+            return f'{hours:02.0f}:{minutes:02.0f}:{seconds:02.0f}'
+
+        self._seconds_elapsed.text = timedelta_string(info.seconds_elapsed)
+        self._seconds_remaining.text = timedelta_string(info.seconds_remaining)
+        self._seconds_total.text = timedelta_string(info.seconds_total)
+
+        if isinstance(info, torrent.CreateTorrentProgress):
+            # Torrent is hashed from fresh files - yummy!
+            throughput = info.bytes_per_second.format(
+                prefix='binary',
+                decimal_places=2,
+                trailing_zeros=True,
             )
-            _log.debug('%s: Getting announce URL from %s', self.name, url)
-            response = await http.get(url, cache=False, user_agent=True)
-            doc = html.parse(response)
-            announce_url_tag = doc.find('input', value=re.compile(r'^https?://.*/announce$'))
-            if announce_url_tag:
-                return announce_url_tag['value']
+            self._throughput.text, self._throughput_unit = throughput.split(' ')
+            self._throughput_unit += '/s'
+            self._current_file_name = fs.basename(info.filepath)
+
+        elif isinstance(info, torrent.FindTorrentProgress):
+            # Torrent hashes are searched for in existing torrents
+            if info.exception:
+                self.job.warn(info.exception)
+            elif info.status == 'verifying':
+                self._activity_indicator.active = True
             else:
-                cmd = f'{__project_name__} set trackers.{self.name}.announce_url <YOUR URL>'
-                raise errors.RequestError(f'Failed to find announce URL - set it manually: {cmd}')
+                self._activity_indicator.active = False
 
-    async def upload(self, tracker_jobs):
-        _log.debug('Uploading %r', tracker_jobs.post_data)
-        upload_url = urllib.parse.urljoin(self.options['base_url'], self._url_path['upload'])
-        response = await http.post(
-            url=upload_url,
-            cache=False,
-            user_agent=True,
-            follow_redirects=False,
-            files={'file_input': {
-                'file': tracker_jobs.torrent_filepath,
-                'mimetype': 'application/octet-stream',
-            }},
-            data=tracker_jobs.post_data,
-        )
-
-        # Upload response should redirect to torrent page via "Location" header
-        torrent_page_url = urllib.parse.urljoin(
-            self.options['base_url'],
-            response.headers.get('Location', ''),
-        )
-        if urllib.parse.urlparse(torrent_page_url).path == self._url_path['torrent']:
-            return str(torrent_page_url)
+            self._throughput.text = f'{info.files_per_second}'
+            self._throughput_unit = 'files/s'
+            self._current_file_name = fs.basename(info.filepath)
+
+        self.invalidate()
+
+    def _get_current_activity(self):
+        if self.job.activity in ('announce_url', 'verifying'):
+            self._activity_indicator.active = True
+        else:
+            self._activity_indicator.active = False
+
+        if self.job.activity == 'announce_url':
+            activity = 'Getting announce URL'
+        elif self.job.activity == 'searching':
+            activity = 'Press <Ctrl-t h> to skip searching for a reusable torrent'
         else:
-            _log.debug('Unexpected torrent page URL: %r', torrent_page_url)
-            doc = html.parse(response)
+            activity = self.job.activity.capitalize()
+
+        return activity
+
+    @functools.cached_property
+    def runtime_widget(self):
+        return self._runtime_widget
+
+
+class AddTorrentJobWidget(JobWidgetBase):
+    def setup(self):
+        pass
+
+    @functools.cached_property
+    def runtime_widget(self):
+        return None
+
+
+class CopyTorrentJobWidget(JobWidgetBase):
+    def setup(self):
+        pass
 
-            # Try to find error message
-            error_tag = doc.find('p', style=re.compile(r'color: red'))
-            try:
-                error_msg = error_tag.string.strip()
-                if error_msg:
-                    raise errors.RequestError(f'Upload failed: {error_msg}')
-            except AttributeError:
-                pass
-
-            # Try to find different type of error message
-            # (e.g. "The exact same torrent file already exists on the site!")
-            try:
-                error_header_tag = doc.find('h2', string=re.compile(r'^\s*Error\s*$'))
-                parent_tag = error_header_tag.parent
-                error_msg_tag = parent_tag.find('p')
-                error_msg = error_msg_tag.string.strip()
-                if error_msg:
-                    raise errors.RequestError(f'Upload failed: {error_msg}')
-            except AttributeError:
-                pass
-
-            # Try to find warning (e.g. "Your torrent has been uploaded however,
-            # you must re-download the torrent file from <a
-            # href="torrents.php?id=123456">here</a>, because of the following
-            # warnings: The torrent did not have the correct announce URL."
-            try:
-                warning_header_tag = doc.find('h1', string=re.compile(r'^\s*Warning\s*$'))
-                content_tag = warning_header_tag.parent
-                warnings = [
-                    warning_tag.get_text().strip()
-                    for warning_tag in content_tag.find_all('li')
-                ]
-                if warnings:
-                    for warning in warnings:
-                        self.warn(warning)
-                    return None
-            except AttributeError:
-                pass
-
-            # Unable to find error message
-            html.dump(response, 'upload.html')
-            raise RuntimeError('Failed to find error message. See upload.html.')
+    @functools.cached_property
+    def runtime_widget(self):
+        return None
```

### Comparing `upsies-2023.5.25/upsies/__init__.py` & `upsies-2023.6.11/upsies/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 __project_name__ = 'upsies'
 __description__ = 'Media metadata aggregator'
 __homepage__ = 'https://upsies.readthedocs.io'
-__version__ = '2023.05.25'
-__author__ = 'plotski'
-__author_email__ = 'plotski@example.org'
+__version__ = '2023.06.11'
 
 
 def application_setup(config):
     """
     This function should be called by the UI ASAP when `config` is available
 
     :param config: :class:`~.configfiles.ConfigFiles` instance
```

### Comparing `upsies-2023.5.25/upsies/constants.py` & `upsies-2023.6.11/upsies/constants.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/defaults.py` & `upsies-2023.6.11/upsies/defaults.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/errors.py` & `upsies-2023.6.11/upsies/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,18 +103,22 @@
     """Image resizing failed"""
 
 
 class ImageOptimizeError(UpsiesError):
     """Image optimization failed"""
 
 
-class TorrentError(UpsiesError):
+class TorrentCreateError(UpsiesError):
     """Torrent file creation failed"""
 
 
+class TorrentAddError(UpsiesError):
+    """Adding torrent to client failed"""
+
+
 def SubprocessError(exception, original_traceback):
     """Attach `original_traceback` to `exception`"""
     exception.original_traceback = f'Subprocess traceback:\n{original_traceback.strip()}'
     return exception
 
 
 class SceneError(UpsiesError):
```

### Comparing `upsies-2023.5.25/upsies/jobs/base.py` & `upsies-2023.6.11/upsies/jobs/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/jobs/custom.py` & `upsies-2023.6.11/upsies/jobs/custom.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/jobs/dialog.py` & `upsies-2023.6.11/upsies/jobs/dialog.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/jobs/imghost.py` & `upsies-2023.6.11/upsies/jobs/imghost.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/jobs/mediainfo.py` & `upsies-2023.6.11/upsies/jobs/mediainfo.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/jobs/poster.py` & `upsies-2023.6.11/upsies/jobs/poster.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/jobs/scene.py` & `upsies-2023.6.11/upsies/jobs/scene.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     async def _search(self):
         try:
             results = await self._predb.search(
                 query=self._content_path,
                 only_existing_releases=False,
             )
         except (errors.RequestError, errors.SceneError) as e:
+            _log.debug('Caught %r', e)
             self.error(e)
         else:
             if results:
                 for result in results:
                     self.send(result)
             else:
                 self.error('No results')
```

### Comparing `upsies-2023.5.25/upsies/jobs/screenshots.py` & `upsies-2023.6.11/upsies/jobs/screenshots.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/jobs/set.py` & `upsies-2023.6.11/upsies/jobs/set.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/jobs/submit.py` & `upsies-2023.6.11/upsies/jobs/submit.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/jobs/torrent.py` & `upsies-2023.6.11/upsies/jobs/torrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         else:
             output_queue.put((daemon.MsgType.info, progress))
 
     kwargs['init_callback'] = init_callback
     kwargs['progress_callback'] = progress_callback
     try:
         torrent_path = torrent.create(*args, **kwargs)
-    except errors.TorrentError as e:
+    except errors.TorrentCreateError as e:
         output_queue.put((daemon.MsgType.error, str(e)))
     else:
         output_queue.put((daemon.MsgType.result, torrent_path))
 
 
 class AddTorrentJob(base.QueueJobBase):
     """
@@ -283,24 +283,19 @@
         self.signal.register('finished', lambda _: setattr(self, 'info', ''))
         self.signal.register('error', lambda _: setattr(self, 'info', ''))
 
     async def handle_input(self, torrent_path):
         _log.debug('Adding %s to %s', torrent_path, self._btclient.name)
         self.signal.emit('adding', torrent_path)
 
-        response = await self._btclient.add_torrent(torrent_path)
-
-        for warning in response.warnings:
-            self.warn(warning)
-
-        for error in response.errors:
-            self.error(error)
-
-        if response.success:
-            infohash = (response.added + response.already_added)[0]
+        try:
+            infohash = await self._btclient.add_torrent(torrent_path)
+        except errors.TorrentAddError as e:
+            self.error(e)
+        else:
             self.send(infohash)
             self.signal.emit('added', infohash)
 
 
 class CopyTorrentJob(base.QueueJobBase):
     """
     Copy file(s)
```

### Comparing `upsies-2023.5.25/upsies/jobs/webdb.py` & `upsies-2023.6.11/upsies/jobs/webdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/__init__.py` & `upsies-2023.6.11/upsies/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/base/_howto.py` & `upsies-2023.6.11/upsies/trackers/base/_howto.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/base/config.py` & `upsies-2023.6.11/upsies/trackers/base/config.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/base/jobs.py` & `upsies-2023.6.11/upsies/trackers/base/jobs.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/base/tracker.py` & `upsies-2023.6.11/upsies/trackers/base/tracker.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/bhd/config.py` & `upsies-2023.6.11/upsies/trackers/bhd/config.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/bhd/jobs.py` & `upsies-2023.6.11/upsies/trackers/bhd/jobs.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/bhd/tracker.py` & `upsies-2023.6.11/upsies/trackers/bhd/tracker.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/dummy.py` & `upsies-2023.6.11/upsies/trackers/dummy.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/mtv/config.py` & `upsies-2023.6.11/upsies/trackers/mtv/config.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/mtv/jobs.py` & `upsies-2023.6.11/upsies/trackers/mtv/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,17 @@
         if self.category_job.is_finished:
             choice = self.get_job_attribute(self.category_job, 'choice')
             return self._category_value_type_map.get(choice)
 
     release_name_separator = '.'
 
     release_name_translation = {
+        'edition': {
+            re.compile(r"^Director's Cut$"): r'DC',
+        },
         'group': {
             re.compile(r'^NOGROUP$'): r'NOGRP',
         },
     }
 
     @functools.cached_property
     def title_job(self):
@@ -150,14 +153,15 @@
             precondition=self.make_precondition('title_job'),
             prejobs=(
                 self.category_job,
                 self.scene_check_job,
                 self.imdb_job,
             ),
             text=self.generate_title,
+            validator=self.validate_title,
             **self.common_job_args(),
         )
 
     async def generate_title(self):
         assert self.scene_check_job.is_finished
         assert self.imdb_job.is_finished
 
@@ -169,14 +173,24 @@
                 assert len(search_results) >= 1, search_results
                 return search_results[0]
 
         # Non-scene release or season pack. We may generate a title.
         await self.release_name.fetch_info(webdb=self.imdb, webdb_id=self.imdb_id)
         return str(self.release_name)
 
+    def validate_title(self, text):
+        if not text.strip():
+            raise ValueError('Title must not be empty')
+
+        match = re.search(rf'(?:{utils.release.DELIM}|$)(UNKNOWN_([A-Z_]+))(?:{utils.release.DELIM}|$)', text)
+        if match:
+            placeholder = match.group(1)
+            name = match.group(2).lower().replace('_', ' ')
+            raise ValueError(f'Replace "{placeholder}" with the correct {name}')
+
     image_host_config = {
         'common': {'thumb_width': 300},
     }
 
     @functools.cached_property
     def description_job(self):
         return jobs.dialog.TextFieldJob(
```

### Comparing `upsies-2023.5.25/upsies/trackers/mtv/tracker.py` & `upsies-2023.6.11/upsies/trackers/mtv/tracker.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/nbl/config.py` & `upsies-2023.6.11/upsies/trackers/nbl/config.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/nbl/jobs.py` & `upsies-2023.6.11/upsies/trackers/nbl/jobs.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/nbl/tracker.py` & `upsies-2023.6.11/upsies/trackers/nbl/tracker.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/ptp/config.py` & `upsies-2023.6.11/upsies/trackers/ptp/config.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/ptp/jobs.py` & `upsies-2023.6.11/upsies/trackers/ptp/jobs.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/ptp/metadata.py` & `upsies-2023.6.11/upsies/trackers/ptp/metadata.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/trackers/ptp/tracker.py` & `upsies-2023.6.11/upsies/trackers/ptp/tracker.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/commands/__init__.py` & `upsies-2023.6.11/upsies/uis/tui/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/commands/base.py` & `upsies-2023.6.11/upsies/uis/tui/commands/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     :param args: Command line arguments
     :param config: :class:`~.configfiles.ConfigFiles` object
     """
 
     _keybindings_description = (
         "You can cancel any command with Escape, Ctrl+c or Ctrl+g.\n"
         "\n"
-        "In the TUI, the usual Emacs keybindings are supported. Here is an incomplete list:\n"
+        "In the TUI, the usual readline/Emacs keybindings are supported. Here is an incomplete list:\n"
         "\n"
         "  Ctrl+f         Move forward character-wise\n"
         "  Ctrl+b         Move backward character-wise\n"
         "  Alt+f          Move forward word-wise\n"
         "  Alt+b          Move backward word-wise\n"
         "  Ctrl+a         Move leftmost position\n"
         "  Ctrl+e         Move rightmost position\n"
```

### Comparing `upsies-2023.5.25/upsies/uis/tui/commands/mediainfo.py` & `upsies-2023.6.11/upsies/uis/tui/commands/mediainfo.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/commands/poster.py` & `upsies-2023.6.11/upsies/uis/tui/commands/poster.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/commands/release_name.py` & `upsies-2023.6.11/upsies/uis/tui/commands/release_name.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/commands/scene.py` & `upsies-2023.6.11/upsies/uis/tui/commands/scene.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/commands/screenshots.py` & `upsies-2023.6.11/upsies/uis/tui/commands/screenshots.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/commands/set.py` & `upsies-2023.6.11/upsies/uis/tui/commands/set.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/commands/submit.py` & `upsies-2023.6.11/upsies/uis/tui/commands/submit.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,13 +192,14 @@
             return utils.btclient.BtClient(
                 name=client_name,
                 url=options['url'],
                 username=options['username'],
                 password=options['password'],
                 download_path=utils.fs.dirname(os.path.abspath(self.args.CONTENT)),
                 check_after_add=options['check_after_add'],
+                category=options.get('category', ''),
             )
 
     def _get_torrent_destination(self):
         return (getattr(self.args, 'copy_to', None)
                 or self.tracker_options.get('copy_to', None)
                 or None)
```

### Comparing `upsies-2023.5.25/upsies/uis/tui/commands/torrent.py` & `upsies-2023.6.11/upsies/uis/tui/commands/torrent.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,15 @@
                 btclient=utils.btclient.BtClient(
                     name=client_name,
                     url=options['url'],
                     username=options['username'],
                     password=options['password'],
                     download_path=self.args.download_path,
                     check_after_add=options['check_after_add'],
+                    category=options.get('category', ''),
                 ),
                 enqueue=self.args.TORRENT,
             ),
         )
 
 
 class torrent_create(CommandBase):
@@ -169,14 +170,15 @@
                 btclient=utils.btclient.BtClient(
                     name=client_name,
                     url=options['url'],
                     username=options['username'],
                     password=options['password'],
                     download_path=utils.fs.dirname(os.path.abspath(self.args.CONTENT)),
                     check_after_add=options['check_after_add'],
+                    category=options.get('category', ''),
                 ),
             )
 
             # Pass CreateTorrentJob output to AddTorrentJob input.
             self.create_torrent_job.signal.register('output', add_torrent_job.enqueue)
 
             # Finish AddTorrentJob when CreateTorrentJob is finished. The
```

### Comparing `upsies-2023.5.25/upsies/uis/tui/commands/upload_images.py` & `upsies-2023.6.11/upsies/uis/tui/commands/upload_images.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/commands/webdb.py` & `upsies-2023.6.11/upsies/uis/tui/commands/webdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/headless.py` & `upsies-2023.6.11/upsies/uis/tui/headless.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/jobwidgets/__init__.py` & `upsies-2023.6.11/upsies/uis/tui/jobwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/jobwidgets/base.py` & `upsies-2023.6.11/upsies/uis/tui/jobwidgets/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/jobwidgets/dialog.py` & `upsies-2023.6.11/upsies/uis/tui/jobwidgets/dialog.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/jobwidgets/imghost.py` & `upsies-2023.6.11/upsies/uis/tui/jobwidgets/imghost.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/jobwidgets/poster.py` & `upsies-2023.6.11/upsies/uis/tui/jobwidgets/poster.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/jobwidgets/scene.py` & `upsies-2023.6.11/upsies/uis/tui/jobwidgets/scene.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/jobwidgets/screenshots.py` & `upsies-2023.6.11/upsies/uis/tui/jobwidgets/screenshots.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/jobwidgets/submit.py` & `upsies-2023.6.11/upsies/uis/tui/jobwidgets/submit.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/jobwidgets/webdb.py` & `upsies-2023.6.11/upsies/uis/tui/jobwidgets/webdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/main.py` & `upsies-2023.6.11/upsies/uis/tui/main.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/style.py` & `upsies-2023.6.11/upsies/uis/tui/style.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/tui.py` & `upsies-2023.6.11/upsies/uis/tui/tui.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/utils.py` & `upsies-2023.6.11/upsies/uis/tui/utils.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/uis/tui/widgets.py` & `upsies-2023.6.11/upsies/uis/tui/widgets.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/__init__.py` & `upsies-2023.6.11/upsies/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/argtypes.py` & `upsies-2023.6.11/upsies/utils/argtypes.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/configfiles.py` & `upsies-2023.6.11/upsies/utils/configfiles.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/country.py` & `upsies-2023.6.11/upsies/utils/country.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/daemon.py` & `upsies-2023.6.11/upsies/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/fs.py` & `upsies-2023.6.11/upsies/utils/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,20 @@
         oldest_files = sorted(filepaths, key=atime)
         files_to_remove = [oldest_files.pop(0)]
         while combined_size(files_to_remove) < size_diff:
             files_to_remove.append(oldest_files.pop(0))
 
         # Actually remove the files
         for file_to_remove in files_to_remove:
-            os.unlink(file_to_remove)
+            # It's possible another process already unlinked this file while we
+            # were still collecting old files.
+            try:
+                os.unlink(file_to_remove)
+            except FileNotFoundError:
+                pass
 
 
 def prune_empty(path, files=False, directories=True):
     """
     Remove empty subdirectories recursively
 
     :param path: Path to directory
```

### Comparing `upsies-2023.5.25/upsies/utils/html.py` & `upsies-2023.6.11/upsies/utils/html.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/http.py` & `upsies-2023.6.11/upsies/utils/http.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/image.py` & `upsies-2023.6.11/upsies/utils/image.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/imghosts/__init__.py` & `upsies-2023.6.11/upsies/utils/imghosts/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/imghosts/base.py` & `upsies-2023.6.11/upsies/utils/imghosts/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/imghosts/common.py` & `upsies-2023.6.11/upsies/utils/imghosts/common.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/imghosts/dummy.py` & `upsies-2023.6.11/upsies/utils/imghosts/dummy.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/imghosts/freeimage.py` & `upsies-2023.6.11/upsies/utils/imghosts/freeimage.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/imghosts/imgbb.py` & `upsies-2023.6.11/upsies/utils/imghosts/imgbb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/imghosts/imgbox.py` & `upsies-2023.6.11/upsies/utils/imghosts/imgbox.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/imghosts/ptpimg.py` & `upsies-2023.6.11/upsies/utils/imghosts/ptpimg.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/predbs/__init__.py` & `upsies-2023.6.11/upsies/utils/predbs/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/predbs/base.py` & `upsies-2023.6.11/upsies/utils/predbs/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,16 +45,20 @@
 
     @property
     @abc.abstractmethod
     def default_config(self):
         """Default user configuration as a dictionary"""
 
     @abc.abstractmethod
-    async def _search(self, keywords, group=None):
-        pass
+    async def _search(self, query):
+        """
+        Perform search
+
+        :param SceneQuery query: Search keywords
+        """
 
     async def search(self, query, only_existing_releases=True):
         """
         Search for scene release
 
         If there are no results and `query` is a directory path that looks like
         a season pack, perform one search per video file in that directory or
@@ -74,17 +78,17 @@
         if isinstance(query, str):
             path = query
             query = utils.predbs.SceneQuery.from_string(query)
         elif isinstance(query, collections.abc.Mapping):
             query = utils.predbs.SceneQuery.from_release(query)
 
         try:
-            results = list(await self._search(query.keywords, group=query.group))
+            results = list(await self._search(query))
         except NotImplementedError:
-            raise errors.RequestError(f'{self.name} does not support this query')
+            raise errors.RequestError(f'{self.name} does not support searching')
 
         if not results and path:
             # Maybe `path` points to season pack?
             # Find episodes and search for them individually.
             return await self._search_for_episodes(path, only_existing_releases)
         else:
             return self._postprocess_search_results(results, query, only_existing_releases)
@@ -177,15 +181,15 @@
         :param str release_name: Exact name of the release
 
         :raise RequestError: if request fails or `release_name` is not found
         """
         try:
             files = await self._release_files(release_name)
         except NotImplementedError:
-            raise errors.RequestError(f'{self.name} does not support this query')
+            raise errors.RequestError(f'{self.name} does not provide file information')
 
         if files:
             return files
         else:
             _log.debug('No such release: %r', release_name)
             files = {}
```

### Comparing `upsies-2023.5.25/upsies/utils/predbs/common.py` & `upsies-2023.6.11/upsies/utils/predbs/common.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/predbs/corruptnet.py` & `upsies-2023.6.11/upsies/utils/predbs/corruptnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 
     # This seems to be specified by the server?
     _results_per_page = 50
 
     # Seems reasonable?
     _max_pages = 10
 
-    async def _search(self, keywords, group):
+    async def _search(self, query):
         combined_results = []
         max_page_value = self._max_pages * self._results_per_page
         for page in range(0, max_page_value, self._results_per_page):
-            results = list(await self._request_page(keywords, group, page))
+            results = list(await self._request_page(query.keywords, query.group, page))
             combined_results.extend(results)
             if len(results) < self._results_per_page:
                 break
         return combined_results
 
     async def _request_page(self, keywords, group, page):
         params = {
```

### Comparing `upsies-2023.5.25/upsies/utils/predbs/multi.py` & `upsies-2023.6.11/upsies/utils/predbs/multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,25 +83,42 @@
         # All predbs are unreachable or don't have `method_name` implemented.
         self._raise(exceptions, method_name)
 
     async def _for_all_predbs(self, method_name, *args, **kwargs):
         # Call `method_name` on all predbs concurrently and yield the return
         # value or RequestError/NotImplementedError as they occur.
         method_calls = [
-            self._call(predb, method_name, *args, **kwargs)
+            asyncio.create_task(
+                self._call(predb, method_name, *args, **kwargs)
+            )
             for predb in self._predbs
         ]
 
-        for coro in asyncio.as_completed(method_calls):
-            try:
-                result = await coro
-            except (NotImplementedError, errors.RequestError) as e:
-                yield e
-            else:
-                yield result
+        try:
+            for coro in asyncio.as_completed(method_calls):
+                try:
+                    result = await coro
+                except (NotImplementedError, errors.RequestError) as e:
+                    yield e
+                else:
+                    yield result
+        finally:
+            # If our caller stops iterating over our yielded `result`s, we may
+            # still have unfinished tasks that will continue to run in the
+            # background. We cancel them here because
+            #   1. nobody cares about their return values anymore
+            #
+            #   2. if one of the tasks raises an exception, asyncio will
+            #      eventually complain about an unhandled exception. Cancelling
+            #      the tasks seems to prevents that.
+            #
+            # NOTE: This is untested functionality because I couldn't reproduce
+            #       this issue in a test case.
+            for task in method_calls:
+                task.cancel()
 
     @async_lru.alru_cache
     async def search(self, *args, **kwargs):
         """
         Search multiple predbs concurrently and return first non-empty results
 
         See :meth:`~.PredbApiBase.search`.
```

### Comparing `upsies-2023.5.25/upsies/utils/predbs/predbclub.py` & `upsies-2023.6.11/upsies/utils/predbs/predbclub.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     label = 'PreDB.club'
 
     default_config = {}
 
     _url_base = b64decode('aHR0cHM6Ly9wcmVkYi5jbHVi').decode('ascii')
     _search_url = f'{_url_base}/api/v1/'
 
-    async def _search(self, keywords, group):
-        q = self._get_q(keywords, group)
+    async def _search(self, query):
+        q = self._get_q(query.keywords, query.group)
         return await self._request_all_pages(q)
 
     def _get_q(self, keywords, group):
         if group:
             keywords = list(keywords)
             keywords.extend(('@team', str(group).replace('@', r'\@').strip()))
         kws = (str(kw).lower().strip() for kw in keywords)
```

### Comparing `upsies-2023.5.25/upsies/utils/predbs/predbde.py` & `upsies-2023.6.11/upsies/utils/predbs/predbde.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     label = 'PreDB.de'
 
     default_config = {}
 
     _url_base = b64decode('cHJlZGIuZGU=').decode('ascii')
     _search_url = f'https://{_url_base}/api/'
 
-    async def _search(self, keywords, group):
-        q = self._get_q(keywords, group)
+    async def _search(self, query):
+        q = self._get_q(query.keywords, query.group)
         if q:
             return await self._request_all_pages(q)
         else:
             return ()
 
     def _get_q(self, keywords, group):
         kws = list(keywords)
@@ -58,27 +58,32 @@
         params = {
             'q': q,
             'page': page,
         }
         _log.debug('%s search: %r, %r', self.label, self._search_url, params)
         response = (await http.get(self._search_url, params=params, cache=True)).json()
 
-        # Report API error or return list of release names
-        if response['status'] != 'success':
+        if response.get('data'):
+            # We found at least one release
+            results = tuple(result['release'] for result in response['data'])
+
+        elif (
+                response.get('status') != 'success'
+                and response.get('message')
+                and response['message'].lower() != 'no results'
+        ):
+            # Report error from API
             raise errors.RequestError(f'{self.label}: {response["message"]}')
+
         else:
-            # Extract release names
-            if response['data']:
-                results = tuple(result['release'] for result in response['data'])
-            else:
-                results = ()
+            results = ()
 
-            # Is there another page of results?
-            if len(results) >= self._max_results_per_page:
-                next_page = page + 1
-            else:
-                next_page = -1
+        # Is there another page of results?
+        if len(results) >= self._max_results_per_page:
+            next_page = page + 1
+        else:
+            next_page = -1
 
-            return results, next_page
+        return results, next_page
 
     async def _release_files(self, release_name):
         raise NotImplementedError()
```

### Comparing `upsies-2023.5.25/upsies/utils/predbs/predbovh.py` & `upsies-2023.6.11/upsies/utils/predbs/predbovh.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     label = 'PreDB.ovh'
 
     default_config = {}
 
     _url_base = b64decode('cHJlZGIub3Zo').decode('ascii')
     _search_url = f'https://{_url_base}/api/v1/'
 
-    async def _search(self, keywords, group):
-        q = self._get_q(keywords, group)
+    async def _search(self, query):
+        q = self._get_q(query.keywords, query.group)
         return await self._request_all_pages(q)
 
     def _get_q(self, keywords, group):
         if group:
             keywords = list(keywords)
             keywords.extend(('@team', str(group).replace('@', r'\@').strip()))
         kws = (str(kw).lower().strip() for kw in keywords)
```

### Comparing `upsies-2023.5.25/upsies/utils/predbs/query.py` & `upsies-2023.6.11/upsies/utils/predbs/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Query scene release
 """
 
 import re
 
-from ... import errors, utils
+from ... import utils
 
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
 natsort = utils.LazyModule(module='natsort', namespace=globals())
 
 
@@ -34,33 +34,33 @@
         """
         Create query from `string`
 
         :param string: Release name or path to release content
 
         `string` is passed to :class:`~.release.ReleaseInfo` and the result is
         passed to :meth:`from_release`.
-
-        :raise SceneError: if :class:`~.release.ReleaseInfo` raises
-            :class:`~.errors.ContentError`
         """
-        try:
-            return cls.from_release(utils.release.ReleaseInfo(string, strict=False))
-        except errors.ContentError as e:
-            raise errors.SceneError(e)
+        release = utils.release.ReleaseInfo(string, strict=False)
+        return cls.from_release(release)
 
     @classmethod
     def from_release(cls, release):
         """
         Create query from :class:`dict`-like object
 
         :param release: :class:`~.release.ReleaseName` or
             :class:`~.release.ReleaseInfo` instance or any :class:`dict`-like
             object with the keys ``type``, ``title``, ``year``, ``episodes``,
             ``resolution``, ``source``, ``video_codec`` and ``group``.
         """
+        if isinstance(release, utils.release.ReleaseName):
+            release = release.release_info
+
+        original_release = release.copy()
+
         # Replace H.264/5 with H264/5
         release['video_codec'] = re.sub(r'\.', '', release.get('video_codec', ''))
 
         # Replace WEB-DL with WEB
         if release.get('source') == 'WEB-DL':
             release['source'] = 'WEB'
 
@@ -80,18 +80,19 @@
         keywords = [release[key] for key in needed_keys
                     if key in release]
 
         query = cls(
             *keywords,
             group=release.get('group', ''),
             episodes=release.get('episodes', {}),
+            release_info=original_release,
         )
         return query
 
-    def __init__(self, *keywords, group='', episodes={}):
+    def __init__(self, *keywords, group='', episodes={}, release_info=None):
         # Split each keyword at spaces
         kws = (k.strip()
                for kw in keywords
                for k in str(kw).split())
 
         # Remove season packs (keep "SxxEyy" but not "Sxx") because scene
         # releases are not season packs and we don't find anything if we look
@@ -113,14 +114,15 @@
         # (I forgot why "-" is removed. Please explain if you know!)
         kws = (kw for kw in kws
                if kw and kw != '-')
 
         self._keywords = tuple(kws)
         self._group = str(group) if group else None
         self._episodes = episodes
+        self._release_info = release_info
 
     @property
     def keywords(self):
         """Sequence of search terms"""
         return self._keywords
 
     @property
@@ -129,14 +131,19 @@
         return self._group
 
     @property
     def episodes(self):
         """:class:`~.release.Episodes`-like mapping"""
         return self._episodes
 
+    @property
+    def release_info(self):
+        """:class:`~.ReleaseInfo` object this query was created from or `None`"""
+        return self._release_info
+
     def __repr__(self):
         args = []
         if self.keywords:
             args.append(', '.join((repr(kw) for kw in self.keywords)))
         if self.group:
             args.append(f'group={self.group!r}')
         if self.episodes:
```

### Comparing `upsies-2023.5.25/upsies/utils/signal.py` & `upsies-2023.6.11/upsies/utils/signal.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/string.py` & `upsies-2023.6.11/upsies/utils/string.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/subproc.py` & `upsies-2023.6.11/upsies/utils/subproc.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/subtitle.py` & `upsies-2023.6.11/upsies/utils/subtitle.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/timestamp.py` & `upsies-2023.6.11/upsies/utils/timestamp.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/torrent.py` & `upsies-2023.6.11/upsies/utils/torrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,22 +76,22 @@
         a :class:`CreateTorrentProgress` or :class:`FindTorrentProgress` object
         as a positional argument
 
     Callbacks can cancel the torrent creation by returning `True` or any other
     truthy value. If `progress_callback` returns :data:`SKIP_SEARCHING`, the
     search for a reusable torrent is cancelled and pieces are hashed normally.
 
-    :raise TorrentError: if anything goes wrong
+    :raise TorrentCreateError: if anything goes wrong
 
     :return: `torrent_path` or `None` if cancelled
     """
     if not announce:
-        raise errors.TorrentError('Announce URL is empty')
+        raise errors.TorrentCreateError('Announce URL is empty')
     if not source:
-        raise errors.TorrentError('Source is empty')
+        raise errors.TorrentCreateError('Source is empty')
 
     # Create Torrent object
     torrent = _get_torrent(
         content_path=content_path,
         exclude=_get_exclude_regexs(exclude),
         announce=announce,
         source=source,
@@ -160,26 +160,26 @@
             source=source,
             randomize_infohash=randomize_infohash,
             private=True,
             created_by=f'{__project_name__} {__version__}',
             creation_date=time.time(),
         )
     except torf.TorfError as e:
-        raise errors.TorrentError(str(e))
+        raise errors.TorrentCreateError(str(e))
 
 
 def _generate_hashes(*, torrent, callback):
     wrapped_callback = _CreateTorrentCallback(callback)
     try:
         torrent.generate(
             callback=wrapped_callback,
             interval=1.0,
         )
     except torf.TorfError as e:
-        raise errors.TorrentError(str(e))
+        raise errors.TorrentCreateError(str(e))
     else:
         return wrapped_callback.return_value
 
 
 def _find_hashes(*, torrent, reuse_torrent_path, callback):
     if not torrent.files:
         # All files are excluded (let someone deal with it)
@@ -189,15 +189,15 @@
     try:
         torrent.reuse(
             _get_reuse_torrent_paths(torrent, reuse_torrent_path),
             callback=wrapped_callback,
             interval=1.0,
         )
     except torf.TorfError as e:
-        raise errors.TorrentError(str(e))
+        raise errors.TorrentCreateError(str(e))
     else:
         return wrapped_callback.return_value
 
 
 def _get_reuse_torrent_paths(torrent, reuse_torrent_path):
     reuse_torrent_paths = []
     if reuse_torrent_path:
@@ -225,24 +225,24 @@
     generic_torrent.write(generic_torrent_path, overwrite=True)
 
 
 def _write_torrent_path(torrent, torrent_path):
     try:
         torrent.write(torrent_path, overwrite=True)
     except torf.TorfError as e:
-        raise errors.TorrentError(str(e))
+        raise errors.TorrentCreateError(str(e))
 
 
 def _get_generic_torrent_path(torrent, create_directory=True):
     directory = constants.GENERIC_TORRENTS_DIRPATH
     if create_directory:
         try:
             fs.mkdir(directory)
         except errors.ContentError as e:
-            raise errors.TorrentError(f'{directory}: {e}')
+            raise errors.TorrentCreateError(f'{directory}: {e}')
 
     cache_id = _get_torrent_id(torrent)
     filename = f'{torrent.name}.{cache_id}.torrent'
     return os.path.join(directory, filename)
 
 
 def _get_torrent_id_info(torrent):
@@ -446,15 +446,15 @@
         progress = FindTorrentProgress(
             files_done=files_done,
             files_total=files_total,
             percent_done=info['percent_done'],
             files_per_second=info['items_per_second'],
             filepath=filepath,
             status=status,
-            exception=errors.TorrentError(str(exception)) if exception else None,
+            exception=errors.TorrentCreateError(str(exception)) if exception else None,
             seconds_elapsed=info['seconds_elapsed'],
             seconds_remaining=info['seconds_remaining'],
             seconds_total=info['seconds_total'],
             time_finished=info['time_finished'],
             time_started=info['time_started'],
         )
         return super().__call__(progress)
@@ -511,15 +511,15 @@
         'time_finished',
         'time_started',
     ),
 )):
     """
     :func:`~.collections.namedtuple` with these attributes:
 
-        - ``exception`` (:class:`~.errors.TorrentError` or `None`)
+        - ``exception`` (:class:`~.errors.TorrentCreateError` or `None`)
         - ``filepath`` (:class:`str`)
         - ``files_done`` (:class:`int`)
         - ``files_per_second`` (:class:`int`)
         - ``files_total`` (:class:`int`)
         - ``percent_done`` (:class:`float`)
         - ``seconds_elapsed`` (:class:`~.datetime.datetime.timedelta`)
         - ``seconds_remaining`` (:class:`~.datetime.datetime.timedelta`)
@@ -546,11 +546,11 @@
         torrent = _get_torrent(
             content_path=content_path,
             exclude=_get_exclude_regexs(exclude),
             announce='http://dummy.local',
             source=None,
             randomize_infohash=False,
         )
-    except errors.TorrentError as e:
+    except errors.TorrentCreateError as e:
         raise errors.ContentError(e)
     else:
         return [str(f) for f in torrent.filepaths]
```

### Comparing `upsies-2023.5.25/upsies/utils/types.py` & `upsies-2023.6.11/upsies/utils/types.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/update.py` & `upsies-2023.6.11/upsies/utils/update.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/video.py` & `upsies-2023.6.11/upsies/utils/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,29 +417,35 @@
     try:
         return int(video_track['BitDepth'])
     except (KeyError, ValueError):
         return 0
 
 
 hdr_formats = {
-    'Dolby Vision': {'HDR_Format': re.compile(r'^Dolby Vision$')},
+    'DV': {
+        # Dolby Vision[ / <more information>]
+        'HDR_Format': re.compile(r'^Dolby Vision'),
+    },
     # "HDR10+ Profile A" or "HDR10+ Profile B"
-    'HDR10+': {'HDR_Format_Compatibility': re.compile(r'HDR10\+')},
+    'HDR10+': {
+        'HDR_Format_Compatibility': re.compile(r'HDR10\+'),
+    },
     'HDR10': (
         {'HDR_Format_Compatibility': re.compile(r'HDR10(?!\+)')},
         {'colour_primaries': re.compile(r'BT\.2020')},
     ),
     'HDR': (
         {'HDR_Format_Compatibility': re.compile(r'HDR')},
         {'HDR_Format': re.compile(r'HDR')},
     ),
 }
 """
-Map HDR format names (e.g. "Dolby Vision") to dictinaries that map mediainfo
-video track fields to regular expressions that must match the fields' values
+Map HDR format names (e.g. "Dolby Vision") to dictionaries that map
+mediainfo video track fields to regular expressions that must match the fields'
+values
 """
 
 @functools.lru_cache(maxsize=None)
 def hdr_format(path, default=NO_DEFAULT_VALUE):
     """
     Return HDR format based on `hdr_formats`, e.g. "HDR10", or empty string
```

### Comparing `upsies-2023.5.25/upsies/utils/webdbs/__init__.py` & `upsies-2023.6.11/upsies/utils/webdbs/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/webdbs/base.py` & `upsies-2023.6.11/upsies/utils/webdbs/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/webdbs/common.py` & `upsies-2023.6.11/upsies/utils/webdbs/common.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/webdbs/imdb.py` & `upsies-2023.6.11/upsies/utils/webdbs/imdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/webdbs/tmdb.py` & `upsies-2023.6.11/upsies/utils/webdbs/tmdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies/utils/webdbs/tvmaze.py` & `upsies-2023.6.11/upsies/utils/webdbs/tvmaze.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.5.25/upsies.egg-info/PKG-INFO` & `upsies-2023.6.11/upsies.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: upsies
-Version: 2023.5.25
+Version: 2023.6.11
 Summary: Media metadata aggregator
-Home-page: https://upsies.readthedocs.io
-Author: plotski
-Author-email: plotski@example.org
+Author-email: plotski <plotski@example.org>
+License: GPL-3.0-or-later
+Project-URL: Repository, https://codeberg.org/plotski/upsies
+Project-URL: Documentation, https://upsies.readthedocs.io
+Project-URL: Bug Tracker, https://codeberg.org/plotski/upsies/issues
+Project-URL: Changelog, https://codeberg.org/plotski/upsies/raw/branch/master/NEWS
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: dev
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/pyversions/upsies
            :target: https://www.python.org/
 .. image:: https://img.shields.io/pypi/l/upsies
            :target: https://www.gnu.org/licenses/gpl-3.0.en.html
 .. image:: https://img.shields.io/pypi/v/upsies
```

