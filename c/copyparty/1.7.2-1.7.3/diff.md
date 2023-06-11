# Comparing `tmp/copyparty-1.7.2.tar.gz` & `tmp/copyparty-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copyparty-1.7.2.tar", last modified: Sat May 13 00:35:13 2023, max compression
+gzip compressed data, was "copyparty-1.7.3.tar", last modified: Sun Jun 11 00:47:49 2023, max compression
```

## Comparing `copyparty-1.7.2.tar` & `copyparty-1.7.3.tar`

### file list

```diff
@@ -1,122 +1,123 @@
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-05-13 00:35:13.243510 copyparty-1.7.2/
--rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-11 12:44:53.000000 copyparty-1.7.2/LICENSE
--rw-r--r--   0 ed        (1000) ed        (1000)    95704 2023-05-13 00:35:13.243510 copyparty-1.7.2/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)    93754 2023-05-13 00:04:44.000000 copyparty-1.7.2/README.md
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-05-13 00:35:13.230510 copyparty-1.7.2/copyparty/
--rw-r--r--   0 ed        (1000) ed        (1000)     1063 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/__init__.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    68805 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/__main__.py
--rw-r--r--   0 ed        (1000) ed        (1000)      249 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/__version__.py
--rw-r--r--   0 ed        (1000) ed        (1000)    65881 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/authsrv.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-05-13 00:35:13.232510 copyparty-1.7.2/copyparty/bos/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/bos/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1560 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/bos/bos.py
--rw-r--r--   0 ed        (1000) ed        (1000)      777 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/bos/path.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3590 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/broker_mp.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3200 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/broker_mpw.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1759 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/broker_thr.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1489 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/broker_util.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6714 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/cfg.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1548 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/dxml.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3932 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/fsutil.py
--rw-r--r--   0 ed        (1000) ed        (1000)    15258 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/ftpd.py
--rw-r--r--   0 ed        (1000) ed        (1000)   122643 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/httpcli.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6891 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/httpconn.py
--rw-r--r--   0 ed        (1000) ed        (1000)    15141 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/httpsrv.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2643 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/ico.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16978 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/mdns.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16844 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/mtag.py
--rw-r--r--   0 ed        (1000) ed        (1000)    11520 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/multicast.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-05-13 00:35:13.232510 copyparty-1.7.2/copyparty/res/
--rw-r--r--   0 ed        (1000) ed        (1000)    10570 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/res/COPYING.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/res/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2876 2023-04-23 21:16:05.000000 copyparty-1.7.2/copyparty/res/insecure.pem
--rw-r--r--   0 ed        (1000) ed        (1000)    10623 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/smbd.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6153 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/ssdp.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2699 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/star.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-05-13 00:35:13.232510 copyparty-1.7.2/copyparty/stolen/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/__init__.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-05-13 00:35:13.234510 copyparty-1.7.2/copyparty/stolen/dnslib/
--rw-r--r--   0 ed        (1000) ed        (1000)      159 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/dnslib/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1182 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/dnslib/bimap.py
--rw-r--r--   0 ed        (1000) ed        (1000)      348 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/dnslib/bit.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1407 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/dnslib/buffer.py
--rw-r--r--   0 ed        (1000) ed        (1000)    20956 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/dnslib/dns.py
--rw-r--r--   0 ed        (1000) ed        (1000)     4893 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/dnslib/label.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2615 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/dnslib/lex.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1810 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/dnslib/ranges.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-05-13 00:35:13.234510 copyparty-1.7.2/copyparty/stolen/ifaddr/
--rw-r--r--   0 ed        (1000) ed        (1000)      463 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/ifaddr/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2626 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/ifaddr/_posix.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6111 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/ifaddr/_shared.py
--rw-r--r--   0 ed        (1000) ed        (1000)     4026 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/ifaddr/_win32.py
--rw-r--r--   0 ed        (1000) ed        (1000)    21469 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/qrcodegen.py
--rw-r--r--   0 ed        (1000) ed        (1000)     5573 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/stolen/surrogateescape.py
--rw-r--r--   0 ed        (1000) ed        (1000)      972 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/sutil.py
--rw-r--r--   0 ed        (1000) ed        (1000)    23625 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/svchub.py
--rw-r--r--   0 ed        (1000) ed        (1000)     8166 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/szip.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16643 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/tcpsrv.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3826 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/th_cli.py
--rw-r--r--   0 ed        (1000) ed        (1000)    22379 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/th_srv.py
--rw-r--r--   0 ed        (1000) ed        (1000)    10585 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/u2idx.py
--rw-r--r--   0 ed        (1000) ed        (1000)   121996 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/up2k.py
--rw-r--r--   0 ed        (1000) ed        (1000)    71993 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/util.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-05-13 00:35:13.238510 copyparty-1.7.2/copyparty/web/
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-05-13 00:35:13.238510 copyparty-1.7.2/copyparty/web/a/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/web/a/__init__.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    32276 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/web/a/partyfuse.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    36247 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/web/a/u2c.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1449 2023-02-20 20:21:49.000000 copyparty-1.7.2/copyparty/web/a/webdav-cfg.bat
--rw-r--r--   0 ed        (1000) ed        (1000)     7296 2023-03-30 21:17:33.000000 copyparty-1.7.2/copyparty/web/baguettebox.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    10960 2023-04-27 21:10:24.000000 copyparty-1.7.2/copyparty/web/browser.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     5286 2023-03-15 22:20:24.000000 copyparty-1.7.2/copyparty/web/browser.html
--rw-r--r--   0 ed        (1000) ed        (1000)    59129 2023-05-11 07:59:05.000000 copyparty-1.7.2/copyparty/web/browser.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1604 2022-12-10 19:54:48.000000 copyparty-1.7.2/copyparty/web/browser2.html
--rw-r--r--   0 ed        (1000) ed        (1000)      585 2022-07-03 13:28:49.000000 copyparty-1.7.2/copyparty/web/cf.html
--rw-r--r--   0 ed        (1000) ed        (1000)      688 2022-07-14 21:26:48.000000 copyparty-1.7.2/copyparty/web/dbg-audio.js.gz
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-05-13 00:35:13.239510 copyparty-1.7.2/copyparty/web/dd/
--rw-r--r--   0 ed        (1000) ed        (1000)      258 2021-09-11 12:44:53.000000 copyparty-1.7.2/copyparty/web/dd/2.png
--rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.7.2/copyparty/web/dd/3.png
--rw-r--r--   0 ed        (1000) ed        (1000)      248 2021-09-11 12:44:53.000000 copyparty-1.7.2/copyparty/web/dd/4.png
--rw-r--r--   0 ed        (1000) ed        (1000)      250 2021-09-11 12:44:53.000000 copyparty-1.7.2/copyparty/web/dd/5.png
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/web/dd/__init__.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-05-13 00:35:13.242510 copyparty-1.7.2/copyparty/web/deps/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-05-13 00:34:58.000000 copyparty-1.7.2/copyparty/web/deps/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3053 2023-02-20 10:55:39.000000 copyparty-1.7.2/copyparty/web/deps/easymde.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    76953 2023-04-01 14:48:07.000000 copyparty-1.7.2/copyparty/web/deps/easymde.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    14819 2023-04-01 14:47:51.000000 copyparty-1.7.2/copyparty/web/deps/marked.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      584 2023-04-01 14:48:09.000000 copyparty-1.7.2/copyparty/web/deps/mini-fa.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2784 2023-04-01 14:48:09.000000 copyparty-1.7.2/copyparty/web/deps/mini-fa.woff
--rw-r--r--   0 ed        (1000) ed        (1000)     1478 2022-12-29 03:41:18.000000 copyparty-1.7.2/copyparty/web/deps/prism.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    41428 2022-12-29 03:41:18.000000 copyparty-1.7.2/copyparty/web/deps/prism.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1647 2022-12-29 03:41:18.000000 copyparty-1.7.2/copyparty/web/deps/prismd.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8612 2023-04-01 14:48:10.000000 copyparty-1.7.2/copyparty/web/deps/scp.woff2
--rw-r--r--   0 ed        (1000) ed        (1000)     7043 2023-04-01 14:23:12.000000 copyparty-1.7.2/copyparty/web/deps/sha512.ac.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8119 2021-07-22 23:48:12.000000 copyparty-1.7.2/copyparty/web/deps/sha512.hw.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2011 2022-10-30 15:38:07.000000 copyparty-1.7.2/copyparty/web/md.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     4063 2022-12-10 20:27:29.000000 copyparty-1.7.2/copyparty/web/md.html
--rw-r--r--   0 ed        (1000) ed        (1000)     4121 2023-03-26 01:52:00.000000 copyparty-1.7.2/copyparty/web/md.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      681 2022-12-01 22:41:28.000000 copyparty-1.7.2/copyparty/web/md2.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8213 2023-01-25 20:58:01.000000 copyparty-1.7.2/copyparty/web/md2.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      929 2022-04-15 15:07:16.000000 copyparty-1.7.2/copyparty/web/mde.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1640 2022-12-10 20:27:33.000000 copyparty-1.7.2/copyparty/web/mde.html
--rw-r--r--   0 ed        (1000) ed        (1000)     2219 2022-12-01 07:23:41.000000 copyparty-1.7.2/copyparty/web/mde.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.7.2/copyparty/web/msg.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      898 2022-12-10 19:57:40.000000 copyparty-1.7.2/copyparty/web/msg.html
--rw-r--r--   0 ed        (1000) ed        (1000)      927 2023-02-17 22:46:57.000000 copyparty-1.7.2/copyparty/web/splash.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     3741 2023-02-19 19:41:20.000000 copyparty-1.7.2/copyparty/web/splash.html
--rw-r--r--   0 ed        (1000) ed        (1000)     1235 2023-02-17 22:28:18.000000 copyparty-1.7.2/copyparty/web/splash.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    10610 2023-05-07 15:13:28.000000 copyparty-1.7.2/copyparty/web/svcs.html
--rw-r--r--   0 ed        (1000) ed        (1000)      520 2022-12-04 17:10:33.000000 copyparty-1.7.2/copyparty/web/svcs.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2419 2023-03-26 02:06:03.000000 copyparty-1.7.2/copyparty/web/ui.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    21544 2023-05-12 23:46:23.000000 copyparty-1.7.2/copyparty/web/up2k.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    13074 2023-05-06 18:53:00.000000 copyparty-1.7.2/copyparty/web/util.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1060 2023-03-02 22:42:45.000000 copyparty-1.7.2/copyparty/web/w.hash.js.gz
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-05-13 00:35:13.231510 copyparty-1.7.2/copyparty.egg-info/
--rw-r--r--   0 ed        (1000) ed        (1000)    95704 2023-05-13 00:35:13.000000 copyparty-1.7.2/copyparty.egg-info/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)     2790 2023-05-13 00:35:13.000000 copyparty-1.7.2/copyparty.egg-info/SOURCES.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        1 2023-05-13 00:35:13.000000 copyparty-1.7.2/copyparty.egg-info/dependency_links.txt
--rw-r--r--   0 ed        (1000) ed        (1000)      128 2023-05-13 00:35:13.000000 copyparty-1.7.2/copyparty.egg-info/entry_points.txt
--rw-r--r--   0 ed        (1000) ed        (1000)      117 2023-05-13 00:35:13.000000 copyparty-1.7.2/copyparty.egg-info/requires.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       10 2023-05-13 00:35:13.000000 copyparty-1.7.2/copyparty.egg-info/top_level.txt
--rw-r--r--   0 ed        (1000) ed        (1000)     4041 2023-05-07 18:02:24.000000 copyparty-1.7.2/pyproject.toml
--rw-r--r--   0 ed        (1000) ed        (1000)       38 2023-05-13 00:35:13.243510 copyparty-1.7.2/setup.cfg
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:49.147480 copyparty-1.7.3/
+-rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-11 12:44:53.000000 copyparty-1.7.3/LICENSE
+-rw-r--r--   0 ed        (1000) ed        (1000)    96291 2023-06-11 00:47:49.147480 copyparty-1.7.3/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)    94341 2023-06-10 22:25:29.000000 copyparty-1.7.3/README.md
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:49.135480 copyparty-1.7.3/copyparty/
+-rw-r--r--   0 ed        (1000) ed        (1000)     1812 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/__init__.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    70633 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/__main__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      249 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/__version__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    65881 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/authsrv.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:49.136480 copyparty-1.7.3/copyparty/bos/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/bos/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1560 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/bos/bos.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      777 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/bos/path.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3590 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/broker_mp.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3200 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/broker_mpw.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1759 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/broker_thr.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1489 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/broker_util.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     7036 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/cert.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6843 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/cfg.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1548 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/dxml.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3932 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/fsutil.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    15317 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/ftpd.py
+-rw-r--r--   0 ed        (1000) ed        (1000)   122873 2023-06-11 00:47:35.000000 copyparty-1.7.3/copyparty/httpcli.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6755 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/httpconn.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    15372 2023-06-11 00:47:35.000000 copyparty-1.7.3/copyparty/httpsrv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2643 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/ico.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    17205 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/mdns.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    16844 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/mtag.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    11520 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/multicast.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:49.137480 copyparty-1.7.3/copyparty/res/
+-rw-r--r--   0 ed        (1000) ed        (1000)    10570 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/res/COPYING.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/res/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2876 2023-04-23 21:16:05.000000 copyparty-1.7.3/copyparty/res/insecure.pem
+-rw-r--r--   0 ed        (1000) ed        (1000)    10623 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/smbd.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6379 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/ssdp.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2699 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/star.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:49.137480 copyparty-1.7.3/copyparty/stolen/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/__init__.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:49.138480 copyparty-1.7.3/copyparty/stolen/dnslib/
+-rw-r--r--   0 ed        (1000) ed        (1000)      159 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/dnslib/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1182 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/dnslib/bimap.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      348 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/dnslib/bit.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1407 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/dnslib/buffer.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    20956 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/dnslib/dns.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     4893 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/dnslib/label.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2615 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/dnslib/lex.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1810 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/dnslib/ranges.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:49.138480 copyparty-1.7.3/copyparty/stolen/ifaddr/
+-rw-r--r--   0 ed        (1000) ed        (1000)      463 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/ifaddr/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2626 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/ifaddr/_posix.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6111 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/ifaddr/_shared.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     4026 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/ifaddr/_win32.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    21469 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/qrcodegen.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     5573 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/stolen/surrogateescape.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      972 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/sutil.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    23803 2023-06-11 00:47:35.000000 copyparty-1.7.3/copyparty/svchub.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     8166 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/szip.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    16721 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/tcpsrv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3826 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/th_cli.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    22379 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/th_srv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    10585 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/u2idx.py
+-rw-r--r--   0 ed        (1000) ed        (1000)   121996 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/up2k.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    72070 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/util.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:49.142480 copyparty-1.7.3/copyparty/web/
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:49.143480 copyparty-1.7.3/copyparty/web/a/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/web/a/__init__.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    32276 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/web/a/partyfuse.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    36247 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/web/a/u2c.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1449 2023-02-20 20:21:49.000000 copyparty-1.7.3/copyparty/web/a/webdav-cfg.bat
+-rw-r--r--   0 ed        (1000) ed        (1000)     7296 2023-03-30 21:17:33.000000 copyparty-1.7.3/copyparty/web/baguettebox.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    10963 2023-06-02 22:21:36.000000 copyparty-1.7.3/copyparty/web/browser.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     5317 2023-06-02 21:39:24.000000 copyparty-1.7.3/copyparty/web/browser.html
+-rw-r--r--   0 ed        (1000) ed        (1000)    59183 2023-06-02 21:41:19.000000 copyparty-1.7.3/copyparty/web/browser.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1604 2022-12-10 19:54:48.000000 copyparty-1.7.3/copyparty/web/browser2.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      585 2022-07-03 13:28:49.000000 copyparty-1.7.3/copyparty/web/cf.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      688 2022-07-14 21:26:48.000000 copyparty-1.7.3/copyparty/web/dbg-audio.js.gz
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:49.143480 copyparty-1.7.3/copyparty/web/dd/
+-rw-r--r--   0 ed        (1000) ed        (1000)      258 2021-09-11 12:44:53.000000 copyparty-1.7.3/copyparty/web/dd/2.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.7.3/copyparty/web/dd/3.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      248 2021-09-11 12:44:53.000000 copyparty-1.7.3/copyparty/web/dd/4.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      250 2021-09-11 12:44:53.000000 copyparty-1.7.3/copyparty/web/dd/5.png
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/web/dd/__init__.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:49.146480 copyparty-1.7.3/copyparty/web/deps/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:34.000000 copyparty-1.7.3/copyparty/web/deps/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3053 2023-02-20 10:55:39.000000 copyparty-1.7.3/copyparty/web/deps/easymde.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    76953 2023-04-01 14:48:07.000000 copyparty-1.7.3/copyparty/web/deps/easymde.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    14819 2023-04-01 14:47:51.000000 copyparty-1.7.3/copyparty/web/deps/marked.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      584 2023-04-01 14:48:09.000000 copyparty-1.7.3/copyparty/web/deps/mini-fa.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2784 2023-04-01 14:48:09.000000 copyparty-1.7.3/copyparty/web/deps/mini-fa.woff
+-rw-r--r--   0 ed        (1000) ed        (1000)     1478 2022-12-29 03:41:18.000000 copyparty-1.7.3/copyparty/web/deps/prism.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    41428 2022-12-29 03:41:18.000000 copyparty-1.7.3/copyparty/web/deps/prism.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1647 2022-12-29 03:41:18.000000 copyparty-1.7.3/copyparty/web/deps/prismd.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8612 2023-04-01 14:48:10.000000 copyparty-1.7.3/copyparty/web/deps/scp.woff2
+-rw-r--r--   0 ed        (1000) ed        (1000)     7043 2023-04-01 14:23:12.000000 copyparty-1.7.3/copyparty/web/deps/sha512.ac.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8119 2021-07-22 23:48:12.000000 copyparty-1.7.3/copyparty/web/deps/sha512.hw.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2011 2022-10-30 15:38:07.000000 copyparty-1.7.3/copyparty/web/md.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     4063 2022-12-10 20:27:29.000000 copyparty-1.7.3/copyparty/web/md.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     4121 2023-03-26 01:52:00.000000 copyparty-1.7.3/copyparty/web/md.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      681 2022-12-01 22:41:28.000000 copyparty-1.7.3/copyparty/web/md2.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8213 2023-01-25 20:58:01.000000 copyparty-1.7.3/copyparty/web/md2.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      929 2022-04-15 15:07:16.000000 copyparty-1.7.3/copyparty/web/mde.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1640 2022-12-10 20:27:33.000000 copyparty-1.7.3/copyparty/web/mde.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     2219 2022-12-01 07:23:41.000000 copyparty-1.7.3/copyparty/web/mde.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.7.3/copyparty/web/msg.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      898 2022-12-10 19:57:40.000000 copyparty-1.7.3/copyparty/web/msg.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      927 2023-02-17 22:46:57.000000 copyparty-1.7.3/copyparty/web/splash.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     3741 2023-02-19 19:41:20.000000 copyparty-1.7.3/copyparty/web/splash.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     1235 2023-02-17 22:28:18.000000 copyparty-1.7.3/copyparty/web/splash.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    10610 2023-05-07 15:13:28.000000 copyparty-1.7.3/copyparty/web/svcs.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      520 2022-12-04 17:10:33.000000 copyparty-1.7.3/copyparty/web/svcs.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2419 2023-03-26 02:06:03.000000 copyparty-1.7.3/copyparty/web/ui.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    21544 2023-05-12 23:46:23.000000 copyparty-1.7.3/copyparty/web/up2k.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    13063 2023-06-10 23:48:10.000000 copyparty-1.7.3/copyparty/web/util.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1060 2023-03-02 22:42:45.000000 copyparty-1.7.3/copyparty/web/w.hash.js.gz
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 00:47:49.135480 copyparty-1.7.3/copyparty.egg-info/
+-rw-r--r--   0 ed        (1000) ed        (1000)    96291 2023-06-11 00:47:49.000000 copyparty-1.7.3/copyparty.egg-info/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)     2808 2023-06-11 00:47:49.000000 copyparty-1.7.3/copyparty.egg-info/SOURCES.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        1 2023-06-11 00:47:49.000000 copyparty-1.7.3/copyparty.egg-info/dependency_links.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)      128 2023-06-11 00:47:49.000000 copyparty-1.7.3/copyparty.egg-info/entry_points.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)      117 2023-06-11 00:47:49.000000 copyparty-1.7.3/copyparty.egg-info/requires.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)       10 2023-06-11 00:47:49.000000 copyparty-1.7.3/copyparty.egg-info/top_level.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)     4007 2023-06-02 21:51:58.000000 copyparty-1.7.3/pyproject.toml
+-rw-r--r--   0 ed        (1000) ed        (1000)       38 2023-06-11 00:47:49.147480 copyparty-1.7.3/setup.cfg
```

### Comparing `copyparty-1.7.2/LICENSE` & `copyparty-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/PKG-INFO` & `copyparty-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyparty
-Version: 1.7.2
+Version: 1.7.3
 Summary:   Portable file server with accelerated resumable uploads, deduplication, WebDAV, FTP, zeroconf, media indexer, video thumbnails, audio transcoding, and write-only folders
 Author-email: ed <copyparty@ocv.me>
 License: MIT
 Project-URL: Source Code, https://github.com/9001/copyparty
 Project-URL: Bug Tracker, https://github.com/9001/copyparty/issues
 Project-URL: Demo Server, https://a.ocv.me/pub/demo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -509,24 +509,26 @@
 * `[↵]` toggles wordwrap
 * `[👀]` show full name on hover (if wordwrap is off)
 
 
 ## thumbnails
 
 press `g` or `田` to toggle grid-view instead of the file listing  and `t` toggles icons / thumbnails
+* can be made default globally with `--grid` or per-volume with volflag `grid`
 
 ![copyparty-thumbs-fs8](https://user-images.githubusercontent.com/241032/129636211-abd20fa2-a953-4366-9423-1c88ebb96ba9.png)
 
 it does static images with Pillow / pyvips / FFmpeg, and uses FFmpeg for video files, so you may want to `--no-thumb` or maybe just `--no-vthumb` depending on how dangerous your users are
 * pyvips is 3x faster than Pillow, Pillow is 3x faster than FFmpeg
 * disable thumbnails for specific volumes with volflag `dthumb` for all, or `dvthumb` / `dathumb` / `dithumb` for video/audio/images only
 
 audio files are covnerted into spectrograms using FFmpeg unless you `--no-athumb` (and some FFmpeg builds may need `--th-ff-swr`)
 
 images with the following names (see `--th-covers`) become the thumbnail of the folder they're in: `folder.png`, `folder.jpg`, `cover.png`, `cover.jpg`
+* and, if you enable [file indexing](#file-indexing), all remaining folders will also get thumbnails (as long as they contain any pics at all)
 
 in the grid/thumbnail view, if the audio player panel is open, songs will start playing when clicked
 * indicated by the audio files having the ▶ icon instead of 💾
 
 
 ## zip downloads
 
@@ -967,22 +969,21 @@
 * `-e2tsr` also deletes all existing tags, doing a full reindex
 * `-e2v` verfies file integrity at startup, comparing hashes from the db
 * `-e2vu` patches the database with the new hashes from the filesystem
 * `-e2vp` panics and kills copyparty instead
 * `--xlink` enables deduplication across volumes
 
 the same arguments can be set as volflags, in addition to `d2d`, `d2ds`, `d2t`, `d2ts`, `d2v` for disabling:
-* `-v ~/music::r:c,e2dsa,e2tsr` does a full reindex of everything on startup
+* `-v ~/music::r:c,e2ds,e2tsr` does a full reindex of everything on startup
 * `-v ~/music::r:c,d2d` disables **all** indexing, even if any `-e2*` are on
 * `-v ~/music::r:c,d2t` disables all `-e2t*` (tags), does not affect `-e2d*`
 * `-v ~/music::r:c,d2ds` disables on-boot scans; only index new uploads
 * `-v ~/music::r:c,d2ts` same except only affecting tags
 
 note:
-* the parser can finally handle `c,e2dsa,e2tsr` so you no longer have to `c,e2dsa:c,e2tsr`
 * `e2tsr` is probably always overkill, since `e2ds`/`e2dsa` would pick up any file modifications and `e2ts` would then reindex those, unless there is a new copyparty version with new parsers and the release note says otherwise
 * the rescan button in the admin panel has no effect unless the volume has `-e2ds` or higher
 * deduplication is possible on windows if you run copyparty as administrator (not saying you should!)
 
 ### exclude-patterns
 
 to save some time,  you can provide a regex pattern for filepaths to only index by filename/path/size/last-modified (and not the hash of the file contents) by setting `--no-hash \.iso$` or the volflag `:c,nohash=\.iso$`, this has the following consequences:
@@ -1609,14 +1610,19 @@
 
 ## https
 
 both HTTP and HTTPS are accepted  by default, but letting a [reverse proxy](#reverse-proxy) handle the https/tls/ssl would be better (probably more secure by default)
 
 copyparty doesn't speak HTTP/2 or QUIC, so using a reverse proxy would solve that as well
 
+if [cfssl](https://github.com/cloudflare/cfssl/releases/latest) is installed, copyparty will automatically create a CA and server-cert on startup
+* the certs are written to `--crt-dir` for distribution, see `--help` for the other `--crt` options
+* this will be a self-signed certificate so you must install your `ca.pem` into all your browsers/devices
+* if you want to avoid the hassle of distributing certs manually, please consider using a reverse proxy
+
 
 # recovering from crashes
 
 ## client crashes
 
 ### frefox wsod
```

### Comparing `copyparty-1.7.2/README.md` & `copyparty-1.7.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -467,24 +467,26 @@
 * `[↵]` toggles wordwrap
 * `[👀]` show full name on hover (if wordwrap is off)
 
 
 ## thumbnails
 
 press `g` or `田` to toggle grid-view instead of the file listing  and `t` toggles icons / thumbnails
+* can be made default globally with `--grid` or per-volume with volflag `grid`
 
 ![copyparty-thumbs-fs8](https://user-images.githubusercontent.com/241032/129636211-abd20fa2-a953-4366-9423-1c88ebb96ba9.png)
 
 it does static images with Pillow / pyvips / FFmpeg, and uses FFmpeg for video files, so you may want to `--no-thumb` or maybe just `--no-vthumb` depending on how dangerous your users are
 * pyvips is 3x faster than Pillow, Pillow is 3x faster than FFmpeg
 * disable thumbnails for specific volumes with volflag `dthumb` for all, or `dvthumb` / `dathumb` / `dithumb` for video/audio/images only
 
 audio files are covnerted into spectrograms using FFmpeg unless you `--no-athumb` (and some FFmpeg builds may need `--th-ff-swr`)
 
 images with the following names (see `--th-covers`) become the thumbnail of the folder they're in: `folder.png`, `folder.jpg`, `cover.png`, `cover.jpg`
+* and, if you enable [file indexing](#file-indexing), all remaining folders will also get thumbnails (as long as they contain any pics at all)
 
 in the grid/thumbnail view, if the audio player panel is open, songs will start playing when clicked
 * indicated by the audio files having the ▶ icon instead of 💾
 
 
 ## zip downloads
 
@@ -925,22 +927,21 @@
 * `-e2tsr` also deletes all existing tags, doing a full reindex
 * `-e2v` verfies file integrity at startup, comparing hashes from the db
 * `-e2vu` patches the database with the new hashes from the filesystem
 * `-e2vp` panics and kills copyparty instead
 * `--xlink` enables deduplication across volumes
 
 the same arguments can be set as volflags, in addition to `d2d`, `d2ds`, `d2t`, `d2ts`, `d2v` for disabling:
-* `-v ~/music::r:c,e2dsa,e2tsr` does a full reindex of everything on startup
+* `-v ~/music::r:c,e2ds,e2tsr` does a full reindex of everything on startup
 * `-v ~/music::r:c,d2d` disables **all** indexing, even if any `-e2*` are on
 * `-v ~/music::r:c,d2t` disables all `-e2t*` (tags), does not affect `-e2d*`
 * `-v ~/music::r:c,d2ds` disables on-boot scans; only index new uploads
 * `-v ~/music::r:c,d2ts` same except only affecting tags
 
 note:
-* the parser can finally handle `c,e2dsa,e2tsr` so you no longer have to `c,e2dsa:c,e2tsr`
 * `e2tsr` is probably always overkill, since `e2ds`/`e2dsa` would pick up any file modifications and `e2ts` would then reindex those, unless there is a new copyparty version with new parsers and the release note says otherwise
 * the rescan button in the admin panel has no effect unless the volume has `-e2ds` or higher
 * deduplication is possible on windows if you run copyparty as administrator (not saying you should!)
 
 ### exclude-patterns
 
 to save some time,  you can provide a regex pattern for filepaths to only index by filename/path/size/last-modified (and not the hash of the file contents) by setting `--no-hash \.iso$` or the volflag `:c,nohash=\.iso$`, this has the following consequences:
@@ -1567,14 +1568,19 @@
 
 ## https
 
 both HTTP and HTTPS are accepted  by default, but letting a [reverse proxy](#reverse-proxy) handle the https/tls/ssl would be better (probably more secure by default)
 
 copyparty doesn't speak HTTP/2 or QUIC, so using a reverse proxy would solve that as well
 
+if [cfssl](https://github.com/cloudflare/cfssl/releases/latest) is installed, copyparty will automatically create a CA and server-cert on startup
+* the certs are written to `--crt-dir` for distribution, see `--help` for the other `--crt` options
+* this will be a self-signed certificate so you must install your `ca.pem` into all your browsers/devices
+* if you want to avoid the hassle of distributing certs manually, please consider using a reverse proxy
+
 
 # recovering from crashes
 
 ## client crashes
 
 ### frefox wsod
```

### Comparing `copyparty-1.7.2/copyparty/__main__.py` & `copyparty-1.7.3/copyparty/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 __author__ = "ed <copyparty@ocv.me>"
 __copyright__ = 2019
 __license__ = "MIT"
 __url__ = "https://github.com/9001/copyparty/"
 
 import argparse
 import base64
-import filecmp
 import locale
 import os
 import re
-import shutil
 import socket
 import sys
 import threading
 import time
 import traceback
 import uuid
 from textwrap import dedent
@@ -232,14 +230,32 @@
             ret = re.sub("[234567=]", "", ret)[:namelen]
         with open(fp, "wb") as f:
             f.write(ret.encode("utf-8") + b"\n")
 
     return ret
 
 
+def get_fk_salt(cert_path)  :
+    fp = os.path.join(E.cfg, "fk-salt.txt")
+    try:
+        with open(fp, "rb") as f:
+            ret = f.read().strip()
+    except:
+        if os.path.exists(cert_path):
+            print("salt from cert")
+            return unicode(os.path.getmtime(cert_path))
+        else:
+            print("salt from os.random")
+            ret = base64.b64encode(os.urandom(18))
+            with open(fp, "wb") as f:
+                f.write(ret + b"\n")
+
+    return ret.decode("utf-8")
+
+
 def ensure_locale()  :
     safe = "en_US.UTF-8"
     for x in [
         safe,
         "English_United States.UTF8",
         "English_United States.1252",
     ]:
@@ -251,53 +267,30 @@
         except:
             continue
 
     t = "setlocale {} failed,\n  sorting and dates might get funky\n"
     warn(t.format(safe))
 
 
-def ensure_cert(al )  :
-    """
-    the default cert (and the entire TLS support) is only here to enable the
-    crypto.subtle javascript API, which is necessary due to the webkit guys
-    being massive memers (https://www.chromium.org/blink/webcrypto)
+def ensure_webdeps()  :
+    ap = os.path.join(E.mod, "web/deps/mini-fa.woff")
+    if os.path.exists(ap):
+        return
 
-    i feel awful about this and so should they
+    warn(
+        """could not find webdeps;
+  if you are running the sfx, or exe, or pypi package, or docker image,
+  then this is a bug! Please let me know so I can fix it, thanks :-)
+  https://github.com/9001/copyparty/issues/new?labels=bug&template=bug_report.md
+
+  however, if you are a dev, or running copyparty from source, and you want
+  full client functionality, you will need to build or obtain the webdeps:
+  https://github.com/9001/copyparty/blob/hovudstraum/docs/devnotes.md#building
     """
-    cert_insec = os.path.join(E.mod, "res/insecure.pem")
-    cert_appdata = os.path.join(E.cfg, "cert.pem")
-    if not os.path.isfile(al.cert):
-        if cert_appdata != al.cert:
-            raise Exception("certificate file does not exist: " + al.cert)
-
-        shutil.copy(cert_insec, al.cert)
-
-    with open(al.cert, "rb") as f:
-        buf = f.read()
-        o1 = buf.find(b" PRIVATE KEY-")
-        o2 = buf.find(b" CERTIFICATE-")
-        m = "unsupported certificate format: "
-        if o1 < 0:
-            raise Exception(m + "no private key inside pem")
-        if o2 < 0:
-            raise Exception(m + "no server certificate inside pem")
-        if o1 > o2:
-            raise Exception(m + "private key must appear before server certificate")
-
-    try:
-        if filecmp.cmp(al.cert, cert_insec):
-            lprint(
-                "\033[33musing default TLS certificate; https will be insecure."
-                + "\033[36m\ncertificate location: {}\033[0m\n".format(al.cert)
-            )
-    except:
-        pass
-
-    # speaking of the default cert,
-    # printf 'NO\n.\n.\n.\n.\ncopyparty-insecure\n.\n' | faketime '2000-01-01 00:00:00' openssl req -x509 -sha256 -newkey rsa:2048 -keyout insecure.pem -out insecure.pem -days $((($(printf %d 0x7fffffff)-$(date +%s --date=2000-01-01T00:00:00Z))/(60*60*24))) -nodes && ls -al insecure.pem && openssl x509 -in insecure.pem -text -noout
+    )
 
 
 def configure_ssl_ver(al )  :
     def terse_sslver(txt )  :
         txt = txt.lower()
         for c in ["_", "v", "."]:
             txt = txt.replace(c, "")
@@ -719,14 +712,32 @@
     ap2.add_argument("--cert", metavar="PATH", type=u, default=cert_path, help="path to TLS certificate")
     ap2.add_argument("--ssl-ver", metavar="LIST", type=u, help="set allowed ssl/tls versions; [\033[32mhelp\033[0m] shows available versions; default is what your python version considers safe")
     ap2.add_argument("--ciphers", metavar="LIST", type=u, help="set allowed ssl/tls ciphers; [\033[32mhelp\033[0m] shows available ciphers")
     ap2.add_argument("--ssl-dbg", action="store_true", help="dump some tls info")
     ap2.add_argument("--ssl-log", metavar="PATH", type=u, help="log master secrets for later decryption in wireshark")
 
 
+def add_cert(ap, cert_path):
+    cert_dir = os.path.dirname(cert_path)
+    ap2 = ap.add_argument_group('TLS certificate generator options')
+    ap2.add_argument("--no-crt", action="store_true", help="disable automatic certificate creation")
+    ap2.add_argument("--crt-ns", metavar="N,N", type=u, default="", help="comma-separated list of FQDNs (domains) to add into the certificate")
+    ap2.add_argument("--crt-exact", action="store_true", help="do not add wildcard entries for each --crt-ns")
+    ap2.add_argument("--crt-noip", action="store_true", help="do not add autodetected IP addresses into cert")
+    ap2.add_argument("--crt-nolo", action="store_true", help="do not add 127.0.0.1 / localhost into cert")
+    ap2.add_argument("--crt-dir", metavar="PATH", default=cert_dir, help="where to save the CA cert")
+    ap2.add_argument("--crt-cdays", metavar="D", type=float, default=3650, help="ca-certificate expiration time in days")
+    ap2.add_argument("--crt-sdays", metavar="D", type=float, default=365, help="server-cert expiration time in days")
+    ap2.add_argument("--crt-cn", metavar="TXT", type=u, default="partyco", help="CA/server-cert common-name")
+    ap2.add_argument("--crt-cnc", metavar="TXT", type=u, default="--crt-cn", help="override CA name")
+    ap2.add_argument("--crt-cns", metavar="TXT", type=u, default="--crt-cn cpp", help="override server-cert name")
+    ap2.add_argument("--crt-back", metavar="HRS", type=float, default=72, help="backdate in hours")
+    ap2.add_argument("--crt-alg", metavar="S-N", type=u, default="ecdsa-256", help="algorithm and keysize; one of these: ecdsa-256 rsa-4096 rsa-2048")
+
+
 def add_zeroconf(ap):
     ap2 = ap.add_argument_group("Zeroconf options")
     ap2.add_argument("-z", action="store_true", help="enable all zeroconf backends (mdns, ssdp)")
     ap2.add_argument("--z-on", metavar="NETS", type=u, default="", help="enable zeroconf ONLY on the comma-separated list of subnets and/or interface names/indexes\n └─example: \033[32meth0, wlo1, virhost0, 192.168.123.0/24, fd00:fda::/96\033[0m")
     ap2.add_argument("--z-off", metavar="NETS", type=u, default="", help="disable zeroconf on the comma-separated list of subnets and/or interface names/indexes")
     ap2.add_argument("--z-chk", metavar="SEC", type=int, default=10, help="check for network changes every SEC seconds (0=disable)")
     ap2.add_argument("-zv", action="store_true", help="verbose all zeroconf backends")
@@ -860,14 +871,16 @@
     ap2.add_argument("--exit", metavar="WHEN", type=u, default="", help="shutdown after WHEN has finished; [\033[32mcfg\033[0m] config parsing, [\033[32midx\033[0m] volscan + multimedia indexing")
 
 
 def add_logging(ap):
     ap2 = ap.add_argument_group('logging options')
     ap2.add_argument("-q", action="store_true", help="quiet")
     ap2.add_argument("-lo", metavar="PATH", type=u, help="logfile, example: \033[32mcpp-%%Y-%%m%%d-%%H%%M%%S.txt.xz")
+    ap2.add_argument("--no-ansi", action="store_true", default=not VT100, help="disable colors; same as environment-variable NO_COLOR")
+    ap2.add_argument("--ansi", action="store_true", help="force colors; overrides environment-variable NO_COLOR")
     ap2.add_argument("--no-voldump", action="store_true", help="do not list volumes and permissions on startup")
     ap2.add_argument("--log-conn", action="store_true", help="debug: print tcp-server msgs")
     ap2.add_argument("--log-htp", action="store_true", help="debug: print http-server threadpool scaling")
     ap2.add_argument("--ihead", metavar="HEADER", type=u, action='append', help="dump incoming header")
     ap2.add_argument("--lf-url", metavar="RE", type=u, default=r"^/\.cpr/|\?th=[wj]$|/\.(_|ql_|DS_Store$|localized$)", help="dont log URLs matching")
 
 
@@ -891,15 +904,15 @@
     ap2.add_argument("--th-no-jpg", action="store_true", help="disable jpg output")
     ap2.add_argument("--th-no-webp", action="store_true", help="disable webp output")
     ap2.add_argument("--th-ff-jpg", action="store_true", help="force jpg output for video thumbs")
     ap2.add_argument("--th-ff-swr", action="store_true", help="use swresample instead of soxr for audio thumbs")
     ap2.add_argument("--th-poke", metavar="SEC", type=int, default=300, help="activity labeling cooldown -- avoids doing keepalive pokes (updating the mtime) on thumbnail folders more often than SEC seconds")
     ap2.add_argument("--th-clean", metavar="SEC", type=int, default=43200, help="cleanup interval; 0=disabled")
     ap2.add_argument("--th-maxage", metavar="SEC", type=int, default=604800, help="max folder age -- folders which haven't been poked for longer than --th-poke seconds will get deleted every --th-clean seconds")
-    ap2.add_argument("--th-covers", metavar="N,N", type=u, default="folder.png,folder.jpg,cover.png,cover.jpg", help="folder thumbnails to stat/look for; case-insensitive if -e2d")
+    ap2.add_argument("--th-covers", metavar="N,N", type=u, default="folder.png,folder.jpg,cover.png,cover.jpg", help="folder thumbnails to stat/look for; enabling -e2d will make these case-insensitive, and also automatically select thumbnails for all folders that contain pics, even if none match this pattern")
     # https://pillow.readthedocs.io/en/stable/handbook/image-file-formats.html
     # https://github.com/libvips/libvips
     # ffmpeg -hide_banner -demuxers | awk '/^ D  /{print$2}' | while IFS= read -r x; do ffmpeg -hide_banner -h demuxer=$x; done | grep -E '^Demuxer |extensions:'
     ap2.add_argument("--th-r-pil", metavar="T,T", type=u, default="avif,avifs,blp,bmp,dcx,dds,dib,emf,eps,fits,flc,fli,fpx,gif,heic,heics,heif,heifs,icns,ico,im,j2p,j2k,jp2,jpeg,jpg,jpx,pbm,pcx,pgm,png,pnm,ppm,psd,sgi,spi,tga,tif,tiff,webp,wmf,xbm,xpm", help="image formats to decode using pillow")
     ap2.add_argument("--th-r-vips", metavar="T,T", type=u, default="avif,exr,fit,fits,fts,gif,hdr,heic,jp2,jpeg,jpg,jpx,jxl,nii,pfm,pgm,png,ppm,svg,tif,tiff,webp", help="image formats to decode using pyvips")
     ap2.add_argument("--th-r-ffi", metavar="T,T", type=u, default="apng,avif,avifs,bmp,dds,dib,fit,fits,fts,gif,hdr,heic,heics,heif,heifs,icns,ico,jp2,jpeg,jpg,jpx,jxl,pbm,pcx,pfm,pgm,png,pnm,ppm,psd,sgi,tga,tif,tiff,webp,xbm,xpm", help="image formats to decode using ffmpeg")
     ap2.add_argument("--th-r-ffv", metavar="T,T", type=u, default="3gp,asf,av1,avc,avi,flv,h264,h265,hevc,m4v,mjpeg,mjpg,mkv,mov,mp4,mpeg,mpeg2,mpegts,mpg,mpg2,mts,nut,ogm,ogv,rm,ts,vob,webm,wmv", help="video formats to decode using ffmpeg")
@@ -953,17 +966,19 @@
     ap2.add_argument("-mth", metavar="M,M,M", type=u, help="tags to hide by default (comma-sep.)",
         default=".vq,.aq,vc,ac,fmt,res,.fps")
     ap2.add_argument("-mtp", metavar="M=[f,]BIN", type=u, action="append", help="read tag M using program BIN to parse the file")
 
 
 def add_ui(ap, retry):
     ap2 = ap.add_argument_group('ui options')
+    ap2.add_argument("--grid", action="store_true", help="show grid/thumbnails by default (volflag=grid)")
     ap2.add_argument("--lang", metavar="LANG", type=u, default="eng", help="language")
     ap2.add_argument("--theme", metavar="NUM", type=int, default=0, help="default theme to use")
     ap2.add_argument("--themes", metavar="NUM", type=int, default=8, help="number of themes installed")
+    ap2.add_argument("--unlist", metavar="REGEX", type=u, default="", help="don't show files matching REGEX in file list. Purely cosmetic! Does not affect API calls, just the browser. Example: [\033[32m\.(js|css)$\033[0m] (volflag=unlist)")
     ap2.add_argument("--favico", metavar="TXT", type=u, default="c 000 none" if retry else "🎉 000 none", help="\033[33mfavicon-text\033[0m [ \033[33mforeground\033[0m [ \033[33mbackground\033[0m ] ], set blank to disable")
     ap2.add_argument("--mpmc", metavar="URL", type=u, default="", help="change the mediaplayer-toggle mouse cursor; URL to a folder with {2..5}.png inside (or disable with [\033[32m.\033[0m])")
     ap2.add_argument("--js-browser", metavar="L", type=u, help="URL to additional JS to include")
     ap2.add_argument("--css-browser", metavar="L", type=u, help="URL to additional CSS to include")
     ap2.add_argument("--html-head", metavar="TXT", type=u, default="", help="text to append to the <head> of all HTML pages")
     ap2.add_argument("--ih", action="store_true", help="if a folder contains index.html, show that instead of the directory listing by default (can be changed in the client settings UI)")
     ap2.add_argument("--textfiles", metavar="CSV", type=u, default="txt,nfo,diz,cue,readme", help="file extensions to present as plaintext")
@@ -1004,28 +1019,26 @@
         formatter_class=formatter,
         prog="copyparty",
         description="http file sharing hub v{} ({})".format(S_VERSION, S_BUILD_DT),
     )
 
     cert_path = os.path.join(E.cfg, "cert.pem")
 
-    try:
-        fk_salt = unicode(os.path.getmtime(cert_path))
-    except:
-        fk_salt = "hunter2"
+    fk_salt = get_fk_salt(cert_path)
 
     hcores = min(CORES, 4)  # optimal on py3.11 @ r5-4500U
 
     tty = os.environ.get("TERM", "").lower() == "linux"
 
     srvname = get_srvname()
 
     add_general(ap, nc, srvname)
     add_network(ap)
     add_tls(ap, cert_path)
+    add_cert(ap, cert_path)
     add_qr(ap, tty)
     add_zeroconf(ap)
     add_zc_mdns(ap)
     add_zc_ssdp(ap)
     add_upload(ap)
     add_db_general(ap, hcores)
     add_db_metadata(ap)
@@ -1102,14 +1115,16 @@
         sys.exit(0)
 
     if EXE:
         print("pybin: {}\n".format(pybin), end="")
 
     ensure_locale()
 
+    ensure_webdeps()
+
     for k, v in zip(argv[1:], argv[2:]):
         if k == "-c" and os.path.isfile(v):
             supp = args_from_cfg(v)
             argv.extend(supp)
 
     for k in argv[1:]:
         v = k[2:]
@@ -1168,24 +1183,26 @@
     try:
         assert al  # type: ignore
         assert dal  # type: ignore
         al.E = E  # __init__ is not shared when oxidized
     except:
         sys.exit(1)
 
-    if HAVE_SSL:
-        ensure_cert(al)
+    if al.ansi:
+        al.no_ansi = False
+    elif not al.no_ansi:
+        al.ansi = VT100
 
     if WINDOWS and not al.keep_qem:
         try:
             disable_quickedit()
         except:
             lprint("\nfailed to disable quick-edit-mode:\n" + min_ex() + "\n")
 
-    if not VT100:
+    if al.ansi:
         al.wintitle = ""
 
     nstrs  = []
     anymod = False
     for ostr in al.v or []:
         m = re_vol.match(ostr)
         if not m:
@@ -1256,14 +1273,15 @@
         if al.ssl_ver:
             configure_ssl_ver(al)
 
         if al.ciphers:
             configure_ssl_ciphers(al)
     else:
         warn("ssl module does not exist; cannot enable https")
+        al.http_only = True
 
     if PY2 and WINDOWS and al.e2d:
         warn(
             "windows py2 cannot do unicode filenames with -e2d\n"
             + "  (if you crash with codec errors then that is why)"
         )
```

### Comparing `copyparty-1.7.2/copyparty/authsrv.py` & `copyparty-1.7.3/copyparty/authsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/bos/bos.py` & `copyparty-1.7.3/copyparty/bos/bos.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/bos/path.py` & `copyparty-1.7.3/copyparty/bos/path.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/broker_mp.py` & `copyparty-1.7.3/copyparty/broker_mp.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/broker_mpw.py` & `copyparty-1.7.3/copyparty/broker_mpw.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/broker_thr.py` & `copyparty-1.7.3/copyparty/broker_thr.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/broker_util.py` & `copyparty-1.7.3/copyparty/broker_util.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/cfg.py` & `copyparty-1.7.3/copyparty/cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         "dotsrch",
         "e2t",
         "e2ts",
         "e2tsr",
         "e2v",
         "e2vu",
         "e2vp",
+        "grid",
         "hardlink",
         "magic",
         "no_sb_md",
         "no_sb_lg",
         "rand",
         "xdev",
         "xlink",
@@ -36,15 +37,15 @@
         ret[k] = k
     return ret
 
 
 def vf_vmap()   :
     """argv-to-volflag: simple values"""
     ret = {}
-    for k in ("lg_sbf", "md_sbf"):
+    for k in ("lg_sbf", "md_sbf", "unlist"):
         ret[k] = k
     return ret
 
 
 def vf_cmap()   :
     """argv-to-volflag: complex/lists"""
     ret = {}
@@ -129,14 +130,16 @@
         "xbr=CMD": "execute CMD before a file rename/move",
         "xar=CMD": "execute CMD after  a file rename/move",
         "xbd=CMD": "execute CMD before a file delete",
         "xad=CMD": "execute CMD after  a file delete",
         "xm=CMD": "execute CMD on message",
     },
     "client and ux": {
+        "grid": "show grid/thumbnails by default",
+        "unlist": "dont list files matching REGEX",
         "html_head=TXT": "includes TXT in the <head>",
         "robots": "allows indexing by search engines (default)",
         "norobots": "kindly asks search engines to leave",
         "no_sb_md": "disable js sandbox for markdown files",
         "no_sb_lg": "disable js sandbox for prologue/epilogue",
         "sb_md": "enable js sandbox for markdown files (default)",
         "sb_lg": "enable js sandbox for prologue/epilogue (default)",
```

### Comparing `copyparty-1.7.2/copyparty/dxml.py` & `copyparty-1.7.3/copyparty/dxml.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/fsutil.py` & `copyparty-1.7.3/copyparty/fsutil.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/ftpd.py` & `copyparty-1.7.3/copyparty/ftpd.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,17 +493,17 @@
             h1.tls_control_required = True
             h1.tls_data_required = True
 
             hs.append([h1, self.args.ftps])
 
         for h_lp in hs:
             h2, lp = h_lp
-            h2.hub = hub
-            h2.args = hub.args
-            h2.authorizer = FtpAuth(hub)
+            FtpHandler.hub = h2.hub = hub
+            FtpHandler.args = h2.args = hub.args
+            FtpHandler.authorizer = h2.authorizer = FtpAuth(hub)
 
             if self.args.ftp_pr:
                 p1, p2 = [int(x) for x in self.args.ftp_pr.split("-")]
                 if self.args.ftp and self.args.ftps:
                     # divide port range in half
                     d = int((p2 - p1) / 2)
                     if lp == self.args.ftp:
```

### Comparing `copyparty-1.7.2/copyparty/httpcli.py` & `copyparty-1.7.3/copyparty/httpcli.py`

 * *Files 0% similar despite different names*

```diff
@@ -7075,592 +7075,606 @@
 0001ba20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ba30: 2020 2072 6561 646d 6520 3d20 662e 7265     readme = f.re
 0001ba40: 6164 2829 2e64 6563 6f64 6528 2275 7466  ad().decode("utf
 0001ba50: 2d38 2229 0a20 2020 2020 2020 2020 2020  -8").           
 0001ba60: 2020 2020 2020 2020 2020 2020 2062 7265               bre
 0001ba70: 616b 0a0a 2020 2020 2020 2020 7666 203d  ak..        vf =
 0001ba80: 2076 6e2e 666c 6167 730a 2020 2020 2020   vn.flags.      
-0001ba90: 2020 6c73 5f72 6574 203d 207b 0a20 2020    ls_ret = {.   
-0001baa0: 2020 2020 2020 2020 2022 6469 7273 223a           "dirs":
-0001bab0: 205b 5d2c 0a20 2020 2020 2020 2020 2020   [],.           
-0001bac0: 2022 6669 6c65 7322 3a20 5b5d 2c0a 2020   "files": [],.  
-0001bad0: 2020 2020 2020 2020 2020 2274 6167 6c69            "tagli
-0001bae0: 7374 223a 205b 5d2c 0a20 2020 2020 2020  st": [],.       
-0001baf0: 2020 2020 2022 7372 7669 6e66 223a 2073       "srvinf": s
-0001bb00: 7276 5f69 6e66 6f74 2c0a 2020 2020 2020  rv_infot,.      
-0001bb10: 2020 2020 2020 2261 6363 7422 3a20 7365        "acct": se
-0001bb20: 6c66 2e75 6e61 6d65 2c0a 2020 2020 2020  lf.uname,.      
-0001bb30: 2020 2020 2020 2269 6478 223a 2065 3264        "idx": e2d
-0001bb40: 2c0a 2020 2020 2020 2020 2020 2020 2269  ,.            "i
-0001bb50: 7461 6722 3a20 6532 742c 0a20 2020 2020  tag": e2t,.     
-0001bb60: 2020 2020 2020 2022 6c69 6665 7469 6d65         "lifetime
-0001bb70: 223a 2076 6e2e 666c 6167 732e 6765 7428  ": vn.flags.get(
-0001bb80: 226c 6966 6574 696d 6522 2920 6f72 2030  "lifetime") or 0
-0001bb90: 2c0a 2020 2020 2020 2020 2020 2020 2266  ,.            "f
-0001bba0: 7261 6e64 223a 2062 6f6f 6c28 766e 2e66  rand": bool(vn.f
-0001bbb0: 6c61 6773 2e67 6574 2822 7261 6e64 2229  lags.get("rand")
-0001bbc0: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
-0001bbd0: 7065 726d 7322 3a20 7065 726d 732c 0a20  perms": perms,. 
-0001bbe0: 2020 2020 2020 2020 2020 2022 6c6f 6775             "logu
-0001bbf0: 6573 223a 206c 6f67 7565 732c 0a20 2020  es": logues,.   
-0001bc00: 2020 2020 2020 2020 2022 7265 6164 6d65           "readme
-0001bc10: 223a 2072 6561 646d 652c 0a20 2020 2020  ": readme,.     
-0001bc20: 2020 207d 0a20 2020 2020 2020 206a 3261     }.        j2a
-0001bc30: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-0001bc40: 2022 7664 6972 223a 2071 756f 7465 7028   "vdir": quotep(
-0001bc50: 7365 6c66 2e76 7061 7468 292c 0a20 2020  self.vpath),.   
-0001bc60: 2020 2020 2020 2020 2022 7670 6e6f 6465           "vpnode
-0001bc70: 7322 3a20 7670 6e6f 6465 732c 0a20 2020  s": vpnodes,.   
-0001bc80: 2020 2020 2020 2020 2022 6669 6c65 7322           "files"
-0001bc90: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
-0001bca0: 2020 226c 7330 223a 204e 6f6e 652c 0a20    "ls0": None,. 
-0001bcb0: 2020 2020 2020 2020 2020 2022 6163 6374             "acct
-0001bcc0: 223a 2073 656c 662e 756e 616d 652c 0a20  ": self.uname,. 
-0001bcd0: 2020 2020 2020 2020 2020 2022 7065 726d             "perm
-0001bce0: 7322 3a20 6a73 6f6e 2e64 756d 7073 2870  s": json.dumps(p
-0001bcf0: 6572 6d73 292c 0a20 2020 2020 2020 2020  erms),.         
-0001bd00: 2020 2022 6c69 6665 7469 6d65 223a 206c     "lifetime": l
-0001bd10: 735f 7265 745b 226c 6966 6574 696d 6522  s_ret["lifetime"
-0001bd20: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
-0001bd30: 6672 616e 6422 3a20 626f 6f6c 2876 6e2e  frand": bool(vn.
-0001bd40: 666c 6167 732e 6765 7428 2272 616e 6422  flags.get("rand"
-0001bd50: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-0001bd60: 2274 6167 6c69 7374 223a 205b 5d2c 0a20  "taglist": [],. 
-0001bd70: 2020 2020 2020 2020 2020 2022 6465 665f             "def_
-0001bd80: 6863 6f6c 7322 3a20 5b5d 2c0a 2020 2020  hcols": [],.    
-0001bd90: 2020 2020 2020 2020 2268 6176 655f 656d          "have_em
-0001bda0: 7022 3a20 7365 6c66 2e61 7267 732e 656d  p": self.args.em
-0001bdb0: 702c 0a20 2020 2020 2020 2020 2020 2022  p,.            "
-0001bdc0: 6861 7665 5f75 7032 6b5f 6964 7822 3a20  have_up2k_idx": 
-0001bdd0: 6532 642c 0a20 2020 2020 2020 2020 2020  e2d,.           
-0001bde0: 2022 6861 7665 5f74 6167 735f 6964 7822   "have_tags_idx"
-0001bdf0: 3a20 6532 742c 0a20 2020 2020 2020 2020  : e2t,.         
-0001be00: 2020 2022 6861 7665 5f61 636f 6465 223a     "have_acode":
-0001be10: 2028 6e6f 7420 7365 6c66 2e61 7267 732e   (not self.args.
-0001be20: 6e6f 5f61 636f 6465 292c 0a20 2020 2020  no_acode),.     
-0001be30: 2020 2020 2020 2022 6861 7665 5f6d 7622         "have_mv"
-0001be40: 3a20 286e 6f74 2073 656c 662e 6172 6773  : (not self.args
-0001be50: 2e6e 6f5f 6d76 292c 0a20 2020 2020 2020  .no_mv),.       
-0001be60: 2020 2020 2022 6861 7665 5f64 656c 223a       "have_del":
-0001be70: 2028 6e6f 7420 7365 6c66 2e61 7267 732e   (not self.args.
-0001be80: 6e6f 5f64 656c 292c 0a20 2020 2020 2020  no_del),.       
-0001be90: 2020 2020 2022 6861 7665 5f7a 6970 223a       "have_zip":
-0001bea0: 2028 6e6f 7420 7365 6c66 2e61 7267 732e   (not self.args.
-0001beb0: 6e6f 5f7a 6970 292c 0a20 2020 2020 2020  no_zip),.       
-0001bec0: 2020 2020 2022 6861 7665 5f75 6e70 6f73       "have_unpos
-0001bed0: 7422 3a20 696e 7428 7365 6c66 2e61 7267  t": int(self.arg
-0001bee0: 732e 756e 706f 7374 292c 0a20 2020 2020  s.unpost),.     
-0001bef0: 2020 2020 2020 2022 6861 7665 5f62 5f75         "have_b_u
-0001bf00: 223a 2028 7365 6c66 2e63 616e 5f77 7269  ": (self.can_wri
-0001bf10: 7465 2061 6e64 2073 656c 662e 7570 6172  te and self.upar
-0001bf20: 616d 2e67 6574 2822 6222 2920 3d3d 2022  am.get("b") == "
-0001bf30: 7522 292c 0a20 2020 2020 2020 2020 2020  u"),.           
-0001bf40: 2022 7362 5f6d 6422 3a20 2222 2069 6620   "sb_md": "" if 
-0001bf50: 226e 6f5f 7362 5f6d 6422 2069 6e20 7666  "no_sb_md" in vf
-0001bf60: 2065 6c73 6520 2876 662e 6765 7428 226d   else (vf.get("m
-0001bf70: 645f 7362 6622 2920 6f72 2022 7922 292c  d_sbf") or "y"),
-0001bf80: 0a20 2020 2020 2020 2020 2020 2022 7362  .            "sb
-0001bf90: 5f6c 6722 3a20 2222 2069 6620 226e 6f5f  _lg": "" if "no_
-0001bfa0: 7362 5f6c 6722 2069 6e20 7666 2065 6c73  sb_lg" in vf els
-0001bfb0: 6520 2876 662e 6765 7428 226c 675f 7362  e (vf.get("lg_sb
-0001bfc0: 6622 2920 6f72 2022 7922 292c 0a20 2020  f") or "y"),.   
-0001bfd0: 2020 2020 2020 2020 2022 7572 6c5f 7375           "url_su
-0001bfe0: 6622 3a20 7572 6c5f 7375 662c 0a20 2020  f": url_suf,.   
-0001bff0: 2020 2020 2020 2020 2022 6c6f 6775 6573           "logues
-0001c000: 223a 206c 6f67 7565 732c 0a20 2020 2020  ": logues,.     
-0001c010: 2020 2020 2020 2022 7265 6164 6d65 223a         "readme":
-0001c020: 2072 6561 646d 652c 0a20 2020 2020 2020   readme,.       
-0001c030: 2020 2020 2022 7469 746c 6522 3a20 6874       "title": ht
-0001c040: 6d6c 5f65 7363 6170 6528 7365 6c66 2e76  ml_escape(self.v
-0001c050: 7061 7468 2c20 6372 6c66 3d54 7275 6529  path, crlf=True)
-0001c060: 206f 7220 22f0 9f92 bef0 9f8e 8922 2c0a   or "........",.
-0001c070: 2020 2020 2020 2020 2020 2020 2273 7276              "srv
-0001c080: 5f69 6e66 6f22 3a20 7372 765f 696e 666f  _info": srv_info
-0001c090: 742c 0a20 2020 2020 2020 2020 2020 2022  t,.            "
-0001c0a0: 6474 6865 6d65 223a 2073 656c 662e 6172  dtheme": self.ar
-0001c0b0: 6773 2e74 6865 6d65 2c0a 2020 2020 2020  gs.theme,.      
-0001c0c0: 2020 2020 2020 2274 6865 6d65 7322 3a20        "themes": 
-0001c0d0: 7365 6c66 2e61 7267 732e 7468 656d 6573  self.args.themes
-0001c0e0: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
-0001c0f0: 7572 626f 6c76 6c22 3a20 7365 6c66 2e61  urbolvl": self.a
-0001c100: 7267 732e 7475 7262 6f2c 0a20 2020 2020  rgs.turbo,.     
-0001c110: 2020 2020 2020 2022 6964 7868 223a 2069         "idxh": i
-0001c120: 6e74 2873 656c 662e 6172 6773 2e69 6829  nt(self.args.ih)
-0001c130: 2c0a 2020 2020 2020 2020 2020 2020 2275  ,.            "u
-0001c140: 3273 6f72 7422 3a20 7365 6c66 2e61 7267  2sort": self.arg
-0001c150: 732e 7532 736f 7274 2c0a 2020 2020 2020  s.u2sort,.      
-0001c160: 2020 7d0a 0a20 2020 2020 2020 2069 6620    }..        if 
-0001c170: 7365 6c66 2e61 7267 732e 6a73 5f62 726f  self.args.js_bro
-0001c180: 7773 6572 3a0a 2020 2020 2020 2020 2020  wser:.          
-0001c190: 2020 6a32 615b 226a 7322 5d20 3d20 7365    j2a["js"] = se
-0001c1a0: 6c66 2e61 7267 732e 6a73 5f62 726f 7773  lf.args.js_brows
-0001c1b0: 6572 0a0a 2020 2020 2020 2020 6966 2073  er..        if s
-0001c1c0: 656c 662e 6172 6773 2e63 7373 5f62 726f  elf.args.css_bro
-0001c1d0: 7773 6572 3a0a 2020 2020 2020 2020 2020  wser:.          
-0001c1e0: 2020 6a32 615b 2263 7373 225d 203d 2073    j2a["css"] = s
-0001c1f0: 656c 662e 6172 6773 2e63 7373 5f62 726f  elf.args.css_bro
-0001c200: 7773 6572 0a0a 2020 2020 2020 2020 6966  wser..        if
-0001c210: 206e 6f74 2073 656c 662e 636f 6e6e 2e68   not self.conn.h
-0001c220: 7372 762e 7072 6973 6d3a 0a20 2020 2020  srv.prism:.     
-0001c230: 2020 2020 2020 206a 3261 5b22 6e6f 5f70         j2a["no_p
-0001c240: 7269 736d 225d 203d 2054 7275 650a 0a20  rism"] = True.. 
-0001c250: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-0001c260: 6c66 2e63 616e 5f72 6561 643a 0a20 2020  lf.can_read:.   
-0001c270: 2020 2020 2020 2020 2069 6620 6973 5f6c           if is_l
-0001c280: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0001c290: 2020 2072 6574 7572 6e20 7365 6c66 2e74     return self.t
-0001c2a0: 785f 6c73 286c 735f 7265 7429 0a0a 2020  x_ls(ls_ret)..  
-0001c2b0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0001c2c0: 2073 7461 742e 535f 4953 4449 5228 7374   stat.S_ISDIR(st
-0001c2d0: 2e73 745f 6d6f 6465 293a 0a20 2020 2020  .st_mode):.     
-0001c2e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0001c2f0: 6e20 7365 6c66 2e74 785f 3430 3428 5472  n self.tx_404(Tr
-0001c300: 7565 290a 0a20 2020 2020 2020 2020 2020  ue)..           
-0001c310: 2069 6620 227a 6970 2220 696e 2073 656c   if "zip" in sel
-0001c320: 662e 7570 6172 616d 206f 7220 2274 6172  f.uparam or "tar
-0001c330: 2220 696e 2073 656c 662e 7570 6172 616d  " in self.uparam
-0001c340: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001c350: 2020 7261 6973 6520 5065 626b 6163 2834    raise Pebkac(4
-0001c360: 3033 290a 0a20 2020 2020 2020 2020 2020  03)..           
-0001c370: 2068 746d 6c20 3d20 7365 6c66 2e6a 3273   html = self.j2s
-0001c380: 2874 706c 2c20 2a2a 6a32 6129 0a20 2020  (tpl, **j2a).   
-0001c390: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-0001c3a0: 706c 7928 6874 6d6c 2e65 6e63 6f64 6528  ply(html.encode(
-0001c3b0: 2275 7466 2d38 222c 2022 7265 706c 6163  "utf-8", "replac
-0001c3c0: 6522 2929 0a20 2020 2020 2020 2020 2020  e")).           
-0001c3d0: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
-0001c3e0: 2020 2020 2020 666f 7220 6b20 696e 205b        for k in [
-0001c3f0: 227a 6970 222c 2022 7461 7222 5d3a 0a20  "zip", "tar"]:. 
-0001c400: 2020 2020 2020 2020 2020 2076 203d 2073             v = s
-0001c410: 656c 662e 7570 6172 616d 2e67 6574 286b  elf.uparam.get(k
-0001c420: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0001c430: 2076 2069 7320 6e6f 7420 4e6f 6e65 3a0a   v is not None:.
-0001c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c450: 7265 7475 726e 2073 656c 662e 7478 5f7a  return self.tx_z
-0001c460: 6970 286b 2c20 762c 2073 656c 662e 7670  ip(k, v, self.vp
-0001c470: 6174 682c 2076 6e2c 2072 656d 2c20 5b5d  ath, vn, rem, []
-0001c480: 2c20 7365 6c66 2e61 7267 732e 6564 290a  , self.args.ed).
-0001c490: 0a20 2020 2020 2020 2066 7372 6f6f 742c  .        fsroot,
-0001c4a0: 2076 6673 5f6c 732c 2076 6673 5f76 6972   vfs_ls, vfs_vir
-0001c4b0: 7420 3d20 766e 2e6c 7328 0a20 2020 2020  t = vn.ls(.     
-0001c4c0: 2020 2020 2020 2072 656d 2c0a 2020 2020         rem,.    
-0001c4d0: 2020 2020 2020 2020 7365 6c66 2e75 6e61          self.una
-0001c4e0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-0001c4f0: 6e6f 7420 7365 6c66 2e61 7267 732e 6e6f  not self.args.no
-0001c500: 5f73 6361 6e64 6972 2c0a 2020 2020 2020  _scandir,.      
-0001c510: 2020 2020 2020 5b5b 5472 7565 2c20 4661        [[True, Fa
-0001c520: 6c73 655d 2c20 5b46 616c 7365 2c20 5472  lse], [False, Tr
-0001c530: 7565 5d5d 2c0a 2020 2020 2020 2020 2020  ue]],.          
-0001c540: 2020 6c73 7461 743d 226c 7422 2069 6e20    lstat="lt" in 
-0001c550: 7365 6c66 2e75 7061 7261 6d2c 0a20 2020  self.uparam,.   
-0001c560: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-0001c570: 7461 7473 203d 207b 6b3a 2076 2066 6f72  tats = {k: v for
-0001c580: 206b 2c20 7620 696e 2076 6673 5f6c 737d   k, v in vfs_ls}
-0001c590: 0a20 2020 2020 2020 206c 735f 6e61 6d65  .        ls_name
-0001c5a0: 7320 3d20 5b78 5b30 5d20 666f 7220 7820  s = [x[0] for x 
-0001c5b0: 696e 2076 6673 5f6c 735d 0a20 2020 2020  in vfs_ls].     
-0001c5c0: 2020 206c 735f 6e61 6d65 732e 6578 7465     ls_names.exte
-0001c5d0: 6e64 286c 6973 7428 7666 735f 7669 7274  nd(list(vfs_virt
-0001c5e0: 2e6b 6579 7328 2929 290a 0a20 2020 2020  .keys()))..     
-0001c5f0: 2020 2023 2063 6865 636b 2066 6f72 206f     # check for o
-0001c600: 6c64 2076 6572 7369 6f6e 7320 6f66 2066  ld versions of f
-0001c610: 696c 6573 2c0a 2020 2020 2020 2020 2320  iles,.        # 
-0001c620: 5b6e 756d 2d62 6163 6b75 7073 2c20 6d6f  [num-backups, mo
-0001c630: 7374 2d72 6563 656e 742c 2068 6973 742d  st-recent, hist-
-0001c640: 7061 7468 5d0a 2020 2020 2020 2020 6869  path].        hi
-0001c650: 7374 2020 2020 203d 207b 7d0a 2020 2020  st     = {}.    
-0001c660: 2020 2020 6869 7374 6469 7220 3d20 6f73      histdir = os
-0001c670: 2e70 6174 682e 6a6f 696e 2866 7372 6f6f  .path.join(fsroo
-0001c680: 742c 2022 2e68 6973 7422 290a 2020 2020  t, ".hist").    
-0001c690: 2020 2020 7074 6e20 3d20 7265 2e63 6f6d      ptn = re.com
-0001c6a0: 7069 6c65 2872 2228 2e2a 295c 2e28 5b30  pile(r"(.*)\.([0
-0001c6b0: 2d39 5d2b 5c2e 5b30 2d39 5d7b 337d 2928  -9]+\.[0-9]{3})(
-0001c6c0: 5c2e 5b5e 5c2e 5d2b 2924 2229 0a20 2020  \.[^\.]+)$").   
-0001c6d0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0001c6e0: 2020 2020 2020 666f 7220 6866 6e20 696e        for hfn in
-0001c6f0: 2062 6f73 2e6c 6973 7464 6972 2868 6973   bos.listdir(his
-0001c700: 7464 6972 293a 0a20 2020 2020 2020 2020  tdir):.         
-0001c710: 2020 2020 2020 206d 203d 2070 746e 2e6d         m = ptn.m
-0001c720: 6174 6368 2868 666e 290a 2020 2020 2020  atch(hfn).      
-0001c730: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0001c740: 206d 3a0a 2020 2020 2020 2020 2020 2020   m:.            
-0001c750: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-0001c760: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001c770: 2020 666e 203d 206d 2e67 726f 7570 2831    fn = m.group(1
-0001c780: 2920 2b20 6d2e 6772 6f75 7028 3329 0a20  ) + m.group(3). 
-0001c790: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0001c7a0: 2c20 7473 2c20 5f20 3d20 6869 7374 2e67  , ts, _ = hist.g
-0001c7b0: 6574 2866 6e2c 2028 302c 2030 2c20 2222  et(fn, (0, 0, ""
-0001c7c0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0001c7d0: 2020 2068 6973 745b 666e 5d20 3d20 286e     hist[fn] = (n
-0001c7e0: 202b 2031 2c20 6d61 7828 7473 2c20 666c   + 1, max(ts, fl
-0001c7f0: 6f61 7428 6d2e 6772 6f75 7028 3229 2929  oat(m.group(2)))
-0001c800: 2c20 6866 6e29 0a20 2020 2020 2020 2065  , hfn).        e
-0001c810: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
-0001c820: 2020 2070 6173 730a 0a20 2020 2020 2020     pass..       
-0001c830: 2023 2073 686f 7720 646f 7466 696c 6573   # show dotfiles
-0001c840: 2069 6620 7065 726d 6974 7465 6420 616e   if permitted an
-0001c850: 6420 7265 7175 6573 7465 640a 2020 2020  d requested.    
-0001c860: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-0001c870: 6172 6773 2e65 6420 6f72 2022 646f 7473  args.ed or "dots
-0001c880: 2220 6e6f 7420 696e 2073 656c 662e 7570  " not in self.up
-0001c890: 6172 616d 3a0a 2020 2020 2020 2020 2020  aram:.          
-0001c8a0: 2020 6c73 5f6e 616d 6573 203d 2065 7863    ls_names = exc
-0001c8b0: 6c75 6465 5f64 6f74 6669 6c65 7328 6c73  lude_dotfiles(ls
-0001c8c0: 5f6e 616d 6573 290a 0a20 2020 2020 2020  _names)..       
-0001c8d0: 2061 6464 5f66 6b20 3d20 766e 2e66 6c61   add_fk = vn.fla
-0001c8e0: 6773 2e67 6574 2822 666b 2229 0a0a 2020  gs.get("fk")..  
-0001c8f0: 2020 2020 2020 6469 7273 203d 205b 5d0a        dirs = [].
-0001c900: 2020 2020 2020 2020 6669 6c65 7320 3d20          files = 
-0001c910: 5b5d 0a20 2020 2020 2020 2066 6f72 2066  [].        for f
-0001c920: 6e20 696e 206c 735f 6e61 6d65 733a 0a20  n in ls_names:. 
-0001c930: 2020 2020 2020 2020 2020 2062 6173 6520             base 
-0001c940: 3d20 2222 0a20 2020 2020 2020 2020 2020  = "".           
-0001c950: 2068 7265 6620 3d20 666e 0a20 2020 2020   href = fn.     
-0001c960: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-0001c970: 5f6c 7320 616e 6420 6e6f 7420 6973 5f6a  _ls and not is_j
-0001c980: 7320 616e 6420 6e6f 7420 7365 6c66 2e74  s and not self.t
-0001c990: 7261 696c 696e 675f 736c 6173 6820 616e  railing_slash an
-0001c9a0: 6420 7670 6174 683a 0a20 2020 2020 2020  d vpath:.       
-0001c9b0: 2020 2020 2020 2020 2062 6173 6520 3d20           base = 
-0001c9c0: 222f 2220 2b20 7670 6174 6820 2b20 222f  "/" + vpath + "/
-0001c9d0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0001c9e0: 2020 6872 6566 203d 2062 6173 6520 2b20    href = base + 
-0001c9f0: 666e 0a0a 2020 2020 2020 2020 2020 2020  fn..            
-0001ca00: 6966 2066 6e20 696e 2076 6673 5f76 6972  if fn in vfs_vir
-0001ca10: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0001ca20: 2020 2066 7370 6174 6820 3d20 7666 735f     fspath = vfs_
-0001ca30: 7669 7274 5b66 6e5d 2e72 6561 6c70 6174  virt[fn].realpat
-0001ca40: 680a 2020 2020 2020 2020 2020 2020 656c  h.            el
-0001ca50: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001ca60: 2020 2020 6673 7061 7468 203d 2066 7372      fspath = fsr
-0001ca70: 6f6f 7420 2b20 222f 2220 2b20 666e 0a0a  oot + "/" + fn..
-0001ca80: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-0001ca90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001caa0: 206c 696e 6620 3d20 7374 6174 732e 6765   linf = stats.ge
-0001cab0: 7428 666e 2920 6f72 2062 6f73 2e6c 7374  t(fn) or bos.lst
-0001cac0: 6174 2866 7370 6174 6829 0a20 2020 2020  at(fspath).     
-0001cad0: 2020 2020 2020 2020 2020 2069 6e66 203d             inf =
-0001cae0: 2062 6f73 2e73 7461 7428 6673 7061 7468   bos.stat(fspath
-0001caf0: 2920 6966 2073 7461 742e 535f 4953 4c4e  ) if stat.S_ISLN
-0001cb00: 4b28 6c69 6e66 2e73 745f 6d6f 6465 2920  K(linf.st_mode) 
-0001cb10: 656c 7365 206c 696e 660a 2020 2020 2020  else linf.      
-0001cb20: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-0001cb30: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001cb40: 6c66 2e6c 6f67 2822 6272 6f6b 656e 2073  lf.log("broken s
-0001cb50: 796d 6c69 6e6b 3a20 7b7d 222e 666f 726d  ymlink: {}".form
-0001cb60: 6174 2872 6570 7228 6673 7061 7468 2929  at(repr(fspath))
-0001cb70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001cb80: 2020 636f 6e74 696e 7565 0a0a 2020 2020    continue..    
-0001cb90: 2020 2020 2020 2020 6973 5f64 6972 203d          is_dir =
-0001cba0: 2073 7461 742e 535f 4953 4449 5228 696e   stat.S_ISDIR(in
-0001cbb0: 662e 7374 5f6d 6f64 6529 0a20 2020 2020  f.st_mode).     
-0001cbc0: 2020 2020 2020 2069 6620 6973 5f64 6972         if is_dir
-0001cbd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001cbe0: 2020 6872 6566 202b 3d20 222f 220a 2020    href += "/".  
-0001cbf0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001cc00: 2073 656c 662e 6172 6773 2e6e 6f5f 7a69   self.args.no_zi
-0001cc10: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
-0001cc20: 2020 2020 2020 206d 6172 6769 6e20 3d20         margin = 
-0001cc30: 2244 4952 220a 2020 2020 2020 2020 2020  "DIR".          
-0001cc40: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc60: 6d61 7267 696e 203d 2027 3c61 2068 7265  margin = '<a hre
-0001cc70: 663d 2225 733f 7a69 7022 2072 656c 3d22  f="%s?zip" rel="
-0001cc80: 6e6f 666f 6c6c 6f77 223e 7a69 703c 2f61  nofollow">zip</a
-0001cc90: 3e27 2025 2028 7175 6f74 6570 2868 7265  >' % (quotep(hre
-0001cca0: 6629 2c29 0a20 2020 2020 2020 2020 2020  f),).           
-0001ccb0: 2065 6c69 6620 666e 2069 6e20 6869 7374   elif fn in hist
-0001ccc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001ccd0: 2020 6d61 7267 696e 203d 2027 3c61 2068    margin = '<a h
-0001cce0: 7265 663d 2225 732e 6869 7374 2f25 7322  ref="%s.hist/%s"
-0001ccf0: 3e23 2573 3c2f 613e 2720 2520 280a 2020  >#%s</a>' % (.  
-0001cd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd10: 2020 6261 7365 2c0a 2020 2020 2020 2020    base,.        
-0001cd20: 2020 2020 2020 2020 2020 2020 6874 6d6c              html
-0001cd30: 5f65 7363 6170 6528 6869 7374 5b66 6e5d  _escape(hist[fn]
-0001cd40: 5b32 5d2c 2071 756f 743d 5472 7565 2c20  [2], quot=True, 
-0001cd50: 6372 6c66 3d54 7275 6529 2c0a 2020 2020  crlf=True),.    
-0001cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd70: 6869 7374 5b66 6e5d 5b30 5d2c 0a20 2020  hist[fn][0],.   
-0001cd80: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0001cd90: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001cda0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001cdb0: 206d 6172 6769 6e20 3d20 222d 220a 0a20   margin = "-".. 
-0001cdc0: 2020 2020 2020 2020 2020 2073 7a20 3d20             sz = 
-0001cdd0: 696e 662e 7374 5f73 697a 650a 2020 2020  inf.st_size.    
-0001cde0: 2020 2020 2020 2020 7a64 203d 2064 6174          zd = dat
-0001cdf0: 6574 696d 652e 7574 6366 726f 6d74 696d  etime.utcfromtim
-0001ce00: 6573 7461 6d70 286c 696e 662e 7374 5f6d  estamp(linf.st_m
-0001ce10: 7469 6d65 290a 2020 2020 2020 2020 2020  time).          
-0001ce20: 2020 6474 203d 2022 2530 3464 2d25 3032    dt = "%04d-%02
-0001ce30: 642d 2530 3264 2025 3032 643a 2530 3264  d-%02d %02d:%02d
-0001ce40: 3a25 3032 6422 2025 2028 0a20 2020 2020  :%02d" % (.     
-0001ce50: 2020 2020 2020 2020 2020 207a 642e 7965             zd.ye
-0001ce60: 6172 2c0a 2020 2020 2020 2020 2020 2020  ar,.            
-0001ce70: 2020 2020 7a64 2e6d 6f6e 7468 2c0a 2020      zd.month,.  
-0001ce80: 2020 2020 2020 2020 2020 2020 2020 7a64                zd
-0001ce90: 2e64 6179 2c0a 2020 2020 2020 2020 2020  .day,.          
-0001cea0: 2020 2020 2020 7a64 2e68 6f75 722c 0a20        zd.hour,. 
-0001ceb0: 2020 2020 2020 2020 2020 2020 2020 207a                 z
-0001cec0: 642e 6d69 6e75 7465 2c0a 2020 2020 2020  d.minute,.      
-0001ced0: 2020 2020 2020 2020 2020 7a64 2e73 6563            zd.sec
-0001cee0: 6f6e 642c 0a20 2020 2020 2020 2020 2020  ond,.           
-0001cef0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-0001cf00: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0001cf10: 2020 2020 2065 7874 203d 2022 2d2d 2d22       ext = "---"
-0001cf20: 2069 6620 6973 5f64 6972 2065 6c73 6520   if is_dir else 
-0001cf30: 666e 2e72 7370 6c69 7428 222e 222c 2031  fn.rsplit(".", 1
-0001cf40: 295b 315d 0a20 2020 2020 2020 2020 2020  )[1].           
-0001cf50: 2020 2020 2069 6620 6c65 6e28 6578 7429       if len(ext)
-0001cf60: 203e 2031 363a 0a20 2020 2020 2020 2020   > 16:.         
-0001cf70: 2020 2020 2020 2020 2020 2065 7874 203d             ext =
-0001cf80: 2065 7874 5b3a 3136 5d0a 2020 2020 2020   ext[:16].      
-0001cf90: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-0001cfa0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-0001cfb0: 7420 3d20 2225 220a 0a20 2020 2020 2020  t = "%"..       
-0001cfc0: 2020 2020 2069 6620 6164 645f 666b 3a0a       if add_fk:.
-0001cfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cfe0: 6872 6566 203d 2022 2573 3f6b 3d25 7322  href = "%s?k=%s"
-0001cff0: 2025 2028 0a20 2020 2020 2020 2020 2020   % (.           
-0001d000: 2020 2020 2020 2020 2071 756f 7465 7028           quotep(
-0001d010: 6872 6566 292c 0a20 2020 2020 2020 2020  href),.         
-0001d020: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001d030: 6765 6e5f 666b 280a 2020 2020 2020 2020  gen_fk(.        
-0001d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d050: 7365 6c66 2e61 7267 732e 666b 5f73 616c  self.args.fk_sal
-0001d060: 742c 2066 7370 6174 682c 2073 7a2c 2030  t, fspath, sz, 0
-0001d070: 2069 6620 414e 5957 494e 2065 6c73 6520   if ANYWIN else 
-0001d080: 696e 662e 7374 5f69 6e6f 0a20 2020 2020  inf.st_ino.     
-0001d090: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001d0a0: 5b3a 6164 645f 666b 5d2c 0a20 2020 2020  [:add_fk],.     
-0001d0b0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0001d0c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0001d0d0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-0001d0e0: 7265 6620 3d20 7175 6f74 6570 2868 7265  ref = quotep(hre
-0001d0f0: 6629 0a0a 2020 2020 2020 2020 2020 2020  f)..            
-0001d100: 6974 656d 203d 207b 0a20 2020 2020 2020  item = {.       
-0001d110: 2020 2020 2020 2020 2022 6c65 6164 223a           "lead":
-0001d120: 206d 6172 6769 6e2c 0a20 2020 2020 2020   margin,.       
-0001d130: 2020 2020 2020 2020 2022 6872 6566 223a           "href":
-0001d140: 2068 7265 662c 0a20 2020 2020 2020 2020   href,.         
-0001d150: 2020 2020 2020 2022 6e61 6d65 223a 2066         "name": f
-0001d160: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-0001d170: 2020 2022 737a 223a 2073 7a2c 0a20 2020     "sz": sz,.   
-0001d180: 2020 2020 2020 2020 2020 2020 2022 6578               "ex
-0001d190: 7422 3a20 6578 742c 0a20 2020 2020 2020  t": ext,.       
-0001d1a0: 2020 2020 2020 2020 2022 6474 223a 2064           "dt": d
-0001d1b0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-0001d1c0: 2020 2022 7473 223a 2069 6e74 286c 696e     "ts": int(lin
-0001d1d0: 662e 7374 5f6d 7469 6d65 292c 0a20 2020  f.st_mtime),.   
-0001d1e0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-0001d1f0: 2020 2020 2020 2069 6620 6973 5f64 6972         if is_dir
-0001d200: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001d210: 2020 6469 7273 2e61 7070 656e 6428 6974    dirs.append(it
-0001d220: 656d 290a 2020 2020 2020 2020 2020 2020  em).            
-0001d230: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001d240: 2020 2020 2020 6669 6c65 732e 6170 7065        files.appe
-0001d250: 6e64 2869 7465 6d29 0a20 2020 2020 2020  nd(item).       
-0001d260: 2020 2020 2020 2020 2069 7465 6d5b 2272           item["r
-0001d270: 6422 5d20 3d20 7265 6d0a 0a20 2020 2020  d"] = rem..     
-0001d280: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-0001d290: 2020 2020 7365 6c66 2e63 6f6f 6b69 6573      self.cookies
-0001d2a0: 2e67 6574 2822 6964 7868 2229 203d 3d20  .get("idxh") == 
-0001d2b0: 2279 220a 2020 2020 2020 2020 2020 2020  "y".            
-0001d2c0: 616e 6420 226c 7322 206e 6f74 2069 6e20  and "ls" not in 
-0001d2d0: 7365 6c66 2e75 7061 7261 6d0a 2020 2020  self.uparam.    
-0001d2e0: 2020 2020 2020 2020 616e 6420 2276 2220          and "v" 
-0001d2f0: 6e6f 7420 696e 2073 656c 662e 7570 6172  not in self.upar
-0001d300: 616d 0a20 2020 2020 2020 2029 3a0a 2020  am.        ):.  
-0001d310: 2020 2020 2020 2020 2020 6964 785f 6874            idx_ht
-0001d320: 6d6c 203d 2073 6574 285b 2269 6e64 6578  ml = set(["index
-0001d330: 2e68 746d 222c 2022 696e 6465 782e 6874  .htm", "index.ht
-0001d340: 6d6c 225d 290a 2020 2020 2020 2020 2020  ml"]).          
-0001d350: 2020 666f 7220 6974 656d 2069 6e20 6669    for item in fi
-0001d360: 6c65 733a 0a20 2020 2020 2020 2020 2020  les:.           
-0001d370: 2020 2020 2069 6620 6974 656d 5b22 6e61       if item["na
-0001d380: 6d65 225d 2069 6e20 6964 785f 6874 6d6c  me"] in idx_html
-0001d390: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001d3a0: 2020 2020 2020 2320 646f 2066 756c 6c20        # do full 
-0001d3b0: 7265 736f 6c76 6520 696e 2063 6173 6520  resolve in case 
-0001d3c0: 6f66 2073 6861 646f 7765 6420 6669 6c65  of shadowed file
-0001d3d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d3e0: 2020 2020 2076 7020 3d20 766a 6f69 6e28       vp = vjoin(
-0001d3f0: 7365 6c66 2e76 7061 7468 2e73 706c 6974  self.vpath.split
-0001d400: 2822 3f22 295b 305d 2c20 6974 656d 5b22  ("?")[0], item["
-0001d410: 6e61 6d65 225d 290a 2020 2020 2020 2020  name"]).        
-0001d420: 2020 2020 2020 2020 2020 2020 766e 2c20              vn, 
-0001d430: 7265 6d20 3d20 7365 6c66 2e61 7372 762e  rem = self.asrv.
-0001d440: 7666 732e 6765 7428 7670 2c20 7365 6c66  vfs.get(vp, self
-0001d450: 2e75 6e61 6d65 2c20 5472 7565 2c20 4661  .uname, True, Fa
-0001d460: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-0001d470: 2020 2020 2020 2020 2061 7020 3d20 766e           ap = vn
-0001d480: 2e63 616e 6f6e 6963 616c 2872 656d 290a  .canonical(rem).
-0001d490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d4a0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0001d4b0: 7478 5f66 696c 6528 6170 2920 2023 2069  tx_file(ap)  # i
-0001d4c0: 7320 6e6f 2d63 6163 6865 0a0a 2020 2020  s no-cache..    
-0001d4d0: 2020 2020 7461 6773 6574 2020 3d20 7365      tagset  = se
-0001d4e0: 7428 290a 2020 2020 2020 2020 666f 7220  t().        for 
-0001d4f0: 6665 2069 6e20 6669 6c65 733a 0a20 2020  fe in files:.   
-0001d500: 2020 2020 2020 2020 2066 6e20 3d20 6665           fn = fe
-0001d510: 5b22 6e61 6d65 225d 0a20 2020 2020 2020  ["name"].       
-0001d520: 2020 2020 2072 6420 3d20 6665 5b22 7264       rd = fe["rd
-0001d530: 225d 0a20 2020 2020 2020 2020 2020 2064  "].            d
-0001d540: 656c 2066 655b 2272 6422 5d0a 2020 2020  el fe["rd"].    
-0001d550: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-0001d560: 6375 723a 0a20 2020 2020 2020 2020 2020  cur:.           
-0001d570: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
-0001d580: 2020 2020 2020 2020 2020 2069 6620 766e             if vn
-0001d590: 2021 3d20 6462 763a 0a20 2020 2020 2020   != dbv:.       
-0001d5a0: 2020 2020 2020 2020 205f 2c20 7264 203d           _, rd =
-0001d5b0: 2076 6e2e 6765 745f 6462 7628 7264 290a   vn.get_dbv(rd).
-0001d5c0: 0a20 2020 2020 2020 2020 2020 2071 203d  .            q =
-0001d5d0: 2022 7365 6c65 6374 206d 742e 6b2c 206d   "select mt.k, m
-0001d5e0: 742e 7620 6672 6f6d 2075 7020 696e 6e65  t.v from up inne
-0001d5f0: 7220 6a6f 696e 206d 7420 6f6e 206d 742e  r join mt on mt.
-0001d600: 7720 3d20 7375 6273 7472 2875 702e 772c  w = substr(up.w,
-0001d610: 312c 3136 2920 7768 6572 6520 7570 2e72  1,16) where up.r
-0001d620: 6420 3d20 3f20 616e 6420 7570 2e66 6e20  d = ? and up.fn 
-0001d630: 3d20 3f20 616e 6420 2b6d 742e 6b20 213d  = ? and +mt.k !=
-0001d640: 2027 7827 220a 2020 2020 2020 2020 2020   'x'".          
-0001d650: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-0001d660: 2020 2020 2020 2072 203d 2069 6375 722e         r = icur.
-0001d670: 6578 6563 7574 6528 712c 2028 7264 2c20  execute(q, (rd, 
-0001d680: 666e 2929 0a20 2020 2020 2020 2020 2020  fn)).           
-0001d690: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-0001d6a0: 6e20 6173 2065 783a 0a20 2020 2020 2020  n as ex:.       
-0001d6b0: 2020 2020 2020 2020 2069 6620 2264 6174           if "dat
-0001d6c0: 6162 6173 6520 6973 206c 6f63 6b65 6422  abase is locked"
-0001d6d0: 2069 6e20 7374 7228 6578 293a 0a20 2020   in str(ex):.   
-0001d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6f0: 2062 7265 616b 0a0a 2020 2020 2020 2020   break..        
-0001d700: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0001d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d720: 2061 7267 7320 3d20 7333 656e 6328 6964   args = s3enc(id
-0001d730: 782e 6d65 6d5f 6375 722c 2072 642c 2066  x.mem_cur, rd, f
-0001d740: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-0001d750: 2020 2020 2020 2072 203d 2069 6375 722e         r = icur.
-0001d760: 6578 6563 7574 6528 712c 2061 7267 7329  execute(q, args)
-0001d770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d780: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-0001d790: 2020 2020 2020 2020 2020 2020 2074 203d               t =
-0001d7a0: 2022 7461 6720 7265 6164 2065 7272 6f72   "tag read error
-0001d7b0: 2c20 7b7d 2f7b 7d5c 6e7b 7d22 0a20 2020  , {}/{}\n{}".   
-0001d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d7d0: 2073 656c 662e 6c6f 6728 742e 666f 726d   self.log(t.form
-0001d7e0: 6174 2872 642c 2066 6e2c 206d 696e 5f65  at(rd, fn, min_e
-0001d7f0: 7828 2929 290a 2020 2020 2020 2020 2020  x())).          
-0001d800: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-0001d810: 0a20 2020 2020 2020 2020 2020 2066 655b  .            fe[
-0001d820: 2274 6167 7322 5d20 3d20 7b6b 3a20 7620  "tags"] = {k: v 
-0001d830: 666f 7220 6b2c 2076 2069 6e20 727d 0a20  for k, v in r}. 
-0001d840: 2020 2020 2020 2020 2020 205f 203d 205b             _ = [
-0001d850: 7461 6773 6574 2e61 6464 286b 2920 666f  tagset.add(k) fo
-0001d860: 7220 6b20 696e 2066 655b 2274 6167 7322  r k in fe["tags"
-0001d870: 5d5d 0a0a 2020 2020 2020 2020 6966 2069  ]]..        if i
-0001d880: 6375 723a 0a20 2020 2020 2020 2020 2020  cur:.           
-0001d890: 2074 6167 6c69 7374 203d 205b 6b20 666f   taglist = [k fo
-0001d8a0: 7220 6b20 696e 2076 6e2e 666c 6167 732e  r k in vn.flags.
-0001d8b0: 6765 7428 226d 7465 222c 2022 2229 2e73  get("mte", "").s
-0001d8c0: 706c 6974 2822 2c22 2920 6966 206b 2069  plit(",") if k i
-0001d8d0: 6e20 7461 6773 6574 5d0a 2020 2020 2020  n tagset].      
-0001d8e0: 2020 2020 2020 666f 7220 6665 2069 6e20        for fe in 
-0001d8f0: 6469 7273 3a0a 2020 2020 2020 2020 2020  dirs:.          
-0001d900: 2020 2020 2020 6665 5b22 7461 6773 225d        fe["tags"]
-0001d910: 203d 207b 7d0a 2020 2020 2020 2020 656c   = {}.        el
-0001d920: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001d930: 7461 676c 6973 7420 3d20 6c69 7374 2874  taglist = list(t
-0001d940: 6167 7365 7429 0a0a 2020 2020 2020 2020  agset)..        
-0001d950: 6966 2069 735f 6c73 3a0a 2020 2020 2020  if is_ls:.      
-0001d960: 2020 2020 2020 6c73 5f72 6574 5b22 6469        ls_ret["di
-0001d970: 7273 225d 203d 2064 6972 730a 2020 2020  rs"] = dirs.    
-0001d980: 2020 2020 2020 2020 6c73 5f72 6574 5b22          ls_ret["
-0001d990: 6669 6c65 7322 5d20 3d20 6669 6c65 730a  files"] = files.
-0001d9a0: 2020 2020 2020 2020 2020 2020 6c73 5f72              ls_r
-0001d9b0: 6574 5b22 7461 676c 6973 7422 5d20 3d20  et["taglist"] = 
-0001d9c0: 7461 676c 6973 740a 2020 2020 2020 2020  taglist.        
-0001d9d0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0001d9e0: 7478 5f6c 7328 6c73 5f72 6574 290a 0a20  tx_ls(ls_ret).. 
-0001d9f0: 2020 2020 2020 2064 6f63 203d 2073 656c         doc = sel
-0001da00: 662e 7570 6172 616d 2e67 6574 2822 646f  f.uparam.get("do
-0001da10: 6322 2920 6966 2073 656c 662e 6361 6e5f  c") if self.can_
-0001da20: 7265 6164 2065 6c73 6520 4e6f 6e65 0a20  read else None. 
-0001da30: 2020 2020 2020 2069 6620 646f 633a 0a20         if doc:. 
-0001da40: 2020 2020 2020 2020 2020 2064 6f63 203d             doc =
-0001da50: 2075 6e71 756f 7465 7028 646f 632e 7265   unquotep(doc.re
-0001da60: 706c 6163 6528 222b 222c 2022 2022 292e  place("+", " ").
-0001da70: 7370 6c69 7428 223f 2229 5b30 5d29 0a20  split("?")[0]). 
-0001da80: 2020 2020 2020 2020 2020 206a 3261 5b22             j2a["
-0001da90: 646f 636e 616d 6522 5d20 3d20 646f 630a  docname"] = doc.
-0001daa0: 2020 2020 2020 2020 2020 2020 646f 6374              doct
-0001dab0: 7874 203d 204e 6f6e 650a 2020 2020 2020  xt = None.      
-0001dac0: 2020 2020 2020 6966 206e 6578 7428 2878        if next((x
-0001dad0: 2066 6f72 2078 2069 6e20 6669 6c65 7320   for x in files 
-0001dae0: 6966 2078 5b22 6e61 6d65 225d 203d 3d20  if x["name"] == 
-0001daf0: 646f 6329 2c20 4e6f 6e65 293a 0a20 2020  doc), None):.   
-0001db00: 2020 2020 2020 2020 2020 2020 2064 6f63               doc
-0001db10: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-0001db20: 6f69 6e28 6162 7370 6174 682c 2064 6f63  oin(abspath, doc
-0001db30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001db40: 2020 737a 203d 2062 6f73 2e70 6174 682e    sz = bos.path.
-0001db50: 6765 7473 697a 6528 646f 6370 6174 6829  getsize(docpath)
-0001db60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001db70: 2069 6620 737a 203c 2031 3032 3420 2a20   if sz < 1024 * 
-0001db80: 7365 6c66 2e61 7267 732e 7478 745f 6d61  self.args.txt_ma
-0001db90: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
-0001dba0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-0001dbb0: 2866 7365 6e63 2864 6f63 7061 7468 292c  (fsenc(docpath),
-0001dbc0: 2022 7262 2229 2061 7320 663a 0a20 2020   "rb") as f:.   
-0001dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dbe0: 2020 2020 2064 6f63 7478 7420 3d20 662e       doctxt = f.
-0001dbf0: 7265 6164 2829 2e64 6563 6f64 6528 2275  read().decode("u
-0001dc00: 7466 2d38 222c 2022 7265 706c 6163 6522  tf-8", "replace"
-0001dc10: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-0001dc20: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001dc30: 2020 2020 7365 6c66 2e6c 6f67 2822 646f      self.log("do
-0001dc40: 6320 3430 343a 205b 7b7d 5d22 2e66 6f72  c 404: [{}]".for
-0001dc50: 6d61 7428 646f 6329 2c20 633d 3629 0a20  mat(doc), c=6). 
-0001dc60: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0001dc70: 6f63 7478 7420 3d20 2228 2074 6578 7466  octxt = "( textf
-0001dc80: 696c 6520 6e6f 7420 666f 756e 6420 2922  ile not found )"
-0001dc90: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0001dca0: 2064 6f63 7478 7420 6973 206e 6f74 204e   doctxt is not N
-0001dcb0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0001dcc0: 2020 2020 206a 3261 5b22 646f 6322 5d20       j2a["doc"] 
-0001dcd0: 3d20 646f 6374 7874 0a0a 2020 2020 2020  = doctxt..      
-0001dce0: 2020 666f 7220 6420 696e 2064 6972 733a    for d in dirs:
-0001dcf0: 0a20 2020 2020 2020 2020 2020 2064 5b22  .            d["
-0001dd00: 6e61 6d65 225d 202b 3d20 222f 220a 0a20  name"] += "/".. 
-0001dd10: 2020 2020 2020 2064 6972 732e 736f 7274         dirs.sort
-0001dd20: 286b 6579 3d69 7465 6d67 6574 7465 7228  (key=itemgetter(
-0001dd30: 226e 616d 6522 2929 0a0a 2020 2020 2020  "name"))..      
-0001dd40: 2020 6966 2069 735f 6a73 3a0a 2020 2020    if is_js:.    
-0001dd50: 2020 2020 2020 2020 6a32 615b 226c 7330          j2a["ls0
-0001dd60: 225d 203d 207b 2264 6972 7322 3a20 6469  "] = {"dirs": di
-0001dd70: 7273 2c20 2266 696c 6573 223a 2066 696c  rs, "files": fil
-0001dd80: 6573 2c20 2274 6167 6c69 7374 223a 2074  es, "taglist": t
-0001dd90: 6167 6c69 7374 7d0a 2020 2020 2020 2020  aglist}.        
-0001dda0: 2020 2020 6a32 615b 2266 696c 6573 225d      j2a["files"]
-0001ddb0: 203d 205b 5d0a 2020 2020 2020 2020 656c   = [].        el
-0001ddc0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001ddd0: 6a32 615b 2266 696c 6573 225d 203d 2064  j2a["files"] = d
-0001dde0: 6972 7320 2b20 6669 6c65 730a 0a20 2020  irs + files..   
-0001ddf0: 2020 2020 206a 3261 5b22 7461 676c 6973       j2a["taglis
-0001de00: 7422 5d20 3d20 7461 676c 6973 740a 2020  t"] = taglist.  
-0001de10: 2020 2020 2020 6a32 615b 2274 7874 5f65        j2a["txt_e
-0001de20: 7874 225d 203d 2073 656c 662e 6172 6773  xt"] = self.args
-0001de30: 2e74 6578 7466 696c 6573 2e72 6570 6c61  .textfiles.repla
-0001de40: 6365 2822 2c22 2c20 2220 2229 0a0a 2020  ce(",", " ")..  
-0001de50: 2020 2020 2020 6966 2022 6d74 6822 2069        if "mth" i
-0001de60: 6e20 766e 2e66 6c61 6773 3a0a 2020 2020  n vn.flags:.    
-0001de70: 2020 2020 2020 2020 6a32 615b 2264 6566          j2a["def
-0001de80: 5f68 636f 6c73 225d 203d 2076 6e2e 666c  _hcols"] = vn.fl
-0001de90: 6167 735b 226d 7468 225d 2e73 706c 6974  ags["mth"].split
-0001dea0: 2822 2c22 290a 0a20 2020 2020 2020 2068  (",")..        h
-0001deb0: 746d 6c20 3d20 7365 6c66 2e6a 3273 2874  tml = self.j2s(t
-0001dec0: 706c 2c20 2a2a 6a32 6129 0a20 2020 2020  pl, **j2a).     
-0001ded0: 2020 2073 656c 662e 7265 706c 7928 6874     self.reply(ht
-0001dee0: 6d6c 2e65 6e63 6f64 6528 2275 7466 2d38  ml.encode("utf-8
-0001def0: 222c 2022 7265 706c 6163 6522 2929 0a20  ", "replace")). 
-0001df00: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0001df10: 7565 0a                                  ue.
+0001ba90: 2020 756e 6c69 7374 203d 2076 662e 6765    unlist = vf.ge
+0001baa0: 7428 2275 6e6c 6973 7422 2c20 2222 290a  t("unlist", "").
+0001bab0: 2020 2020 2020 2020 6c73 5f72 6574 203d          ls_ret =
+0001bac0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+0001bad0: 6469 7273 223a 205b 5d2c 0a20 2020 2020  dirs": [],.     
+0001bae0: 2020 2020 2020 2022 6669 6c65 7322 3a20         "files": 
+0001baf0: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+0001bb00: 2274 6167 6c69 7374 223a 205b 5d2c 0a20  "taglist": [],. 
+0001bb10: 2020 2020 2020 2020 2020 2022 7372 7669             "srvi
+0001bb20: 6e66 223a 2073 7276 5f69 6e66 6f74 2c0a  nf": srv_infot,.
+0001bb30: 2020 2020 2020 2020 2020 2020 2261 6363              "acc
+0001bb40: 7422 3a20 7365 6c66 2e75 6e61 6d65 2c0a  t": self.uname,.
+0001bb50: 2020 2020 2020 2020 2020 2020 2269 6478              "idx
+0001bb60: 223a 2065 3264 2c0a 2020 2020 2020 2020  ": e2d,.        
+0001bb70: 2020 2020 2269 7461 6722 3a20 6532 742c      "itag": e2t,
+0001bb80: 0a20 2020 2020 2020 2020 2020 2022 6c69  .            "li
+0001bb90: 6665 7469 6d65 223a 2076 6e2e 666c 6167  fetime": vn.flag
+0001bba0: 732e 6765 7428 226c 6966 6574 696d 6522  s.get("lifetime"
+0001bbb0: 2920 6f72 2030 2c0a 2020 2020 2020 2020  ) or 0,.        
+0001bbc0: 2020 2020 2266 7261 6e64 223a 2062 6f6f      "frand": boo
+0001bbd0: 6c28 766e 2e66 6c61 6773 2e67 6574 2822  l(vn.flags.get("
+0001bbe0: 7261 6e64 2229 292c 0a20 2020 2020 2020  rand")),.       
+0001bbf0: 2020 2020 2022 756e 6c69 7374 223a 2075       "unlist": u
+0001bc00: 6e6c 6973 742c 0a20 2020 2020 2020 2020  nlist,.         
+0001bc10: 2020 2022 7065 726d 7322 3a20 7065 726d     "perms": perm
+0001bc20: 732c 0a20 2020 2020 2020 2020 2020 2022  s,.            "
+0001bc30: 6c6f 6775 6573 223a 206c 6f67 7565 732c  logues": logues,
+0001bc40: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+0001bc50: 6164 6d65 223a 2072 6561 646d 652c 0a20  adme": readme,. 
+0001bc60: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+0001bc70: 206a 3261 203d 207b 0a20 2020 2020 2020   j2a = {.       
+0001bc80: 2020 2020 2022 7664 6972 223a 2071 756f       "vdir": quo
+0001bc90: 7465 7028 7365 6c66 2e76 7061 7468 292c  tep(self.vpath),
+0001bca0: 0a20 2020 2020 2020 2020 2020 2022 7670  .            "vp
+0001bcb0: 6e6f 6465 7322 3a20 7670 6e6f 6465 732c  nodes": vpnodes,
+0001bcc0: 0a20 2020 2020 2020 2020 2020 2022 6669  .            "fi
+0001bcd0: 6c65 7322 3a20 5b5d 2c0a 2020 2020 2020  les": [],.      
+0001bce0: 2020 2020 2020 226c 7330 223a 204e 6f6e        "ls0": Non
+0001bcf0: 652c 0a20 2020 2020 2020 2020 2020 2022  e,.            "
+0001bd00: 6163 6374 223a 2073 656c 662e 756e 616d  acct": self.unam
+0001bd10: 652c 0a20 2020 2020 2020 2020 2020 2022  e,.            "
+0001bd20: 7065 726d 7322 3a20 6a73 6f6e 2e64 756d  perms": json.dum
+0001bd30: 7073 2870 6572 6d73 292c 0a20 2020 2020  ps(perms),.     
+0001bd40: 2020 2020 2020 2022 6c69 6665 7469 6d65         "lifetime
+0001bd50: 223a 206c 735f 7265 745b 226c 6966 6574  ": ls_ret["lifet
+0001bd60: 696d 6522 5d2c 0a20 2020 2020 2020 2020  ime"],.         
+0001bd70: 2020 2022 6672 616e 6422 3a20 626f 6f6c     "frand": bool
+0001bd80: 2876 6e2e 666c 6167 732e 6765 7428 2272  (vn.flags.get("r
+0001bd90: 616e 6422 2929 2c0a 2020 2020 2020 2020  and")),.        
+0001bda0: 2020 2020 2274 6167 6c69 7374 223a 205b      "taglist": [
+0001bdb0: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
+0001bdc0: 6465 665f 6863 6f6c 7322 3a20 5b5d 2c0a  def_hcols": [],.
+0001bdd0: 2020 2020 2020 2020 2020 2020 2268 6176              "hav
+0001bde0: 655f 656d 7022 3a20 7365 6c66 2e61 7267  e_emp": self.arg
+0001bdf0: 732e 656d 702c 0a20 2020 2020 2020 2020  s.emp,.         
+0001be00: 2020 2022 6861 7665 5f75 7032 6b5f 6964     "have_up2k_id
+0001be10: 7822 3a20 6532 642c 0a20 2020 2020 2020  x": e2d,.       
+0001be20: 2020 2020 2022 6861 7665 5f74 6167 735f       "have_tags_
+0001be30: 6964 7822 3a20 6532 742c 0a20 2020 2020  idx": e2t,.     
+0001be40: 2020 2020 2020 2022 6861 7665 5f61 636f         "have_aco
+0001be50: 6465 223a 2028 6e6f 7420 7365 6c66 2e61  de": (not self.a
+0001be60: 7267 732e 6e6f 5f61 636f 6465 292c 0a20  rgs.no_acode),. 
+0001be70: 2020 2020 2020 2020 2020 2022 6861 7665             "have
+0001be80: 5f6d 7622 3a20 286e 6f74 2073 656c 662e  _mv": (not self.
+0001be90: 6172 6773 2e6e 6f5f 6d76 292c 0a20 2020  args.no_mv),.   
+0001bea0: 2020 2020 2020 2020 2022 6861 7665 5f64           "have_d
+0001beb0: 656c 223a 2028 6e6f 7420 7365 6c66 2e61  el": (not self.a
+0001bec0: 7267 732e 6e6f 5f64 656c 292c 0a20 2020  rgs.no_del),.   
+0001bed0: 2020 2020 2020 2020 2022 6861 7665 5f7a           "have_z
+0001bee0: 6970 223a 2028 6e6f 7420 7365 6c66 2e61  ip": (not self.a
+0001bef0: 7267 732e 6e6f 5f7a 6970 292c 0a20 2020  rgs.no_zip),.   
+0001bf00: 2020 2020 2020 2020 2022 6861 7665 5f75           "have_u
+0001bf10: 6e70 6f73 7422 3a20 696e 7428 7365 6c66  npost": int(self
+0001bf20: 2e61 7267 732e 756e 706f 7374 292c 0a20  .args.unpost),. 
+0001bf30: 2020 2020 2020 2020 2020 2022 6861 7665             "have
+0001bf40: 5f62 5f75 223a 2028 7365 6c66 2e63 616e  _b_u": (self.can
+0001bf50: 5f77 7269 7465 2061 6e64 2073 656c 662e  _write and self.
+0001bf60: 7570 6172 616d 2e67 6574 2822 6222 2920  uparam.get("b") 
+0001bf70: 3d3d 2022 7522 292c 0a20 2020 2020 2020  == "u"),.       
+0001bf80: 2020 2020 2022 7362 5f6d 6422 3a20 2222       "sb_md": ""
+0001bf90: 2069 6620 226e 6f5f 7362 5f6d 6422 2069   if "no_sb_md" i
+0001bfa0: 6e20 7666 2065 6c73 6520 2876 662e 6765  n vf else (vf.ge
+0001bfb0: 7428 226d 645f 7362 6622 2920 6f72 2022  t("md_sbf") or "
+0001bfc0: 7922 292c 0a20 2020 2020 2020 2020 2020  y"),.           
+0001bfd0: 2022 7362 5f6c 6722 3a20 2222 2069 6620   "sb_lg": "" if 
+0001bfe0: 226e 6f5f 7362 5f6c 6722 2069 6e20 7666  "no_sb_lg" in vf
+0001bff0: 2065 6c73 6520 2876 662e 6765 7428 226c   else (vf.get("l
+0001c000: 675f 7362 6622 2920 6f72 2022 7922 292c  g_sbf") or "y"),
+0001c010: 0a20 2020 2020 2020 2020 2020 2022 7572  .            "ur
+0001c020: 6c5f 7375 6622 3a20 7572 6c5f 7375 662c  l_suf": url_suf,
+0001c030: 0a20 2020 2020 2020 2020 2020 2022 6c6f  .            "lo
+0001c040: 6775 6573 223a 206c 6f67 7565 732c 0a20  gues": logues,. 
+0001c050: 2020 2020 2020 2020 2020 2022 7265 6164             "read
+0001c060: 6d65 223a 2072 6561 646d 652c 0a20 2020  me": readme,.   
+0001c070: 2020 2020 2020 2020 2022 7469 746c 6522           "title"
+0001c080: 3a20 6874 6d6c 5f65 7363 6170 6528 7365  : html_escape(se
+0001c090: 6c66 2e76 7061 7468 2c20 6372 6c66 3d54  lf.vpath, crlf=T
+0001c0a0: 7275 6529 206f 7220 22f0 9f92 bef0 9f8e  rue) or ".......
+0001c0b0: 8922 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+0001c0c0: 2273 7276 5f69 6e66 6f22 3a20 7372 765f  "srv_info": srv_
+0001c0d0: 696e 666f 742c 0a20 2020 2020 2020 2020  infot,.         
+0001c0e0: 2020 2022 6467 7269 6422 3a20 2267 7269     "dgrid": "gri
+0001c0f0: 6422 2069 6e20 7666 2c0a 2020 2020 2020  d" in vf,.      
+0001c100: 2020 2020 2020 2275 6e6c 6973 7422 3a20        "unlist": 
+0001c110: 756e 6c69 7374 2c0a 2020 2020 2020 2020  unlist,.        
+0001c120: 2020 2020 2264 7468 656d 6522 3a20 7365      "dtheme": se
+0001c130: 6c66 2e61 7267 732e 7468 656d 652c 0a20  lf.args.theme,. 
+0001c140: 2020 2020 2020 2020 2020 2022 7468 656d             "them
+0001c150: 6573 223a 2073 656c 662e 6172 6773 2e74  es": self.args.t
+0001c160: 6865 6d65 732c 0a20 2020 2020 2020 2020  hemes,.         
+0001c170: 2020 2022 7475 7262 6f6c 766c 223a 2073     "turbolvl": s
+0001c180: 656c 662e 6172 6773 2e74 7572 626f 2c0a  elf.args.turbo,.
+0001c190: 2020 2020 2020 2020 2020 2020 2269 6478              "idx
+0001c1a0: 6822 3a20 696e 7428 7365 6c66 2e61 7267  h": int(self.arg
+0001c1b0: 732e 6968 292c 0a20 2020 2020 2020 2020  s.ih),.         
+0001c1c0: 2020 2022 7532 736f 7274 223a 2073 656c     "u2sort": sel
+0001c1d0: 662e 6172 6773 2e75 3273 6f72 742c 0a20  f.args.u2sort,. 
+0001c1e0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+0001c1f0: 2020 6966 2073 656c 662e 6172 6773 2e6a    if self.args.j
+0001c200: 735f 6272 6f77 7365 723a 0a20 2020 2020  s_browser:.     
+0001c210: 2020 2020 2020 206a 3261 5b22 6a73 225d         j2a["js"]
+0001c220: 203d 2073 656c 662e 6172 6773 2e6a 735f   = self.args.js_
+0001c230: 6272 6f77 7365 720a 0a20 2020 2020 2020  browser..       
+0001c240: 2069 6620 7365 6c66 2e61 7267 732e 6373   if self.args.cs
+0001c250: 735f 6272 6f77 7365 723a 0a20 2020 2020  s_browser:.     
+0001c260: 2020 2020 2020 206a 3261 5b22 6373 7322         j2a["css"
+0001c270: 5d20 3d20 7365 6c66 2e61 7267 732e 6373  ] = self.args.cs
+0001c280: 735f 6272 6f77 7365 720a 0a20 2020 2020  s_browser..     
+0001c290: 2020 2069 6620 6e6f 7420 7365 6c66 2e63     if not self.c
+0001c2a0: 6f6e 6e2e 6873 7276 2e70 7269 736d 3a0a  onn.hsrv.prism:.
+0001c2b0: 2020 2020 2020 2020 2020 2020 6a32 615b              j2a[
+0001c2c0: 226e 6f5f 7072 6973 6d22 5d20 3d20 5472  "no_prism"] = Tr
+0001c2d0: 7565 0a0a 2020 2020 2020 2020 6966 206e  ue..        if n
+0001c2e0: 6f74 2073 656c 662e 6361 6e5f 7265 6164  ot self.can_read
+0001c2f0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0001c300: 2069 735f 6c73 3a0a 2020 2020 2020 2020   is_ls:.        
+0001c310: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0001c320: 656c 662e 7478 5f6c 7328 6c73 5f72 6574  elf.tx_ls(ls_ret
+0001c330: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0001c340: 6620 6e6f 7420 7374 6174 2e53 5f49 5344  f not stat.S_ISD
+0001c350: 4952 2873 742e 7374 5f6d 6f64 6529 3a0a  IR(st.st_mode):.
+0001c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c370: 7265 7475 726e 2073 656c 662e 7478 5f34  return self.tx_4
+0001c380: 3034 2854 7275 6529 0a0a 2020 2020 2020  04(True)..      
+0001c390: 2020 2020 2020 6966 2022 7a69 7022 2069        if "zip" i
+0001c3a0: 6e20 7365 6c66 2e75 7061 7261 6d20 6f72  n self.uparam or
+0001c3b0: 2022 7461 7222 2069 6e20 7365 6c66 2e75   "tar" in self.u
+0001c3c0: 7061 7261 6d3a 0a20 2020 2020 2020 2020  param:.         
+0001c3d0: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
+0001c3e0: 6b61 6328 3430 3329 0a0a 2020 2020 2020  kac(403)..      
+0001c3f0: 2020 2020 2020 6874 6d6c 203d 2073 656c        html = sel
+0001c400: 662e 6a32 7328 7470 6c2c 202a 2a6a 3261  f.j2s(tpl, **j2a
+0001c410: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0001c420: 6c66 2e72 6570 6c79 2868 746d 6c2e 656e  lf.reply(html.en
+0001c430: 636f 6465 2822 7574 662d 3822 2c20 2272  code("utf-8", "r
+0001c440: 6570 6c61 6365 2229 290a 2020 2020 2020  eplace")).      
+0001c450: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+0001c460: 650a 0a20 2020 2020 2020 2066 6f72 206b  e..        for k
+0001c470: 2069 6e20 5b22 7a69 7022 2c20 2274 6172   in ["zip", "tar
+0001c480: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+0001c490: 7620 3d20 7365 6c66 2e75 7061 7261 6d2e  v = self.uparam.
+0001c4a0: 6765 7428 6b29 0a20 2020 2020 2020 2020  get(k).         
+0001c4b0: 2020 2069 6620 7620 6973 206e 6f74 204e     if v is not N
+0001c4c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0001c4d0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0001c4e0: 2e74 785f 7a69 7028 6b2c 2076 2c20 7365  .tx_zip(k, v, se
+0001c4f0: 6c66 2e76 7061 7468 2c20 766e 2c20 7265  lf.vpath, vn, re
+0001c500: 6d2c 205b 5d2c 2073 656c 662e 6172 6773  m, [], self.args
+0001c510: 2e65 6429 0a0a 2020 2020 2020 2020 6673  .ed)..        fs
+0001c520: 726f 6f74 2c20 7666 735f 6c73 2c20 7666  root, vfs_ls, vf
+0001c530: 735f 7669 7274 203d 2076 6e2e 6c73 280a  s_virt = vn.ls(.
+0001c540: 2020 2020 2020 2020 2020 2020 7265 6d2c              rem,
+0001c550: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001c560: 662e 756e 616d 652c 0a20 2020 2020 2020  f.uname,.       
+0001c570: 2020 2020 206e 6f74 2073 656c 662e 6172       not self.ar
+0001c580: 6773 2e6e 6f5f 7363 616e 6469 722c 0a20  gs.no_scandir,. 
+0001c590: 2020 2020 2020 2020 2020 205b 5b54 7275             [[Tru
+0001c5a0: 652c 2046 616c 7365 5d2c 205b 4661 6c73  e, False], [Fals
+0001c5b0: 652c 2054 7275 655d 5d2c 0a20 2020 2020  e, True]],.     
+0001c5c0: 2020 2020 2020 206c 7374 6174 3d22 6c74         lstat="lt
+0001c5d0: 2220 696e 2073 656c 662e 7570 6172 616d  " in self.uparam
+0001c5e0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+0001c5f0: 2020 2020 7374 6174 7320 3d20 7b6b 3a20      stats = {k: 
+0001c600: 7620 666f 7220 6b2c 2076 2069 6e20 7666  v for k, v in vf
+0001c610: 735f 6c73 7d0a 2020 2020 2020 2020 6c73  s_ls}.        ls
+0001c620: 5f6e 616d 6573 203d 205b 785b 305d 2066  _names = [x[0] f
+0001c630: 6f72 2078 2069 6e20 7666 735f 6c73 5d0a  or x in vfs_ls].
+0001c640: 2020 2020 2020 2020 6c73 5f6e 616d 6573          ls_names
+0001c650: 2e65 7874 656e 6428 6c69 7374 2876 6673  .extend(list(vfs
+0001c660: 5f76 6972 742e 6b65 7973 2829 2929 0a0a  _virt.keys()))..
+0001c670: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
+0001c680: 666f 7220 6f6c 6420 7665 7273 696f 6e73  for old versions
+0001c690: 206f 6620 6669 6c65 732c 0a20 2020 2020   of files,.     
+0001c6a0: 2020 2023 205b 6e75 6d2d 6261 636b 7570     # [num-backup
+0001c6b0: 732c 206d 6f73 742d 7265 6365 6e74 2c20  s, most-recent, 
+0001c6c0: 6869 7374 2d70 6174 685d 0a20 2020 2020  hist-path].     
+0001c6d0: 2020 2068 6973 7420 2020 2020 3d20 7b7d     hist     = {}
+0001c6e0: 0a20 2020 2020 2020 2068 6973 7464 6972  .        histdir
+0001c6f0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+0001c700: 6673 726f 6f74 2c20 222e 6869 7374 2229  fsroot, ".hist")
+0001c710: 0a20 2020 2020 2020 2070 746e 203d 2072  .        ptn = r
+0001c720: 652e 636f 6d70 696c 6528 7222 282e 2a29  e.compile(r"(.*)
+0001c730: 5c2e 285b 302d 395d 2b5c 2e5b 302d 395d  \.([0-9]+\.[0-9]
+0001c740: 7b33 7d29 285c 2e5b 5e5c 2e5d 2b29 2422  {3})(\.[^\.]+)$"
+0001c750: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
+0001c760: 2020 2020 2020 2020 2020 2066 6f72 2068             for h
+0001c770: 666e 2069 6e20 626f 732e 6c69 7374 6469  fn in bos.listdi
+0001c780: 7228 6869 7374 6469 7229 3a0a 2020 2020  r(histdir):.    
+0001c790: 2020 2020 2020 2020 2020 2020 6d20 3d20              m = 
+0001c7a0: 7074 6e2e 6d61 7463 6828 6866 6e29 0a20  ptn.match(hfn). 
+0001c7b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001c7c0: 6620 6e6f 7420 6d3a 0a20 2020 2020 2020  f not m:.       
+0001c7d0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+0001c7e0: 7469 6e75 650a 0a20 2020 2020 2020 2020  tinue..         
+0001c7f0: 2020 2020 2020 2066 6e20 3d20 6d2e 6772         fn = m.gr
+0001c800: 6f75 7028 3129 202b 206d 2e67 726f 7570  oup(1) + m.group
+0001c810: 2833 290a 2020 2020 2020 2020 2020 2020  (3).            
+0001c820: 2020 2020 6e2c 2074 732c 205f 203d 2068      n, ts, _ = h
+0001c830: 6973 742e 6765 7428 666e 2c20 2830 2c20  ist.get(fn, (0, 
+0001c840: 302c 2022 2229 290a 2020 2020 2020 2020  0, "")).        
+0001c850: 2020 2020 2020 2020 6869 7374 5b66 6e5d          hist[fn]
+0001c860: 203d 2028 6e20 2b20 312c 206d 6178 2874   = (n + 1, max(t
+0001c870: 732c 2066 6c6f 6174 286d 2e67 726f 7570  s, float(m.group
+0001c880: 2832 2929 292c 2068 666e 290a 2020 2020  (2))), hfn).    
+0001c890: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
+0001c8a0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+0001c8b0: 2020 2020 2020 2320 7368 6f77 2064 6f74        # show dot
+0001c8c0: 6669 6c65 7320 6966 2070 6572 6d69 7474  files if permitt
+0001c8d0: 6564 2061 6e64 2072 6571 7565 7374 6564  ed and requested
+0001c8e0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0001c8f0: 7365 6c66 2e61 7267 732e 6564 206f 7220  self.args.ed or 
+0001c900: 2264 6f74 7322 206e 6f74 2069 6e20 7365  "dots" not in se
+0001c910: 6c66 2e75 7061 7261 6d3a 0a20 2020 2020  lf.uparam:.     
+0001c920: 2020 2020 2020 206c 735f 6e61 6d65 7320         ls_names 
+0001c930: 3d20 6578 636c 7564 655f 646f 7466 696c  = exclude_dotfil
+0001c940: 6573 286c 735f 6e61 6d65 7329 0a0a 2020  es(ls_names)..  
+0001c950: 2020 2020 2020 6164 645f 666b 203d 2076        add_fk = v
+0001c960: 6e2e 666c 6167 732e 6765 7428 2266 6b22  n.flags.get("fk"
+0001c970: 290a 0a20 2020 2020 2020 2064 6972 7320  )..        dirs 
+0001c980: 3d20 5b5d 0a20 2020 2020 2020 2066 696c  = [].        fil
+0001c990: 6573 203d 205b 5d0a 2020 2020 2020 2020  es = [].        
+0001c9a0: 666f 7220 666e 2069 6e20 6c73 5f6e 616d  for fn in ls_nam
+0001c9b0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+0001c9c0: 6261 7365 203d 2022 220a 2020 2020 2020  base = "".      
+0001c9d0: 2020 2020 2020 6872 6566 203d 2066 6e0a        href = fn.
+0001c9e0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0001c9f0: 6f74 2069 735f 6c73 2061 6e64 206e 6f74  ot is_ls and not
+0001ca00: 2069 735f 6a73 2061 6e64 206e 6f74 2073   is_js and not s
+0001ca10: 656c 662e 7472 6169 6c69 6e67 5f73 6c61  elf.trailing_sla
+0001ca20: 7368 2061 6e64 2076 7061 7468 3a0a 2020  sh and vpath:.  
+0001ca30: 2020 2020 2020 2020 2020 2020 2020 6261                ba
+0001ca40: 7365 203d 2022 2f22 202b 2076 7061 7468  se = "/" + vpath
+0001ca50: 202b 2022 2f22 0a20 2020 2020 2020 2020   + "/".         
+0001ca60: 2020 2020 2020 2068 7265 6620 3d20 6261         href = ba
+0001ca70: 7365 202b 2066 6e0a 0a20 2020 2020 2020  se + fn..       
+0001ca80: 2020 2020 2069 6620 666e 2069 6e20 7666       if fn in vf
+0001ca90: 735f 7669 7274 3a0a 2020 2020 2020 2020  s_virt:.        
+0001caa0: 2020 2020 2020 2020 6673 7061 7468 203d          fspath =
+0001cab0: 2076 6673 5f76 6972 745b 666e 5d2e 7265   vfs_virt[fn].re
+0001cac0: 616c 7061 7468 0a20 2020 2020 2020 2020  alpath.         
+0001cad0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001cae0: 2020 2020 2020 2020 2066 7370 6174 6820           fspath 
+0001caf0: 3d20 6673 726f 6f74 202b 2022 2f22 202b  = fsroot + "/" +
+0001cb00: 2066 6e0a 0a20 2020 2020 2020 2020 2020   fn..           
+0001cb10: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0001cb20: 2020 2020 2020 6c69 6e66 203d 2073 7461        linf = sta
+0001cb30: 7473 2e67 6574 2866 6e29 206f 7220 626f  ts.get(fn) or bo
+0001cb40: 732e 6c73 7461 7428 6673 7061 7468 290a  s.lstat(fspath).
+0001cb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cb60: 696e 6620 3d20 626f 732e 7374 6174 2866  inf = bos.stat(f
+0001cb70: 7370 6174 6829 2069 6620 7374 6174 2e53  spath) if stat.S
+0001cb80: 5f49 534c 4e4b 286c 696e 662e 7374 5f6d  _ISLNK(linf.st_m
+0001cb90: 6f64 6529 2065 6c73 6520 6c69 6e66 0a20  ode) else linf. 
+0001cba0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+0001cbb0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0001cbc0: 2020 2073 656c 662e 6c6f 6728 2262 726f     self.log("bro
+0001cbd0: 6b65 6e20 7379 6d6c 696e 6b3a 207b 7d22  ken symlink: {}"
+0001cbe0: 2e66 6f72 6d61 7428 7265 7072 2866 7370  .format(repr(fsp
+0001cbf0: 6174 6829 2929 0a20 2020 2020 2020 2020  ath))).         
+0001cc00: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+0001cc10: 0a20 2020 2020 2020 2020 2020 2069 735f  .            is_
+0001cc20: 6469 7220 3d20 7374 6174 2e53 5f49 5344  dir = stat.S_ISD
+0001cc30: 4952 2869 6e66 2e73 745f 6d6f 6465 290a  IR(inf.st_mode).
+0001cc40: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0001cc50: 735f 6469 723a 0a20 2020 2020 2020 2020  s_dir:.         
+0001cc60: 2020 2020 2020 2068 7265 6620 2b3d 2022         href += "
+0001cc70: 2f22 0a20 2020 2020 2020 2020 2020 2020  /".             
+0001cc80: 2020 2069 6620 7365 6c66 2e61 7267 732e     if self.args.
+0001cc90: 6e6f 5f7a 6970 3a0a 2020 2020 2020 2020  no_zip:.        
+0001cca0: 2020 2020 2020 2020 2020 2020 6d61 7267              marg
+0001ccb0: 696e 203d 2022 4449 5222 0a20 2020 2020  in = "DIR".     
+0001ccc0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001ccd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001cce0: 2020 2020 206d 6172 6769 6e20 3d20 273c       margin = '<
+0001ccf0: 6120 6872 6566 3d22 2573 3f7a 6970 2220  a href="%s?zip" 
+0001cd00: 7265 6c3d 226e 6f66 6f6c 6c6f 7722 3e7a  rel="nofollow">z
+0001cd10: 6970 3c2f 613e 2720 2520 2871 756f 7465  ip</a>' % (quote
+0001cd20: 7028 6872 6566 292c 290a 2020 2020 2020  p(href),).      
+0001cd30: 2020 2020 2020 656c 6966 2066 6e20 696e        elif fn in
+0001cd40: 2068 6973 743a 0a20 2020 2020 2020 2020   hist:.         
+0001cd50: 2020 2020 2020 206d 6172 6769 6e20 3d20         margin = 
+0001cd60: 273c 6120 6872 6566 3d22 2573 2e68 6973  '<a href="%s.his
+0001cd70: 742f 2573 223e 2325 733c 2f61 3e27 2025  t/%s">#%s</a>' %
+0001cd80: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0001cd90: 2020 2020 2020 2062 6173 652c 0a20 2020         base,.   
+0001cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cdb0: 2068 746d 6c5f 6573 6361 7065 2868 6973   html_escape(his
+0001cdc0: 745b 666e 5d5b 325d 2c20 7175 6f74 3d54  t[fn][2], quot=T
+0001cdd0: 7275 652c 2063 726c 663d 5472 7565 292c  rue, crlf=True),
+0001cde0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001cdf0: 2020 2020 2068 6973 745b 666e 5d5b 305d       hist[fn][0]
+0001ce00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001ce10: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0001ce20: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001ce30: 2020 2020 2020 6d61 7267 696e 203d 2022        margin = "
+0001ce40: 2d22 0a0a 2020 2020 2020 2020 2020 2020  -"..            
+0001ce50: 737a 203d 2069 6e66 2e73 745f 7369 7a65  sz = inf.st_size
+0001ce60: 0a20 2020 2020 2020 2020 2020 207a 6420  .            zd 
+0001ce70: 3d20 6461 7465 7469 6d65 2e75 7463 6672  = datetime.utcfr
+0001ce80: 6f6d 7469 6d65 7374 616d 7028 6c69 6e66  omtimestamp(linf
+0001ce90: 2e73 745f 6d74 696d 6529 0a20 2020 2020  .st_mtime).     
+0001cea0: 2020 2020 2020 2064 7420 3d20 2225 3034         dt = "%04
+0001ceb0: 642d 2530 3264 2d25 3032 6420 2530 3264  d-%02d-%02d %02d
+0001cec0: 3a25 3032 643a 2530 3264 2220 2520 280a  :%02d:%02d" % (.
+0001ced0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cee0: 7a64 2e79 6561 722c 0a20 2020 2020 2020  zd.year,.       
+0001cef0: 2020 2020 2020 2020 207a 642e 6d6f 6e74           zd.mont
+0001cf00: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
+0001cf10: 2020 207a 642e 6461 792c 0a20 2020 2020     zd.day,.     
+0001cf20: 2020 2020 2020 2020 2020 207a 642e 686f             zd.ho
+0001cf30: 7572 2c0a 2020 2020 2020 2020 2020 2020  ur,.            
+0001cf40: 2020 2020 7a64 2e6d 696e 7574 652c 0a20      zd.minute,. 
+0001cf50: 2020 2020 2020 2020 2020 2020 2020 207a                 z
+0001cf60: 642e 7365 636f 6e64 2c0a 2020 2020 2020  d.second,.      
+0001cf70: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0001cf80: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0001cf90: 2020 2020 2020 2020 2020 6578 7420 3d20            ext = 
+0001cfa0: 222d 2d2d 2220 6966 2069 735f 6469 7220  "---" if is_dir 
+0001cfb0: 656c 7365 2066 6e2e 7273 706c 6974 2822  else fn.rsplit("
+0001cfc0: 2e22 2c20 3129 5b31 5d0a 2020 2020 2020  .", 1)[1].      
+0001cfd0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+0001cfe0: 2865 7874 2920 3e20 3136 3a0a 2020 2020  (ext) > 16:.    
+0001cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d000: 6578 7420 3d20 6578 745b 3a31 365d 0a20  ext = ext[:16]. 
+0001d010: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+0001d020: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0001d030: 2020 2065 7874 203d 2022 2522 0a0a 2020     ext = "%"..  
+0001d040: 2020 2020 2020 2020 2020 6966 2061 6464            if add
+0001d050: 5f66 6b3a 0a20 2020 2020 2020 2020 2020  _fk:.           
+0001d060: 2020 2020 2068 7265 6620 3d20 2225 733f       href = "%s?
+0001d070: 6b3d 2573 2220 2520 280a 2020 2020 2020  k=%s" % (.      
+0001d080: 2020 2020 2020 2020 2020 2020 2020 7175                qu
+0001d090: 6f74 6570 2868 7265 6629 2c0a 2020 2020  otep(href),.    
+0001d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d0b0: 7365 6c66 2e67 656e 5f66 6b28 0a20 2020  self.gen_fk(.   
+0001d0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d0d0: 2020 2020 2073 656c 662e 6172 6773 2e66       self.args.f
+0001d0e0: 6b5f 7361 6c74 2c20 6673 7061 7468 2c20  k_salt, fspath, 
+0001d0f0: 737a 2c20 3020 6966 2041 4e59 5749 4e20  sz, 0 if ANYWIN 
+0001d100: 656c 7365 2069 6e66 2e73 745f 696e 6f0a  else inf.st_ino.
+0001d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d120: 2020 2020 295b 3a61 6464 5f66 6b5d 2c0a      )[:add_fk],.
+0001d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d140: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0001d150: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0001d160: 2020 2020 6872 6566 203d 2071 756f 7465      href = quote
+0001d170: 7028 6872 6566 290a 0a20 2020 2020 2020  p(href)..       
+0001d180: 2020 2020 2069 7465 6d20 3d20 7b0a 2020       item = {.  
+0001d190: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+0001d1a0: 6561 6422 3a20 6d61 7267 696e 2c0a 2020  ead": margin,.  
+0001d1b0: 2020 2020 2020 2020 2020 2020 2020 2268                "h
+0001d1c0: 7265 6622 3a20 6872 6566 2c0a 2020 2020  ref": href,.    
+0001d1d0: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
+0001d1e0: 6522 3a20 666e 2c0a 2020 2020 2020 2020  e": fn,.        
+0001d1f0: 2020 2020 2020 2020 2273 7a22 3a20 737a          "sz": sz
+0001d200: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001d210: 2020 2265 7874 223a 2065 7874 2c0a 2020    "ext": ext,.  
+0001d220: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+0001d230: 7422 3a20 6474 2c0a 2020 2020 2020 2020  t": dt,.        
+0001d240: 2020 2020 2020 2020 2274 7322 3a20 696e          "ts": in
+0001d250: 7428 6c69 6e66 2e73 745f 6d74 696d 6529  t(linf.st_mtime)
+0001d260: 2c0a 2020 2020 2020 2020 2020 2020 7d0a  ,.            }.
+0001d270: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0001d280: 735f 6469 723a 0a20 2020 2020 2020 2020  s_dir:.         
+0001d290: 2020 2020 2020 2064 6972 732e 6170 7065         dirs.appe
+0001d2a0: 6e64 2869 7465 6d29 0a20 2020 2020 2020  nd(item).       
+0001d2b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001d2c0: 2020 2020 2020 2020 2020 2066 696c 6573             files
+0001d2d0: 2e61 7070 656e 6428 6974 656d 290a 2020  .append(item).  
+0001d2e0: 2020 2020 2020 2020 2020 2020 2020 6974                it
+0001d2f0: 656d 5b22 7264 225d 203d 2072 656d 0a0a  em["rd"] = rem..
+0001d300: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
+0001d310: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0001d320: 6f6b 6965 732e 6765 7428 2269 6478 6822  okies.get("idxh"
+0001d330: 2920 3d3d 2022 7922 0a20 2020 2020 2020  ) == "y".       
+0001d340: 2020 2020 2061 6e64 2022 6c73 2220 6e6f       and "ls" no
+0001d350: 7420 696e 2073 656c 662e 7570 6172 616d  t in self.uparam
+0001d360: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0001d370: 2022 7622 206e 6f74 2069 6e20 7365 6c66   "v" not in self
+0001d380: 2e75 7061 7261 6d0a 2020 2020 2020 2020  .uparam.        
+0001d390: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+0001d3a0: 6478 5f68 746d 6c20 3d20 7365 7428 5b22  dx_html = set(["
+0001d3b0: 696e 6465 782e 6874 6d22 2c20 2269 6e64  index.htm", "ind
+0001d3c0: 6578 2e68 746d 6c22 5d29 0a20 2020 2020  ex.html"]).     
+0001d3d0: 2020 2020 2020 2066 6f72 2069 7465 6d20         for item 
+0001d3e0: 696e 2066 696c 6573 3a0a 2020 2020 2020  in files:.      
+0001d3f0: 2020 2020 2020 2020 2020 6966 2069 7465            if ite
+0001d400: 6d5b 226e 616d 6522 5d20 696e 2069 6478  m["name"] in idx
+0001d410: 5f68 746d 6c3a 0a20 2020 2020 2020 2020  _html:.         
+0001d420: 2020 2020 2020 2020 2020 2023 2064 6f20             # do 
+0001d430: 6675 6c6c 2072 6573 6f6c 7665 2069 6e20  full resolve in 
+0001d440: 6361 7365 206f 6620 7368 6164 6f77 6564  case of shadowed
+0001d450: 2066 696c 650a 2020 2020 2020 2020 2020   file.          
+0001d460: 2020 2020 2020 2020 2020 7670 203d 2076            vp = v
+0001d470: 6a6f 696e 2873 656c 662e 7670 6174 682e  join(self.vpath.
+0001d480: 7370 6c69 7428 223f 2229 5b30 5d2c 2069  split("?")[0], i
+0001d490: 7465 6d5b 226e 616d 6522 5d29 0a20 2020  tem["name"]).   
+0001d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4b0: 2076 6e2c 2072 656d 203d 2073 656c 662e   vn, rem = self.
+0001d4c0: 6173 7276 2e76 6673 2e67 6574 2876 702c  asrv.vfs.get(vp,
+0001d4d0: 2073 656c 662e 756e 616d 652c 2054 7275   self.uname, Tru
+0001d4e0: 652c 2046 616c 7365 290a 2020 2020 2020  e, False).      
+0001d4f0: 2020 2020 2020 2020 2020 2020 2020 6170                ap
+0001d500: 203d 2076 6e2e 6361 6e6f 6e69 6361 6c28   = vn.canonical(
+0001d510: 7265 6d29 0a20 2020 2020 2020 2020 2020  rem).           
+0001d520: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001d530: 7365 6c66 2e74 785f 6669 6c65 2861 7029  self.tx_file(ap)
+0001d540: 2020 2320 6973 206e 6f2d 6361 6368 650a    # is no-cache.
+0001d550: 0a20 2020 2020 2020 2074 6167 7365 7420  .        tagset 
+0001d560: 203d 2073 6574 2829 0a20 2020 2020 2020   = set().       
+0001d570: 2066 6f72 2066 6520 696e 2066 696c 6573   for fe in files
+0001d580: 3a0a 2020 2020 2020 2020 2020 2020 666e  :.            fn
+0001d590: 203d 2066 655b 226e 616d 6522 5d0a 2020   = fe["name"].  
+0001d5a0: 2020 2020 2020 2020 2020 7264 203d 2066            rd = f
+0001d5b0: 655b 2272 6422 5d0a 2020 2020 2020 2020  e["rd"].        
+0001d5c0: 2020 2020 6465 6c20 6665 5b22 7264 225d      del fe["rd"]
+0001d5d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001d5e0: 6e6f 7420 6963 7572 3a0a 2020 2020 2020  not icur:.      
+0001d5f0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+0001d600: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
+0001d610: 6966 2076 6e20 213d 2064 6276 3a0a 2020  if vn != dbv:.  
+0001d620: 2020 2020 2020 2020 2020 2020 2020 5f2c                _,
+0001d630: 2072 6420 3d20 766e 2e67 6574 5f64 6276   rd = vn.get_dbv
+0001d640: 2872 6429 0a0a 2020 2020 2020 2020 2020  (rd)..          
+0001d650: 2020 7120 3d20 2273 656c 6563 7420 6d74    q = "select mt
+0001d660: 2e6b 2c20 6d74 2e76 2066 726f 6d20 7570  .k, mt.v from up
+0001d670: 2069 6e6e 6572 206a 6f69 6e20 6d74 206f   inner join mt o
+0001d680: 6e20 6d74 2e77 203d 2073 7562 7374 7228  n mt.w = substr(
+0001d690: 7570 2e77 2c31 2c31 3629 2077 6865 7265  up.w,1,16) where
+0001d6a0: 2075 702e 7264 203d 203f 2061 6e64 2075   up.rd = ? and u
+0001d6b0: 702e 666e 203d 203f 2061 6e64 202b 6d74  p.fn = ? and +mt
+0001d6c0: 2e6b 2021 3d20 2778 2722 0a20 2020 2020  .k != 'x'".     
+0001d6d0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0001d6e0: 2020 2020 2020 2020 2020 2020 7220 3d20              r = 
+0001d6f0: 6963 7572 2e65 7865 6375 7465 2871 2c20  icur.execute(q, 
+0001d700: 2872 642c 2066 6e29 290a 2020 2020 2020  (rd, fn)).      
+0001d710: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+0001d720: 6570 7469 6f6e 2061 7320 6578 3a0a 2020  eption as ex:.  
+0001d730: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001d740: 2022 6461 7461 6261 7365 2069 7320 6c6f   "database is lo
+0001d750: 636b 6564 2220 696e 2073 7472 2865 7829  cked" in str(ex)
+0001d760: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001d770: 2020 2020 2020 6272 6561 6b0a 0a20 2020        break..   
+0001d780: 2020 2020 2020 2020 2020 2020 2074 7279               try
+0001d790: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001d7a0: 2020 2020 2020 6172 6773 203d 2073 3365        args = s3e
+0001d7b0: 6e63 2869 6478 2e6d 656d 5f63 7572 2c20  nc(idx.mem_cur, 
+0001d7c0: 7264 2c20 666e 290a 2020 2020 2020 2020  rd, fn).        
+0001d7d0: 2020 2020 2020 2020 2020 2020 7220 3d20              r = 
+0001d7e0: 6963 7572 2e65 7865 6375 7465 2871 2c20  icur.execute(q, 
+0001d7f0: 6172 6773 290a 2020 2020 2020 2020 2020  args).          
+0001d800: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+0001d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d820: 2020 7420 3d20 2274 6167 2072 6561 6420    t = "tag read 
+0001d830: 6572 726f 722c 207b 7d2f 7b7d 5c6e 7b7d  error, {}/{}\n{}
+0001d840: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0001d850: 2020 2020 2020 7365 6c66 2e6c 6f67 2874        self.log(t
+0001d860: 2e66 6f72 6d61 7428 7264 2c20 666e 2c20  .format(rd, fn, 
+0001d870: 6d69 6e5f 6578 2829 2929 0a20 2020 2020  min_ex())).     
+0001d880: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0001d890: 7265 616b 0a0a 2020 2020 2020 2020 2020  reak..          
+0001d8a0: 2020 6665 5b22 7461 6773 225d 203d 207b    fe["tags"] = {
+0001d8b0: 6b3a 2076 2066 6f72 206b 2c20 7620 696e  k: v for k, v in
+0001d8c0: 2072 7d0a 2020 2020 2020 2020 2020 2020   r}.            
+0001d8d0: 5f20 3d20 5b74 6167 7365 742e 6164 6428  _ = [tagset.add(
+0001d8e0: 6b29 2066 6f72 206b 2069 6e20 6665 5b22  k) for k in fe["
+0001d8f0: 7461 6773 225d 5d0a 0a20 2020 2020 2020  tags"]]..       
+0001d900: 2069 6620 6963 7572 3a0a 2020 2020 2020   if icur:.      
+0001d910: 2020 2020 2020 7461 676c 6973 7420 3d20        taglist = 
+0001d920: 5b6b 2066 6f72 206b 2069 6e20 766e 2e66  [k for k in vn.f
+0001d930: 6c61 6773 2e67 6574 2822 6d74 6522 2c20  lags.get("mte", 
+0001d940: 2222 292e 7370 6c69 7428 222c 2229 2069  "").split(",") i
+0001d950: 6620 6b20 696e 2074 6167 7365 745d 0a20  f k in tagset]. 
+0001d960: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
+0001d970: 6520 696e 2064 6972 733a 0a20 2020 2020  e in dirs:.     
+0001d980: 2020 2020 2020 2020 2020 2066 655b 2274             fe["t
+0001d990: 6167 7322 5d20 3d20 7b7d 0a20 2020 2020  ags"] = {}.     
+0001d9a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001d9b0: 2020 2020 2074 6167 6c69 7374 203d 206c       taglist = l
+0001d9c0: 6973 7428 7461 6773 6574 290a 0a20 2020  ist(tagset)..   
+0001d9d0: 2020 2020 2069 6620 6973 5f6c 733a 0a20       if is_ls:. 
+0001d9e0: 2020 2020 2020 2020 2020 206c 735f 7265             ls_re
+0001d9f0: 745b 2264 6972 7322 5d20 3d20 6469 7273  t["dirs"] = dirs
+0001da00: 0a20 2020 2020 2020 2020 2020 206c 735f  .            ls_
+0001da10: 7265 745b 2266 696c 6573 225d 203d 2066  ret["files"] = f
+0001da20: 696c 6573 0a20 2020 2020 2020 2020 2020  iles.           
+0001da30: 206c 735f 7265 745b 2274 6167 6c69 7374   ls_ret["taglist
+0001da40: 225d 203d 2074 6167 6c69 7374 0a20 2020  "] = taglist.   
+0001da50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001da60: 7365 6c66 2e74 785f 6c73 286c 735f 7265  self.tx_ls(ls_re
+0001da70: 7429 0a0a 2020 2020 2020 2020 646f 6320  t)..        doc 
+0001da80: 3d20 7365 6c66 2e75 7061 7261 6d2e 6765  = self.uparam.ge
+0001da90: 7428 2264 6f63 2229 2069 6620 7365 6c66  t("doc") if self
+0001daa0: 2e63 616e 5f72 6561 6420 656c 7365 204e  .can_read else N
+0001dab0: 6f6e 650a 2020 2020 2020 2020 6966 2064  one.        if d
+0001dac0: 6f63 3a0a 2020 2020 2020 2020 2020 2020  oc:.            
+0001dad0: 646f 6320 3d20 756e 7175 6f74 6570 2864  doc = unquotep(d
+0001dae0: 6f63 2e72 6570 6c61 6365 2822 2b22 2c20  oc.replace("+", 
+0001daf0: 2220 2229 2e73 706c 6974 2822 3f22 295b  " ").split("?")[
+0001db00: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
+0001db10: 6a32 615b 2264 6f63 6e61 6d65 225d 203d  j2a["docname"] =
+0001db20: 2064 6f63 0a20 2020 2020 2020 2020 2020   doc.           
+0001db30: 2064 6f63 7478 7420 3d20 4e6f 6e65 0a20   doctxt = None. 
+0001db40: 2020 2020 2020 2020 2020 2069 6620 6e65             if ne
+0001db50: 7874 2828 7820 666f 7220 7820 696e 2066  xt((x for x in f
+0001db60: 696c 6573 2069 6620 785b 226e 616d 6522  iles if x["name"
+0001db70: 5d20 3d3d 2064 6f63 292c 204e 6f6e 6529  ] == doc), None)
+0001db80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001db90: 2020 646f 6370 6174 6820 3d20 6f73 2e70    docpath = os.p
+0001dba0: 6174 682e 6a6f 696e 2861 6273 7061 7468  ath.join(abspath
+0001dbb0: 2c20 646f 6329 0a20 2020 2020 2020 2020  , doc).         
+0001dbc0: 2020 2020 2020 2073 7a20 3d20 626f 732e         sz = bos.
+0001dbd0: 7061 7468 2e67 6574 7369 7a65 2864 6f63  path.getsize(doc
+0001dbe0: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
+0001dbf0: 2020 2020 2020 6966 2073 7a20 3c20 3130        if sz < 10
+0001dc00: 3234 202a 2073 656c 662e 6172 6773 2e74  24 * self.args.t
+0001dc10: 7874 5f6d 6178 3a0a 2020 2020 2020 2020  xt_max:.        
+0001dc20: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0001dc30: 206f 7065 6e28 6673 656e 6328 646f 6370   open(fsenc(docp
+0001dc40: 6174 6829 2c20 2272 6222 2920 6173 2066  ath), "rb") as f
+0001dc50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001dc60: 2020 2020 2020 2020 2020 646f 6374 7874            doctxt
+0001dc70: 203d 2066 2e72 6561 6428 292e 6465 636f   = f.read().deco
+0001dc80: 6465 2822 7574 662d 3822 2c20 2272 6570  de("utf-8", "rep
+0001dc90: 6c61 6365 2229 0a20 2020 2020 2020 2020  lace").         
+0001dca0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001dcb0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
+0001dcc0: 6728 2264 6f63 2034 3034 3a20 5b7b 7d5d  g("doc 404: [{}]
+0001dcd0: 222e 666f 726d 6174 2864 6f63 292c 2063  ".format(doc), c
+0001dce0: 3d36 290a 2020 2020 2020 2020 2020 2020  =6).            
+0001dcf0: 2020 2020 646f 6374 7874 203d 2022 2820      doctxt = "( 
+0001dd00: 7465 7874 6669 6c65 206e 6f74 2066 6f75  textfile not fou
+0001dd10: 6e64 2029 220a 0a20 2020 2020 2020 2020  nd )"..         
+0001dd20: 2020 2069 6620 646f 6374 7874 2069 7320     if doctxt is 
+0001dd30: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0001dd40: 2020 2020 2020 2020 2020 6a32 615b 2264            j2a["d
+0001dd50: 6f63 225d 203d 2064 6f63 7478 740a 0a20  oc"] = doctxt.. 
+0001dd60: 2020 2020 2020 2066 6f72 2064 2069 6e20         for d in 
+0001dd70: 6469 7273 3a0a 2020 2020 2020 2020 2020  dirs:.          
+0001dd80: 2020 645b 226e 616d 6522 5d20 2b3d 2022    d["name"] += "
+0001dd90: 2f22 0a0a 2020 2020 2020 2020 6469 7273  /"..        dirs
+0001dda0: 2e73 6f72 7428 6b65 793d 6974 656d 6765  .sort(key=itemge
+0001ddb0: 7474 6572 2822 6e61 6d65 2229 290a 0a20  tter("name")).. 
+0001ddc0: 2020 2020 2020 2069 6620 6973 5f6a 733a         if is_js:
+0001ddd0: 0a20 2020 2020 2020 2020 2020 206a 3261  .            j2a
+0001dde0: 5b22 6c73 3022 5d20 3d20 7b0a 2020 2020  ["ls0"] = {.    
+0001ddf0: 2020 2020 2020 2020 2020 2020 2264 6972              "dir
+0001de00: 7322 3a20 6469 7273 2c0a 2020 2020 2020  s": dirs,.      
+0001de10: 2020 2020 2020 2020 2020 2266 696c 6573            "files
+0001de20: 223a 2066 696c 6573 2c0a 2020 2020 2020  ": files,.      
+0001de30: 2020 2020 2020 2020 2020 2274 6167 6c69            "tagli
+0001de40: 7374 223a 2074 6167 6c69 7374 2c0a 2020  st": taglist,.  
+0001de50: 2020 2020 2020 2020 2020 2020 2020 2275                "u
+0001de60: 6e6c 6973 7422 3a20 756e 6c69 7374 2c0a  nlist": unlist,.
+0001de70: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+0001de80: 2020 2020 2020 2020 2020 6a32 615b 2266            j2a["f
+0001de90: 696c 6573 225d 203d 205b 5d0a 2020 2020  iles"] = [].    
+0001dea0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001deb0: 2020 2020 2020 6a32 615b 2266 696c 6573        j2a["files
+0001dec0: 225d 203d 2064 6972 7320 2b20 6669 6c65  "] = dirs + file
+0001ded0: 730a 0a20 2020 2020 2020 206a 3261 5b22  s..        j2a["
+0001dee0: 7461 676c 6973 7422 5d20 3d20 7461 676c  taglist"] = tagl
+0001def0: 6973 740a 2020 2020 2020 2020 6a32 615b  ist.        j2a[
+0001df00: 2274 7874 5f65 7874 225d 203d 2073 656c  "txt_ext"] = sel
+0001df10: 662e 6172 6773 2e74 6578 7466 696c 6573  f.args.textfiles
+0001df20: 2e72 6570 6c61 6365 2822 2c22 2c20 2220  .replace(",", " 
+0001df30: 2229 0a0a 2020 2020 2020 2020 6966 2022  ")..        if "
+0001df40: 6d74 6822 2069 6e20 766e 2e66 6c61 6773  mth" in vn.flags
+0001df50: 3a0a 2020 2020 2020 2020 2020 2020 6a32  :.            j2
+0001df60: 615b 2264 6566 5f68 636f 6c73 225d 203d  a["def_hcols"] =
+0001df70: 2076 6e2e 666c 6167 735b 226d 7468 225d   vn.flags["mth"]
+0001df80: 2e73 706c 6974 2822 2c22 290a 0a20 2020  .split(",")..   
+0001df90: 2020 2020 2068 746d 6c20 3d20 7365 6c66       html = self
+0001dfa0: 2e6a 3273 2874 706c 2c20 2a2a 6a32 6129  .j2s(tpl, **j2a)
+0001dfb0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+0001dfc0: 706c 7928 6874 6d6c 2e65 6e63 6f64 6528  ply(html.encode(
+0001dfd0: 2275 7466 2d38 222c 2022 7265 706c 6163  "utf-8", "replac
+0001dfe0: 6522 2929 0a20 2020 2020 2020 2072 6574  e")).        ret
+0001dff0: 7572 6e20 5472 7565 0a                   urn True.
```

### Comparing `copyparty-1.7.2/copyparty/httpconn.py` & `copyparty-1.7.3/copyparty/httpconn.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,14 @@
 import argparse  # typechk
 import os
 import re
 import socket
 import threading  # typechk
 import time
 
-try:
-    HAVE_SSL = True
-    import ssl
-except:
-    HAVE_SSL = False
-
 from . import util as Util
 from .__init__ import TYPE_CHECKING, EnvParams
 from .authsrv import AuthSrv  # typechk
 from .httpcli import HttpCli
 from .ico import Ico
 from .mtag import HAVE_FFMPEG
 from .th_cli import ThumbCli
@@ -47,15 +41,14 @@
         self.addr = addr
         self.hsrv = hsrv
 
         self.mutex  = hsrv.mutex  # mypy404
         self.args  = hsrv.args  # mypy404
         self.E  = self.args.E
         self.asrv  = hsrv.asrv  # mypy404
-        self.cert_path = hsrv.cert_path
         self.u2fh  = hsrv.u2fh  # mypy404
         self.iphash  = hsrv.broker.iphash
         self.bans   = hsrv.bans
         self.aclose   = hsrv.aclose
 
         enth = (HAVE_PIL or HAVE_VIPS or HAVE_FFMPEG) and not self.args.no_thumb
         self.thumbcli  = ThumbCli(hsrv) if enth else None  # mypy404
@@ -107,15 +100,15 @@
         if not self.u2idx:
             self.u2idx = self.hsrv.get_u2idx(str(self.addr))
 
         return self.u2idx
 
     def _detect_https(self)  :
         method = None
-        if self.cert_path:
+        if True:
             try:
                 method = self.s.recv(4, socket.MSG_PEEK)
             except socket.timeout:
                 return False
             except AttributeError:
                 # jython does not support msg_peek; forget about https
                 method = self.s.recv(4)
@@ -141,29 +134,29 @@
 
     def run(self)  :
         self.s.settimeout(10)
 
         self.sr = None
         if self.args.https_only:
             is_https = True
-        elif self.args.http_only or not HAVE_SSL:
+        elif self.args.http_only:
             is_https = False
         else:
             # raise Exception("asdf")
             is_https = self._detect_https()
 
         if is_https:
             if self.sr:
                 self.log("TODO: cannot do https in jython", c="1;31")
                 return
 
             self.log_src = self.log_src.replace("[36m", "[35m")
             try:
                 ctx = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
-                ctx.load_cert_chain(self.cert_path)
+                ctx.load_cert_chain(self.args.cert)
                 if self.args.ssl_ver:
                     ctx.options &= ~self.args.ssl_flags_en
                     ctx.options |= self.args.ssl_flags_de
                     # print(repr(ctx.options))
 
                 if self.args.ssl_log:
                     try:
```

### Comparing `copyparty-1.7.2/copyparty/httpsrv.py` & `copyparty-1.7.3/copyparty/httpsrv.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,31 @@
   you do not have jinja2 installed,\033[33m
   choose one of these:\033[0m
    * apt install python-jinja2
    * {} -m pip install --user jinja2
    * (try another python version, if you have one)
    * (try copyparty.sfx instead)
 """.format(
-            os.path.basename(sys.executable)
+            sys.executable
+        )
+    )
+    sys.exit(1)
+except SyntaxError:
+    if EXE:
+        raise
+
+    print(
+        """\033[1;31m
+  your jinja2 version is incompatible with your python version;\033[33m
+  please try to replace it with an older version:\033[0m
+   * {} -m pip install --user jinja2==2.11.3
+   * (try another python version, if you have one)
+   * (try copyparty.sfx instead)
+""".format(
+            sys.executable
         )
     )
     sys.exit(1)
 
 from .bos import bos
 from .httpconn import HttpConn
 from .u2idx import U2idx
@@ -124,20 +140,14 @@
             self.mallow += zs.split()
 
         if self.args.zs:
             from .ssdp import SSDPr
 
             self.ssdp = SSDPr(broker)
 
-        cert_path = self.args.cert
-        if bos.path.exists(cert_path):
-            self.cert_path = cert_path
-        else:
-            self.cert_path = ""
-
         if self.tp_q:
             self.start_threads(4)
 
         if nid:
             if self.args.stackmon:
                 start_stackmon(self.args.stackmon, nid)
```

### Comparing `copyparty-1.7.2/copyparty/ico.py` & `copyparty-1.7.3/copyparty/ico.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/mdns.py` & `copyparty-1.7.3/copyparty/mdns.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # coding: utf-8
 from __future__ import print_function, unicode_literals
 
+import errno
 import random
 import select
 import socket
 import time
 
 from ipaddress import IPv4Network, IPv6Network
 
@@ -269,14 +270,26 @@
             return
 
         self.build_replies()
         Daemon(self.send_probes)
         zf = time.time() + 2
         self.probing = zf  # cant unicast so give everyone an extra sec
         self.unsolicited = [zf, zf + 1, zf + 3, zf + 7]  # rfc-8.3
+
+        try:
+            self.run2()
+        except OSError as ex:
+            if ex.errno != errno.EBADF:
+                raise
+
+            self.log("stopping due to {}".format(ex), "90")
+
+        self.log("stopped", 2)
+
+    def run2(self)  :
         last_hop = time.time()
         ihop = self.args.mc_hop
         while self.running:
             timeout = (
                 0.02 + random.random() * 0.07
                 if self.probing or self.q or self.defend or self.unsolicited
                 else (last_hop + ihop if ihop else 180)
@@ -306,16 +319,14 @@
                 continue
 
             if self.probing < time.time():
                 t = "probe ok; announcing [{}]"
                 self.log(t.format(self.hn[:-1]), 2)
                 self.probing = 0
 
-        self.log("stopped", 2)
-
     def stop(self, panic=False)  :
         self.running = False
         for srv in self.srv.values():
             try:
                 if panic:
                     srv.sck.close()
                 else:
```

### Comparing `copyparty-1.7.2/copyparty/mtag.py` & `copyparty-1.7.3/copyparty/mtag.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/multicast.py` & `copyparty-1.7.3/copyparty/multicast.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/res/COPYING.txt` & `copyparty-1.7.3/copyparty/res/COPYING.txt`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/res/insecure.pem` & `copyparty-1.7.3/copyparty/res/insecure.pem`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/smbd.py` & `copyparty-1.7.3/copyparty/smbd.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/ssdp.py` & `copyparty-1.7.3/copyparty/ssdp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # coding: utf-8
 from __future__ import print_function, unicode_literals
 
+import errno
 import re
 import select
 import socket
 from email.utils import formatdate
 
 from .__init__ import TYPE_CHECKING
 from .multicast import MC_Sck, MCast
@@ -121,14 +122,25 @@
             hp = hp or next((x[1] for x in tcps if x[0] == "::"), 0)
             if not hp:
                 hp = tcps[0][1]
                 self.log("assuming port {} for {}".format(hp, srv.ip), 3)
             srv.hport = hp
 
         self.log("listening")
+        try:
+            self.run2()
+        except OSError as ex:
+            if ex.errno != errno.EBADF:
+                raise
+
+            self.log("stopping due to {}".format(ex), "90")
+
+        self.log("stopped", 2)
+
+    def run2(self)  :
         while self.running:
             rdy = select.select(self.srv, [], [], self.args.z_chk or 180)
             rx  = rdy[0]  # type: ignore
             self.rxc.cln()
             buf = b""
             addr = ("0", 0)
             for sck in rx:
@@ -140,16 +152,14 @@
                         break
 
                     t = "{} {} \033[33m|{}| {}\n{}".format(
                         self.srv[sck].name, addr, len(buf), repr(buf)[2:-1], min_ex()
                     )
                     self.log(t, 6)
 
-        self.log("stopped", 2)
-
     def stop(self)  :
         self.running = False
         for srv in self.srv.values():
             try:
                 srv.sck.close()
             except:
                 pass
```

### Comparing `copyparty-1.7.2/copyparty/star.py` & `copyparty-1.7.3/copyparty/star.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/stolen/dnslib/bimap.py` & `copyparty-1.7.3/copyparty/stolen/dnslib/bimap.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/stolen/dnslib/buffer.py` & `copyparty-1.7.3/copyparty/stolen/dnslib/buffer.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/stolen/dnslib/dns.py` & `copyparty-1.7.3/copyparty/stolen/dnslib/dns.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/stolen/dnslib/label.py` & `copyparty-1.7.3/copyparty/stolen/dnslib/label.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/stolen/dnslib/lex.py` & `copyparty-1.7.3/copyparty/stolen/dnslib/lex.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/stolen/dnslib/ranges.py` & `copyparty-1.7.3/copyparty/stolen/dnslib/ranges.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/stolen/ifaddr/_posix.py` & `copyparty-1.7.3/copyparty/stolen/ifaddr/_posix.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/stolen/ifaddr/_shared.py` & `copyparty-1.7.3/copyparty/stolen/ifaddr/_shared.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/stolen/ifaddr/_win32.py` & `copyparty-1.7.3/copyparty/stolen/ifaddr/_win32.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/stolen/qrcodegen.py` & `copyparty-1.7.3/copyparty/stolen/qrcodegen.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/stolen/surrogateescape.py` & `copyparty-1.7.3/copyparty/stolen/surrogateescape.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/sutil.py` & `copyparty-1.7.3/copyparty/sutil.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/svchub.py` & `copyparty-1.7.3/copyparty/svchub.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import time
 from datetime import datetime, timedelta
 
 # from inspect import currentframe
 # print(currentframe().f_lineno)
 
 
-from .__init__ import ANYWIN, EXE, MACOS, TYPE_CHECKING, VT100, EnvParams, unicode
+from .__init__ import ANYWIN, EXE, MACOS, TYPE_CHECKING, EnvParams, unicode
 from .authsrv import AuthSrv
 from .mtag import HAVE_FFMPEG, HAVE_FFPROBE
 from .tcpsrv import TcpSrv
 from .th_srv import HAVE_PIL, HAVE_VIPS, HAVE_WEBP, ThumbSrv
 from .up2k import Up2k
 from .util import (
     FFMPEG_URL,
@@ -70,14 +70,15 @@
         argv ,
         printed ,
     )  :
         self.args = args
         self.dargs = dargs
         self.argv = argv
         self.E  = args.E
+        self.no_ansi = args.no_ansi
         self.logf  = None
         self.logf_base_fn = ""
         self.stop_req = False
         self.stopping = False
         self.stopped = False
         self.reload_req = False
         self.reloading = False
@@ -671,19 +672,23 @@
 
     def _log_enabled(self, src , msg , c   = 0)  :
         """handles logging from all components"""
         with self.log_mutex:
             now = time.time()
             if now >= self.next_day:
                 dt = datetime.utcfromtimestamp(now)
-                print("\033[36m{}\033[0m\n".format(dt.strftime("%Y-%m-%d")), end="")
+                zs = "{}\n" if self.no_ansi else "\033[36m{}\033[0m\n"
+                zs = zs.format(dt.strftime("%Y-%m-%d"))
+                print(zs, end="")
                 self._set_next_day()
+                if self.logf:
+                    self.logf.write(zs)
 
             fmt = "\033[36m%s \033[33m%-21s \033[0m%s\n"
-            if not VT100:
+            if self.no_ansi:
                 fmt = "%s %-21s %s\n"
                 if "\033" in msg:
                     msg = ansi_re.sub("", msg)
                 if "\033" in src:
                     src = ansi_re.sub("", src)
             elif c:
                 if isinstance(c, int):
```

### Comparing `copyparty-1.7.2/copyparty/szip.py` & `copyparty-1.7.3/copyparty/szip.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/tcpsrv.py` & `copyparty-1.7.3/copyparty/tcpsrv.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 import os
 import re
 import socket
 import sys
 import time
 
-from .__init__ import ANYWIN, PY2, TYPE_CHECKING, VT100, unicode
+from .__init__ import ANYWIN, PY2, TYPE_CHECKING, unicode
 from .stolen.qrcodegen import QrCode
+from .cert import gencert
 from .util import (
     E_ACCESS,
     E_ADDR_IN_USE,
     E_ADDR_NOT_AVAIL,
     E_UNREACH,
     Netdev,
     min_ex,
@@ -288,14 +289,15 @@
         self.bound = bound
         self.nsrv = len(srvs)
         self._distribute_netdevs()
 
     def _distribute_netdevs(self):
         self.hub.broker.say("set_netdevs", self.netdevs)
         self.hub.start_zeroconf()
+        gencert(self.log, self.args, self.netdevs)
 
     def shutdown(self)  :
         self.stopping = True
         try:
             for srv in self.srv:
                 srv.close()
         except:
@@ -494,15 +496,15 @@
                 tw, th = termsize()
                 tsz = min(tw // 2, th)
                 zoom = 1 if qrc.size + pad * 2 >= tsz else 2
             except:
                 zoom = 1
 
         qr = qrc.render(zoom, pad)
-        if not VT100:
+        if self.args.no_ansi:
             return "{}\n{}".format(txt, qr)
 
         halfc = "\033[40;48;5;{0}m{1}\033[47;48;5;{2}m"
         if not fg:
             halfc = "\033[0;40m{1}\033[0;47m"
 
         def ansify(m )  :
```

### Comparing `copyparty-1.7.2/copyparty/th_cli.py` & `copyparty-1.7.3/copyparty/th_cli.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/th_srv.py` & `copyparty-1.7.3/copyparty/th_srv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/u2idx.py` & `copyparty-1.7.3/copyparty/u2idx.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/up2k.py` & `copyparty-1.7.3/copyparty/up2k.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/util.py` & `copyparty-1.7.3/copyparty/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1999,14 +1999,16 @@
                 # on windows in particular, drain rx until client shuts
                 if not sck.recv(32 * 1024):
                     break
 
             sck.shutdown(socket.SHUT_RDWR)
         except:
             pass
+    except Exception as ex:
+        log("shut({}): {}".format(fd, ex), "90")
     finally:
         td = time.time() - t0
         if td >= 1:
             log("shut({}) in {:.3f} sec".format(fd, td), "90")
 
         sck.close()
```

### Comparing `copyparty-1.7.2/copyparty/web/a/partyfuse.py` & `copyparty-1.7.3/copyparty/web/a/partyfuse.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/a/u2c.py` & `copyparty-1.7.3/copyparty/web/a/u2c.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/a/webdav-cfg.bat` & `copyparty-1.7.3/copyparty/web/a/webdav-cfg.bat`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/baguettebox.js.gz` & `copyparty-1.7.3/copyparty/web/baguettebox.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/browser.html` & `copyparty-1.7.3/copyparty/web/browser.html`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,15 @@
 	<div id="widget"></div>
 
 	<script>
 		var SR = {{ r|tojson }},
 			TS = "{{ ts }}",
 			acct = "{{ acct }}",
 			perms = {{ perms }},
+			dgrid = {{ dgrid|tojson }},
 			themes = {{ themes }},
 			dtheme = "{{ dtheme }}",
 			srvinf = "{{ srv_info }}",
 			lang = "{{ lang }}",
 			dfavico = "{{ favico }}",
 			def_hcols = {{ def_hcols|tojson }},
 			have_up2k_idx = {{ have_up2k_idx|tojson }},
```

### Comparing `copyparty-1.7.2/copyparty/web/browser.js.gz` & `copyparty-1.7.3/copyparty/web/browser.js.gz`

 * *Files 26% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browser.js", last modified: Thu May 11 07:59:05 2023, max compression, from Unix
+gzip compressed data, was "browser.js", last modified: Fri Jun  2 21:41:19 2023, max compression, from Unix
```

#### browser.js

##### js-beautify {}

```diff
@@ -4569,15 +4569,15 @@
                 sethash('g' + r.bbox[i].imageElement.getAttribute('ref'));
             }
         })[0];
     };
 
     bcfg_bind(r, 'thumbs', 'thumbs', true, r.setdirty);
     bcfg_bind(r, 'sel', 'gridsel', false, r.loadsel);
-    bcfg_bind(r, 'en', 'griden', false, function(v) {
+    bcfg_bind(r, 'en', 'griden', dgrid, function(v) {
         v ? loadgrid() : r.setvis(true);
         pbar.onresize();
         vbar.onresize();
     });
     ebi('wtgrid').onclick = ebi('griden').onclick;
 
     return r;
@@ -5764,14 +5764,20 @@
         var nodes = res.dirs.concat(res.files),
             html = mk_files_header(res.taglist),
             sel = r.lsc === res ? msel.getsel() : [],
             plain = [],
             seen = {};
 
         r.lsc = res;
+        if (res.unlist) {
+            var ptn = new RegExp(res.unlist);
+            for (var a = nodes.length - 1; a >= 0; a--)
+                if (ptn.exec(nodes[a].href.split('?')[0]))
+                    nodes.splice(a, 1);
+        }
         nodes = sortfiles(nodes);
         window.removeEventListener('scroll', r.tscroll);
         r.trunc = nodes.length > r.nvis && location.hash.length < 2;
         if (r.trunc) {
             for (var a = r.lim; a < nodes.length; a++) {
                 var tn = nodes[a],
                     tns = Object.keys(tn.tags || {});
```

### Comparing `copyparty-1.7.2/copyparty/web/browser2.html` & `copyparty-1.7.3/copyparty/web/browser2.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/cf.html` & `copyparty-1.7.3/copyparty/web/cf.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/dbg-audio.js.gz` & `copyparty-1.7.3/copyparty/web/dbg-audio.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/deps/easymde.css.gz` & `copyparty-1.7.3/copyparty/web/deps/easymde.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/deps/easymde.js.gz` & `copyparty-1.7.3/copyparty/web/deps/easymde.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/deps/marked.js.gz` & `copyparty-1.7.3/copyparty/web/deps/marked.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/deps/mini-fa.css.gz` & `copyparty-1.7.3/copyparty/web/deps/mini-fa.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/deps/mini-fa.woff` & `copyparty-1.7.3/copyparty/web/deps/mini-fa.woff`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/deps/prism.css.gz` & `copyparty-1.7.3/copyparty/web/deps/prism.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/deps/prism.js.gz` & `copyparty-1.7.3/copyparty/web/deps/prism.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/deps/prismd.css.gz` & `copyparty-1.7.3/copyparty/web/deps/prismd.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/deps/scp.woff2` & `copyparty-1.7.3/copyparty/web/deps/scp.woff2`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/deps/sha512.ac.js.gz` & `copyparty-1.7.3/copyparty/web/deps/sha512.ac.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/deps/sha512.hw.js.gz` & `copyparty-1.7.3/copyparty/web/deps/sha512.hw.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/md.css.gz` & `copyparty-1.7.3/copyparty/web/md.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/md.html` & `copyparty-1.7.3/copyparty/web/md.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/md.js.gz` & `copyparty-1.7.3/copyparty/web/md.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/md2.css.gz` & `copyparty-1.7.3/copyparty/web/md2.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/md2.js.gz` & `copyparty-1.7.3/copyparty/web/md2.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/mde.css.gz` & `copyparty-1.7.3/copyparty/web/mde.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/mde.html` & `copyparty-1.7.3/copyparty/web/mde.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/mde.js.gz` & `copyparty-1.7.3/copyparty/web/mde.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/msg.html` & `copyparty-1.7.3/copyparty/web/msg.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/splash.css.gz` & `copyparty-1.7.3/copyparty/web/splash.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/splash.html` & `copyparty-1.7.3/copyparty/web/splash.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/splash.js.gz` & `copyparty-1.7.3/copyparty/web/splash.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/svcs.html` & `copyparty-1.7.3/copyparty/web/svcs.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/svcs.js.gz` & `copyparty-1.7.3/copyparty/web/svcs.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/ui.css.gz` & `copyparty-1.7.3/copyparty/web/ui.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/up2k.js.gz` & `copyparty-1.7.3/copyparty/web/up2k.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty/web/w.hash.js.gz` & `copyparty-1.7.3/copyparty/web/w.hash.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.2/copyparty.egg-info/PKG-INFO` & `copyparty-1.7.3/copyparty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyparty
-Version: 1.7.2
+Version: 1.7.3
 Summary:   Portable file server with accelerated resumable uploads, deduplication, WebDAV, FTP, zeroconf, media indexer, video thumbnails, audio transcoding, and write-only folders
 Author-email: ed <copyparty@ocv.me>
 License: MIT
 Project-URL: Source Code, https://github.com/9001/copyparty
 Project-URL: Bug Tracker, https://github.com/9001/copyparty/issues
 Project-URL: Demo Server, https://a.ocv.me/pub/demo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -509,24 +509,26 @@
 * `[↵]` toggles wordwrap
 * `[👀]` show full name on hover (if wordwrap is off)
 
 
 ## thumbnails
 
 press `g` or `田` to toggle grid-view instead of the file listing  and `t` toggles icons / thumbnails
+* can be made default globally with `--grid` or per-volume with volflag `grid`
 
 ![copyparty-thumbs-fs8](https://user-images.githubusercontent.com/241032/129636211-abd20fa2-a953-4366-9423-1c88ebb96ba9.png)
 
 it does static images with Pillow / pyvips / FFmpeg, and uses FFmpeg for video files, so you may want to `--no-thumb` or maybe just `--no-vthumb` depending on how dangerous your users are
 * pyvips is 3x faster than Pillow, Pillow is 3x faster than FFmpeg
 * disable thumbnails for specific volumes with volflag `dthumb` for all, or `dvthumb` / `dathumb` / `dithumb` for video/audio/images only
 
 audio files are covnerted into spectrograms using FFmpeg unless you `--no-athumb` (and some FFmpeg builds may need `--th-ff-swr`)
 
 images with the following names (see `--th-covers`) become the thumbnail of the folder they're in: `folder.png`, `folder.jpg`, `cover.png`, `cover.jpg`
+* and, if you enable [file indexing](#file-indexing), all remaining folders will also get thumbnails (as long as they contain any pics at all)
 
 in the grid/thumbnail view, if the audio player panel is open, songs will start playing when clicked
 * indicated by the audio files having the ▶ icon instead of 💾
 
 
 ## zip downloads
 
@@ -967,22 +969,21 @@
 * `-e2tsr` also deletes all existing tags, doing a full reindex
 * `-e2v` verfies file integrity at startup, comparing hashes from the db
 * `-e2vu` patches the database with the new hashes from the filesystem
 * `-e2vp` panics and kills copyparty instead
 * `--xlink` enables deduplication across volumes
 
 the same arguments can be set as volflags, in addition to `d2d`, `d2ds`, `d2t`, `d2ts`, `d2v` for disabling:
-* `-v ~/music::r:c,e2dsa,e2tsr` does a full reindex of everything on startup
+* `-v ~/music::r:c,e2ds,e2tsr` does a full reindex of everything on startup
 * `-v ~/music::r:c,d2d` disables **all** indexing, even if any `-e2*` are on
 * `-v ~/music::r:c,d2t` disables all `-e2t*` (tags), does not affect `-e2d*`
 * `-v ~/music::r:c,d2ds` disables on-boot scans; only index new uploads
 * `-v ~/music::r:c,d2ts` same except only affecting tags
 
 note:
-* the parser can finally handle `c,e2dsa,e2tsr` so you no longer have to `c,e2dsa:c,e2tsr`
 * `e2tsr` is probably always overkill, since `e2ds`/`e2dsa` would pick up any file modifications and `e2ts` would then reindex those, unless there is a new copyparty version with new parsers and the release note says otherwise
 * the rescan button in the admin panel has no effect unless the volume has `-e2ds` or higher
 * deduplication is possible on windows if you run copyparty as administrator (not saying you should!)
 
 ### exclude-patterns
 
 to save some time,  you can provide a regex pattern for filepaths to only index by filename/path/size/last-modified (and not the hash of the file contents) by setting `--no-hash \.iso$` or the volflag `:c,nohash=\.iso$`, this has the following consequences:
@@ -1609,14 +1610,19 @@
 
 ## https
 
 both HTTP and HTTPS are accepted  by default, but letting a [reverse proxy](#reverse-proxy) handle the https/tls/ssl would be better (probably more secure by default)
 
 copyparty doesn't speak HTTP/2 or QUIC, so using a reverse proxy would solve that as well
 
+if [cfssl](https://github.com/cloudflare/cfssl/releases/latest) is installed, copyparty will automatically create a CA and server-cert on startup
+* the certs are written to `--crt-dir` for distribution, see `--help` for the other `--crt` options
+* this will be a self-signed certificate so you must install your `ca.pem` into all your browsers/devices
+* if you want to avoid the hassle of distributing certs manually, please consider using a reverse proxy
+
 
 # recovering from crashes
 
 ## client crashes
 
 ### frefox wsod
```

### Comparing `copyparty-1.7.2/copyparty.egg-info/SOURCES.txt` & `copyparty-1.7.3/copyparty.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 copyparty/__main__.py
 copyparty/__version__.py
 copyparty/authsrv.py
 copyparty/broker_mp.py
 copyparty/broker_mpw.py
 copyparty/broker_thr.py
 copyparty/broker_util.py
+copyparty/cert.py
 copyparty/cfg.py
 copyparty/dxml.py
 copyparty/fsutil.py
 copyparty/ftpd.py
 copyparty/httpcli.py
 copyparty/httpconn.py
 copyparty/httpsrv.py
```

### Comparing `copyparty-1.7.2/pyproject.toml` & `copyparty-1.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,14 @@
 [tool.black]
 required-version = '21.12b0'
 target-version = ['py27']
 
 [tool.isort]
 profile = "black"
 include_trailing_comma = true
-force_sort_within_sections = true
 
 [tool.bandit]
 skips = ["B104", "B110", "B112"]
 
 # =====================================================================
 
 [tool.pylint.MAIN]
```

