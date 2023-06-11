# Comparing `tmp/gentoo-update-0.1.2.tar.gz` & `tmp/gentoo-update-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentoo-update-0.1.2.tar", last modified: Thu Jun  8 22:52:08 2023, max compression
+gzip compressed data, was "gentoo-update-0.1.3.tar", last modified: Sun Jun 11 19:07:15 2023, max compression
```

## Comparing `gentoo-update-0.1.2.tar` & `gentoo-update-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:52:08.308775 gentoo-update-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-08 22:51:56.000000 gentoo-update-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-08 22:52:08.308775 gentoo-update-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-08 22:51:56.000000 gentoo-update-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:52:08.308775 gentoo-update-0.1.2/gentoo_update/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 22:51:56.000000 gentoo-update-0.1.2/gentoo_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-06-08 22:51:56.000000 gentoo-update-0.1.2/gentoo_update/gentoo_update.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4545 2023-06-08 22:51:56.000000 gentoo-update-0.1.2/gentoo_update/updater.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:52:08.308775 gentoo-update-0.1.2/gentoo_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-08 22:52:08.000000 gentoo-update-0.1.2/gentoo_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-08 22:52:08.000000 gentoo-update-0.1.2/gentoo_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:52:08.000000 gentoo-update-0.1.2/gentoo_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 22:52:08.000000 gentoo-update-0.1.2/gentoo_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 22:52:08.000000 gentoo-update-0.1.2/gentoo_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-08 22:52:08.308775 gentoo-update-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 22:51:56.000000 gentoo-update-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:52:08.308775 gentoo-update-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-08 22:51:56.000000 gentoo-update-0.1.2/tests/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:15.576996 gentoo-update-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-11 19:07:15.576996 gentoo-update-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:15.576996 gentoo-update-0.1.3/gentoo_update/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/gentoo_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/gentoo_update/gentoo_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/gentoo_update/shell_runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4545 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/gentoo_update/updater.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:15.576996 gentoo-update-0.1.3/gentoo_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-11 19:07:15.000000 gentoo-update-0.1.3/gentoo_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-11 19:07:15.000000 gentoo-update-0.1.3/gentoo_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:07:15.000000 gentoo-update-0.1.3/gentoo_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-11 19:07:15.000000 gentoo-update-0.1.3/gentoo_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-11 19:07:15.000000 gentoo-update-0.1.3/gentoo_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-11 19:07:15.576996 gentoo-update-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:15.576996 gentoo-update-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/tests/test_updater.py
```

### Comparing `gentoo-update-0.1.2/LICENSE` & `gentoo-update-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.2/PKG-INFO` & `gentoo-update-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-Metadata-Version: 2.1
-Name: gentoo-update
-Version: 0.1.2
-Summary: Gentoo Linux updater
-Home-page: https://github.com/Lab-Brat/gentoo_update
-Author: Lab-Brat
-Author-email: labbrat_social@pm.me
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ### Gentoo Updater
 
-`gentoo-update` is a tool that automates installing updates on Gentoo Linux. 
+`gentoo-update` is a tool that automates updates on Gentoo Linux. 
 By default it only installs security updates from [GLSA](https://security.gentoo.org/glsa/), 
-but it also provides support to update `@world`.  
+but it can also be used to update `@world`.  
 
 This project 
 [originates](https://wiki.gentoo.org/wiki/Google_Summer_of_Code/2023/Ideas/Automated_Gentoo_system_updater) 
 from 2023 Google Summer of Code.
 
 
 #### Usage
-`gentoo-update` can be easily installed with pip (ebuild coming soon):
+`gentoo-update` is in [GURU](https://wiki.gentoo.org/wiki/Project:GURU) 
+overlay, and can be installed using emerge:
+```bash
+emerge --ask app-admin/gentoo_update
+```
+Because the project is in early stage of development it's not considered stable 
+and is masked by `~amd64`. To unmask it run:
 ```bash
-pip install gentoo_update
+echo 'app-admin/gentoo_update ~amd64' >> /etc/portage/package.accept_keywords/gentoo_update
+```
+
+Alternatively, updater can be installed with pip:
+```
+pip install gentoo_update --break-system-packages
 ```
 
 Here are some usage examples:
 * Basic security update
 ```bash
 gentoo-update
 ```
@@ -44,8 +40,8 @@
 * Full system update, show elogs and news
 ```bash
 gentoo-update --update-mode full --read-logs y --read-news y
 ```
 
 The detailed explanation of command flags can be found in `--help`.  
 Information on testing can be found in tests directory 
-[readme](gentoo_update/blob/main/tests/README.md)
+[readme](tests/README.md)
```

### Comparing `gentoo-update-0.1.2/gentoo_update/updater.sh` & `gentoo-update-0.1.3/gentoo_update/updater.sh`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.2/gentoo_update.egg-info/PKG-INFO` & `gentoo-update-0.1.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 Metadata-Version: 2.1
 Name: gentoo-update
-Version: 0.1.2
+Version: 0.1.3
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Gentoo Updater
 
-`gentoo-update` is a tool that automates installing updates on Gentoo Linux. 
+`gentoo-update` is a tool that automates updates on Gentoo Linux. 
 By default it only installs security updates from [GLSA](https://security.gentoo.org/glsa/), 
-but it also provides support to update `@world`.  
+but it can also be used to update `@world`.  
 
 This project 
 [originates](https://wiki.gentoo.org/wiki/Google_Summer_of_Code/2023/Ideas/Automated_Gentoo_system_updater) 
 from 2023 Google Summer of Code.
 
 
 #### Usage
-`gentoo-update` can be easily installed with pip (ebuild coming soon):
+`gentoo-update` is in [GURU](https://wiki.gentoo.org/wiki/Project:GURU) 
+overlay, and can be installed using emerge:
 ```bash
-pip install gentoo_update
+emerge --ask app-admin/gentoo_update
+```
+Because the project is in early stage of development it's not considered stable 
+and is masked by `~amd64`. To unmask it run:
+```bash
+echo 'app-admin/gentoo_update ~amd64' >> /etc/portage/package.accept_keywords/gentoo_update
+```
+
+Alternatively, updater can be installed with pip:
+```
+pip install gentoo_update --break-system-packages
 ```
 
 Here are some usage examples:
 * Basic security update
 ```bash
 gentoo-update
 ```
@@ -44,8 +55,8 @@
 * Full system update, show elogs and news
 ```bash
 gentoo-update --update-mode full --read-logs y --read-news y
 ```
 
 The detailed explanation of command flags can be found in `--help`.  
 Information on testing can be found in tests directory 
-[readme](gentoo_update/blob/main/tests/README.md)
+[readme](tests/README.md)
```

### Comparing `gentoo-update-0.1.2/setup.cfg` & `gentoo-update-0.1.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [metadata]
 name = gentoo-update
-version = 0.1.2
 description = Gentoo Linux updater
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Lab-Brat
 author_email = labbrat_social@pm.me
 url = https://github.com/Lab-Brat/gentoo_update
 license = MIT
```

