# Comparing `tmp/towalink_tlm-0.1.9.tar.gz` & `tmp/towalink_tlm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "towalink_tlm-0.1.9.tar", last modified: Thu Jul  7 20:07:30 2022, max compression
+gzip compressed data, was "towalink_tlm-0.2.0.tar", last modified: Sun Jun 11 07:58:12 2023, max compression
```

## Comparing `towalink_tlm-0.1.9.tar` & `towalink_tlm-0.2.0.tar`

### file list

```diff
@@ -1,92 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:30.011951 towalink_tlm-0.1.9/
--rwxrw-r--   0 root         (0) root         (0)    34523 2020-08-22 10:31:22.000000 towalink_tlm-0.1.9/LICENSE
--rwxrw-r--   0 root         (0) root         (0)       92 2020-08-22 10:32:22.000000 towalink_tlm-0.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1697 2022-07-07 20:07:30.011951 towalink_tlm-0.1.9/PKG-INFO
--rwxrw-r--   0 root         (0) root         (0)      496 2022-07-06 20:18:16.000000 towalink_tlm-0.1.9/README.md
--rwxrw-r--   0 root         (0) root         (0)       97 2022-07-07 20:07:30.011951 towalink_tlm-0.1.9/setup.cfg
--rwxrw-r--   0 root         (0) root         (0)     1977 2022-07-06 20:19:13.000000 towalink_tlm-0.1.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.111932 towalink_tlm-0.1.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.431939 towalink_tlm-0.1.9/src/tlm/
--rwxrw-r--   0 root         (0) root         (0)    12039 2022-07-06 20:10:54.000000 towalink_tlm-0.1.9/src/tlm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.431939 towalink_tlm-0.1.9/src/tlm/ansible/
--rwxrw-r--   0 root         (0) root         (0)      314 2021-05-25 19:45:01.000000 towalink_tlm-0.1.9/src/tlm/ansible/node.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.111932 towalink_tlm-0.1.9/src/tlm/ansible/roles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.111932 towalink_tlm-0.1.9/src/tlm/ansible/roles/bird/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.111932 towalink_tlm-0.1.9/src/tlm/ansible/roles/bird/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.527941 towalink_tlm-0.1.9/src/tlm/ansible/roles/bird/files/etc_apt_preferencesd/
--rwxrw-r--   0 root         (0) root         (0)      232 2020-09-08 12:46:36.000000 towalink_tlm-0.1.9/src/tlm/ansible/roles/bird/files/etc_apt_preferencesd/debian-testing
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.543941 towalink_tlm-0.1.9/src/tlm/ansible/roles/bird/tasks/
--rwxrw-r--   0 root         (0) root         (0)     2727 2022-07-06 20:50:24.000000 towalink_tlm-0.1.9/src/tlm/ansible/roles/bird/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.111932 towalink_tlm-0.1.9/src/tlm/ansible/roles/bird-lg-proxy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.107932 towalink_tlm-0.1.9/src/tlm/ansible/roles/bird-lg-proxy/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.467940 towalink_tlm-0.1.9/src/tlm/ansible/roles/bird-lg-proxy/files/etc_initd/
--rwxrw-r--   0 root         (0) root         (0)      263 2021-05-25 20:25:16.000000 towalink_tlm-0.1.9/src/tlm/ansible/roles/bird-lg-proxy/files/etc_initd/towalink_bird-lg-proxy
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.491940 towalink_tlm-0.1.9/src/tlm/ansible/roles/bird-lg-proxy/files/etc_systemd_system/
--rwxrw-r--   0 root         (0) root         (0)      393 2021-05-25 20:42:14.000000 towalink_tlm-0.1.9/src/tlm/ansible/roles/bird-lg-proxy/files/etc_systemd_system/towalink_bird-lg-proxy.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.499940 towalink_tlm-0.1.9/src/tlm/ansible/roles/bird-lg-proxy/tasks/
--rwxrw-r--   0 root         (0) root         (0)     1262 2021-09-19 16:04:20.000000 towalink_tlm-0.1.9/src/tlm/ansible/roles/bird-lg-proxy/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.111932 towalink_tlm-0.1.9/src/tlm/ansible/roles/nodeconfig/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.111932 towalink_tlm-0.1.9/src/tlm/ansible/roles/nodeconfig/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.543941 towalink_tlm-0.1.9/src/tlm/ansible/roles/nodeconfig/files/opt_towalink_scripts/
--rwxrw-r--   0 root         (0) root         (0)      297 2020-09-07 15:14:20.000000 towalink_tlm-0.1.9/src/tlm/ansible/roles/nodeconfig/files/opt_towalink_scripts/rsync-nodecfg.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.563942 towalink_tlm-0.1.9/src/tlm/ansible/roles/nodeconfig/tasks/
--rwxrw-r--   0 root         (0) root         (0)     2336 2020-11-23 09:46:52.000000 towalink_tlm-0.1.9/src/tlm/ansible/roles/nodeconfig/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.111932 towalink_tlm-0.1.9/src/tlm/ansible/roles/startup/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.111932 towalink_tlm-0.1.9/src/tlm/ansible/roles/startup/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.583942 towalink_tlm-0.1.9/src/tlm/ansible/roles/startup/files/etc_initd/
--rwxrw-r--   0 root         (0) root         (0)      216 2020-09-10 18:23:39.000000 towalink_tlm-0.1.9/src/tlm/ansible/roles/startup/files/etc_initd/towalink_startup
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.595942 towalink_tlm-0.1.9/src/tlm/ansible/roles/startup/files/etc_systemd_system/
--rwxrw-r--   0 root         (0) root         (0)      330 2020-09-11 10:10:47.000000 towalink_tlm-0.1.9/src/tlm/ansible/roles/startup/files/etc_systemd_system/towalink_startup.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.619943 towalink_tlm-0.1.9/src/tlm/ansible/roles/startup/files/opt_towalink_startup/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.643943 towalink_tlm-0.1.9/src/tlm/ansible/roles/startup/files/opt_towalink_startup/scripts/
--rwxrw-r--   0 root         (0) root         (0)      317 2020-06-21 21:01:14.000000 towalink_tlm-0.1.9/src/tlm/ansible/roles/startup/files/opt_towalink_startup/scripts/wireguard
--rwxrw-r--   0 root         (0) root         (0)      250 2020-06-21 20:25:57.000000 towalink_tlm-0.1.9/src/tlm/ansible/roles/startup/files/opt_towalink_startup/towalink.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.667944 towalink_tlm-0.1.9/src/tlm/ansible/roles/startup/tasks/
--rwxrw-r--   0 root         (0) root         (0)     1115 2020-09-08 10:25:54.000000 towalink_tlm-0.1.9/src/tlm/ansible/roles/startup/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.111932 towalink_tlm-0.1.9/src/tlm/ansible/roles/system/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.111932 towalink_tlm-0.1.9/src/tlm/ansible/roles/system/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.691944 towalink_tlm-0.1.9/src/tlm/ansible/roles/system/files/unused_etc_sysctld/
--rwxrw-r--   0 root         (0) root         (0)      309 2020-09-10 17:23:27.000000 towalink_tlm-0.1.9/src/tlm/ansible/roles/system/files/unused_etc_sysctld/towalink.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.711945 towalink_tlm-0.1.9/src/tlm/ansible/roles/system/tasks/
--rwxrw-r--   0 root         (0) root         (0)      589 2020-09-11 14:09:00.000000 towalink_tlm-0.1.9/src/tlm/ansible/roles/system/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.723945 towalink_tlm-0.1.9/src/tlm/ansible/vars/
--rwxrw-r--   0 root         (0) root         (0)      137 2020-10-03 21:23:15.000000 towalink_tlm-0.1.9/src/tlm/ansible/vars/external_vars.yml
--rwxrw-r--   0 root         (0) root         (0)     4639 2021-06-16 18:55:44.000000 towalink_tlm-0.1.9/src/tlm/ansiblecaller.py
--rwxrw-r--   0 root         (0) root         (0)     1430 2020-06-02 19:29:15.000000 towalink_tlm-0.1.9/src/tlm/configfilecopier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.851948 towalink_tlm-0.1.9/src/tlm/configmanager/
--rwxrw-r--   0 root         (0) root         (0)        0 2020-06-15 18:25:35.000000 towalink_tlm-0.1.9/src/tlm/configmanager/__init__.py
--rwxrw-r--   0 root         (0) root         (0)     8002 2020-11-23 20:47:19.000000 towalink_tlm-0.1.9/src/tlm/configmanager/configmanager.py
--rwxrw-r--   0 root         (0) root         (0)     3738 2020-09-18 20:20:25.000000 towalink_tlm-0.1.9/src/tlm/configmanager/generatedconfig.py
--rwxrw-r--   0 root         (0) root         (0)     1688 2020-07-25 19:44:05.000000 towalink_tlm-0.1.9/src/tlm/configmanager/nodeconfig.py
--rwxrw-r--   0 root         (0) root         (0)     1503 2020-07-25 19:45:52.000000 towalink_tlm-0.1.9/src/tlm/configmanager/siteconfig.py
--rwxrw-r--   0 root         (0) root         (0)     6433 2020-09-17 19:42:31.000000 towalink_tlm-0.1.9/src/tlm/configmanager/tomlconfig.py
--rwxrw-r--   0 root         (0) root         (0)     4205 2021-05-27 20:26:40.000000 towalink_tlm-0.1.9/src/tlm/configmanager/tomlconfighierarchy.py
--rwxrw-r--   0 root         (0) root         (0)     5778 2020-07-12 20:32:32.000000 towalink_tlm-0.1.9/src/tlm/configmanager/yamlconfig.py
--rwxrw-r--   0 root         (0) root         (0)    18444 2022-07-06 20:17:16.000000 towalink_tlm-0.1.9/src/tlm/configorchestrator.py
--rwxrw-r--   0 root         (0) root         (0)     1330 2020-06-24 20:38:54.000000 towalink_tlm-0.1.9/src/tlm/directorycomparer.py
--rwxrw-r--   0 root         (0) root         (0)      891 2020-06-25 20:50:01.000000 towalink_tlm-0.1.9/src/tlm/exceptionlogger.py
--rwxrw-r--   0 root         (0) root         (0)     5170 2020-09-06 18:30:57.000000 towalink_tlm-0.1.9/src/tlm/exechelper.py
--rwxrw-r--   0 root         (0) root         (0)     2492 2021-06-16 19:49:03.000000 towalink_tlm-0.1.9/src/tlm/filesync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.883948 towalink_tlm-0.1.9/src/tlm/healthcheck/
--rwxrw-r--   0 root         (0) root         (0)        0 2019-02-17 19:11:58.000000 towalink_tlm-0.1.9/src/tlm/healthcheck/__init__.py
--rwxrw-r--   0 root         (0) root         (0)     1528 2019-02-18 20:17:29.000000 towalink_tlm-0.1.9/src/tlm/healthcheck/cmdexec.py
--rwxrw-r--   0 root         (0) root         (0)      854 2019-08-16 08:59:31.000000 towalink_tlm-0.1.9/src/tlm/healthcheck/ping.py
--rwxrw-r--   0 root         (0) root         (0)     3347 2020-07-12 20:29:48.000000 towalink_tlm-0.1.9/src/tlm/jinjatransformer.py
--rwxrw-r--   0 root         (0) root         (0)     3052 2020-12-23 22:09:57.000000 towalink_tlm-0.1.9/src/tlm/management_interface.py
--rwxrw-r--   0 root         (0) root         (0)    18806 2020-09-14 19:37:54.000000 towalink_tlm-0.1.9/src/tlm/nodeattacher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:29.991950 towalink_tlm-0.1.9/src/tlm/skeleton/
--rwxrw-r--   0 root         (0) root         (0)      160 2020-09-12 09:56:45.000000 towalink_tlm-0.1.9/src/tlm/skeleton/LICENSE
--rwxrw-r--   0 root         (0) root         (0)     2806 2020-10-07 16:06:09.000000 towalink_tlm-0.1.9/src/tlm/skeleton/bird.conf.jinja
--rwxrw-r--   0 root         (0) root         (0)      317 2021-01-03 10:19:56.000000 towalink_tlm-0.1.9/src/tlm/skeleton/bird_neighbors.conf.jinja
--rwxrw-r--   0 root         (0) root         (0)       46 2020-09-11 15:09:58.000000 towalink_tlm-0.1.9/src/tlm/skeleton/bird_site-template.conf.jinja
--rwxrw-r--   0 root         (0) root         (0)     1644 2020-09-27 20:09:05.000000 towalink_tlm-0.1.9/src/tlm/skeleton/config.toml
--rwxrw-r--   0 root         (0) root         (0)      330 2020-09-11 18:12:23.000000 towalink_tlm-0.1.9/src/tlm/skeleton/startup_loopback.jinja
--rwxrw-r--   0 root         (0) root         (0)      545 2020-09-11 15:09:40.000000 towalink_tlm-0.1.9/src/tlm/skeleton/tlwg.conf.jinja
--rwxrw-r--   0 root         (0) root         (0)    13870 2022-07-06 20:11:24.000000 towalink_tlm-0.1.9/src/tlm/towalinkmanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 20:07:30.011951 towalink_tlm-0.1.9/src/towalink_tlm.egg-info/
--rwxrw-r--   0 root         (0) root         (0)     1697 2022-07-07 20:07:28.000000 towalink_tlm-0.1.9/src/towalink_tlm.egg-info/PKG-INFO
--rwxrw-r--   0 root         (0) root         (0)     2208 2022-07-07 20:07:28.000000 towalink_tlm-0.1.9/src/towalink_tlm.egg-info/SOURCES.txt
--rwxrw-r--   0 root         (0) root         (0)        1 2022-07-07 20:07:28.000000 towalink_tlm-0.1.9/src/towalink_tlm.egg-info/dependency_links.txt
--rwxrw-r--   0 root         (0) root         (0)       52 2022-07-07 20:07:28.000000 towalink_tlm-0.1.9/src/towalink_tlm.egg-info/entry_points.txt
--rwxrw-r--   0 root         (0) root         (0)       72 2022-07-07 20:07:28.000000 towalink_tlm-0.1.9/src/towalink_tlm.egg-info/requires.txt
--rwxrw-r--   0 root         (0) root         (0)        4 2022-07-07 20:07:28.000000 towalink_tlm-0.1.9/src/towalink_tlm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:12.559374 towalink_tlm-0.2.0/
+-rwxrw-r--   0 root         (0) root         (0)    34523 2020-08-22 10:31:22.000000 towalink_tlm-0.2.0/LICENSE
+-rwxrw-r--   0 root         (0) root         (0)       92 2020-08-22 10:32:22.000000 towalink_tlm-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-06-11 07:58:12.587373 towalink_tlm-0.2.0/PKG-INFO
+-rwxrw-r--   0 root         (0) root         (0)      496 2023-06-03 20:36:23.000000 towalink_tlm-0.2.0/README.md
+-rwxrw-r--   0 root         (0) root         (0)       97 2023-06-11 07:58:12.639373 towalink_tlm-0.2.0/setup.cfg
+-rwxrw-r--   0 root         (0) root         (0)     1885 2023-06-03 20:36:23.000000 towalink_tlm-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:04.359489 towalink_tlm-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:06.675456 towalink_tlm-0.2.0/src/tlm/
+-rwxrw-r--   0 root         (0) root         (0)    13045 2023-06-03 20:36:23.000000 towalink_tlm-0.2.0/src/tlm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:06.799455 towalink_tlm-0.2.0/src/tlm/ansible/
+-rwxrw-r--   0 root         (0) root         (0)      312 2023-05-21 17:49:12.000000 towalink_tlm-0.2.0/src/tlm/ansible/node.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:04.139492 towalink_tlm-0.2.0/src/tlm/ansible/roles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:03.811496 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:03.783497 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:07.267448 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird/files/etc_apt_preferencesd/
+-rwxrw-r--   0 root         (0) root         (0)      232 2020-09-08 12:46:36.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird/files/etc_apt_preferencesd/debian-testing
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:07.403446 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird/tasks/
+-rwxrw-r--   0 root         (0) root         (0)     2727 2022-07-06 20:50:24.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:03.699498 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:03.675498 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:06.907453 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/files/etc_initd/
+-rwxrw-r--   0 root         (0) root         (0)      265 2023-06-11 07:52:39.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/files/etc_initd/towalink_bird-lg-proxy
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:07.019451 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/files/etc_systemd_system/
+-rwxrw-r--   0 root         (0) root         (0)      395 2023-06-11 07:53:03.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/files/etc_systemd_system/towalink_bird-lg-proxy.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:07.127450 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/tasks/
+-rwxrw-r--   0 root         (0) root         (0)     1262 2021-09-19 16:04:20.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:03.919495 towalink_tlm-0.2.0/src/tlm/ansible/roles/nodeconfig/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:03.891495 towalink_tlm-0.2.0/src/tlm/ansible/roles/nodeconfig/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:07.543444 towalink_tlm-0.2.0/src/tlm/ansible/roles/nodeconfig/files/opt_towalink_scripts/
+-rwxrw-r--   0 root         (0) root         (0)      297 2020-09-07 15:14:20.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/nodeconfig/files/opt_towalink_scripts/rsync-nodecfg.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:07.727442 towalink_tlm-0.2.0/src/tlm/ansible/roles/nodeconfig/tasks/
+-rwxrw-r--   0 root         (0) root         (0)     2336 2020-11-23 09:46:52.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/nodeconfig/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:04.111492 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:04.055493 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:08.003438 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/etc_initd/
+-rwxrw-r--   0 root         (0) root         (0)      216 2020-09-10 18:23:39.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/etc_initd/towalink_startup
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:08.135436 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/etc_systemd_system/
+-rwxrw-r--   0 root         (0) root         (0)      330 2020-09-11 10:10:47.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/etc_systemd_system/towalink_startup.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:08.299434 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/opt_towalink_startup/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:08.427432 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/opt_towalink_startup/scripts/
+-rwxrw-r--   0 root         (0) root         (0)      317 2020-06-21 21:01:14.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/opt_towalink_startup/scripts/wireguard
+-rwxrw-r--   0 root         (0) root         (0)      250 2020-06-21 20:25:57.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/opt_towalink_startup/towalink.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:08.583430 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/tasks/
+-rwxrw-r--   0 root         (0) root         (0)     1115 2020-09-08 10:25:54.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:04.223491 towalink_tlm-0.2.0/src/tlm/ansible/roles/system/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:04.195491 towalink_tlm-0.2.0/src/tlm/ansible/roles/system/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:08.735427 towalink_tlm-0.2.0/src/tlm/ansible/roles/system/files/unused_etc_sysctld/
+-rwxrw-r--   0 root         (0) root         (0)      309 2020-09-10 17:23:27.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/system/files/unused_etc_sysctld/towalink.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:08.887425 towalink_tlm-0.2.0/src/tlm/ansible/roles/system/tasks/
+-rwxrw-r--   0 root         (0) root         (0)      589 2020-09-11 14:09:00.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/system/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:09.219421 towalink_tlm-0.2.0/src/tlm/ansible/vars/
+-rwxrw-r--   0 root         (0) root         (0)      137 2020-10-03 21:23:15.000000 towalink_tlm-0.2.0/src/tlm/ansible/vars/external_vars.yml
+-rwxrw-r--   0 root         (0) root         (0)     4639 2021-06-16 18:55:44.000000 towalink_tlm-0.2.0/src/tlm/ansiblecaller.py
+-rwxrw-r--   0 root         (0) root         (0)     1430 2020-06-02 19:29:15.000000 towalink_tlm-0.2.0/src/tlm/configfilecopier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:10.383404 towalink_tlm-0.2.0/src/tlm/configmanager/
+-rwxrw-r--   0 root         (0) root         (0)        0 2020-06-15 18:25:35.000000 towalink_tlm-0.2.0/src/tlm/configmanager/__init__.py
+-rwxrw-r--   0 root         (0) root         (0)     8002 2020-11-23 20:47:19.000000 towalink_tlm-0.2.0/src/tlm/configmanager/configmanager.py
+-rwxrw-r--   0 root         (0) root         (0)     3738 2020-09-18 20:20:25.000000 towalink_tlm-0.2.0/src/tlm/configmanager/generatedconfig.py
+-rwxrw-r--   0 root         (0) root         (0)     1688 2020-07-25 19:44:05.000000 towalink_tlm-0.2.0/src/tlm/configmanager/nodeconfig.py
+-rwxrw-r--   0 root         (0) root         (0)     1503 2020-07-25 19:45:52.000000 towalink_tlm-0.2.0/src/tlm/configmanager/siteconfig.py
+-rwxrw-r--   0 root         (0) root         (0)     6433 2020-09-17 19:42:31.000000 towalink_tlm-0.2.0/src/tlm/configmanager/tomlconfig.py
+-rwxrw-r--   0 root         (0) root         (0)     4205 2021-05-27 20:26:40.000000 towalink_tlm-0.2.0/src/tlm/configmanager/tomlconfighierarchy.py
+-rwxrw-r--   0 root         (0) root         (0)     2408 2023-06-03 20:36:25.000000 towalink_tlm-0.2.0/src/tlm/configmanager/wireguard.py
+-rwxrw-r--   0 root         (0) root         (0)     5778 2020-07-12 20:32:32.000000 towalink_tlm-0.2.0/src/tlm/configmanager/yamlconfig.py
+-rwxrw-r--   0 root         (0) root         (0)    18466 2023-06-09 15:59:39.000000 towalink_tlm-0.2.0/src/tlm/configorchestrator.py
+-rwxrw-r--   0 root         (0) root         (0)     1330 2020-06-24 20:38:54.000000 towalink_tlm-0.2.0/src/tlm/directorycomparer.py
+-rwxrw-r--   0 root         (0) root         (0)      891 2020-06-25 20:50:01.000000 towalink_tlm-0.2.0/src/tlm/exceptionlogger.py
+-rwxrw-r--   0 root         (0) root         (0)     5170 2020-09-06 18:30:57.000000 towalink_tlm-0.2.0/src/tlm/exechelper.py
+-rwxrw-r--   0 root         (0) root         (0)     2492 2021-06-16 19:49:03.000000 towalink_tlm-0.2.0/src/tlm/filesync.py
+-rwxrw-r--   0 root         (0) root         (0)     3533 2023-06-09 16:27:34.000000 towalink_tlm-0.2.0/src/tlm/gitcaller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:10.719400 towalink_tlm-0.2.0/src/tlm/healthcheck/
+-rwxrw-r--   0 root         (0) root         (0)        0 2023-06-03 20:36:25.000000 towalink_tlm-0.2.0/src/tlm/healthcheck/__init__.py
+-rwxrw-r--   0 root         (0) root         (0)     1489 2023-06-03 20:36:25.000000 towalink_tlm-0.2.0/src/tlm/healthcheck/cmdexec.py
+-rwxrw-r--   0 root         (0) root         (0)      831 2023-06-03 20:36:25.000000 towalink_tlm-0.2.0/src/tlm/healthcheck/ping.py
+-rwxrw-r--   0 root         (0) root         (0)     3347 2020-07-12 20:29:48.000000 towalink_tlm-0.2.0/src/tlm/jinjatransformer.py
+-rwxrw-r--   0 root         (0) root         (0)     3082 2023-06-09 15:57:54.000000 towalink_tlm-0.2.0/src/tlm/management_interface.py
+-rwxrw-r--   0 root         (0) root         (0)    18840 2023-06-09 15:59:51.000000 towalink_tlm-0.2.0/src/tlm/nodeattacher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:11.747385 towalink_tlm-0.2.0/src/tlm/skeleton/
+-rwxrw-r--   0 root         (0) root         (0)      160 2020-09-12 09:56:45.000000 towalink_tlm-0.2.0/src/tlm/skeleton/LICENSE
+-rwxrw-r--   0 root         (0) root         (0)     2811 2023-06-03 20:36:24.000000 towalink_tlm-0.2.0/src/tlm/skeleton/bird.conf.jinja
+-rwxrw-r--   0 root         (0) root         (0)      322 2023-06-03 20:36:24.000000 towalink_tlm-0.2.0/src/tlm/skeleton/bird_neighbors.conf.jinja
+-rwxrw-r--   0 root         (0) root         (0)       46 2020-09-11 15:09:58.000000 towalink_tlm-0.2.0/src/tlm/skeleton/bird_site-template.conf.jinja
+-rwxrw-r--   0 root         (0) root         (0)     1644 2020-09-27 20:09:05.000000 towalink_tlm-0.2.0/src/tlm/skeleton/config.toml
+-rwxrw-r--   0 root         (0) root         (0)      330 2020-09-11 18:12:23.000000 towalink_tlm-0.2.0/src/tlm/skeleton/startup_loopback.jinja
+-rwxrw-r--   0 root         (0) root         (0)      545 2020-09-11 15:09:40.000000 towalink_tlm-0.2.0/src/tlm/skeleton/tlwg.conf.jinja
+-rwxrw-r--   0 root         (0) root         (0)    14437 2023-06-03 20:49:12.000000 towalink_tlm-0.2.0/src/tlm/towalinkmanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:12.451375 towalink_tlm-0.2.0/src/towalink_tlm.egg-info/
+-rwxrw-r--   0 root         (0) root         (0)     1526 2023-06-11 07:58:03.000000 towalink_tlm-0.2.0/src/towalink_tlm.egg-info/PKG-INFO
+-rwxrw-r--   0 root         (0) root         (0)     2264 2023-06-11 07:58:03.000000 towalink_tlm-0.2.0/src/towalink_tlm.egg-info/SOURCES.txt
+-rwxrw-r--   0 root         (0) root         (0)        1 2023-06-11 07:58:03.000000 towalink_tlm-0.2.0/src/towalink_tlm.egg-info/dependency_links.txt
+-rwxrw-r--   0 root         (0) root         (0)       33 2023-06-11 07:58:03.000000 towalink_tlm-0.2.0/src/towalink_tlm.egg-info/entry_points.txt
+-rwxrw-r--   0 root         (0) root         (0)       72 2023-06-11 07:58:03.000000 towalink_tlm-0.2.0/src/towalink_tlm.egg-info/requires.txt
+-rwxrw-r--   0 root         (0) root         (0)        4 2023-06-11 07:58:03.000000 towalink_tlm-0.2.0/src/towalink_tlm.egg-info/top_level.txt
```

### Comparing `towalink_tlm-0.1.9/LICENSE` & `towalink_tlm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/PKG-INFO` & `towalink_tlm-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: towalink_tlm
-Version: 0.1.9
+Version: 0.2.0
 Summary: command line tool for configuring and managing a Towalink installation
 Home-page: https://www.towalink.net
 Author: The Towalink Project
 Author-email: pypi.tlm@towalink.net
-License: UNKNOWN
 Project-URL: Project homepage, https://www.towalink.net
 Project-URL: Repository, https://www.github.com/towalink/tlm
 Project-URL: Documentation, https://towalink.readthedocs.io
-Description: # tlm - Towalink Manager
-        
-        Tool for configuring and managing a Towalink installation.
-        
-        ---
-        
-        ## Documentation
-        
-        The documentation of the Towalink project can be found at https://towalink.readthedocs.io
-        
-        ---
-        
-        ## License
-        
-        [![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
-        
-        - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
-        - Copyright 2020-2022 © <a href="https://www.towalink.net" target="_blank">Dirk Henrici</a>.
-        
 Keywords: Towalink VPN SD-WAN WireGuard
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# tlm - Towalink Manager
+
+Tool for configuring and managing a Towalink installation.
+
+---
+
+## Documentation
+
+The documentation of the Towalink project can be found at https://towalink.readthedocs.io
+
+---
+
+## License
+
+[![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
+
+- **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
+- Copyright 2020-2023 © <a href="https://www.towalink.net" target="_blank">Dirk Henrici</a>.
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: towalink_tlm Version: 0.1.9 Summary: command line
+Metadata-Version: 2.1 Name: towalink_tlm Version: 0.2.0 Summary: command line
 tool for configuring and managing a Towalink installation Home-page: https://
 www.towalink.net Author: The Towalink Project Author-email:
-pypi.tlm@towalink.net License: UNKNOWN Project-URL: Project homepage, https://
-www.towalink.net Project-URL: Repository, https://www.github.com/towalink/tlm
-Project-URL: Documentation, https://towalink.readthedocs.io Description: # tlm
-- Towalink Manager Tool for configuring and managing a Towalink installation. -
--- ## Documentation The documentation of the Towalink project can be found at
-https://towalink.readthedocs.io --- ## License [![License](http://
-img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://
-opensource.org/licenses/AGPL-3.0) - **[AGPL3 license](https://opensource.org/
-licenses/AGPL-3.0)** - Copyright 2020-2022 Â© Dirk_Henrici. Keywords: Towalink
-VPN SD-WAN WireGuard Platform: UNKNOWN Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Operating System :: POSIX :: Linux Classifier: Development Status
-:: 3 - Alpha Classifier: Intended Audience :: System Administrators Classifier:
-Intended Audience :: Information Technology Classifier: Intended Audience ::
-Telecommunications Industry Classifier: Topic :: System :: Networking Requires-
-Python: >=3.6 Description-Content-Type: text/markdown
+pypi.tlm@towalink.net Project-URL: Project homepage, https://www.towalink.net
+Project-URL: Repository, https://www.github.com/towalink/tlm Project-URL:
+Documentation, https://towalink.readthedocs.io Keywords: Towalink VPN SD-WAN
+WireGuard Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU Affero
+General Public License v3 or later (AGPLv3+) Classifier: Operating System ::
+POSIX :: Linux Classifier: Development Status :: 4 - Beta Classifier: Intended
+Audience :: System Administrators Classifier: Intended Audience :: Information
+Technology Classifier: Intended Audience :: Telecommunications Industry
+Classifier: Topic :: System :: Networking Requires-Python: >=3.6 Description-
+Content-Type: text/markdown License-File: LICENSE # tlm - Towalink Manager Tool
+for configuring and managing a Towalink installation. --- ## Documentation The
+documentation of the Towalink project can be found at https://
+towalink.readthedocs.io --- ## License [![License](http://img.shields.io/:
+license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/
+AGPL-3.0) - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)** -
+Copyright 2020-2023 Â© Dirk_Henrici.
```

### Comparing `towalink_tlm-0.1.9/setup.py` & `towalink_tlm-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup_kwargs = {
     'name': 'towalink_tlm',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'author': 'The Towalink Project',
     'author_email': 'pypi.tlm@towalink.net',
     'description': 'command line tool for configuring and managing a Towalink installation',
     'long_description': long_description,
     'long_description_content_type': 'text/markdown',
     'url': 'https://www.towalink.net',
     'packages': setuptools.find_packages('src'),
@@ -30,17 +30,15 @@
         tlm=tlm:main
     ''',
     'classifiers': [
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Operating System :: POSIX :: Linux',
-        #'Development Status :: 2 - Pre-Alpha',
-        'Development Status :: 3 - Alpha',
-        #'Development Status :: 4 - Beta',
+        'Development Status :: 4 - Beta',
         #'Development Status :: 5 - Production/Stable',
         'Intended Audience :: System Administrators',
         'Intended Audience :: Information Technology',
         'Intended Audience :: Telecommunications Industry',
         'Topic :: System :: Networking'
     ],
     'python_requires': '>=3.6',
```

### Comparing `towalink_tlm-0.1.9/src/tlm/__init__.py` & `towalink_tlm-0.2.0/src/tlm/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 """tlm: a command line tool for configuring and managing a Towalink installation"""
 
 """
 Towalink
-Copyright (C) 2020-2022 Dirk Henrici
+Copyright (C) 2020-2023 Dirk Henrici
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Affero General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -66,29 +66,30 @@
     print('          %s remove node <nodename>.<sitename>' % name)
     print('          %s remove node <nodeid>' % name)
     print('          %s set global <attr> <value>' % name)
     print('          %s set site <sitename> <attr> <value>' % name)
     print('          %s set node <nodename>.<sitename> <attr> <value>' % name)
     print('          %s set node <nodeid> <attr> <value>' % name)
     print('          %s list changed' % name)
-    print('          %s commit all' % name)
-    print('          %s commit site <sitename>' % name)
-    print('          %s commit node <nodename>.<sitename>' % name)
+    print('          %s commit -m mymessage all' % name)
+    print('          %s commit -m mymessage site <sitename>' % name)
+    print('          %s commit -m mymessage node <nodename>.<sitename>' % name)
     print('          %s activate all' % name)
     print('          %s activate site <sitename> <version>' % name)
     print('          %s activate node <nodename>.<sitename> <version>' % name)
     print('          %s attach node <nodename>.<sitename>' % name)
     print('          %s ansible all <arguments...>' % name)
     print('          %s ansible site <sitename> <arguments...>' % name)
     print('          %s ansible node <nodename>.<sitename> <arguments...>' % name)
     print('          %s ansible node <nodeid> <arguments...>' % name)
     print('          %s ansible-playbook all <arguments...>' % name)
     print('          %s ansible-playbook site <sitename> <arguments...>' % name)
     print('          %s ansible-playbook node <nodename>.<sitename> <arguments...>' % name)
     print('          %s ansible-playbook node <nodeid> <arguments...>' % name)
+    print('          %s git <git arguments...>' % name)
     print()
 
 def show_usage_and_exit(text = None):
     """Show information on command line arguments and exit with error"""
     if text is not None:
         print(text)
     print()
@@ -160,23 +161,31 @@
         elif expected_args == 4:
             return args[2], args[3]
         elif expected_args == 5:
             return args[2], args[4], args[4]
         else:
             raise ValueError('unsupported number of arguments')
 
+    # Workaround to convert "tlm commit -m message" into "tlm -m message commit" so that it can then be parsed regularly
+    if (len(sys.argv) > 3) and (sys.argv[2] == '-m'):
+        sys.argv = [ sys.argv[0], sys.argv[2], sys.argv[3], sys.argv[1] ] + sys.argv[4:]
+    # Parse arguments using "getopt"
     try:
-        opts, args = getopt.getopt(sys.argv[1:], 'l:?', ['help', 'loglevel='])
+        opts, args = getopt.getopt(sys.argv[1:], 'm:l:?', ['help', 'loglevel='])
     except getopt.GetoptError as ex:
         # Print help information and exit
         show_usage_and_exit(ex) # will print something like "option -a not recognized"
+    # Evaluate parsed arguments
+    message = None
     loglevel = logging.INFO
     for o, a in opts:
         if o in ('-?', '--help'):
             show_usage_and_exit()
+        elif o == '-m':
+            message = a
         elif o in ('-l', '--loglevel'):
             a = a.lower()
             if a == 'debug':
               loglevel = logging.DEBUG
             elif a == 'info':
               loglevel = logging.INFO
             elif a == 'warning':
@@ -186,29 +195,33 @@
             else:
                 show_usage_and_exit('invalid loglevel')
         else:
             assert False, 'unhandled option'
     if len(args) == 0:
         show_usage_and_exit('Welcome to Towalink!')
     operation = args[0]
-    if not operation in ['list', 'show', 'show-all', 'show_all', 'query', 'add', 'create', 'del', 'delete', 'remove', 'set', 'commit', 'activate', 'attach', 'ansible', 'ansible-playbook', 'ansible_playbook']:
+    if not operation in ['list', 'show', 'show-all', 'show_all', 'query', 'add', 'create', 'del', 'delete', 'remove', 'set', 'commit', 'activate', 'attach', 'ansible', 'ansible-playbook', 'ansible_playbook', 'git']:
         show_usage_and_exit(f'provided operation [{operation}] is invalid')
     # Deal with synonyms    
     if operation == 'query':
         operation = 'show'
     if operation == 'create':
         operation = 'add'
     if (operation == 'delete') or (operation == 'remove'):
         operation = 'del'
     # Two arguments are obligatory
     if len(args) < 2:
         show_usage_and_exit('not enough arguments provided for this operation')
-    # Case when three arguments are expected: <operation> <entity> [identifier]
-    method = operation + '_' + args[1]
+    # Evaluate operation
+    if operation == 'git':
+        method = 'git'
+    else:  # case when three arguments are expected: <operation> <entity> [identifier]
+        method = operation + '_' + args[1]
     entity_id = None
+    arguments = args[2:]
     if method == 'list_sites':
         expect_arg(None)
     elif method == 'list_nodes':
         entity_id = expect_arg('site')
     elif method == 'show_global':
         expect_arg(None)
     elif method == 'show_site':
@@ -257,24 +270,33 @@
         _ = expect_arg('nodeany')
     elif (method == 'ansible-playbook_all') or (method == 'ansible_playbook_all'):
         _ = expect_arg('globalany')
     elif (method == 'ansible-playbook_site') or (method == 'ansible_playbook_site'):
         _ = expect_arg('siteany')
     elif (method == 'ansible-playbook_node') or (method == 'ansible_playbook_node'):
         _ = expect_arg('nodeany')
+    elif method == 'git':
+        _ = expect_arg('globalany')
+        arguments = args[1:]  # forward all git arguments
     else:
         show_usage_and_exit('the provided combination of operation and entity is not supported')
-    method = method.replace('-', '_') # dashes are not supported in method names in Python
-    return loglevel, method, args[2:]
+    method = method.replace('-', '_')  # dashes are not supported in method names in Python
+    kwarguments = dict()
+    if message is not None:
+        if operation == 'commit':
+            kwarguments['message'] = message
+        else:
+            show_usage_and_exit('"-m" may only be provided for "tlm commit"')
+    return loglevel, method, arguments, kwarguments
 
 def main():
     """Main function"""
-    loglevel, method, method_args = parseopts()
+    loglevel, method, method_args, method_kwargs = parseopts()
     logging.basicConfig(format='%(asctime)s %(levelname)s %(module)s: %(message)s', level=loglevel)  # use %(name)s instead of %(module) to include hierarchy information, see https://docs.python.org/2/library/logging.html
     logger = logging.getLogger(__name__)
     tlm = towalinkmanager.TLM()
     method = getattr(tlm, method)
-    exceptionlogger.call(method, *method_args, reraise_exceptions=True)
+    exceptionlogger.call(method, *method_args, **method_kwargs, reraise_exceptions=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `towalink_tlm-0.1.9/src/tlm/ansible/roles/bird/tasks/main.yml` & `towalink_tlm-0.2.0/src/tlm/ansible/roles/bird/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/ansible/roles/bird-lg-proxy/tasks/main.yml` & `towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/ansible/roles/nodeconfig/tasks/main.yml` & `towalink_tlm-0.2.0/src/tlm/ansible/roles/nodeconfig/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/ansible/roles/startup/tasks/main.yml` & `towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/ansible/roles/system/tasks/main.yml` & `towalink_tlm-0.2.0/src/tlm/ansible/roles/system/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/ansiblecaller.py` & `towalink_tlm-0.2.0/src/tlm/ansiblecaller.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/configfilecopier.py` & `towalink_tlm-0.2.0/src/tlm/configfilecopier.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/configmanager/configmanager.py` & `towalink_tlm-0.2.0/src/tlm/configmanager/configmanager.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/configmanager/generatedconfig.py` & `towalink_tlm-0.2.0/src/tlm/configmanager/generatedconfig.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/configmanager/nodeconfig.py` & `towalink_tlm-0.2.0/src/tlm/configmanager/nodeconfig.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/configmanager/siteconfig.py` & `towalink_tlm-0.2.0/src/tlm/configmanager/siteconfig.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/configmanager/tomlconfig.py` & `towalink_tlm-0.2.0/src/tlm/configmanager/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/configmanager/tomlconfighierarchy.py` & `towalink_tlm-0.2.0/src/tlm/configmanager/tomlconfighierarchy.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/configmanager/yamlconfig.py` & `towalink_tlm-0.2.0/src/tlm/configmanager/yamlconfig.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/configorchestrator.py` & `towalink_tlm-0.2.0/src/tlm/configorchestrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 
 
 logger = logging.getLogger(__name__)
 NAME_TEMPOUTPUT_DIRECTORY = 'tmp'
 NAME_OUTPUT_DIRECTORY = 'new'
 NODE_CONFIG_PATH = '/etc/towalink/configs'
 WG_INTERFACE = 'tlwg_mgmt'
+WG_LISTENPORT = 51820
 
 
 class ConfigOrchestrator():
     """Class for managing the complete config directory hierarchy"""
 
     def __init__(self, confdir='/etc/towalink'):
-        """Constructor"""
+        """Initializer"""
         self.confdir = confdir
         self.prepare_confdir()
         self.confdir_effective = os.path.join(self.confdir, 'effective')
         self.cm = configmanager.ConfigManager(confdir)
         if not os.path.exists(self.confdir_effective):
             os.makedirs(self.confdir_effective)
         self.mgmt_if = management_interface.MgmtInterface(WG_INTERFACE)
@@ -86,15 +87,15 @@
             next = 'v' + str(latest + 1)
             latest = 'v' + str(latest)
         return latest, next
 
     def render_template_files(self, data, dir):
         """Renders the Jinja template files in the given directory using the provided data dictionary"""
         jt = jinjatransformer.JinjaTransformer(templatedir=dir, globalvars=dict({'grains': dict({'id': 'test'})}))
-        # Normal JInga template files
+        # Normal Jinga template files
         jt.render_templatefiles_to_files(dir, data=data, filter_ignore=['tlwg.conf.jinja'])
         # Wireguard interface configs
         for wglink in data.get('wg_links', dict()).values():
             jt.render_templatefile_to_file('tlwg.conf.jinja', os.path.join(dir, wglink['wg_ifname']+'.conf'), data=wglink)
 
     def update_node(self, node_id):
         """Updates all config files of a single node"""
```

### Comparing `towalink_tlm-0.1.9/src/tlm/directorycomparer.py` & `towalink_tlm-0.2.0/src/tlm/directorycomparer.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/exceptionlogger.py` & `towalink_tlm-0.2.0/src/tlm/exceptionlogger.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/exechelper.py` & `towalink_tlm-0.2.0/src/tlm/exechelper.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/filesync.py` & `towalink_tlm-0.2.0/src/tlm/filesync.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/healthcheck/cmdexec.py` & `towalink_tlm-0.2.0/src/tlm/healthcheck/cmdexec.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import logging;
-import shlex;
-import subprocess;
-
-logger = logging.getLogger(__name__);
-
-
-def execute_local(command, suppressoutput = True, suppresserrors = True, suppresslogging = False):
-    """Execute a command"""
-    if not suppresslogging:
-        logger.debug('Executing [{0}]'.format(command));
-    args = shlex.split(command);
-    nsp = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE);
-    out, err = nsp.communicate();
-    if err is not None:
-        err = err.decode('utf8');
-        if not suppresserrors and (len(err) > 0):
-            logger.error(err);
-    out = out.decode('utf8');
-    if not suppressoutput and (len(out) > 0):
-        print(out);       
-    nsp.wait();
-    return nsp.returncode, command, out, err;
-
-def execute(env_type, env_id, env_ns, command, suppressoutput = True, suppresserrors = True, suppresslogging = False):
-    """Execute a command in the given environment"""
-    if env_ns is not None:
-        command = 'ip netns exec {0} '.format(env_ns) + command;
-    if env_type is None:
-        pass;
-    elif env_type == 'pct':
-        command = 'pct exec {0} -- '.format(env_id) + command;
-    elif env_type == 'pveshell':
-        command = 'pveshell {0} -c '.format(env_id) + command;
-    elif env_type == 'vmshell':
-        command = 'vmshell {0} -c '.format(env_id) + command;
-    else:
-        raise ValueError('Invalid env_type specified')
-    return execute_local(command, suppressoutput, suppresserrors, suppresslogging);
+import logging;
+import shlex;
+import subprocess;
+
+logger = logging.getLogger(__name__);
+
+
+def execute_local(command, suppressoutput = True, suppresserrors = True, suppresslogging = False):
+    """Execute a command"""
+    if not suppresslogging:
+        logger.debug('Executing [{0}]'.format(command));
+    args = shlex.split(command);
+    nsp = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE);
+    out, err = nsp.communicate();
+    if err is not None:
+        err = err.decode('utf8');
+        if not suppresserrors and (len(err) > 0):
+            logger.error(err);
+    out = out.decode('utf8');
+    if not suppressoutput and (len(out) > 0):
+        print(out);       
+    nsp.wait();
+    return nsp.returncode, command, out, err;
+
+def execute(env_type, env_id, env_ns, command, suppressoutput = True, suppresserrors = True, suppresslogging = False):
+    """Execute a command in the given environment"""
+    if env_ns is not None:
+        command = 'ip netns exec {0} '.format(env_ns) + command;
+    if env_type is None:
+        pass;
+    elif env_type == 'pct':
+        command = 'pct exec {0} -- '.format(env_id) + command;
+    elif env_type == 'pveshell':
+        command = 'pveshell {0} -c '.format(env_id) + command;
+    elif env_type == 'vmshell':
+        command = 'vmshell {0} -c '.format(env_id) + command;
+    else:
+        raise ValueError('Invalid env_type specified')
+    return execute_local(command, suppressoutput, suppresserrors, suppresslogging);
```

### Comparing `towalink_tlm-0.1.9/src/tlm/healthcheck/ping.py` & `towalink_tlm-0.2.0/src/tlm/healthcheck/ping.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from . import cmdexec;
-
-
-def ping(info, env_type, env_id, env_ns, dest, src = None, count = 1, wait = 3, deadline = 3, quiet = True):
-    """Checks whether a destination is reachable by an echo request"""
-    cmd = 'ping';
-    if src is not None:
-        cmd += ' -I ' + src;
-    if count is not None:
-        cmd += ' -c ' + str(count);
-    if wait is not None:
-        cmd += ' -W ' + str(wait);
-    if deadline is not None:
-        cmd += ' -w ' + str(deadline);
-    if quiet:
-        cmd += ' -q';
-    cmd += ' ' + dest;
-    returncode, fullcmd, out, err = cmdexec.execute(env_type, env_id, env_ns, cmd);
-    details = fullcmd;
-    if len(out) > 0: 
-        detail = details + '\n' + 'STDOUT: ' + out; 
-    if len(err) > 0: 
-        detail = details + '\n' + 'STDERR: ' + err; 
+from . import cmdexec;
+
+
+def ping(info, env_type, env_id, env_ns, dest, src = None, count = 1, wait = 3, deadline = 3, quiet = True):
+    """Checks whether a destination is reachable by an echo request"""
+    cmd = 'ping';
+    if src is not None:
+        cmd += ' -I ' + src;
+    if count is not None:
+        cmd += ' -c ' + str(count);
+    if wait is not None:
+        cmd += ' -W ' + str(wait);
+    if deadline is not None:
+        cmd += ' -w ' + str(deadline);
+    if quiet:
+        cmd += ' -q';
+    cmd += ' ' + dest;
+    returncode, fullcmd, out, err = cmdexec.execute(env_type, env_id, env_ns, cmd);
+    details = fullcmd;
+    if len(out) > 0: 
+        detail = details + '\n' + 'STDOUT: ' + out; 
+    if len(err) > 0: 
+        detail = details + '\n' + 'STDERR: ' + err; 
     return (returncode == 0), cmd, info, details;
```

### Comparing `towalink_tlm-0.1.9/src/tlm/jinjatransformer.py` & `towalink_tlm-0.2.0/src/tlm/jinjatransformer.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/management_interface.py` & `towalink_tlm-0.2.0/src/tlm/management_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 
 logger = logging.getLogger(__name__);
 
 
 class MgmtInterface(object):
     """Class for configuring and managing the WireGuard management interface"""
     
-    def __init__(self, wg_interface):
+    def __init__(self, wg_interface, wg_listenport=51820):
         """Object initialization"""
         self.wg_interface = wg_interface 
+        self.wg_listenport = wg_listenport 
         self._wg_public = None
         self.wgconfig = wgconfig.WGConfig(self.wg_interface)
         try:
             self.wgconfig.read_file()
         except FileNotFoundError:
             self.ensure_configuration()
             
@@ -35,15 +36,15 @@
         if self._wg_public is None:
             self._wg_public = wgexec.get_publickey(self.wgconfig.interface['PrivateKey'])
         return self._wg_public
     
     def ensure_configuration(self):
         """Makes sure that the WireGuard interface has a basic configuration"""        
         self.wgconfig.add_attr(None, 'PrivateKey', wgexec.generate_privatekey())
-        self.wgconfig.add_attr(None, 'ListenPort', 51820) # *** we need to get the listenport from config
+        self.wgconfig.add_attr(None, 'ListenPort', self.wg_listenport)
         self.wgconfig.add_attr(None, 'Address', 'fe80::1')
         self.wgconfig.write_file()
 
     def ensure_service(self):
         """Makes sure that the management interface is up and starts on boot"""
         eh = exechelper.ExecHelper()
         eh.start_service(self.wgservice)
```

### Comparing `towalink_tlm-0.1.9/src/tlm/nodeattacher.py` & `towalink_tlm-0.2.0/src/tlm/nodeattacher.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         self.data['wg_shared'] = wg.generate_presharedkey()
         self.data['wg_peer_endpoint'] = mgmt_wg_endpoint
         self.data['wg_peer_public'] = mgmt_wg_public
         self.data['wg_peer_allowedips'] = ['fe80::1/128']
 
     def configure_mgmt_interface(self, nodeconfig):
         """Configures the management interface for the newly attached node"""
-        mi = management_interface.MgmtInterface(configorchestrator.WG_INTERFACE)
+        mi = management_interface.MgmtInterface(configorchestrator.WG_INTERFACE, configorchestrator.WG_LISTENPORT)
         node_id = nodeconfig.get_item('node_id')
         wg_public = nodeconfig.get_item('attach_wg_public')
         wg_shared = nodeconfig.get_item('attach_wg_shared')
         linklocal = configorchestrator.ConfigOrchestrator.get_ipaddress_byoffset('fe80::0/64', node_id, add_prefixlen=True, keep_prefixlen=False)
         wg_allowedips = [linklocal]
         mi.remove_peer_byallowedip(linklocal) # remove a possibly existing old entry for this node id
         mi.add_peer(wg_public=wg_public, wg_shared=wg_shared, wg_allowedips=wg_allowedips, node_id=node_id)
```

### Comparing `towalink_tlm-0.1.9/src/tlm/skeleton/bird.conf.jinja` & `towalink_tlm-0.2.0/src/tlm/skeleton/bird.conf.jinja`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         export none;
     };
 }
 
 protocol static static6 {
     check link; 
 
-{%- for peer, peerdata in bgp_peers.items() %}
+{%- for peer, peerdata in bgp_peers.items()|sort %}
     route {{peerdata.loopback_ipv6.partition('/')[0]}}/128 via "{{peerdata.ifname_local}}";
 {%- endfor %}
 
     ipv6 {
         export none;
     };
 }
```

### Comparing `towalink_tlm-0.1.9/src/tlm/skeleton/config.toml` & `towalink_tlm-0.2.0/src/tlm/skeleton/config.toml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/skeleton/tlwg.conf.jinja` & `towalink_tlm-0.2.0/src/tlm/skeleton/tlwg.conf.jinja`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.1.9/src/tlm/towalinkmanager.py` & `towalink_tlm-0.2.0/src/tlm/towalinkmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 
 import ast
 import logging
 import pprint
 
 from . import ansiblecaller
 from . import configorchestrator
+from . import gitcaller
 from . import nodeattacher
 
 
 logger = logging.getLogger(__name__);
 ATTR_MGMT_ADDRESS = 'attach_mgmt_address'
 
 
 class TLM():
     """Interface class to control the current Towalink installation"""
     co = None # holds an instance of ConfigOrchestrator
 
-    def __init__(self):
-        """Constructor"""
-#        self.co = configorchestrator.ConfigOrchestrator('/mnt/hdd1/dirk/AnnikaDirk/Versionsverwaltung/towalink/tlm/example/etc/towalink/')
-        self.co = configorchestrator.ConfigOrchestrator()
+    def __init__(self, confdir='/etc/towalink'):
+        """Initializer"""
+        self.confdir = confdir
+        self.co = configorchestrator.ConfigOrchestrator(confdir)
         #self.co.update_all()
         #self.co.process_new_configversion_all()
 
     def get_nodeid(self, node):
         """Returns the id of the specified node"""
         if node.isnumeric():
             node = int(node)
@@ -212,57 +213,63 @@
             self.set_conf(self.co.cm.nodes[node], attr, value)
         except KeyError:
             print('The specified node does not exist')            
 
     def list_changed(self):
         """Prints all sites with changes configuration"""
         self.co.update_all()
-        nodes, changed = self.co.process_new_configversion_all(dryrun = True)
-        if self.print_nodes(changed, reference_complete_cfg = True) == 0:
+        nodes, changed = self.co.process_new_configversion_all(dryrun=True)
+        if self.print_nodes(changed, reference_complete_cfg=True) == 0:
             print('No node configuration has changed')
 
-    def commit_all(self):
+    def commit_all(self, message=None):
         """Creates a new version of effective configuration for all nodes"""
         self.co.cm.update_generated_config()
         self.co.update_all()
         nodes, changed = self.co.process_new_configversion_all()
-        if self.print_nodes(changed, reference_complete_cfg = True) == 0:
+        if self.print_nodes(changed, reference_complete_cfg=True) == 0:
             print('No node configuration has changed; no new version created')
+        else:
+            gitcaller.Git.call_git_commit(self.confdir, message)
         print('Mirroring any existing configs to nodes...')
         self.co.mirror_node_configs(nodes.keys())
-        print('Done')
+        print('Done (hint: use "tlm activate" to activate a new configuration)')
 
-    def commit_site(self, site):
+    def commit_site(self, site, message=None):
         """Creates a new version of effective configuration for all nodes of the given site"""
         self.co.cm.update_generated_config()
         self.co.update_site(site)
         nodes, changed = self.co.process_new_configversion_site(site)
-        if self.print_nodes(changed, reference_complete_cfg = True) == 0:
+        if self.print_nodes(changed, reference_complete_cfg=True) == 0:
             print('No node configuration has changed; no new version created')
+        else:
+            gitcaller.Git.call_git_commit(self.confdir, message)
         print(f'Mirroring any existing configs to {len(nodes)} node(s)...')
         self.co.mirror_node_configs(nodes.keys())
-        print('Done')
+        print('Done (hint: use "tlm activate" to activate a new configuration)')
 
-    def commit_node(self, node):
+    def commit_node(self, node, message=None):
         """Creates a new version of effective configuration for the given node"""
         try:
             node = self.get_nodeid(node)
         except ValueError as e:
             print(e)
             return
         self.co.cm.update_generated_config()
         self.co.update_node(node)
         changed = self.co.process_new_configversion(node)
         changed = {node: self.co.cm.nodes[node]} if changed else dict()
         nodes = [node]
-        if self.print_nodes(changed, reference_complete_cfg = True) == 0:
+        if self.print_nodes(changed, reference_complete_cfg=True) == 0:
             print('Node configuration has not changed; nothing done')
+        else:
+            gitcaller.Git.call_git_commit(self.confdir, message)
         print('Mirroring any existing configs to node...')
         self.co.mirror_node_configs(nodes)
-        print('Done')
+        print('Done (hint: use "tlm activate" to activate a new configuration)')
 
     def attach_node(self, node):
         """Pairs a config-requesting device as the provided node"""
         try:
             nodeconfig = self.get_node(node)
             na = nodeattacher.NodeAttacher()
             na.attach_node(nodeconfig=nodeconfig, interactive=True) 
@@ -362,7 +369,11 @@
     def ansible_node(self, node, *ansible_args):
         """Calls 'ansible' for the given node"""
         return self.ansible_generic_node(node, *ansible_args, playbook=False)
 
     def ansible_playbook_node(self, node, *ansible_args):
         """Calls 'ansible-playbook' for the given node"""
         return self.ansible_generic_node(node, *ansible_args, playbook=True)
+
+    def git(self, *git_args):
+        """Calls 'git' for the Towalink config directory as local repository"""
+        return gitcaller.Git.call_git(self.confdir, *git_args)
```

### Comparing `towalink_tlm-0.1.9/src/towalink_tlm.egg-info/PKG-INFO` & `towalink_tlm-0.2.0/src/towalink_tlm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: towalink-tlm
-Version: 0.1.9
+Version: 0.2.0
 Summary: command line tool for configuring and managing a Towalink installation
 Home-page: https://www.towalink.net
 Author: The Towalink Project
 Author-email: pypi.tlm@towalink.net
-License: UNKNOWN
 Project-URL: Project homepage, https://www.towalink.net
 Project-URL: Repository, https://www.github.com/towalink/tlm
 Project-URL: Documentation, https://towalink.readthedocs.io
-Description: # tlm - Towalink Manager
-        
-        Tool for configuring and managing a Towalink installation.
-        
-        ---
-        
-        ## Documentation
-        
-        The documentation of the Towalink project can be found at https://towalink.readthedocs.io
-        
-        ---
-        
-        ## License
-        
-        [![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
-        
-        - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
-        - Copyright 2020-2022 © <a href="https://www.towalink.net" target="_blank">Dirk Henrici</a>.
-        
 Keywords: Towalink VPN SD-WAN WireGuard
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# tlm - Towalink Manager
+
+Tool for configuring and managing a Towalink installation.
+
+---
+
+## Documentation
+
+The documentation of the Towalink project can be found at https://towalink.readthedocs.io
+
+---
+
+## License
+
+[![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
+
+- **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
+- Copyright 2020-2023 © <a href="https://www.towalink.net" target="_blank">Dirk Henrici</a>.
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: towalink-tlm Version: 0.1.9 Summary: command line
+Metadata-Version: 2.1 Name: towalink-tlm Version: 0.2.0 Summary: command line
 tool for configuring and managing a Towalink installation Home-page: https://
 www.towalink.net Author: The Towalink Project Author-email:
-pypi.tlm@towalink.net License: UNKNOWN Project-URL: Project homepage, https://
-www.towalink.net Project-URL: Repository, https://www.github.com/towalink/tlm
-Project-URL: Documentation, https://towalink.readthedocs.io Description: # tlm
-- Towalink Manager Tool for configuring and managing a Towalink installation. -
--- ## Documentation The documentation of the Towalink project can be found at
-https://towalink.readthedocs.io --- ## License [![License](http://
-img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://
-opensource.org/licenses/AGPL-3.0) - **[AGPL3 license](https://opensource.org/
-licenses/AGPL-3.0)** - Copyright 2020-2022 Â© Dirk_Henrici. Keywords: Towalink
-VPN SD-WAN WireGuard Platform: UNKNOWN Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Operating System :: POSIX :: Linux Classifier: Development Status
-:: 3 - Alpha Classifier: Intended Audience :: System Administrators Classifier:
-Intended Audience :: Information Technology Classifier: Intended Audience ::
-Telecommunications Industry Classifier: Topic :: System :: Networking Requires-
-Python: >=3.6 Description-Content-Type: text/markdown
+pypi.tlm@towalink.net Project-URL: Project homepage, https://www.towalink.net
+Project-URL: Repository, https://www.github.com/towalink/tlm Project-URL:
+Documentation, https://towalink.readthedocs.io Keywords: Towalink VPN SD-WAN
+WireGuard Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU Affero
+General Public License v3 or later (AGPLv3+) Classifier: Operating System ::
+POSIX :: Linux Classifier: Development Status :: 4 - Beta Classifier: Intended
+Audience :: System Administrators Classifier: Intended Audience :: Information
+Technology Classifier: Intended Audience :: Telecommunications Industry
+Classifier: Topic :: System :: Networking Requires-Python: >=3.6 Description-
+Content-Type: text/markdown License-File: LICENSE # tlm - Towalink Manager Tool
+for configuring and managing a Towalink installation. --- ## Documentation The
+documentation of the Towalink project can be found at https://
+towalink.readthedocs.io --- ## License [![License](http://img.shields.io/:
+license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/
+AGPL-3.0) - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)** -
+Copyright 2020-2023 Â© Dirk_Henrici.
```

### Comparing `towalink_tlm-0.1.9/src/towalink_tlm.egg-info/SOURCES.txt` & `towalink_tlm-0.2.0/src/towalink_tlm.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/tlm/ansiblecaller.py
 src/tlm/configfilecopier.py
 src/tlm/configorchestrator.py
 src/tlm/directorycomparer.py
 src/tlm/exceptionlogger.py
 src/tlm/exechelper.py
 src/tlm/filesync.py
+src/tlm/gitcaller.py
 src/tlm/jinjatransformer.py
 src/tlm/management_interface.py
 src/tlm/nodeattacher.py
 src/tlm/towalinkmanager.py
 src/tlm/ansible/node.yml
 src/tlm/ansible/roles/bird-lg-proxy/files/etc_initd/towalink_bird-lg-proxy
 src/tlm/ansible/roles/bird-lg-proxy/files/etc_systemd_system/towalink_bird-lg-proxy.service
@@ -34,14 +35,15 @@
 src/tlm/configmanager/__init__.py
 src/tlm/configmanager/configmanager.py
 src/tlm/configmanager/generatedconfig.py
 src/tlm/configmanager/nodeconfig.py
 src/tlm/configmanager/siteconfig.py
 src/tlm/configmanager/tomlconfig.py
 src/tlm/configmanager/tomlconfighierarchy.py
+src/tlm/configmanager/wireguard.py
 src/tlm/configmanager/yamlconfig.py
 src/tlm/healthcheck/__init__.py
 src/tlm/healthcheck/cmdexec.py
 src/tlm/healthcheck/ping.py
 src/tlm/skeleton/LICENSE
 src/tlm/skeleton/bird.conf.jinja
 src/tlm/skeleton/bird_neighbors.conf.jinja
```

