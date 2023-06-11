# Comparing `tmp/copyparty-1.7.5.tar.gz` & `tmp/copyparty-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copyparty-1.7.5.tar", last modified: Sun Jun 11 02:06:52 2023, max compression
+gzip compressed data, was "copyparty-1.7.6.tar", last modified: Sun Jun 11 09:02:00 2023, max compression
```

## Comparing `copyparty-1.7.5.tar` & `copyparty-1.7.6.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:52.794853 copyparty-1.7.5/
--rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-11 12:44:53.000000 copyparty-1.7.5/LICENSE
--rw-r--r--   0 ed        (1000) ed        (1000)    96291 2023-06-11 02:06:52.794853 copyparty-1.7.5/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)    94341 2023-06-10 22:25:29.000000 copyparty-1.7.5/README.md
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:52.781853 copyparty-1.7.5/copyparty/
--rw-r--r--   0 ed        (1000) ed        (1000)     1812 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/__init__.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    70588 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/__main__.py
--rw-r--r--   0 ed        (1000) ed        (1000)      249 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/__version__.py
--rw-r--r--   0 ed        (1000) ed        (1000)    65881 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/authsrv.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:52.782853 copyparty-1.7.5/copyparty/bos/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/bos/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1560 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/bos/bos.py
--rw-r--r--   0 ed        (1000) ed        (1000)      777 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/bos/path.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3590 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/broker_mp.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3200 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/broker_mpw.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1759 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/broker_thr.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1489 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/broker_util.py
--rw-r--r--   0 ed        (1000) ed        (1000)     7036 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/cert.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6843 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/cfg.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1548 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/dxml.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3932 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/fsutil.py
--rw-r--r--   0 ed        (1000) ed        (1000)    15317 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/ftpd.py
--rw-r--r--   0 ed        (1000) ed        (1000)   122873 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/httpcli.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6825 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/httpconn.py
--rw-r--r--   0 ed        (1000) ed        (1000)    15372 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/httpsrv.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2643 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/ico.py
--rw-r--r--   0 ed        (1000) ed        (1000)    17205 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/mdns.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16844 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/mtag.py
--rw-r--r--   0 ed        (1000) ed        (1000)    11520 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/multicast.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:52.783853 copyparty-1.7.5/copyparty/res/
--rw-r--r--   0 ed        (1000) ed        (1000)    10570 2023-06-11 02:06:37.000000 copyparty-1.7.5/copyparty/res/COPYING.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/res/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2876 2023-04-23 21:16:05.000000 copyparty-1.7.5/copyparty/res/insecure.pem
--rw-r--r--   0 ed        (1000) ed        (1000)    10623 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/smbd.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6379 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/ssdp.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2699 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/star.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:52.783853 copyparty-1.7.5/copyparty/stolen/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/__init__.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:52.784853 copyparty-1.7.5/copyparty/stolen/dnslib/
--rw-r--r--   0 ed        (1000) ed        (1000)      159 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/dnslib/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1182 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/dnslib/bimap.py
--rw-r--r--   0 ed        (1000) ed        (1000)      348 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/dnslib/bit.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1407 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/dnslib/buffer.py
--rw-r--r--   0 ed        (1000) ed        (1000)    20956 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/dnslib/dns.py
--rw-r--r--   0 ed        (1000) ed        (1000)     4893 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/dnslib/label.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2615 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/dnslib/lex.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1810 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/dnslib/ranges.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:52.784853 copyparty-1.7.5/copyparty/stolen/ifaddr/
--rw-r--r--   0 ed        (1000) ed        (1000)      463 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/ifaddr/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2626 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/ifaddr/_posix.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6111 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/ifaddr/_shared.py
--rw-r--r--   0 ed        (1000) ed        (1000)     4026 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/ifaddr/_win32.py
--rw-r--r--   0 ed        (1000) ed        (1000)    21469 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/qrcodegen.py
--rw-r--r--   0 ed        (1000) ed        (1000)     5573 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/stolen/surrogateescape.py
--rw-r--r--   0 ed        (1000) ed        (1000)      972 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/sutil.py
--rw-r--r--   0 ed        (1000) ed        (1000)    23803 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/svchub.py
--rw-r--r--   0 ed        (1000) ed        (1000)     8166 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/szip.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16721 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/tcpsrv.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3826 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/th_cli.py
--rw-r--r--   0 ed        (1000) ed        (1000)    22379 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/th_srv.py
--rw-r--r--   0 ed        (1000) ed        (1000)    10585 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/u2idx.py
--rw-r--r--   0 ed        (1000) ed        (1000)   121996 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/up2k.py
--rw-r--r--   0 ed        (1000) ed        (1000)    72070 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/util.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:52.789853 copyparty-1.7.5/copyparty/web/
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:52.790853 copyparty-1.7.5/copyparty/web/a/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/web/a/__init__.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    32276 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/web/a/partyfuse.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    36247 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/web/a/u2c.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1449 2023-02-20 20:21:49.000000 copyparty-1.7.5/copyparty/web/a/webdav-cfg.bat
--rw-r--r--   0 ed        (1000) ed        (1000)     7296 2023-03-30 21:17:33.000000 copyparty-1.7.5/copyparty/web/baguettebox.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    10963 2023-06-02 22:21:36.000000 copyparty-1.7.5/copyparty/web/browser.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     5317 2023-06-02 21:39:24.000000 copyparty-1.7.5/copyparty/web/browser.html
--rw-r--r--   0 ed        (1000) ed        (1000)    59183 2023-06-02 21:41:19.000000 copyparty-1.7.5/copyparty/web/browser.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1604 2022-12-10 19:54:48.000000 copyparty-1.7.5/copyparty/web/browser2.html
--rw-r--r--   0 ed        (1000) ed        (1000)      585 2022-07-03 13:28:49.000000 copyparty-1.7.5/copyparty/web/cf.html
--rw-r--r--   0 ed        (1000) ed        (1000)      688 2022-07-14 21:26:48.000000 copyparty-1.7.5/copyparty/web/dbg-audio.js.gz
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:52.791853 copyparty-1.7.5/copyparty/web/dd/
--rw-r--r--   0 ed        (1000) ed        (1000)      258 2021-09-11 12:44:53.000000 copyparty-1.7.5/copyparty/web/dd/2.png
--rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.7.5/copyparty/web/dd/3.png
--rw-r--r--   0 ed        (1000) ed        (1000)      248 2021-09-11 12:44:53.000000 copyparty-1.7.5/copyparty/web/dd/4.png
--rw-r--r--   0 ed        (1000) ed        (1000)      250 2021-09-11 12:44:53.000000 copyparty-1.7.5/copyparty/web/dd/5.png
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/web/dd/__init__.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:52.793853 copyparty-1.7.5/copyparty/web/deps/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:38.000000 copyparty-1.7.5/copyparty/web/deps/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3053 2023-02-20 10:55:39.000000 copyparty-1.7.5/copyparty/web/deps/easymde.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    76953 2023-04-01 14:48:07.000000 copyparty-1.7.5/copyparty/web/deps/easymde.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    14819 2023-04-01 14:47:51.000000 copyparty-1.7.5/copyparty/web/deps/marked.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      584 2023-04-01 14:48:09.000000 copyparty-1.7.5/copyparty/web/deps/mini-fa.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2784 2023-04-01 14:48:09.000000 copyparty-1.7.5/copyparty/web/deps/mini-fa.woff
--rw-r--r--   0 ed        (1000) ed        (1000)     1478 2022-12-29 03:41:18.000000 copyparty-1.7.5/copyparty/web/deps/prism.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    41428 2022-12-29 03:41:18.000000 copyparty-1.7.5/copyparty/web/deps/prism.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1647 2022-12-29 03:41:18.000000 copyparty-1.7.5/copyparty/web/deps/prismd.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8612 2023-04-01 14:48:10.000000 copyparty-1.7.5/copyparty/web/deps/scp.woff2
--rw-r--r--   0 ed        (1000) ed        (1000)     7043 2023-04-01 14:23:12.000000 copyparty-1.7.5/copyparty/web/deps/sha512.ac.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8119 2021-07-22 23:48:12.000000 copyparty-1.7.5/copyparty/web/deps/sha512.hw.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2011 2022-10-30 15:38:07.000000 copyparty-1.7.5/copyparty/web/md.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     4063 2022-12-10 20:27:29.000000 copyparty-1.7.5/copyparty/web/md.html
--rw-r--r--   0 ed        (1000) ed        (1000)     4121 2023-03-26 01:52:00.000000 copyparty-1.7.5/copyparty/web/md.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      681 2022-12-01 22:41:28.000000 copyparty-1.7.5/copyparty/web/md2.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8213 2023-01-25 20:58:01.000000 copyparty-1.7.5/copyparty/web/md2.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      929 2022-04-15 15:07:16.000000 copyparty-1.7.5/copyparty/web/mde.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1640 2022-12-10 20:27:33.000000 copyparty-1.7.5/copyparty/web/mde.html
--rw-r--r--   0 ed        (1000) ed        (1000)     2219 2022-12-01 07:23:41.000000 copyparty-1.7.5/copyparty/web/mde.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.7.5/copyparty/web/msg.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      898 2022-12-10 19:57:40.000000 copyparty-1.7.5/copyparty/web/msg.html
--rw-r--r--   0 ed        (1000) ed        (1000)      927 2023-02-17 22:46:57.000000 copyparty-1.7.5/copyparty/web/splash.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     3741 2023-02-19 19:41:20.000000 copyparty-1.7.5/copyparty/web/splash.html
--rw-r--r--   0 ed        (1000) ed        (1000)     1235 2023-02-17 22:28:18.000000 copyparty-1.7.5/copyparty/web/splash.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    10610 2023-05-07 15:13:28.000000 copyparty-1.7.5/copyparty/web/svcs.html
--rw-r--r--   0 ed        (1000) ed        (1000)      520 2022-12-04 17:10:33.000000 copyparty-1.7.5/copyparty/web/svcs.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2419 2023-03-26 02:06:03.000000 copyparty-1.7.5/copyparty/web/ui.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    21544 2023-05-12 23:46:23.000000 copyparty-1.7.5/copyparty/web/up2k.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    13063 2023-06-10 23:48:10.000000 copyparty-1.7.5/copyparty/web/util.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1060 2023-03-02 22:42:45.000000 copyparty-1.7.5/copyparty/web/w.hash.js.gz
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 02:06:52.782853 copyparty-1.7.5/copyparty.egg-info/
--rw-r--r--   0 ed        (1000) ed        (1000)    96291 2023-06-11 02:06:52.000000 copyparty-1.7.5/copyparty.egg-info/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)     2808 2023-06-11 02:06:52.000000 copyparty-1.7.5/copyparty.egg-info/SOURCES.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        1 2023-06-11 02:06:52.000000 copyparty-1.7.5/copyparty.egg-info/dependency_links.txt
--rw-r--r--   0 ed        (1000) ed        (1000)      128 2023-06-11 02:06:52.000000 copyparty-1.7.5/copyparty.egg-info/entry_points.txt
--rw-r--r--   0 ed        (1000) ed        (1000)      117 2023-06-11 02:06:52.000000 copyparty-1.7.5/copyparty.egg-info/requires.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       10 2023-06-11 02:06:52.000000 copyparty-1.7.5/copyparty.egg-info/top_level.txt
--rw-r--r--   0 ed        (1000) ed        (1000)     4007 2023-06-02 21:51:58.000000 copyparty-1.7.5/pyproject.toml
--rw-r--r--   0 ed        (1000) ed        (1000)       38 2023-06-11 02:06:52.794853 copyparty-1.7.5/setup.cfg
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 09:02:00.493966 copyparty-1.7.6/
+-rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-11 12:44:53.000000 copyparty-1.7.6/LICENSE
+-rw-r--r--   0 ed        (1000) ed        (1000)    96291 2023-06-11 09:02:00.493966 copyparty-1.7.6/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)    94341 2023-06-10 22:25:29.000000 copyparty-1.7.6/README.md
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 09:02:00.481966 copyparty-1.7.6/copyparty/
+-rw-r--r--   0 ed        (1000) ed        (1000)     1812 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/__init__.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    70588 2023-06-11 09:01:46.000000 copyparty-1.7.6/copyparty/__main__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      249 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/__version__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    65881 2023-06-11 09:01:46.000000 copyparty-1.7.6/copyparty/authsrv.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 09:02:00.482966 copyparty-1.7.6/copyparty/bos/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/bos/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1560 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/bos/bos.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      777 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/bos/path.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3590 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/broker_mp.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3200 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/broker_mpw.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1759 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/broker_thr.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1489 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/broker_util.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     7035 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/cert.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6843 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/cfg.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1548 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/dxml.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3932 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/fsutil.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    15317 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/ftpd.py
+-rw-r--r--   0 ed        (1000) ed        (1000)   122873 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/httpcli.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6825 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/httpconn.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    15372 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/httpsrv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2643 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/ico.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    17205 2023-06-11 09:01:46.000000 copyparty-1.7.6/copyparty/mdns.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    16844 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/mtag.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    11520 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/multicast.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 09:02:00.483966 copyparty-1.7.6/copyparty/res/
+-rw-r--r--   0 ed        (1000) ed        (1000)    10570 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/res/COPYING.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/res/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2876 2023-04-23 21:16:05.000000 copyparty-1.7.6/copyparty/res/insecure.pem
+-rw-r--r--   0 ed        (1000) ed        (1000)    10623 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/smbd.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6379 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/ssdp.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2699 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/star.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 09:02:00.483966 copyparty-1.7.6/copyparty/stolen/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/__init__.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 09:02:00.484966 copyparty-1.7.6/copyparty/stolen/dnslib/
+-rw-r--r--   0 ed        (1000) ed        (1000)      159 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/dnslib/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1182 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/dnslib/bimap.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      348 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/dnslib/bit.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1407 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/dnslib/buffer.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    20956 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/dnslib/dns.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     4893 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/dnslib/label.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2615 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/dnslib/lex.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1810 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/dnslib/ranges.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 09:02:00.485966 copyparty-1.7.6/copyparty/stolen/ifaddr/
+-rw-r--r--   0 ed        (1000) ed        (1000)      463 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/ifaddr/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2626 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/ifaddr/_posix.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6111 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/ifaddr/_shared.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     4026 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/ifaddr/_win32.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    21469 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/qrcodegen.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     5573 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/stolen/surrogateescape.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      972 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/sutil.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    24336 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/svchub.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     8166 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/szip.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    16753 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/tcpsrv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3826 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/th_cli.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    22379 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/th_srv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    10585 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/u2idx.py
+-rw-r--r--   0 ed        (1000) ed        (1000)   121996 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/up2k.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    72070 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/util.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 09:02:00.488966 copyparty-1.7.6/copyparty/web/
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 09:02:00.489966 copyparty-1.7.6/copyparty/web/a/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/web/a/__init__.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    32276 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/web/a/partyfuse.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    36247 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/web/a/u2c.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1449 2023-02-20 20:21:49.000000 copyparty-1.7.6/copyparty/web/a/webdav-cfg.bat
+-rw-r--r--   0 ed        (1000) ed        (1000)     7296 2023-03-30 21:17:33.000000 copyparty-1.7.6/copyparty/web/baguettebox.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    10963 2023-06-02 22:21:36.000000 copyparty-1.7.6/copyparty/web/browser.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     5317 2023-06-02 21:39:24.000000 copyparty-1.7.6/copyparty/web/browser.html
+-rw-r--r--   0 ed        (1000) ed        (1000)    59183 2023-06-02 21:41:19.000000 copyparty-1.7.6/copyparty/web/browser.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1604 2022-12-10 19:54:48.000000 copyparty-1.7.6/copyparty/web/browser2.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      585 2022-07-03 13:28:49.000000 copyparty-1.7.6/copyparty/web/cf.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      688 2022-07-14 21:26:48.000000 copyparty-1.7.6/copyparty/web/dbg-audio.js.gz
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 09:02:00.490966 copyparty-1.7.6/copyparty/web/dd/
+-rw-r--r--   0 ed        (1000) ed        (1000)      258 2021-09-11 12:44:53.000000 copyparty-1.7.6/copyparty/web/dd/2.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.7.6/copyparty/web/dd/3.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      248 2021-09-11 12:44:53.000000 copyparty-1.7.6/copyparty/web/dd/4.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      250 2021-09-11 12:44:53.000000 copyparty-1.7.6/copyparty/web/dd/5.png
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/web/dd/__init__.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 09:02:00.492966 copyparty-1.7.6/copyparty/web/deps/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-06-11 09:01:45.000000 copyparty-1.7.6/copyparty/web/deps/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3053 2023-02-20 10:55:39.000000 copyparty-1.7.6/copyparty/web/deps/easymde.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    76953 2023-04-01 14:48:07.000000 copyparty-1.7.6/copyparty/web/deps/easymde.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    14819 2023-04-01 14:47:51.000000 copyparty-1.7.6/copyparty/web/deps/marked.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      584 2023-04-01 14:48:09.000000 copyparty-1.7.6/copyparty/web/deps/mini-fa.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2784 2023-04-01 14:48:09.000000 copyparty-1.7.6/copyparty/web/deps/mini-fa.woff
+-rw-r--r--   0 ed        (1000) ed        (1000)     1478 2022-12-29 03:41:18.000000 copyparty-1.7.6/copyparty/web/deps/prism.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    41428 2022-12-29 03:41:18.000000 copyparty-1.7.6/copyparty/web/deps/prism.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1647 2022-12-29 03:41:18.000000 copyparty-1.7.6/copyparty/web/deps/prismd.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8612 2023-04-01 14:48:10.000000 copyparty-1.7.6/copyparty/web/deps/scp.woff2
+-rw-r--r--   0 ed        (1000) ed        (1000)     7043 2023-04-01 14:23:12.000000 copyparty-1.7.6/copyparty/web/deps/sha512.ac.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8119 2021-07-22 23:48:12.000000 copyparty-1.7.6/copyparty/web/deps/sha512.hw.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2011 2022-10-30 15:38:07.000000 copyparty-1.7.6/copyparty/web/md.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     4063 2022-12-10 20:27:29.000000 copyparty-1.7.6/copyparty/web/md.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     4121 2023-03-26 01:52:00.000000 copyparty-1.7.6/copyparty/web/md.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      681 2022-12-01 22:41:28.000000 copyparty-1.7.6/copyparty/web/md2.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8213 2023-01-25 20:58:01.000000 copyparty-1.7.6/copyparty/web/md2.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      929 2022-04-15 15:07:16.000000 copyparty-1.7.6/copyparty/web/mde.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1640 2022-12-10 20:27:33.000000 copyparty-1.7.6/copyparty/web/mde.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     2219 2022-12-01 07:23:41.000000 copyparty-1.7.6/copyparty/web/mde.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.7.6/copyparty/web/msg.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      898 2022-12-10 19:57:40.000000 copyparty-1.7.6/copyparty/web/msg.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      927 2023-02-17 22:46:57.000000 copyparty-1.7.6/copyparty/web/splash.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     3741 2023-02-19 19:41:20.000000 copyparty-1.7.6/copyparty/web/splash.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     1235 2023-02-17 22:28:18.000000 copyparty-1.7.6/copyparty/web/splash.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    10610 2023-05-07 15:13:28.000000 copyparty-1.7.6/copyparty/web/svcs.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      520 2022-12-04 17:10:33.000000 copyparty-1.7.6/copyparty/web/svcs.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2419 2023-03-26 02:06:03.000000 copyparty-1.7.6/copyparty/web/ui.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    21544 2023-05-12 23:46:23.000000 copyparty-1.7.6/copyparty/web/up2k.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    13063 2023-06-10 23:48:10.000000 copyparty-1.7.6/copyparty/web/util.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1060 2023-03-02 22:42:45.000000 copyparty-1.7.6/copyparty/web/w.hash.js.gz
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-06-11 09:02:00.482966 copyparty-1.7.6/copyparty.egg-info/
+-rw-r--r--   0 ed        (1000) ed        (1000)    96291 2023-06-11 09:02:00.000000 copyparty-1.7.6/copyparty.egg-info/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)     2808 2023-06-11 09:02:00.000000 copyparty-1.7.6/copyparty.egg-info/SOURCES.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        1 2023-06-11 09:02:00.000000 copyparty-1.7.6/copyparty.egg-info/dependency_links.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)      128 2023-06-11 09:02:00.000000 copyparty-1.7.6/copyparty.egg-info/entry_points.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)      117 2023-06-11 09:02:00.000000 copyparty-1.7.6/copyparty.egg-info/requires.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)       10 2023-06-11 09:02:00.000000 copyparty-1.7.6/copyparty.egg-info/top_level.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)     4007 2023-06-02 21:51:58.000000 copyparty-1.7.6/pyproject.toml
+-rw-r--r--   0 ed        (1000) ed        (1000)       38 2023-06-11 09:02:00.493966 copyparty-1.7.6/setup.cfg
```

### Comparing `copyparty-1.7.5/LICENSE` & `copyparty-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/PKG-INFO` & `copyparty-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyparty
-Version: 1.7.5
+Version: 1.7.6
 Summary:   Portable file server with accelerated resumable uploads, deduplication, WebDAV, FTP, zeroconf, media indexer, video thumbnails, audio transcoding, and write-only folders
 Author-email: ed <copyparty@ocv.me>
 License: MIT
 Project-URL: Source Code, https://github.com/9001/copyparty
 Project-URL: Bug Tracker, https://github.com/9001/copyparty/issues
 Project-URL: Demo Server, https://a.ocv.me/pub/demo/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `copyparty-1.7.5/README.md` & `copyparty-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/__init__.py` & `copyparty-1.7.6/copyparty/__init__.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/__main__.py` & `copyparty-1.7.6/copyparty/__main__.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/authsrv.py` & `copyparty-1.7.6/copyparty/authsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/bos/bos.py` & `copyparty-1.7.6/copyparty/bos/bos.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/bos/path.py` & `copyparty-1.7.6/copyparty/bos/path.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/broker_mp.py` & `copyparty-1.7.6/copyparty/broker_mp.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/broker_mpw.py` & `copyparty-1.7.6/copyparty/broker_mpw.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/broker_thr.py` & `copyparty-1.7.6/copyparty/broker_thr.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/broker_util.py` & `copyparty-1.7.6/copyparty/broker_util.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/cert.py` & `copyparty-1.7.6/copyparty/cert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import os
+import calendar
 import errno
-import time
+import filecmp
 import json
+import os
 import shutil
-import filecmp
-import calendar
-
-from .util import runcmd, Netdev
+import time
 
+from .util import Netdev, runcmd
 
 HAVE_CFSSL = True
 
 
 def ensure_cert(log , args)  :
     """
     the default cert (and the entire TLS support) is only here to enable the
```

### Comparing `copyparty-1.7.5/copyparty/cfg.py` & `copyparty-1.7.6/copyparty/cfg.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/dxml.py` & `copyparty-1.7.6/copyparty/dxml.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/fsutil.py` & `copyparty-1.7.6/copyparty/fsutil.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/ftpd.py` & `copyparty-1.7.6/copyparty/ftpd.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/httpcli.py` & `copyparty-1.7.6/copyparty/httpcli.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/httpconn.py` & `copyparty-1.7.6/copyparty/httpconn.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/httpsrv.py` & `copyparty-1.7.6/copyparty/httpsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/ico.py` & `copyparty-1.7.6/copyparty/ico.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/mdns.py` & `copyparty-1.7.6/copyparty/mdns.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/mtag.py` & `copyparty-1.7.6/copyparty/mtag.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/multicast.py` & `copyparty-1.7.6/copyparty/multicast.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/res/COPYING.txt` & `copyparty-1.7.6/copyparty/res/COPYING.txt`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/res/insecure.pem` & `copyparty-1.7.6/copyparty/res/insecure.pem`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/smbd.py` & `copyparty-1.7.6/copyparty/smbd.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/ssdp.py` & `copyparty-1.7.6/copyparty/ssdp.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/star.py` & `copyparty-1.7.6/copyparty/star.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/stolen/dnslib/bimap.py` & `copyparty-1.7.6/copyparty/stolen/dnslib/bimap.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/stolen/dnslib/buffer.py` & `copyparty-1.7.6/copyparty/stolen/dnslib/buffer.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/stolen/dnslib/dns.py` & `copyparty-1.7.6/copyparty/stolen/dnslib/dns.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/stolen/dnslib/label.py` & `copyparty-1.7.6/copyparty/stolen/dnslib/label.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/stolen/dnslib/lex.py` & `copyparty-1.7.6/copyparty/stolen/dnslib/lex.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/stolen/dnslib/ranges.py` & `copyparty-1.7.6/copyparty/stolen/dnslib/ranges.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/stolen/ifaddr/_posix.py` & `copyparty-1.7.6/copyparty/stolen/ifaddr/_posix.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/stolen/ifaddr/_shared.py` & `copyparty-1.7.6/copyparty/stolen/ifaddr/_shared.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/stolen/ifaddr/_win32.py` & `copyparty-1.7.6/copyparty/stolen/ifaddr/_win32.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/stolen/qrcodegen.py` & `copyparty-1.7.6/copyparty/stolen/qrcodegen.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/stolen/surrogateescape.py` & `copyparty-1.7.6/copyparty/stolen/surrogateescape.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/sutil.py` & `copyparty-1.7.6/copyparty/sutil.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/svchub.py` & `copyparty-1.7.6/copyparty/svchub.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 # from inspect import currentframe
 # print(currentframe().f_lineno)
 
 
 from .__init__ import ANYWIN, EXE, MACOS, TYPE_CHECKING, EnvParams, unicode
 from .authsrv import AuthSrv
+from .cert import ensure_cert
 from .mtag import HAVE_FFMPEG, HAVE_FFPROBE
 from .tcpsrv import TcpSrv
 from .th_srv import HAVE_PIL, HAVE_VIPS, HAVE_WEBP, ThumbSrv
 from .up2k import Up2k
 from .util import (
     FFMPEG_URL,
     VERSIONS,
@@ -229,15 +230,16 @@
             zms += "d"
         if not args.http_only:
             zms += "D"
 
         if args.ftp or args.ftps:
             from .ftpd import Ftpd
 
-            self.ftpd = Ftpd(self)
+            self.ftpd  = None
+            Daemon(self.start_ftpd, "start_ftpd")
             zms += "f" if args.ftp else "F"
 
         if args.smb:
             # impacket.dcerpc is noisy about listen timeouts
             sto = socket.getdefaulttimeout()
             socket.setdefaulttimeout(None)
 
@@ -259,14 +261,36 @@
         if self.check_mp_enable():
             from .broker_mp import BrokerMp as Broker
         else:
             from .broker_thr import BrokerThr as Broker  # type: ignore
 
         self.broker = Broker(self)
 
+    def start_ftpd(self)  :
+        time.sleep(30)
+        if self.ftpd:
+            return
+
+        self.restart_ftpd()
+
+    def restart_ftpd(self)  :
+        if not hasattr(self, "ftpd"):
+            return
+
+        from .ftpd import Ftpd
+
+        if self.ftpd:
+            return  # todo
+
+        if not os.path.exists(self.args.cert):
+            ensure_cert(self.log, self.args)
+
+        self.ftpd = Ftpd(self)
+        self.log("root", "started FTPd")
+
     def thr_httpsrv_up(self)  :
         time.sleep(1 if self.args.ign_ebind_all else 5)
         expected = self.broker.num_workers * self.tcpsrv.nsrv
         failed = expected - self.httpsrv_up
         if not failed:
             return
```

### Comparing `copyparty-1.7.5/copyparty/szip.py` & `copyparty-1.7.6/copyparty/szip.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/tcpsrv.py` & `copyparty-1.7.6/copyparty/tcpsrv.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import os
 import re
 import socket
 import sys
 import time
 
 from .__init__ import ANYWIN, PY2, TYPE_CHECKING, unicode
-from .stolen.qrcodegen import QrCode
 from .cert import gencert
+from .stolen.qrcodegen import QrCode
 from .util import (
     E_ACCESS,
     E_ADDR_IN_USE,
     E_ADDR_NOT_AVAIL,
     E_UNREACH,
     Netdev,
     min_ex,
@@ -290,14 +290,15 @@
         self.nsrv = len(srvs)
         self._distribute_netdevs()
 
     def _distribute_netdevs(self):
         self.hub.broker.say("set_netdevs", self.netdevs)
         self.hub.start_zeroconf()
         gencert(self.log, self.args, self.netdevs)
+        self.hub.restart_ftpd()
 
     def shutdown(self)  :
         self.stopping = True
         try:
             for srv in self.srv:
                 srv.close()
         except:
```

### Comparing `copyparty-1.7.5/copyparty/th_cli.py` & `copyparty-1.7.6/copyparty/th_cli.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/th_srv.py` & `copyparty-1.7.6/copyparty/th_srv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/u2idx.py` & `copyparty-1.7.6/copyparty/u2idx.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/up2k.py` & `copyparty-1.7.6/copyparty/up2k.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/util.py` & `copyparty-1.7.6/copyparty/util.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/a/partyfuse.py` & `copyparty-1.7.6/copyparty/web/a/partyfuse.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/a/u2c.py` & `copyparty-1.7.6/copyparty/web/a/u2c.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/a/webdav-cfg.bat` & `copyparty-1.7.6/copyparty/web/a/webdav-cfg.bat`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/baguettebox.js.gz` & `copyparty-1.7.6/copyparty/web/baguettebox.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/browser.css.gz` & `copyparty-1.7.6/copyparty/web/browser.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/browser.html` & `copyparty-1.7.6/copyparty/web/browser.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/browser.js.gz` & `copyparty-1.7.6/copyparty/web/browser.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/browser2.html` & `copyparty-1.7.6/copyparty/web/browser2.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/cf.html` & `copyparty-1.7.6/copyparty/web/cf.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/dbg-audio.js.gz` & `copyparty-1.7.6/copyparty/web/dbg-audio.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/deps/easymde.css.gz` & `copyparty-1.7.6/copyparty/web/deps/easymde.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/deps/easymde.js.gz` & `copyparty-1.7.6/copyparty/web/deps/easymde.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/deps/marked.js.gz` & `copyparty-1.7.6/copyparty/web/deps/marked.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/deps/mini-fa.css.gz` & `copyparty-1.7.6/copyparty/web/deps/mini-fa.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/deps/mini-fa.woff` & `copyparty-1.7.6/copyparty/web/deps/mini-fa.woff`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/deps/prism.css.gz` & `copyparty-1.7.6/copyparty/web/deps/prism.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/deps/prism.js.gz` & `copyparty-1.7.6/copyparty/web/deps/prism.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/deps/prismd.css.gz` & `copyparty-1.7.6/copyparty/web/deps/prismd.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/deps/scp.woff2` & `copyparty-1.7.6/copyparty/web/deps/scp.woff2`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/deps/sha512.ac.js.gz` & `copyparty-1.7.6/copyparty/web/deps/sha512.ac.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/deps/sha512.hw.js.gz` & `copyparty-1.7.6/copyparty/web/deps/sha512.hw.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/md.css.gz` & `copyparty-1.7.6/copyparty/web/md.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/md.html` & `copyparty-1.7.6/copyparty/web/md.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/md.js.gz` & `copyparty-1.7.6/copyparty/web/md.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/md2.css.gz` & `copyparty-1.7.6/copyparty/web/md2.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/md2.js.gz` & `copyparty-1.7.6/copyparty/web/md2.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/mde.css.gz` & `copyparty-1.7.6/copyparty/web/mde.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/mde.html` & `copyparty-1.7.6/copyparty/web/mde.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/mde.js.gz` & `copyparty-1.7.6/copyparty/web/mde.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/msg.html` & `copyparty-1.7.6/copyparty/web/msg.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/splash.css.gz` & `copyparty-1.7.6/copyparty/web/splash.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/splash.html` & `copyparty-1.7.6/copyparty/web/splash.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/splash.js.gz` & `copyparty-1.7.6/copyparty/web/splash.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/svcs.html` & `copyparty-1.7.6/copyparty/web/svcs.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/svcs.js.gz` & `copyparty-1.7.6/copyparty/web/svcs.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/ui.css.gz` & `copyparty-1.7.6/copyparty/web/ui.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/up2k.js.gz` & `copyparty-1.7.6/copyparty/web/up2k.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/util.js.gz` & `copyparty-1.7.6/copyparty/web/util.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty/web/w.hash.js.gz` & `copyparty-1.7.6/copyparty/web/w.hash.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/copyparty.egg-info/PKG-INFO` & `copyparty-1.7.6/copyparty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyparty
-Version: 1.7.5
+Version: 1.7.6
 Summary:   Portable file server with accelerated resumable uploads, deduplication, WebDAV, FTP, zeroconf, media indexer, video thumbnails, audio transcoding, and write-only folders
 Author-email: ed <copyparty@ocv.me>
 License: MIT
 Project-URL: Source Code, https://github.com/9001/copyparty
 Project-URL: Bug Tracker, https://github.com/9001/copyparty/issues
 Project-URL: Demo Server, https://a.ocv.me/pub/demo/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `copyparty-1.7.5/copyparty.egg-info/SOURCES.txt` & `copyparty-1.7.6/copyparty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copyparty-1.7.5/pyproject.toml` & `copyparty-1.7.6/pyproject.toml`

 * *Files identical despite different names*

