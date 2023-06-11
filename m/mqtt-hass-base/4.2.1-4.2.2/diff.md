# Comparing `tmp/mqtt-hass-base-4.2.1.tar.gz` & `tmp/mqtt-hass-base-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt-hass-base-4.2.1.tar", last modified: Fri Mar 31 16:53:56 2023, max compression
+gzip compressed data, was "mqtt-hass-base-4.2.2.tar", last modified: Sun Jun 11 02:42:28 2023, max compression
```

## Comparing `mqtt-hass-base-4.2.1.tar` & `mqtt-hass-base-4.2.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 16:53:56.071191 mqtt-hass-base-4.2.1/
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     1830 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3322 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1015 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    19948 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)    11344 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1372 2023-03-31 16:53:56.071191 mqtt-hass-base-4.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)    34804 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt-hass-base.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 16:53:56.067191 mqtt-hass-base-4.2.1/mqtt_hass_base/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/const.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/daemon.py
--rw-rw-rw-   0 root         (0) root         (0)     8877 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/device.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 16:53:56.067191 mqtt-hass-base-4.2.1/mqtt_hass_base/entity/
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/entity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5183 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/entity/binarysensor.py
--rw-rw-rw-   0 root         (0) root         (0)     3980 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/entity/button.py
--rw-rw-rw-   0 root         (0) root         (0)     6983 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/entity/common.py
--rw-rw-rw-   0 root         (0) root         (0)     6104 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/entity/light.py
--rw-rw-rw-   0 root         (0) root         (0)     5045 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/entity/lock.py
--rw-rw-rw-   0 root         (0) root         (0)     6067 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/entity/number.py
--rw-rw-rw-   0 root         (0) root         (0)     4367 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/entity/sensor.py
--rw-rw-rw-   0 root         (0) root         (0)     4870 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/entity/switch.py
--rw-rw-rw-   0 root         (0) root         (0)     7290 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/entity/vacuum.py
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/error.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/mqtt_hass_base/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 16:53:56.067191 mqtt-hass-base-4.2.1/mqtt_hass_base.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1372 2023-03-31 16:53:56.000000 mqtt-hass-base-4.2.1/mqtt_hass_base.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1219 2023-03-31 16:53:56.000000 mqtt-hass-base-4.2.1/mqtt_hass_base.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 16:53:56.000000 mqtt-hass-base-4.2.1/mqtt_hass_base.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-03-31 16:53:56.000000 mqtt-hass-base-4.2.1/mqtt_hass_base.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-03-31 16:53:56.000000 mqtt-hass-base-4.2.1/mqtt_hass_base.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1358 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2600 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/renovate.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 16:53:56.067191 mqtt-hass-base-4.2.1/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/scripts/run-mqtt-docker-for-tests.sh
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-03-31 16:53:56.071191 mqtt-hass-base-4.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 16:53:56.071191 mqtt-hass-base-4.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    11443 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/tests/test_daemon.py
--rw-rw-rw-   0 root         (0) root         (0)     5978 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/tests/test_device.py
--rw-rw-rw-   0 root         (0) root         (0)     5103 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/tests/test_entities_binsensor.py
--rw-rw-rw-   0 root         (0) root         (0)     5223 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/tests/test_entities_button.py
--rw-rw-rw-   0 root         (0) root         (0)     3265 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/tests/test_entities_common.py
--rw-rw-rw-   0 root         (0) root         (0)     6256 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/tests/test_entities_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4518 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/tests/test_entities_lock.py
--rw-rw-rw-   0 root         (0) root         (0)     3957 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/tests/test_entities_number.py
--rw-rw-rw-   0 root         (0) root         (0)     4006 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/tests/test_entities_sensor.py
--rw-rw-rw-   0 root         (0) root         (0)     5932 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/tests/test_entities_switch.py
--rw-rw-rw-   0 root         (0) root         (0)     5010 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/tests/test_entities_vacuum.py
--rw-rw-rw-   0 root         (0) root         (0)     2126 2023-03-31 16:53:34.000000 mqtt-hass-base-4.2.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 02:42:28.173817 mqtt-hass-base-4.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3322 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    19948 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-06-11 02:42:28.173817 mqtt-hass-base-4.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    34804 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt-hass-base.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 02:42:28.173817 mqtt-hass-base-4.2.2/mqtt_hass_base/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/const.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/daemon.py
+-rw-rw-rw-   0 root         (0) root         (0)     8877 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/device.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 02:42:28.173817 mqtt-hass-base-4.2.2/mqtt_hass_base/entity/
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/entity/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5183 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/entity/binarysensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3980 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/entity/button.py
+-rw-rw-rw-   0 root         (0) root         (0)     6983 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/entity/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     6104 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/entity/light.py
+-rw-rw-rw-   0 root         (0) root         (0)     5045 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/entity/lock.py
+-rw-rw-rw-   0 root         (0) root         (0)     6067 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/entity/number.py
+-rw-rw-rw-   0 root         (0) root         (0)     4367 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/entity/sensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4870 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/entity/switch.py
+-rw-rw-rw-   0 root         (0) root         (0)     7290 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/entity/vacuum.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/error.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/mqtt_hass_base/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 02:42:28.173817 mqtt-hass-base-4.2.2/mqtt_hass_base.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-06-11 02:42:28.000000 mqtt-hass-base-4.2.2/mqtt_hass_base.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-06-11 02:42:28.000000 mqtt-hass-base-4.2.2/mqtt_hass_base.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 02:42:28.000000 mqtt-hass-base-4.2.2/mqtt_hass_base.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-11 02:42:28.000000 mqtt-hass-base-4.2.2/mqtt_hass_base.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-11 02:42:28.000000 mqtt-hass-base-4.2.2/mqtt_hass_base.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/renovate.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 02:42:28.173817 mqtt-hass-base-4.2.2/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/scripts/run-mqtt-docker-for-tests.sh
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-06-11 02:42:28.173817 mqtt-hass-base-4.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 02:42:28.173817 mqtt-hass-base-4.2.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    11443 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/tests/test_daemon.py
+-rw-rw-rw-   0 root         (0) root         (0)     5978 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/tests/test_device.py
+-rw-rw-rw-   0 root         (0) root         (0)     5103 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/tests/test_entities_binsensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5223 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/tests/test_entities_button.py
+-rw-rw-rw-   0 root         (0) root         (0)     3265 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/tests/test_entities_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     6256 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/tests/test_entities_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4518 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/tests/test_entities_lock.py
+-rw-rw-rw-   0 root         (0) root         (0)     3957 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/tests/test_entities_number.py
+-rw-rw-rw-   0 root         (0) root         (0)     4006 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/tests/test_entities_sensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5932 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/tests/test_entities_switch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5010 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/tests/test_entities_vacuum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2126 2023-06-11 02:42:21.000000 mqtt-hass-base-4.2.2/tox.ini
```

### Comparing `mqtt-hass-base-4.2.1/.gitignore` & `mqtt-hass-base-4.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/.gitlab-ci.yml` & `mqtt-hass-base-4.2.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/.pre-commit-config.yaml` & `mqtt-hass-base-4.2.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/PyCQA/flake8/
-  rev: 5.0.4
+  rev: 6.0.0
   hooks:
   - id: flake8
     additional_dependencies: [flake8-docstrings]
 
 - repo: https://github.com/PyCQA/isort
   rev: 5.12.0
   hooks:
@@ -38,8 +38,8 @@
   hooks:
   - id: mypy
     args: [--strict, --pretty, --show-error-codes]
     additional_dependencies:
       - "asyncio_mqtt==0.16.1"
       - "pytest-asyncio==0.21.0"
       - "types-paho-mqtt==1.6.0.6"
-      - "homeassistant-stubs==2023.3.6"
+      - "homeassistant-stubs==2023.6.1"
```

### Comparing `mqtt-hass-base-4.2.1/.pylintrc` & `mqtt-hass-base-4.2.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/LICENSE.txt` & `mqtt-hass-base-4.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/PKG-INFO` & `mqtt-hass-base-4.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-hass-base
-Version: 4.2.1
+Version: 4.2.2
 Summary: Bases to build mqtt daemon compatible with Home Assistant
 Home-page: https://gitlab.com/ttblt-oss/hass/mqtt-hass-base
 Author-email: Thibault Cohen <titilambert@gmail.com>
 License: Apache-2.0
 Project-URL: Source Code, https://gitlab.com/ttblt-oss/hass/mqtt_hass_base
 Project-URL: Bug Reports, https://gitlab.com/ttblt-oss/hass/mqtt-hass-base/-/issues
 Project-URL: Home-page, https://gitlab.com/ttblt-oss/hass/mqtt_hass_base
```

### Comparing `mqtt-hass-base-4.2.1/README.md` & `mqtt-hass-base-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/mqtt-hass-base.png` & `mqtt-hass-base-4.2.2/mqtt-hass-base.png`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/mqtt_hass_base/daemon.py` & `mqtt-hass-base-4.2.2/mqtt_hass_base/daemon.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/mqtt_hass_base/device.py` & `mqtt-hass-base-4.2.2/mqtt_hass_base/device.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/mqtt_hass_base/entity/__init__.py` & `mqtt-hass-base-4.2.2/mqtt_hass_base/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/mqtt_hass_base/entity/binarysensor.py` & `mqtt-hass-base-4.2.2/mqtt_hass_base/entity/binarysensor.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/mqtt_hass_base/entity/button.py` & `mqtt-hass-base-4.2.2/mqtt_hass_base/entity/button.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/mqtt_hass_base/entity/common.py` & `mqtt-hass-base-4.2.2/mqtt_hass_base/entity/common.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/mqtt_hass_base/entity/light.py` & `mqtt-hass-base-4.2.2/mqtt_hass_base/entity/light.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/mqtt_hass_base/entity/lock.py` & `mqtt-hass-base-4.2.2/mqtt_hass_base/entity/lock.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/mqtt_hass_base/entity/number.py` & `mqtt-hass-base-4.2.2/mqtt_hass_base/entity/number.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/mqtt_hass_base/entity/sensor.py` & `mqtt-hass-base-4.2.2/mqtt_hass_base/entity/sensor.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/mqtt_hass_base/entity/switch.py` & `mqtt-hass-base-4.2.2/mqtt_hass_base/entity/switch.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/mqtt_hass_base/entity/vacuum.py` & `mqtt-hass-base-4.2.2/mqtt_hass_base/entity/vacuum.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/mqtt_hass_base.egg-info/PKG-INFO` & `mqtt-hass-base-4.2.2/mqtt_hass_base.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-hass-base
-Version: 4.2.1
+Version: 4.2.2
 Summary: Bases to build mqtt daemon compatible with Home Assistant
 Home-page: https://gitlab.com/ttblt-oss/hass/mqtt-hass-base
 Author-email: Thibault Cohen <titilambert@gmail.com>
 License: Apache-2.0
 Project-URL: Source Code, https://gitlab.com/ttblt-oss/hass/mqtt_hass_base
 Project-URL: Bug Reports, https://gitlab.com/ttblt-oss/hass/mqtt-hass-base/-/issues
 Project-URL: Home-page, https://gitlab.com/ttblt-oss/hass/mqtt_hass_base
```

### Comparing `mqtt-hass-base-4.2.1/mqtt_hass_base.egg-info/SOURCES.txt` & `mqtt-hass-base-4.2.2/mqtt_hass_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/pyproject.toml` & `mqtt-hass-base-4.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/renovate.json` & `mqtt-hass-base-4.2.2/renovate.json`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/tests/test_daemon.py` & `mqtt-hass-base-4.2.2/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/tests/test_device.py` & `mqtt-hass-base-4.2.2/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/tests/test_entities_binsensor.py` & `mqtt-hass-base-4.2.2/tests/test_entities_binsensor.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/tests/test_entities_button.py` & `mqtt-hass-base-4.2.2/tests/test_entities_button.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/tests/test_entities_common.py` & `mqtt-hass-base-4.2.2/tests/test_entities_common.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/tests/test_entities_light.py` & `mqtt-hass-base-4.2.2/tests/test_entities_light.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/tests/test_entities_lock.py` & `mqtt-hass-base-4.2.2/tests/test_entities_lock.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/tests/test_entities_number.py` & `mqtt-hass-base-4.2.2/tests/test_entities_number.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/tests/test_entities_sensor.py` & `mqtt-hass-base-4.2.2/tests/test_entities_sensor.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/tests/test_entities_switch.py` & `mqtt-hass-base-4.2.2/tests/test_entities_switch.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/tests/test_entities_vacuum.py` & `mqtt-hass-base-4.2.2/tests/test_entities_vacuum.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.1/tox.ini` & `mqtt-hass-base-4.2.2/tox.ini`

 * *Files identical despite different names*

