# Comparing `tmp/py-Ayiin-0.4.5.dev1.tar.gz` & `tmp/py-Ayiin-0.4.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.4.5.dev1.tar", last modified: Fri Jun  9 15:18:59 2023, max compression
+gzip compressed data, was "py-Ayiin-0.4.6.dev1.tar", last modified: Sun Jun 11 02:28:46 2023, max compression
```

## Comparing `py-Ayiin-0.4.5.dev1.tar` & `py-Ayiin-0.4.6.dev1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:59.695193 py-Ayiin-0.4.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 15:18:59.695193 py-Ayiin-0.4.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:59.691192 py-Ayiin-0.4.5.dev1/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:59.691192 py-Ayiin-0.4.5.dev1/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38778 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:59.691192 py-Ayiin-0.4.5.dev1/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33549 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:59.691192 py-Ayiin-0.4.5.dev1/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/methods/_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:59.691192 py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:59.695193 py-Ayiin-0.4.5.dev1/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/resources/Logo Ayiin.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/resources/Youtube.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/resources/ayiin_music.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/resources/ayiin_ubot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/resources/ayiin_userbot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/resources/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/resources/default.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/resources/font.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/resources/font2.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:59.695193 py-Ayiin-0.4.5.dev1/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:59.695193 py-Ayiin-0.4.5.dev1/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:18:59.695193 py-Ayiin-0.4.5.dev1/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 15:18:59.000000 py-Ayiin-0.4.5.dev1/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-09 15:18:59.000000 py-Ayiin-0.4.5.dev1/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:18:59.000000 py-Ayiin-0.4.5.dev1/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-09 15:18:59.000000 py-Ayiin-0.4.5.dev1/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 15:18:59.000000 py-Ayiin-0.4.5.dev1/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 15:18:59.695193 py-Ayiin-0.4.5.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-09 15:18:47.000000 py-Ayiin-0.4.5.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:28:46.862806 py-Ayiin-0.4.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-11 02:28:46.862806 py-Ayiin-0.4.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:28:46.838806 py-Ayiin-0.4.6.dev1/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:28:46.838806 py-Ayiin-0.4.6.dev1/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38778 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:28:46.846806 py-Ayiin-0.4.6.dev1/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33773 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:28:46.850806 py-Ayiin-0.4.6.dev1/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/methods/_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:28:46.854806 py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:28:46.858806 py-Ayiin-0.4.6.dev1/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/resources/Logo Ayiin.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/resources/Youtube.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/resources/ayiin_music.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/resources/ayiin_ubot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/resources/ayiin_userbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/resources/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/resources/default.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/resources/font.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/resources/font2.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:28:46.858806 py-Ayiin-0.4.6.dev1/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:28:46.858806 py-Ayiin-0.4.6.dev1/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:28:46.862806 py-Ayiin-0.4.6.dev1/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-11 02:28:46.000000 py-Ayiin-0.4.6.dev1/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-11 02:28:46.000000 py-Ayiin-0.4.6.dev1/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 02:28:46.000000 py-Ayiin-0.4.6.dev1/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-11 02:28:46.000000 py-Ayiin-0.4.6.dev1/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 02:28:46.000000 py-Ayiin-0.4.6.dev1/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 02:28:46.862806 py-Ayiin-0.4.6.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-11 02:28:38.000000 py-Ayiin-0.4.6.dev1/setup.py
```

### Comparing `py-Ayiin-0.4.5.dev1/LICENSE` & `py-Ayiin-0.4.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/NOTICE` & `py-Ayiin-0.4.6.dev1/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/PKG-INFO` & `py-Ayiin-0.4.6.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.5.dev1
+Version: 0.4.6.dev1
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.5.dev1/README.md` & `py-Ayiin-0.4.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/Clients/client.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/Clients/client.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/Clients/pytgcalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/Clients/startup.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/__init__.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,25 +48,31 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.4.5.dev01"
+__version__ = "0.4.6.dev01"
 ayiin_ver = "0.1.1"
 prem_version = "0.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
 ]
 
+BLACKLIST_CHAT = [
+    -1001797285258,  # AyiinChatsNew
+    -1001675396283,  # AyiinXdSupport
+    -1001473548283,  # SharingUserbot
+]
+
 GCAST_BLACKLIST = [
     -1001797285258,  # AyiinChatsNew
     -1001675396283,  # AyiinXdSupport
     -1001473548283,  # SharingUserbot
     -1001433238829,  # TedeSupport
     -1001476936696,  # AnosSupport
     -1001327032795,  # UltroidSupport
```

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/__main__.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/assistant.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/assistant.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     InlineKeyboardMarkup,
     InlineQueryResultArticle,
     InputTextMessageContent
 )
 
 from fipper.handlers import CallbackQueryHandler, InlineQueryHandler
 
+from pyAyiin.dB.langs import get_lang, get_string
+
 from .config import Var as Variable
 from .decorator import is_admin_or_owner
 from .Clients import *
 
 
 Var = Variable()
 
@@ -48,14 +50,15 @@
     ]
 ]
 
 
 
 def inline(
     pattern: str = None,
+    langs: bool = False,
     group: int = 0,
     client_only: bool = False,
 ):
     """- Main Decorator To Register Commands. -"""
     filterm = (
         filters.regex(pattern=pattern)
     )
@@ -78,15 +81,20 @@
                 await iq.answer(
                     results,
                     switch_pm_text=f"🤖: Assistant of {OWNER}",
                     switch_pm_parameter="start",
                 )
                 return
             try:
-                await func(tgbot, iq)
+                if langs:
+                    lang = await get_lang(iq.from_user.id)
+                    _ = get_string(lang)
+                    await func(tgbot, iq, _)
+                else:
+                    await func(tgbot, iq)
             except BaseException:
                 logging.error(
                     f"Exception - {func.__module__} - {func.__name__}"
                 )
                 TZZ = pytz.timezone(Var.TZ)
                 datetime_tz = datetime.now(TZZ)
                 text = "<b>!ERROR - REPORT!</b>\n\n"
@@ -113,14 +121,15 @@
         tgbot.add_handler(InlineQueryHandler(func_, filters=filter_s), group=group)
 
 
 def callback(
     pattern: str = None,
     group: int = 0,
     from_users: list = [],
+    langs: bool = False,
     client_only: bool = False,
     users: bool = False,
     admins: bool = False,
 ):
     """- Main Decorator To Register Commands. -"""
     filterm = (
         filters.regex(pattern=pattern)
@@ -145,15 +154,20 @@
                 cq.message, from_users
             ):
                 return await cq.answer(
                     "Lu Bukan Admin Di Gc Ini Tod...",
                     show_alert=True,
                 )
             try:
-                await func(tgbot, cq)
+                if langs:
+                    lang = await get_lang(cq.from_user.id)
+                    _ = get_string(lang)
+                    await func(tgbot, cq, _)
+                else:
+                    await func(tgbot, cq)
             except MessageNotModified:
                     pass
             except MessageIdInvalid:
                 logging.warning(
                     "Please Don't Delete Commands While it's Processing..."
                 )
             except UserNotParticipant:
```

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/config.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/__init__.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/absen.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/admins.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/auth.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/gban.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/langs.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/langs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import yaml
 
 from os import listdir
+from typing import Any, Dict, List, Union
 
 from ._core import mongodb
 
 
 langdb = mongodb.langs
 
 langm = {}
@@ -27,14 +28,25 @@
 async def set_lang(user_id: int, lang: str):
     langm[user_id] = lang
     await langdb.update_one(
         {"user_id": user_id}, {"$set": {"lang": lang}}, upsert=True
     )
 
 
+def get_languages() -> Dict[str, Union[str, List[str]]]:
+    return {
+        code: {
+            "nama": languages[code]["nama"],
+            "asli": languages[code]["asli"],
+            "penulis": languages[code]["penulis"],
+        }
+        for code in languages
+    }
+
+
 def get_string(lang: str):
     return languages[lang]
 
 
 async def import_lang(file_path):
     for filename in listdir(file_path):
         if filename.endswith(".yml"):
```

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/logdb.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/premium.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/start.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/sudo.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/variable.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/dB/welcome.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/decorator.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,21 +63,21 @@
         )
 
     def decorator(func):
         async def wrapper(client, message):
             message.client = client
             chat_type = message.chat.type
             if admin_only and not await is_admin_or_owner(
-                message, (client.me).id
+                message, client.me.id
             ):
                 await eor(
                     message, "<code>Perintah Ini Hanya Bisa Digunakan Jika Anda Admin Di Group Ini!</code>"
                 )
                 return
-            if group_only and chat_type != (ChatType.GROUP, ChatType.SUPERGROUP):
+            if group_only and chat_type not in [ChatType.GROUP, ChatType.SUPERGROUP]:
                 await eor(message, "<code>Apakah Ini Grup Tod?</code>")
                 return
             if channel_only and chat_type != ChatType.CHANNEL:
                 await eor(message, "Perintah Ini Hanya Bisa Digunakan Di Channel!")
                 return
             if pm_only and chat_type != ChatType.PRIVATE:
                 await eor(message, "<code>Perintah Ini Hanya Bisa Digunakan Di PM!</code>")
@@ -127,20 +127,25 @@
                         logging.error(text)
         add_handler(filterm, wrapper, cmd)
         return wrapper
 
     return decorator
 
 
-def listen(filter_s):
+def listen(filter_s, langs: bool = False,):
     """Simple Decorator To Handel Custom Filters"""
     def decorator(func):
         async def wrapper(client, message):
             try:
-                await func(client, message)
+                if langs:
+                    lang = await get_lang(client.me.id)
+                    _ = get_string(lang)
+                    await func(client, message, _)
+                else:
+                    await func(client, message)
             except StopPropagation:
                 raise StopPropagation
             except ContinuePropagation:
                 raise ContinuePropagation
             except UserNotParticipant:
                 pass
             except MessageEmpty:
```

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/exceptions.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/methods/__init__.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/methods/_database.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/methods/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/methods/_misc.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/methods/changer.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/methods/converter.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/methods/func.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/methods/funcb.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/methods/funcb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/methods/helpers.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/methods/hosting.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/methods/inlinebot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/methods/queue.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/resources/Logo Ayiin.jpg` & `py-Ayiin-0.4.6.dev1/pyAyiin/resources/Logo Ayiin.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/resources/Youtube.jpeg` & `py-Ayiin-0.4.6.dev1/pyAyiin/resources/Youtube.jpeg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/resources/ayiin_music.jpg` & `py-Ayiin-0.4.6.dev1/pyAyiin/resources/ayiin_music.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/resources/ayiin_ubot.jpg` & `py-Ayiin-0.4.6.dev1/pyAyiin/resources/ayiin_ubot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/resources/ayiin_userbot.jpg` & `py-Ayiin-0.4.6.dev1/pyAyiin/resources/ayiin_userbot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/resources/blank.png` & `py-Ayiin-0.4.6.dev1/pyAyiin/resources/blank.png`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/resources/default.ttf` & `py-Ayiin-0.4.6.dev1/pyAyiin/resources/default.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/resources/font.ttf` & `py-Ayiin-0.4.6.dev1/pyAyiin/resources/font.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/resources/font2.ttf` & `py-Ayiin-0.4.6.dev1/pyAyiin/resources/font2.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/pyAyiin/xd.py` & `py-Ayiin-0.4.6.dev1/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.4.6.dev1/py_Ayiin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.5.dev1
+Version: 0.4.6.dev1
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.5.dev1/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.4.6.dev1/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.5.dev1/setup.py` & `py-Ayiin-0.4.6.dev1/setup.py`

 * *Files identical despite different names*

