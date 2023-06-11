# Comparing `tmp/tconnectsync-0.9.3.tar.gz` & `tmp/tconnectsync-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tconnectsync-0.9.3.tar", last modified: Sat Feb  4 05:20:03 2023, max compression
+gzip compressed data, was "tconnectsync-0.9.4.tar", last modified: Sun Jun 11 04:32:06 2023, max compression
```

## Comparing `tconnectsync-0.9.3.tar` & `tconnectsync-0.9.4.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 05:20:03.961338 tconnectsync-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-02-04 05:20:03.961338 tconnectsync-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-04 05:20:03.961338 tconnectsync-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 05:20:03.957338 tconnectsync-0.9.3/tconnectsync/
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 05:20:03.957338 tconnectsync-0.9.3/tconnectsync/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/api/android.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/api/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/api/controliq.py
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/api/webui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/api/ws2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/autoupdate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 05:20:03.957338 tconnectsync-0.9.3/tconnectsync/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/domain/bolus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/domain/device_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/domain/therapy_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/domain/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/nightscout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 05:20:03.961338 tconnectsync-0.9.3/tconnectsync/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/parser/ciq_therapy_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/parser/nightscout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/parser/tconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/secret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 05:20:03.961338 tconnectsync-0.9.3/tconnectsync/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/sync/basal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/sync/bolus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/sync/cgm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/sync/iob.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/sync/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/sync/pump_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 05:20:03.961338 tconnectsync-0.9.3/tconnectsync/util/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/util/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-04 05:19:53.000000 tconnectsync-0.9.3/tconnectsync/util/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 05:20:03.961338 tconnectsync-0.9.3/tconnectsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-02-04 05:20:03.000000 tconnectsync-0.9.3/tconnectsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-02-04 05:20:03.000000 tconnectsync-0.9.3/tconnectsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 05:20:03.000000 tconnectsync-0.9.3/tconnectsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-04 05:20:03.000000 tconnectsync-0.9.3/tconnectsync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-04 05:20:03.000000 tconnectsync-0.9.3/tconnectsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-04 05:20:03.000000 tconnectsync-0.9.3/tconnectsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:32:06.003666 tconnectsync-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23738 2023-06-11 04:32:06.003666 tconnectsync-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23200 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-11 04:32:06.003666 tconnectsync-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:32:05.995666 tconnectsync-0.9.4/tconnectsync/
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:32:05.995666 tconnectsync-0.9.4/tconnectsync/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/api/android.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/api/controliq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/api/webui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/api/ws2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/autoupdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:32:05.995666 tconnectsync-0.9.4/tconnectsync/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/domain/bolus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/domain/device_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/domain/therapy_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/domain/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/nightscout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:32:05.999666 tconnectsync-0.9.4/tconnectsync/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/parser/ciq_therapy_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/parser/nightscout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/parser/tconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/secret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:32:05.999666 tconnectsync-0.9.4/tconnectsync/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/sync/basal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/sync/bolus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/sync/cgm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/sync/iob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/sync/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/sync/pump_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:32:05.999666 tconnectsync-0.9.4/tconnectsync/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/util/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tconnectsync/util/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:32:06.003666 tconnectsync-0.9.4/tconnectsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23738 2023-06-11 04:32:05.000000 tconnectsync-0.9.4/tconnectsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-11 04:32:05.000000 tconnectsync-0.9.4/tconnectsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 04:32:05.000000 tconnectsync-0.9.4/tconnectsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-11 04:32:05.000000 tconnectsync-0.9.4/tconnectsync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 04:32:05.000000 tconnectsync-0.9.4/tconnectsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 04:32:05.000000 tconnectsync-0.9.4/tconnectsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:32:06.003666 tconnectsync-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tests/test_autoupdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41692 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-11 04:31:52.000000 tconnectsync-0.9.4/tests/test_secret.py
```

### Comparing `tconnectsync-0.9.3/LICENSE.md` & `tconnectsync-0.9.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/PKG-INFO` & `tconnectsync-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tconnectsync
-Version: 0.9.3
+Version: 0.9.4
 Summary: Syncs Tandem t:connect pump data to Nightscout for the t:slim X2
 Home-page: https://github.com/jwoglom/tconnectsync
 Author: James Woglom
 Author-email: j@wogloms.net
 Project-URL: Bug Tracker, https://github.com/jwoglom/tconnectsync/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -133,29 +133,31 @@
 
 * **On MacOS:** Open Terminal. Install [Homebrew](https://brew.sh/), and then run `brew install python3`
 * **On Linux:** Follow your distribution's specific instructions.
   - For Debian/Ubuntu based distros, `sudo apt install python3 python3-pip`
   - For CentOS/Rocky Linux 8: 
     - `sudo dnf install python39-pip`
     - `sudo alternatives --set python /usr/bin/python3.9` 
-* **On Windows:** Install Ubuntu under the [Windows Subsystem for Linux](https://ubuntu.com/wsl).
-  Open the Ubuntu Terminal, then run `sudo apt install python3 python3-pip`.
-  Perform the remainder of the steps under the Ubuntu environment.
+* **On Windows:** 
+  - **With WSL:** Install Ubuntu under the [Windows Subsystem for Linux](https://ubuntu.com/wsl).
+    Open the Ubuntu Terminal, then run `sudo apt install python3 python3-pip`.
+    Perform the remainder of the steps under the Ubuntu environment.
+  - **Native:** Alternatively, you can run tconnectsync in native Windows with no modifications. However, this is less well-tested (open a GitHub issue if you experience any problems).
 
 Now install the `tconnectsync` package with pip:
 
 ```
 $ pip3 install tconnectsync
 ```
 To install into a user environment instead of system-wide for a more contained install:
 ````
 $ pip3 install --user tconnectsync
 ````
   - This will place the tconnectsync binary file at ``/home/<username>/.local/bin/tconnectsync``
-
+  - For non-WSL Windows, it will be in ``<PYTHON DIRECTORY>\Lib\site-packages\tconnectsync``
 
 If the pip3 command is not found, run `python3 -m pip install tconnectsync` instead.
 
 After this, you should be able to view tconnectsync's help with:
 ```
 $ tconnectsync --help
 usage: tconnectsync [-h] [--version] [--pretend] [-v] [--start-date START_DATE] [--end-date END_DATE] [--days DAYS] [--auto-update] [--check-login]
@@ -178,15 +180,15 @@
                         Specifies what data should be synchronized between tconnect and Nightscout.
 ```
 
 Move the `.env` file you created to the following folder:
 
 * **MacOS:** `/Users/<username>/.config/tconnectsync/.env`
 * **Linux:** `$HOME/.config/tconnectsync/.env`
-* **Windows:** `$HOME/.config/tconnectsync/.env` (inside WSL)
+* **Windows:** `$HOME/.config/tconnectsync/.env` (inside WSL) OR `C:\Users\<username>\.config\tconnectsync` (native Windows)
 
 ```
 $ tconnectsync --check-login
 ```
 
 If you receive no errors, then you can move on to the **Running Tconnectsync Continuously** section.
 
@@ -413,14 +415,28 @@
 An example of a user crontab `crontab -e` if not running system-wide, which runs every 15 minutes:
 ```
 */15 * * * * /path/to/tconnectsync/run.sh
 ```
 
 You can use one of the same `run.sh` files referenced above, but remove the `--auto-update` flag since you are handling the functionality for running the script periodically yourself.
 
+### For Native Windows 
+
+Create a batch file 'tconnectsync.bat' file containing:
+
+```
+python "C:\Users\<USERNAME>\AppData\Local\Programs\Python\<PYTHONVERSIONDIRECTORY>\Lib\site-packages\tconnectsync\main.py" --auto-update
+```
+
+If `python` does not exist in your path, specify the full path to `python.exe`.
+
+If main.py doesn't exist in `C:\Users\<USERNAME>\AppData\Local\Programs\Python\<PYTHONVERSIONDIRECTORY>\Lib\site-packages\tconnectsync\`, create it to match the copy in this repository.
+
+[Use Windows Task Scheduler](https://www.windowscentral.com/how-create-automated-task-using-task-scheduler-windows-10) to run this batch file on a scheduled basis.
+
 ## Tandem APIs
 
 This application utilizes three separate Tandem APIs for obtaining t:connect data, referenced here by the identifying part of their URLs:
 
 * [**controliq**](https://github.com/jwoglom/tconnectsync/blob/master/tconnectsync/api/controliq.py) - Contains Control:IQ related data, namely a timeline of all Basal events uploaded by the pump, separated by type (temp basals, algorithmically-updated basals, or profile-updated basals). Additionally includes CGM and Bolus data.
 * [**android**](https://github.com/jwoglom/tconnectsync/blob/master/tconnectsync/api/android.py) - Used internally by the t:connect Android app, these API endpoints were discovered by reverse-engineering the Android app. Most of the API endpoints are used for uploading pump data, and tconnectsync uses one endpoint which returns the most recent event ID uploaded by the pump, so we know when more data has been uploaded.
 * [**tconnectws2**](https://github.com/jwoglom/tconnectsync/blob/master/tconnectsync/api/ws2.py) - More legacy than the others, this seems to power the bulk of the main t:connect website. It is used as a last resort due to severe performance issues with this API (see https://github.com/jwoglom/tconnectsync/issues/43). We can use it to retrieve a CSV export of non-ControlIQ basal data, as well as bolus and IOB data. It is only used for bolus data as a fallback, and for pump-reported IOB data if requested. Full tracking of pump events also uses a limited version of this API.
```

### Comparing `tconnectsync-0.9.3/README.md` & `tconnectsync-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -118,29 +118,31 @@
 
 * **On MacOS:** Open Terminal. Install [Homebrew](https://brew.sh/), and then run `brew install python3`
 * **On Linux:** Follow your distribution's specific instructions.
   - For Debian/Ubuntu based distros, `sudo apt install python3 python3-pip`
   - For CentOS/Rocky Linux 8: 
     - `sudo dnf install python39-pip`
     - `sudo alternatives --set python /usr/bin/python3.9` 
-* **On Windows:** Install Ubuntu under the [Windows Subsystem for Linux](https://ubuntu.com/wsl).
-  Open the Ubuntu Terminal, then run `sudo apt install python3 python3-pip`.
-  Perform the remainder of the steps under the Ubuntu environment.
+* **On Windows:** 
+  - **With WSL:** Install Ubuntu under the [Windows Subsystem for Linux](https://ubuntu.com/wsl).
+    Open the Ubuntu Terminal, then run `sudo apt install python3 python3-pip`.
+    Perform the remainder of the steps under the Ubuntu environment.
+  - **Native:** Alternatively, you can run tconnectsync in native Windows with no modifications. However, this is less well-tested (open a GitHub issue if you experience any problems).
 
 Now install the `tconnectsync` package with pip:
 
 ```
 $ pip3 install tconnectsync
 ```
 To install into a user environment instead of system-wide for a more contained install:
 ````
 $ pip3 install --user tconnectsync
 ````
   - This will place the tconnectsync binary file at ``/home/<username>/.local/bin/tconnectsync``
-
+  - For non-WSL Windows, it will be in ``<PYTHON DIRECTORY>\Lib\site-packages\tconnectsync``
 
 If the pip3 command is not found, run `python3 -m pip install tconnectsync` instead.
 
 After this, you should be able to view tconnectsync's help with:
 ```
 $ tconnectsync --help
 usage: tconnectsync [-h] [--version] [--pretend] [-v] [--start-date START_DATE] [--end-date END_DATE] [--days DAYS] [--auto-update] [--check-login]
@@ -163,15 +165,15 @@
                         Specifies what data should be synchronized between tconnect and Nightscout.
 ```
 
 Move the `.env` file you created to the following folder:
 
 * **MacOS:** `/Users/<username>/.config/tconnectsync/.env`
 * **Linux:** `$HOME/.config/tconnectsync/.env`
-* **Windows:** `$HOME/.config/tconnectsync/.env` (inside WSL)
+* **Windows:** `$HOME/.config/tconnectsync/.env` (inside WSL) OR `C:\Users\<username>\.config\tconnectsync` (native Windows)
 
 ```
 $ tconnectsync --check-login
 ```
 
 If you receive no errors, then you can move on to the **Running Tconnectsync Continuously** section.
 
@@ -398,14 +400,28 @@
 An example of a user crontab `crontab -e` if not running system-wide, which runs every 15 minutes:
 ```
 */15 * * * * /path/to/tconnectsync/run.sh
 ```
 
 You can use one of the same `run.sh` files referenced above, but remove the `--auto-update` flag since you are handling the functionality for running the script periodically yourself.
 
+### For Native Windows 
+
+Create a batch file 'tconnectsync.bat' file containing:
+
+```
+python "C:\Users\<USERNAME>\AppData\Local\Programs\Python\<PYTHONVERSIONDIRECTORY>\Lib\site-packages\tconnectsync\main.py" --auto-update
+```
+
+If `python` does not exist in your path, specify the full path to `python.exe`.
+
+If main.py doesn't exist in `C:\Users\<USERNAME>\AppData\Local\Programs\Python\<PYTHONVERSIONDIRECTORY>\Lib\site-packages\tconnectsync\`, create it to match the copy in this repository.
+
+[Use Windows Task Scheduler](https://www.windowscentral.com/how-create-automated-task-using-task-scheduler-windows-10) to run this batch file on a scheduled basis.
+
 ## Tandem APIs
 
 This application utilizes three separate Tandem APIs for obtaining t:connect data, referenced here by the identifying part of their URLs:
 
 * [**controliq**](https://github.com/jwoglom/tconnectsync/blob/master/tconnectsync/api/controliq.py) - Contains Control:IQ related data, namely a timeline of all Basal events uploaded by the pump, separated by type (temp basals, algorithmically-updated basals, or profile-updated basals). Additionally includes CGM and Bolus data.
 * [**android**](https://github.com/jwoglom/tconnectsync/blob/master/tconnectsync/api/android.py) - Used internally by the t:connect Android app, these API endpoints were discovered by reverse-engineering the Android app. Most of the API endpoints are used for uploading pump data, and tconnectsync uses one endpoint which returns the most recent event ID uploaded by the pump, so we know when more data has been uploaded.
 * [**tconnectws2**](https://github.com/jwoglom/tconnectsync/blob/master/tconnectsync/api/ws2.py) - More legacy than the others, this seems to power the bulk of the main t:connect website. It is used as a last resort due to severe performance issues with this API (see https://github.com/jwoglom/tconnectsync/issues/43). We can use it to retrieve a CSV export of non-ControlIQ basal data, as well as bolus and IOB data. It is only used for bolus data as a fallback, and for pump-reported IOB data if requested. Full tracking of pump events also uses a limited version of this API.
```

### Comparing `tconnectsync-0.9.3/setup.cfg` & `tconnectsync-0.9.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tconnectsync
-version = 0.9.3
+version = 0.9.4
 author = James Woglom
 author_email = j@wogloms.net
 description = Syncs Tandem t:connect pump data to Nightscout for the t:slim X2
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jwoglom/tconnectsync
 project_urls =
```

### Comparing `tconnectsync-0.9.3/tconnectsync/__init__.py` & `tconnectsync-0.9.4/tconnectsync/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 
 try:
     from .secret import (
         TCONNECT_EMAIL,
         TCONNECT_PASSWORD,
         NS_URL,
         NS_SECRET,
-        NS_SKIP_TLS_VERIFY
+        NS_SKIP_TLS_VERIFY,
+        PUMP_SERIAL_NUMBER
     )
     from . import secret
-except Exception:
-    print('Unable to read secret.py')
+except Exception as e:
+    print('Unable to read secrets from secret.py', e)
     sys.exit(1)
 
 
 try:
     __version__ = pkg_resources.require("tconnectsync")[0].version
 except Exception:
     __version__ = "UNKNOWN"
@@ -69,14 +70,24 @@
     else:
         time_end = datetime.datetime.now()
         time_start = time_end - datetime.timedelta(days=args.days)
 
     if time_end < time_start:
         raise Exception('time_start must be before time_end')
 
+
+    if TCONNECT_EMAIL == 'email@email.com':
+        logging.warn('NO USERNAME WAS PROVIDED. Ensure you have set TCONNECT_EMAIL appropriately.')
+    if TCONNECT_PASSWORD == 'password':
+        logging.warn('NO PASSWORD WAS PROVIDED. Ensure you have set TCONNECT_PASSWORD appropriately.')
+    if NS_URL == 'https://yournightscouturl/':
+        logging.warn('NO NIGHTSCOUT URL WAS PROVIDED. Ensure your have set NS_URL appropriately.')
+    if PUMP_SERIAL_NUMBER == '11111111':
+        logging.warn('NO PUMP SERIAL NUMBER WAS PROVIDED. Ensure you have set PUMP_SERIAL_NUMBER appropriately.')
+
     tconnect = TConnectApi(TCONNECT_EMAIL, TCONNECT_PASSWORD)
 
     nightscout = NightscoutApi(NS_URL, NS_SECRET, NS_SKIP_TLS_VERIFY)
 
     if args.check_login:
         return check_login(tconnect, time_start, time_end)
```

### Comparing `tconnectsync-0.9.3/tconnectsync/api/__init__.py` & `tconnectsync-0.9.4/tconnectsync/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/api/android.py` & `tconnectsync-0.9.4/tconnectsync/api/android.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/api/common.py` & `tconnectsync-0.9.4/tconnectsync/api/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,11 +123,11 @@
         ranges.append((cur_s, end))
     
     return ranges
 
 class ApiException(Exception):
     def __init__(self, status_code, text, *args, **kwargs):
         self.status_code = status_code
-        super().__init__('%s (HTTP %s)' % (text, status_code), *args, **kwargs)
+        super().__init__('%s%s' % (text, ' (HTTP %s)' % status_code if status_code else ''), *args, **kwargs)
 
 class ApiLoginException(ApiException):
     pass
```

### Comparing `tconnectsync-0.9.3/tconnectsync/api/controliq.py` & `tconnectsync-0.9.4/tconnectsync/api/controliq.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import urllib
 import arrow
 import time
 import logging
 
 from bs4 import BeautifulSoup
 
-from ..util import timeago
+from ..util import timeago, cap_length
 from .common import parse_date, base_headers, base_session, ApiException, ApiLoginException
 
 logger = logging.getLogger(__name__)
 
 class ControlIQApi:
     BASE_URL = 'https://tdcservices.tandemdiabetes.com/'
     LOGIN_URL = 'https://tconnect.tandemdiabetes.com/login.aspx?ReturnUrl=%2f'
 
-    LAST_CONFIRMED_SOFTWARE_VERSION = 't:connect 7.14.0.1'
+    LAST_CONFIRMED_SOFTWARE_VERSION = 't:connect 7.15.0.1'
 
     userGuid = None
     accessToken = None
     accessTokenExpiresAt = None
     tconnect_software_ver = None
 
     def __init__(self, email, password):
@@ -30,20 +30,28 @@
         logger.info("Logging in to ControlIQApi...")
         with base_session() as s:
             initial = s.get(self.LOGIN_URL, headers=base_headers())
             soup = BeautifulSoup(initial.content, features='lxml')
             data = self._build_login_data(email, password, soup)
 
             req = s.post(self.LOGIN_URL, data=data, headers={'Referer': self.LOGIN_URL, **base_headers()}, allow_redirects=False)
+            # HTTP 200 is reported when credentials are incorrect
+            if req.status_code == 200:
+                login_error = self._find_login_error(req.text)
+                if not login_error:
+                    login_error = 'Check your login credentials.'
+                raise ApiLoginException(None, 'Error logging in to t:connect: %s' % login_error)
+
             if req.status_code != 302:
-                raise ApiLoginException(req.status_code, 'Error logging in to t:connect. Check your login credentials.')
+                raise ApiLoginException(req.status_code, 'Error logging in to t:connect')
 
 
             fwd = s.post(urllib.parse.urljoin(self.LOGIN_URL, req.headers['Location']), cookies=req.cookies, headers=base_headers())
             if fwd.status_code != 200:
+                logger.warn("Received non-HTTP 200: %s" % req.text)
                 raise ApiException(fwd.status_code, 'Error retrieving t:connect login cookies.')
 
             self.userGuid = req.cookies['UserGUID']
             self.accessToken = req.cookies['accessToken']
             self.accessTokenExpiresAt = req.cookies['accessTokenExpiresAt']
             logger.info("Logged in to ControlIQApi successfully (expiration: %s, %s)" % (self.accessTokenExpiresAt, timeago(self.accessTokenExpiresAt)))
             self.loginSession = s
@@ -75,14 +83,22 @@
             "__EVENTVALIDATION": soup.select_one("#__EVENTVALIDATION")["value"],
             "ctl00$ContentBody$LoginControl$txtLoginEmailAddress": email,
             "txtLoginEmailAddress_ClientState": '{"enabled":true,"emptyMessage":"","validationText":"%s","valueAsString":"%s","lastSetTextBoxValue":"%s"}' % (email, email, email),
             "ctl00$ContentBody$LoginControl$txtLoginPassword": password,
             "txtLoginPassword_ClientState": '{"enabled":true,"emptyMessage":"","validationText":"%s","valueAsString":"%s","lastSetTextBoxValue":"%s"}' % (password, password, password)
         }
 
+    def _find_login_error(self, text):
+        try:
+            soup = BeautifulSoup(text, features='lxml')
+            notice_error = soup.select_one(".notice_error").text.strip()
+            return notice_error
+        except Exception:
+            return None
+
     def needs_relogin(self):
         diff = (arrow.get(self.accessTokenExpiresAt) - arrow.get())
         return (diff.seconds <= 5 * 60)
 
     def api_headers(self):
         if not self.accessToken:
             raise Exception('No access token provided')
```

### Comparing `tconnectsync-0.9.3/tconnectsync/api/webui.py` & `tconnectsync-0.9.4/tconnectsync/api/webui.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/api/ws2.py` & `tconnectsync-0.9.4/tconnectsync/api/ws2.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/autoupdate.py` & `tconnectsync-0.9.4/tconnectsync/autoupdate.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/check.py` & `tconnectsync-0.9.4/tconnectsync/check.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/domain/bolus.py` & `tconnectsync-0.9.4/tconnectsync/domain/bolus.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/domain/device_settings.py` & `tconnectsync-0.9.4/tconnectsync/domain/device_settings.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/domain/therapy_event.py` & `tconnectsync-0.9.4/tconnectsync/domain/therapy_event.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/domain/utility.py` & `tconnectsync-0.9.4/tconnectsync/domain/utility.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/features.py` & `tconnectsync-0.9.4/tconnectsync/features.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/nightscout.py` & `tconnectsync-0.9.4/tconnectsync/nightscout.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/parser/ciq_therapy_events.py` & `tconnectsync-0.9.4/tconnectsync/parser/ciq_therapy_events.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/parser/nightscout.py` & `tconnectsync-0.9.4/tconnectsync/parser/nightscout.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/parser/tconnect.py` & `tconnectsync-0.9.4/tconnectsync/parser/tconnect.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/process.py` & `tconnectsync-0.9.4/tconnectsync/process.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/secret.py` & `tconnectsync-0.9.4/tconnectsync/secret.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/sync/basal.py` & `tconnectsync-0.9.4/tconnectsync/sync/basal.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/sync/bolus.py` & `tconnectsync-0.9.4/tconnectsync/sync/bolus.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/sync/cgm.py` & `tconnectsync-0.9.4/tconnectsync/sync/cgm.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/sync/iob.py` & `tconnectsync-0.9.4/tconnectsync/sync/iob.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/sync/profile.py` & `tconnectsync-0.9.4/tconnectsync/sync/profile.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/sync/pump_events.py` & `tconnectsync-0.9.4/tconnectsync/sync/pump_events.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync/util/__init__.py` & `tconnectsync-0.9.4/tconnectsync/util/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,8 +24,13 @@
     if suffix and input_string.endswith(suffix):
         return input_string[:-len(suffix)]
     return input_string
 
 def removeprefix(input_string, prefix):
     if prefix and input_string.startswith(prefix):
         return input_string[len(prefix):]
-    return input_string
+    return input_string
+
+def cap_length(text, maxlen):
+    if not text or len(text) <= maxlen:
+        return text
+    return '%s[...]%s' % (text[:maxlen//2], text[maxlen//-2:])
```

### Comparing `tconnectsync-0.9.3/tconnectsync/util/cli.py` & `tconnectsync-0.9.4/tconnectsync/util/cli.py`

 * *Files identical despite different names*

### Comparing `tconnectsync-0.9.3/tconnectsync.egg-info/PKG-INFO` & `tconnectsync-0.9.4/tconnectsync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tconnectsync
-Version: 0.9.3
+Version: 0.9.4
 Summary: Syncs Tandem t:connect pump data to Nightscout for the t:slim X2
 Home-page: https://github.com/jwoglom/tconnectsync
 Author: James Woglom
 Author-email: j@wogloms.net
 Project-URL: Bug Tracker, https://github.com/jwoglom/tconnectsync/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -133,29 +133,31 @@
 
 * **On MacOS:** Open Terminal. Install [Homebrew](https://brew.sh/), and then run `brew install python3`
 * **On Linux:** Follow your distribution's specific instructions.
   - For Debian/Ubuntu based distros, `sudo apt install python3 python3-pip`
   - For CentOS/Rocky Linux 8: 
     - `sudo dnf install python39-pip`
     - `sudo alternatives --set python /usr/bin/python3.9` 
-* **On Windows:** Install Ubuntu under the [Windows Subsystem for Linux](https://ubuntu.com/wsl).
-  Open the Ubuntu Terminal, then run `sudo apt install python3 python3-pip`.
-  Perform the remainder of the steps under the Ubuntu environment.
+* **On Windows:** 
+  - **With WSL:** Install Ubuntu under the [Windows Subsystem for Linux](https://ubuntu.com/wsl).
+    Open the Ubuntu Terminal, then run `sudo apt install python3 python3-pip`.
+    Perform the remainder of the steps under the Ubuntu environment.
+  - **Native:** Alternatively, you can run tconnectsync in native Windows with no modifications. However, this is less well-tested (open a GitHub issue if you experience any problems).
 
 Now install the `tconnectsync` package with pip:
 
 ```
 $ pip3 install tconnectsync
 ```
 To install into a user environment instead of system-wide for a more contained install:
 ````
 $ pip3 install --user tconnectsync
 ````
   - This will place the tconnectsync binary file at ``/home/<username>/.local/bin/tconnectsync``
-
+  - For non-WSL Windows, it will be in ``<PYTHON DIRECTORY>\Lib\site-packages\tconnectsync``
 
 If the pip3 command is not found, run `python3 -m pip install tconnectsync` instead.
 
 After this, you should be able to view tconnectsync's help with:
 ```
 $ tconnectsync --help
 usage: tconnectsync [-h] [--version] [--pretend] [-v] [--start-date START_DATE] [--end-date END_DATE] [--days DAYS] [--auto-update] [--check-login]
@@ -178,15 +180,15 @@
                         Specifies what data should be synchronized between tconnect and Nightscout.
 ```
 
 Move the `.env` file you created to the following folder:
 
 * **MacOS:** `/Users/<username>/.config/tconnectsync/.env`
 * **Linux:** `$HOME/.config/tconnectsync/.env`
-* **Windows:** `$HOME/.config/tconnectsync/.env` (inside WSL)
+* **Windows:** `$HOME/.config/tconnectsync/.env` (inside WSL) OR `C:\Users\<username>\.config\tconnectsync` (native Windows)
 
 ```
 $ tconnectsync --check-login
 ```
 
 If you receive no errors, then you can move on to the **Running Tconnectsync Continuously** section.
 
@@ -413,14 +415,28 @@
 An example of a user crontab `crontab -e` if not running system-wide, which runs every 15 minutes:
 ```
 */15 * * * * /path/to/tconnectsync/run.sh
 ```
 
 You can use one of the same `run.sh` files referenced above, but remove the `--auto-update` flag since you are handling the functionality for running the script periodically yourself.
 
+### For Native Windows 
+
+Create a batch file 'tconnectsync.bat' file containing:
+
+```
+python "C:\Users\<USERNAME>\AppData\Local\Programs\Python\<PYTHONVERSIONDIRECTORY>\Lib\site-packages\tconnectsync\main.py" --auto-update
+```
+
+If `python` does not exist in your path, specify the full path to `python.exe`.
+
+If main.py doesn't exist in `C:\Users\<USERNAME>\AppData\Local\Programs\Python\<PYTHONVERSIONDIRECTORY>\Lib\site-packages\tconnectsync\`, create it to match the copy in this repository.
+
+[Use Windows Task Scheduler](https://www.windowscentral.com/how-create-automated-task-using-task-scheduler-windows-10) to run this batch file on a scheduled basis.
+
 ## Tandem APIs
 
 This application utilizes three separate Tandem APIs for obtaining t:connect data, referenced here by the identifying part of their URLs:
 
 * [**controliq**](https://github.com/jwoglom/tconnectsync/blob/master/tconnectsync/api/controliq.py) - Contains Control:IQ related data, namely a timeline of all Basal events uploaded by the pump, separated by type (temp basals, algorithmically-updated basals, or profile-updated basals). Additionally includes CGM and Bolus data.
 * [**android**](https://github.com/jwoglom/tconnectsync/blob/master/tconnectsync/api/android.py) - Used internally by the t:connect Android app, these API endpoints were discovered by reverse-engineering the Android app. Most of the API endpoints are used for uploading pump data, and tconnectsync uses one endpoint which returns the most recent event ID uploaded by the pump, so we know when more data has been uploaded.
 * [**tconnectws2**](https://github.com/jwoglom/tconnectsync/blob/master/tconnectsync/api/ws2.py) - More legacy than the others, this seems to power the bulk of the main t:connect website. It is used as a last resort due to severe performance issues with this API (see https://github.com/jwoglom/tconnectsync/issues/43). We can use it to retrieve a CSV export of non-ControlIQ basal data, as well as bolus and IOB data. It is only used for bolus data as a fallback, and for pump-reported IOB data if requested. Full tracking of pump events also uses a limited version of this API.
```

### Comparing `tconnectsync-0.9.3/tconnectsync.egg-info/SOURCES.txt` & `tconnectsync-0.9.4/tconnectsync.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -36,8 +36,11 @@
 ./tconnectsync/util/cli.py
 ./tconnectsync/util/constants.py
 tconnectsync.egg-info/PKG-INFO
 tconnectsync.egg-info/SOURCES.txt
 tconnectsync.egg-info/dependency_links.txt
 tconnectsync.egg-info/entry_points.txt
 tconnectsync.egg-info/requires.txt
-tconnectsync.egg-info/top_level.txt
+tconnectsync.egg-info/top_level.txt
+tests/test_autoupdate.py
+tests/test_process.py
+tests/test_secret.py
```

