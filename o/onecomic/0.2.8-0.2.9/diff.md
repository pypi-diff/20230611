# Comparing `tmp/onecomic-0.2.8.tar.gz` & `tmp/onecomic-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onecomic-0.2.8.tar", last modified: Sun Jul 11 15:11:30 2021, max compression
+gzip compressed data, was "dist/onecomic-0.2.9.tar", last modified: Sat Jul 17 03:04:06 2021, max compression
```

## Comparing `onecomic-0.2.8.tar` & `onecomic-0.2.9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-11 15:11:30.000000 onecomic-0.2.8/
--rwxrwxrwx   0 key       (1000) key       (1000)    35149 2021-01-30 03:49:09.000000 onecomic-0.2.8/LICENSE
--rwxrwxrwx   0 key       (1000) key       (1000)       25 2021-04-15 14:51:13.000000 onecomic-0.2.8/MANIFEST.in
--rwxrwxrwx   0 key       (1000) key       (1000)     1155 2021-07-11 15:11:30.000000 onecomic-0.2.8/PKG-INFO
--rwxrwxrwx   0 key       (1000) key       (1000)      413 2021-02-09 02:41:36.000000 onecomic-0.2.8/README.md
-drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-11 15:11:30.000000 onecomic-0.2.8/bin/
--rwxrwxrwx   0 key       (1000) key       (1000)       60 2021-02-14 15:13:51.000000 onecomic-0.2.8/bin/onecomic
-drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-11 15:11:30.000000 onecomic-0.2.8/onecomic/
--rwxrwxrwx   0 key       (1000) key       (1000)       60 2021-07-11 15:09:46.000000 onecomic-0.2.8/onecomic/__init__.py
--rwxrwxrwx   0 key       (1000) key       (1000)       52 2021-01-30 03:49:09.000000 onecomic-0.2.8/onecomic/__main__.py
--rwxrwxrwx   0 key       (1000) key       (1000)    16833 2021-06-20 12:42:07.000000 onecomic-0.2.8/onecomic/cli.py
--rwxrwxrwx   0 key       (1000) key       (1000)    13844 2021-04-10 12:56:18.000000 onecomic-0.2.8/onecomic/comicbook.py
--rwxrwxrwx   0 key       (1000) key       (1000)     4529 2021-06-20 12:41:44.000000 onecomic-0.2.8/onecomic/config.py
--rwxrwxrwx   0 key       (1000) key       (1000)    14904 2021-07-10 05:21:03.000000 onecomic-0.2.8/onecomic/crawlerbase.py
--rwxrwxrwx   0 key       (1000) key       (1000)     1156 2021-03-09 14:42:54.000000 onecomic-0.2.8/onecomic/exceptions.py
--rwxrwxrwx   0 key       (1000) key       (1000)     4858 2021-06-20 13:28:34.000000 onecomic-0.2.8/onecomic/image.py
-drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-11 15:11:30.000000 onecomic-0.2.8/onecomic/js/
--rwxrwxrwx   0 key       (1000) key       (1000)     4485 2021-01-30 03:49:09.000000 onecomic-0.2.8/onecomic/js/cocomanhua.js
--rwxrwxrwx   0 key       (1000) key       (1000)    13069 2021-04-15 14:52:47.000000 onecomic-0.2.8/onecomic/js/laimanhua_base64.js
--rwxrwxrwx   0 key       (1000) key       (1000)      325 2021-01-30 03:49:09.000000 onecomic-0.2.8/onecomic/patch.py
-drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-11 15:11:30.000000 onecomic-0.2.8/onecomic/proxy/
--rwxrwxrwx   0 key       (1000) key       (1000)      794 2021-03-27 07:45:40.000000 onecomic-0.2.8/onecomic/proxy/__init__.py
--rwxrwxrwx   0 key       (1000) key       (1000)      587 2021-06-27 03:17:05.000000 onecomic-0.2.8/onecomic/proxy/kuaidaili.py
--rwxrwxrwx   0 key       (1000) key       (1000)     3411 2021-06-26 01:46:33.000000 onecomic-0.2.8/onecomic/session.py
-drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-11 15:11:30.000000 onecomic-0.2.8/onecomic/site/
--rwxrwxrwx   0 key       (1000) key       (1000)        0 2021-01-30 17:05:03.000000 onecomic-0.2.8/onecomic/site/__init__.py
--rwxrwxrwx   0 key       (1000) key       (1000)     4761 2021-03-10 13:01:17.000000 onecomic-0.2.8/onecomic/site/acg456.py
--rwxrwxrwx   0 key       (1000) key       (1000)    10216 2021-04-10 13:24:35.000000 onecomic-0.2.8/onecomic/site/bilibili.py
--rwxrwxrwx   0 key       (1000) key       (1000)     6570 2021-07-11 02:33:27.000000 onecomic-0.2.8/onecomic/site/boodo.py
--rwxrwxrwx   0 key       (1000) key       (1000)     4915 2021-03-10 13:01:39.000000 onecomic-0.2.8/onecomic/site/c177pic.py
--rwxrwxrwx   0 key       (1000) key       (1000)     6705 2021-04-04 08:25:31.000000 onecomic-0.2.8/onecomic/site/c18comic.py
--rwxrwxrwx   0 key       (1000) key       (1000)     3743 2021-03-10 13:03:30.000000 onecomic-0.2.8/onecomic/site/c18hmmcg.py
--rwxrwxrwx   0 key       (1000) key       (1000)     6686 2021-03-10 13:08:21.000000 onecomic-0.2.8/onecomic/site/c2animx.py
--rwxrwxrwx   0 key       (1000) key       (1000)     2635 2021-04-04 08:40:34.000000 onecomic-0.2.8/onecomic/site/c2feimh.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5330 2021-07-11 02:33:38.000000 onecomic-0.2.8/onecomic/site/c3250mh.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5056 2021-03-10 13:08:38.000000 onecomic-0.2.8/onecomic/site/c36mh.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5370 2021-06-20 12:57:47.000000 onecomic-0.2.8/onecomic/site/c55comic.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5833 2021-06-26 01:15:57.000000 onecomic-0.2.8/onecomic/site/c77mh.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5639 2021-04-10 13:52:16.000000 onecomic-0.2.8/onecomic/site/cocomanhua.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5924 2021-06-26 01:01:48.000000 onecomic-0.2.8/onecomic/site/copymanga.py
--rwxrwxrwx   0 key       (1000) key       (1000)     8418 2021-06-26 01:11:47.000000 onecomic-0.2.8/onecomic/site/dm5.py
--rwxrwxrwx   0 key       (1000) key       (1000)     6351 2021-06-26 01:13:07.000000 onecomic-0.2.8/onecomic/site/dmzj.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5274 2021-07-04 14:08:27.000000 onecomic-0.2.8/onecomic/site/gufengmh8.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5992 2021-06-26 01:07:10.000000 onecomic-0.2.8/onecomic/site/jmzj.py
--rwxrwxrwx   0 key       (1000) key       (1000)     6442 2021-06-26 01:39:27.000000 onecomic-0.2.8/onecomic/site/kuaikan.py
--rwxrwxrwx   0 key       (1000) key       (1000)     6056 2021-04-15 14:52:29.000000 onecomic-0.2.8/onecomic/site/laimanhua.py
--rwxrwxrwx   0 key       (1000) key       (1000)     6391 2021-03-10 13:12:46.000000 onecomic-0.2.8/onecomic/site/manhuadb.py
--rwxrwxrwx   0 key       (1000) key       (1000)     8888 2021-07-11 13:58:34.000000 onecomic-0.2.8/onecomic/site/manhuagui.py
--rwxrwxrwx   0 key       (1000) key       (1000)     4060 2021-03-10 13:13:12.000000 onecomic-0.2.8/onecomic/site/manhuatai.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5295 2021-04-10 12:35:32.000000 onecomic-0.2.8/onecomic/site/mh1234.py
--rwxrwxrwx   0 key       (1000) key       (1000)     6284 2021-06-26 01:58:49.000000 onecomic-0.2.8/onecomic/site/mh160.py
--rwxrwxrwx   0 key       (1000) key       (1000)     3778 2021-03-10 13:14:25.000000 onecomic-0.2.8/onecomic/site/mmkk.py
--rwxrwxrwx   0 key       (1000) key       (1000)     8240 2021-07-11 15:06:44.000000 onecomic-0.2.8/onecomic/site/myfcomic.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5237 2021-03-10 13:14:50.000000 onecomic-0.2.8/onecomic/site/nhentai.py
--rwxrwxrwx   0 key       (1000) key       (1000)     4642 2021-06-26 01:35:25.000000 onecomic-0.2.8/onecomic/site/nvshens.py
--rwxrwxrwx   0 key       (1000) key       (1000)     2705 2021-06-26 01:36:04.000000 onecomic-0.2.8/onecomic/site/picxxxx.py
--rwxrwxrwx   0 key       (1000) key       (1000)     4035 2021-03-10 13:15:54.000000 onecomic-0.2.8/onecomic/site/pufei8.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5111 2021-06-26 11:31:11.000000 onecomic-0.2.8/onecomic/site/qiman6.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5892 2021-06-26 12:35:07.000000 onecomic-0.2.8/onecomic/site/qimiaomh.py
--rwxrwxrwx   0 key       (1000) key       (1000)     4413 2021-06-20 13:30:15.000000 onecomic-0.2.8/onecomic/site/qootoon.py
--rwxrwxrwx   0 key       (1000) key       (1000)     7497 2021-03-10 13:18:51.000000 onecomic-0.2.8/onecomic/site/qq.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5120 2021-06-26 11:31:22.000000 onecomic-0.2.8/onecomic/site/sixmh6.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5309 2021-06-26 01:46:42.000000 onecomic-0.2.8/onecomic/site/toomics.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5938 2021-03-10 13:19:15.000000 onecomic-0.2.8/onecomic/site/tuhao456.py
--rwxrwxrwx   0 key       (1000) key       (1000)     5700 2021-06-26 01:35:46.000000 onecomic-0.2.8/onecomic/site/twhentai.py
--rwxrwxrwx   0 key       (1000) key       (1000)     7489 2021-03-10 13:19:59.000000 onecomic-0.2.8/onecomic/site/u17.py
--rwxrwxrwx   0 key       (1000) key       (1000)     4127 2021-06-26 00:52:41.000000 onecomic-0.2.8/onecomic/site/webtoons.py
--rwxrwxrwx   0 key       (1000) key       (1000)     6249 2021-06-26 01:31:36.000000 onecomic-0.2.8/onecomic/site/wnacg.py
--rwxrwxrwx   0 key       (1000) key       (1000)     3965 2021-03-10 13:21:06.000000 onecomic-0.2.8/onecomic/site/xiuren.py
--rwxrwxrwx   0 key       (1000) key       (1000)     3394 2021-04-10 13:24:58.000000 onecomic-0.2.8/onecomic/site/ykmh.py
--rwxrwxrwx   0 key       (1000) key       (1000)     7174 2021-03-11 14:21:13.000000 onecomic-0.2.8/onecomic/site/yymh889.py
-drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-11 15:11:30.000000 onecomic-0.2.8/onecomic/utils/
--rwxrwxrwx   0 key       (1000) key       (1000)     5248 2021-01-30 03:49:09.000000 onecomic-0.2.8/onecomic/utils/__init__.py
--rwxrwxrwx   0 key       (1000) key       (1000)     2658 2021-01-30 03:49:09.000000 onecomic-0.2.8/onecomic/utils/_img2pdf.py
--rwxrwxrwx   0 key       (1000) key       (1000)     2940 2021-01-30 03:49:09.000000 onecomic-0.2.8/onecomic/utils/mail.py
--rwxrwxrwx   0 key       (1000) key       (1000)     1154 2021-01-30 03:49:09.000000 onecomic-0.2.8/onecomic/worker.py
-drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-11 15:11:30.000000 onecomic-0.2.8/onecomic.egg-info/
--rwxrwxrwx   0 key       (1000) key       (1000)     1155 2021-07-11 15:11:29.000000 onecomic-0.2.8/onecomic.egg-info/PKG-INFO
--rwxrwxrwx   0 key       (1000) key       (1000)     1785 2021-07-11 15:11:29.000000 onecomic-0.2.8/onecomic.egg-info/SOURCES.txt
--rwxrwxrwx   0 key       (1000) key       (1000)        1 2021-07-11 15:11:29.000000 onecomic-0.2.8/onecomic.egg-info/dependency_links.txt
--rwxrwxrwx   0 key       (1000) key       (1000)       73 2021-07-11 15:11:29.000000 onecomic-0.2.8/onecomic.egg-info/requires.txt
--rwxrwxrwx   0 key       (1000) key       (1000)        9 2021-07-11 15:11:29.000000 onecomic-0.2.8/onecomic.egg-info/top_level.txt
--rwxrwxrwx   0 key       (1000) key       (1000)      131 2021-07-11 15:11:30.000000 onecomic-0.2.8/setup.cfg
--rwxrwxrwx   0 key       (1000) key       (1000)     3541 2021-06-26 01:28:20.000000 onecomic-0.2.8/setup.py
-drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-11 15:11:30.000000 onecomic-0.2.8/test/
--rwxrwxrwx   0 key       (1000) key       (1000)     4454 2021-07-11 15:08:55.000000 onecomic-0.2.8/test/test_crawler.py
+drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-17 03:04:06.000000 onecomic-0.2.9/
+-rwxrwxrwx   0 key       (1000) key       (1000)    35149 2021-01-30 03:49:09.000000 onecomic-0.2.9/LICENSE
+-rwxrwxrwx   0 key       (1000) key       (1000)       25 2021-04-15 14:51:13.000000 onecomic-0.2.9/MANIFEST.in
+-rwxrwxrwx   0 key       (1000) key       (1000)     1155 2021-07-17 03:04:06.000000 onecomic-0.2.9/PKG-INFO
+-rwxrwxrwx   0 key       (1000) key       (1000)      413 2021-02-09 02:41:36.000000 onecomic-0.2.9/README.md
+drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-17 03:04:06.000000 onecomic-0.2.9/bin/
+-rwxrwxrwx   0 key       (1000) key       (1000)       60 2021-02-14 15:13:51.000000 onecomic-0.2.9/bin/onecomic
+drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-17 03:04:06.000000 onecomic-0.2.9/onecomic/
+-rwxrwxrwx   0 key       (1000) key       (1000)       60 2021-07-17 03:03:45.000000 onecomic-0.2.9/onecomic/__init__.py
+-rwxrwxrwx   0 key       (1000) key       (1000)       52 2021-01-30 03:49:09.000000 onecomic-0.2.9/onecomic/__main__.py
+-rwxrwxrwx   0 key       (1000) key       (1000)    16833 2021-06-20 12:42:07.000000 onecomic-0.2.9/onecomic/cli.py
+-rwxrwxrwx   0 key       (1000) key       (1000)    13844 2021-04-10 12:56:18.000000 onecomic-0.2.9/onecomic/comicbook.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     4529 2021-06-20 12:41:44.000000 onecomic-0.2.9/onecomic/config.py
+-rwxrwxrwx   0 key       (1000) key       (1000)    14904 2021-07-10 05:21:03.000000 onecomic-0.2.9/onecomic/crawlerbase.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     1156 2021-03-09 14:42:54.000000 onecomic-0.2.9/onecomic/exceptions.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     4858 2021-06-20 13:28:34.000000 onecomic-0.2.9/onecomic/image.py
+drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-17 03:04:06.000000 onecomic-0.2.9/onecomic/js/
+-rwxrwxrwx   0 key       (1000) key       (1000)     4485 2021-01-30 03:49:09.000000 onecomic-0.2.9/onecomic/js/cocomanhua.js
+-rwxrwxrwx   0 key       (1000) key       (1000)    13069 2021-04-15 14:52:47.000000 onecomic-0.2.9/onecomic/js/laimanhua_base64.js
+-rwxrwxrwx   0 key       (1000) key       (1000)      325 2021-01-30 03:49:09.000000 onecomic-0.2.9/onecomic/patch.py
+drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-17 03:04:06.000000 onecomic-0.2.9/onecomic/proxy/
+-rwxrwxrwx   0 key       (1000) key       (1000)      794 2021-03-27 07:45:40.000000 onecomic-0.2.9/onecomic/proxy/__init__.py
+-rwxrwxrwx   0 key       (1000) key       (1000)      587 2021-06-27 03:17:05.000000 onecomic-0.2.9/onecomic/proxy/kuaidaili.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     3411 2021-06-26 01:46:33.000000 onecomic-0.2.9/onecomic/session.py
+drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-17 03:04:06.000000 onecomic-0.2.9/onecomic/site/
+-rwxrwxrwx   0 key       (1000) key       (1000)        0 2021-01-30 17:05:03.000000 onecomic-0.2.9/onecomic/site/__init__.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     4761 2021-03-10 13:01:17.000000 onecomic-0.2.9/onecomic/site/acg456.py
+-rwxrwxrwx   0 key       (1000) key       (1000)    10216 2021-04-10 13:24:35.000000 onecomic-0.2.9/onecomic/site/bilibili.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     6570 2021-07-11 02:33:27.000000 onecomic-0.2.9/onecomic/site/boodo.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     4915 2021-03-10 13:01:39.000000 onecomic-0.2.9/onecomic/site/c177pic.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     6705 2021-04-04 08:25:31.000000 onecomic-0.2.9/onecomic/site/c18comic.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     3743 2021-03-10 13:03:30.000000 onecomic-0.2.9/onecomic/site/c18hmmcg.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     6686 2021-03-10 13:08:21.000000 onecomic-0.2.9/onecomic/site/c2animx.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     2635 2021-04-04 08:40:34.000000 onecomic-0.2.9/onecomic/site/c2feimh.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5732 2021-07-17 03:02:28.000000 onecomic-0.2.9/onecomic/site/c3250mh.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5056 2021-03-10 13:08:38.000000 onecomic-0.2.9/onecomic/site/c36mh.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5370 2021-06-20 12:57:47.000000 onecomic-0.2.9/onecomic/site/c55comic.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5833 2021-06-26 01:15:57.000000 onecomic-0.2.9/onecomic/site/c77mh.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5639 2021-04-10 13:52:16.000000 onecomic-0.2.9/onecomic/site/cocomanhua.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5924 2021-06-26 01:01:48.000000 onecomic-0.2.9/onecomic/site/copymanga.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     8418 2021-06-26 01:11:47.000000 onecomic-0.2.9/onecomic/site/dm5.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     6351 2021-06-26 01:13:07.000000 onecomic-0.2.9/onecomic/site/dmzj.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5274 2021-07-04 14:08:27.000000 onecomic-0.2.9/onecomic/site/gufengmh8.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5992 2021-06-26 01:07:10.000000 onecomic-0.2.9/onecomic/site/jmzj.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     6442 2021-06-26 01:39:27.000000 onecomic-0.2.9/onecomic/site/kuaikan.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     6056 2021-04-15 14:52:29.000000 onecomic-0.2.9/onecomic/site/laimanhua.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     6391 2021-03-10 13:12:46.000000 onecomic-0.2.9/onecomic/site/manhuadb.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     8888 2021-07-11 13:58:34.000000 onecomic-0.2.9/onecomic/site/manhuagui.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     4060 2021-03-10 13:13:12.000000 onecomic-0.2.9/onecomic/site/manhuatai.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5295 2021-04-10 12:35:32.000000 onecomic-0.2.9/onecomic/site/mh1234.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     6284 2021-06-26 01:58:49.000000 onecomic-0.2.9/onecomic/site/mh160.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     3778 2021-03-10 13:14:25.000000 onecomic-0.2.9/onecomic/site/mmkk.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     8240 2021-07-11 15:06:44.000000 onecomic-0.2.9/onecomic/site/myfcomic.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5237 2021-03-10 13:14:50.000000 onecomic-0.2.9/onecomic/site/nhentai.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     4642 2021-06-26 01:35:25.000000 onecomic-0.2.9/onecomic/site/nvshens.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     2705 2021-06-26 01:36:04.000000 onecomic-0.2.9/onecomic/site/picxxxx.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     4035 2021-03-10 13:15:54.000000 onecomic-0.2.9/onecomic/site/pufei8.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5111 2021-06-26 11:31:11.000000 onecomic-0.2.9/onecomic/site/qiman6.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5892 2021-06-26 12:35:07.000000 onecomic-0.2.9/onecomic/site/qimiaomh.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     4413 2021-06-20 13:30:15.000000 onecomic-0.2.9/onecomic/site/qootoon.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     7497 2021-03-10 13:18:51.000000 onecomic-0.2.9/onecomic/site/qq.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5120 2021-06-26 11:31:22.000000 onecomic-0.2.9/onecomic/site/sixmh6.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5309 2021-06-26 01:46:42.000000 onecomic-0.2.9/onecomic/site/toomics.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5938 2021-03-10 13:19:15.000000 onecomic-0.2.9/onecomic/site/tuhao456.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     5700 2021-06-26 01:35:46.000000 onecomic-0.2.9/onecomic/site/twhentai.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     7489 2021-03-10 13:19:59.000000 onecomic-0.2.9/onecomic/site/u17.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     4127 2021-06-26 00:52:41.000000 onecomic-0.2.9/onecomic/site/webtoons.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     6249 2021-06-26 01:31:36.000000 onecomic-0.2.9/onecomic/site/wnacg.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     3965 2021-03-10 13:21:06.000000 onecomic-0.2.9/onecomic/site/xiuren.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     3394 2021-04-10 13:24:58.000000 onecomic-0.2.9/onecomic/site/ykmh.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     7174 2021-03-11 14:21:13.000000 onecomic-0.2.9/onecomic/site/yymh889.py
+drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-17 03:04:06.000000 onecomic-0.2.9/onecomic/utils/
+-rwxrwxrwx   0 key       (1000) key       (1000)     5248 2021-01-30 03:49:09.000000 onecomic-0.2.9/onecomic/utils/__init__.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     2658 2021-01-30 03:49:09.000000 onecomic-0.2.9/onecomic/utils/_img2pdf.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     2940 2021-01-30 03:49:09.000000 onecomic-0.2.9/onecomic/utils/mail.py
+-rwxrwxrwx   0 key       (1000) key       (1000)     1154 2021-01-30 03:49:09.000000 onecomic-0.2.9/onecomic/worker.py
+drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-17 03:04:06.000000 onecomic-0.2.9/onecomic.egg-info/
+-rwxrwxrwx   0 key       (1000) key       (1000)     1155 2021-07-17 03:04:06.000000 onecomic-0.2.9/onecomic.egg-info/PKG-INFO
+-rwxrwxrwx   0 key       (1000) key       (1000)     1785 2021-07-17 03:04:06.000000 onecomic-0.2.9/onecomic.egg-info/SOURCES.txt
+-rwxrwxrwx   0 key       (1000) key       (1000)        1 2021-07-17 03:04:06.000000 onecomic-0.2.9/onecomic.egg-info/dependency_links.txt
+-rwxrwxrwx   0 key       (1000) key       (1000)       73 2021-07-17 03:04:06.000000 onecomic-0.2.9/onecomic.egg-info/requires.txt
+-rwxrwxrwx   0 key       (1000) key       (1000)        9 2021-07-17 03:04:06.000000 onecomic-0.2.9/onecomic.egg-info/top_level.txt
+-rwxrwxrwx   0 key       (1000) key       (1000)      131 2021-07-17 03:04:06.000000 onecomic-0.2.9/setup.cfg
+-rwxrwxrwx   0 key       (1000) key       (1000)     3541 2021-06-26 01:28:20.000000 onecomic-0.2.9/setup.py
+drwxrwxrwx   0 key       (1000) key       (1000)        0 2021-07-17 03:04:06.000000 onecomic-0.2.9/test/
+-rwxrwxrwx   0 key       (1000) key       (1000)     4454 2021-07-11 15:08:55.000000 onecomic-0.2.9/test/test_crawler.py
```

### Comparing `onecomic-0.2.8/LICENSE` & `onecomic-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/PKG-INFO` & `onecomic-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onecomic
-Version: 0.2.8
+Version: 0.2.9
 Summary: onecomic
 Home-page: https://github.com/hardwarecode/onecomic
 Author: hardwarecode
 Author-email: 
 License: GPL-3.0 License
 Description: 
         # 一本漫画
```

### Comparing `onecomic-0.2.8/onecomic/cli.py` & `onecomic-0.2.9/onecomic/cli.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/comicbook.py` & `onecomic-0.2.9/onecomic/comicbook.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/config.py` & `onecomic-0.2.9/onecomic/config.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/crawlerbase.py` & `onecomic-0.2.9/onecomic/crawlerbase.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/exceptions.py` & `onecomic-0.2.9/onecomic/exceptions.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/image.py` & `onecomic-0.2.9/onecomic/image.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/js/cocomanhua.js` & `onecomic-0.2.9/onecomic/js/cocomanhua.js`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/js/laimanhua_base64.js` & `onecomic-0.2.9/onecomic/js/laimanhua_base64.js`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/proxy/__init__.py` & `onecomic-0.2.9/onecomic/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/proxy/kuaidaili.py` & `onecomic-0.2.9/onecomic/proxy/kuaidaili.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/session.py` & `onecomic-0.2.9/onecomic/session.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/acg456.py` & `onecomic-0.2.9/onecomic/site/acg456.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/bilibili.py` & `onecomic-0.2.9/onecomic/site/bilibili.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/boodo.py` & `onecomic-0.2.9/onecomic/site/boodo.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/c177pic.py` & `onecomic-0.2.9/onecomic/site/c177pic.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/c18comic.py` & `onecomic-0.2.9/onecomic/site/c18comic.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/c18hmmcg.py` & `onecomic-0.2.9/onecomic/site/c18hmmcg.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/c2animx.py` & `onecomic-0.2.9/onecomic/site/c2animx.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/c2feimh.py` & `onecomic-0.2.9/onecomic/site/c2feimh.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/c3250mh.py` & `onecomic-0.2.9/onecomic/site/c3250mh.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,21 @@
             pass
         return book
 
     def get_chapter_image_urls(self, citem):
         soup = self.get_soup(citem.source_url)
         image_urls = [div.img.get('src') for div in
                       soup.find('div', {'class': 'comiclist'}).find_all('div', {'class': 'comicpage'})]
+        pages = [i.get('value') for i in soup.find("select", {'class': "selectpage"}).find_all('option')]
+        for page in pages[1:]:
+            soup = self.get_soup(citem.source_url, params={'page': page})
+            image_urls.extend(
+                [div.img.get('src') for div in
+                 soup.find('div', {'class': 'comiclist'}).find_all('div', {'class': 'comicpage'})]
+            )
         return image_urls
 
     def latest(self, page=1):
         url = urljoin(self.SITE_INDEX, "/update.html?page=%s" % page)
         soup = self.get_soup(url)
         result = self.new_search_result_item()
         for li in soup.find('ul', {'class': 'comic-update'}).find_all('li'):
```

### Comparing `onecomic-0.2.8/onecomic/site/c36mh.py` & `onecomic-0.2.9/onecomic/site/c36mh.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/c55comic.py` & `onecomic-0.2.9/onecomic/site/c55comic.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/c77mh.py` & `onecomic-0.2.9/onecomic/site/c77mh.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/cocomanhua.py` & `onecomic-0.2.9/onecomic/site/cocomanhua.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/copymanga.py` & `onecomic-0.2.9/onecomic/site/copymanga.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/dm5.py` & `onecomic-0.2.9/onecomic/site/dm5.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/dmzj.py` & `onecomic-0.2.9/onecomic/site/dmzj.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/gufengmh8.py` & `onecomic-0.2.9/onecomic/site/gufengmh8.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/jmzj.py` & `onecomic-0.2.9/onecomic/site/jmzj.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/kuaikan.py` & `onecomic-0.2.9/onecomic/site/kuaikan.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/laimanhua.py` & `onecomic-0.2.9/onecomic/site/laimanhua.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/manhuadb.py` & `onecomic-0.2.9/onecomic/site/manhuadb.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/manhuagui.py` & `onecomic-0.2.9/onecomic/site/manhuagui.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/manhuatai.py` & `onecomic-0.2.9/onecomic/site/manhuatai.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/mh1234.py` & `onecomic-0.2.9/onecomic/site/mh1234.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/mh160.py` & `onecomic-0.2.9/onecomic/site/mh160.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/mmkk.py` & `onecomic-0.2.9/onecomic/site/mmkk.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/myfcomic.py` & `onecomic-0.2.9/onecomic/site/myfcomic.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/nhentai.py` & `onecomic-0.2.9/onecomic/site/nhentai.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/nvshens.py` & `onecomic-0.2.9/onecomic/site/nvshens.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/picxxxx.py` & `onecomic-0.2.9/onecomic/site/picxxxx.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/pufei8.py` & `onecomic-0.2.9/onecomic/site/pufei8.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/qiman6.py` & `onecomic-0.2.9/onecomic/site/qiman6.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/qimiaomh.py` & `onecomic-0.2.9/onecomic/site/qimiaomh.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/qootoon.py` & `onecomic-0.2.9/onecomic/site/qootoon.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/qq.py` & `onecomic-0.2.9/onecomic/site/qq.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/sixmh6.py` & `onecomic-0.2.9/onecomic/site/sixmh6.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/toomics.py` & `onecomic-0.2.9/onecomic/site/toomics.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/tuhao456.py` & `onecomic-0.2.9/onecomic/site/tuhao456.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/twhentai.py` & `onecomic-0.2.9/onecomic/site/twhentai.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/u17.py` & `onecomic-0.2.9/onecomic/site/u17.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/webtoons.py` & `onecomic-0.2.9/onecomic/site/webtoons.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/wnacg.py` & `onecomic-0.2.9/onecomic/site/wnacg.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/xiuren.py` & `onecomic-0.2.9/onecomic/site/xiuren.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/ykmh.py` & `onecomic-0.2.9/onecomic/site/ykmh.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/site/yymh889.py` & `onecomic-0.2.9/onecomic/site/yymh889.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/utils/__init__.py` & `onecomic-0.2.9/onecomic/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/utils/_img2pdf.py` & `onecomic-0.2.9/onecomic/utils/_img2pdf.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/utils/mail.py` & `onecomic-0.2.9/onecomic/utils/mail.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic/worker.py` & `onecomic-0.2.9/onecomic/worker.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/onecomic.egg-info/PKG-INFO` & `onecomic-0.2.9/onecomic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onecomic
-Version: 0.2.8
+Version: 0.2.9
 Summary: onecomic
 Home-page: https://github.com/hardwarecode/onecomic
 Author: hardwarecode
 Author-email: 
 License: GPL-3.0 License
 Description: 
         # 一本漫画
```

### Comparing `onecomic-0.2.8/onecomic.egg-info/SOURCES.txt` & `onecomic-0.2.9/onecomic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/setup.py` & `onecomic-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `onecomic-0.2.8/test/test_crawler.py` & `onecomic-0.2.9/test/test_crawler.py`

 * *Files identical despite different names*

