# Comparing `tmp/circuitpython-mag-cal-1.2.2.tar.gz` & `tmp/circuitpython-mag-cal-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-mag-cal-1.2.2.tar", last modified: Sun Jun  4 12:39:19 2023, max compression
+gzip compressed data, was "circuitpython-mag-cal-1.3.0.tar", last modified: Sun Jun 11 14:08:05 2023, max compression
```

## Comparing `circuitpython-mag-cal-1.2.2.tar` & `circuitpython-mag-cal-1.3.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:39:19.325937 circuitpython-mag-cal-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:39:19.317937 circuitpython-mag-cal-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:39:19.317937 circuitpython-mag-cal-1.2.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:39:19.317937 circuitpython-mag-cal-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:39:19.317937 circuitpython-mag-cal-1.2.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-04 12:39:19.325937 circuitpython-mag-cal-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:39:19.317937 circuitpython-mag-cal-1.2.2/circuitpython_mag_cal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-04 12:39:19.000000 circuitpython-mag-cal-1.2.2/circuitpython_mag_cal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-04 12:39:19.000000 circuitpython-mag-cal-1.2.2/circuitpython_mag_cal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:39:19.000000 circuitpython-mag-cal-1.2.2/circuitpython_mag_cal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-04 12:39:19.000000 circuitpython-mag-cal-1.2.2/circuitpython_mag_cal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-04 12:39:19.000000 circuitpython-mag-cal-1.2.2/circuitpython_mag_cal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:39:19.321937 circuitpython-mag-cal-1.2.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:39:19.321937 circuitpython-mag-cal-1.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/docs/howto.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/docs/howto.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:39:19.321937 circuitpython-mag-cal-1.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-04 12:39:11.000000 circuitpython-mag-cal-1.2.2/examples/mag_cal_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:39:19.321937 circuitpython-mag-cal-1.2.2/mag_cal/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-04 12:39:11.000000 circuitpython-mag-cal-1.2.2/mag_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-04 12:39:11.000000 circuitpython-mag-cal-1.2.2/mag_cal/axes.py
--rw-r--r--   0 runner    (1001) docker     (123)    29838 2023-06-04 12:39:11.000000 circuitpython-mag-cal-1.2.2/mag_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-04 12:39:11.000000 circuitpython-mag-cal-1.2.2/mag_cal/lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-06-04 12:39:11.000000 circuitpython-mag-cal-1.2.2/mag_cal/nm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-04 12:39:11.000000 circuitpython-mag-cal-1.2.2/mag_cal/rbf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-06-04 12:39:11.000000 circuitpython-mag-cal-1.2.2/mag_cal/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-04 12:39:11.000000 circuitpython-mag-cal-1.2.2/mag_cal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-04 12:39:11.000000 circuitpython-mag-cal-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 12:39:19.325937 circuitpython-mag-cal-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:39:19.321937 circuitpython-mag-cal-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:39:11.000000 circuitpython-mag-cal-1.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:39:19.317937 circuitpython-mag-cal-1.2.2/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:39:19.325937 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/ab.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/ab.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/ai.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/ai.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/bh.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/bh.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/bi.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/bi.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/ee.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/ee.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/fb.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/fb.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/hj.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/hj.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/hj2.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/hj2.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/jd.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 12:39:00.000000 circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/jd.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-04 12:39:11.000000 circuitpython-mag-cal-1.2.2/tests/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-06-04 12:39:11.000000 circuitpython-mag-cal-1.2.2/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-04 12:39:11.000000 circuitpython-mag-cal-1.2.2/tests/test_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:08:05.718836 circuitpython-mag-cal-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:08:05.702835 circuitpython-mag-cal-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:08:05.702835 circuitpython-mag-cal-1.3.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:08:05.702835 circuitpython-mag-cal-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:08:05.706835 circuitpython-mag-cal-1.3.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-11 14:08:05.718836 circuitpython-mag-cal-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:08:05.706835 circuitpython-mag-cal-1.3.0/circuitpython_mag_cal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-11 14:08:05.000000 circuitpython-mag-cal-1.3.0/circuitpython_mag_cal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-11 14:08:05.000000 circuitpython-mag-cal-1.3.0/circuitpython_mag_cal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 14:08:05.000000 circuitpython-mag-cal-1.3.0/circuitpython_mag_cal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-11 14:08:05.000000 circuitpython-mag-cal-1.3.0/circuitpython_mag_cal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 14:08:05.000000 circuitpython-mag-cal-1.3.0/circuitpython_mag_cal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:08:05.710836 circuitpython-mag-cal-1.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:08:05.710836 circuitpython-mag-cal-1.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/docs/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/docs/howto.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:08:05.710836 circuitpython-mag-cal-1.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-11 14:07:57.000000 circuitpython-mag-cal-1.3.0/examples/mag_cal_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:08:05.710836 circuitpython-mag-cal-1.3.0/mag_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-11 14:07:57.000000 circuitpython-mag-cal-1.3.0/mag_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-11 14:07:57.000000 circuitpython-mag-cal-1.3.0/mag_cal/axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30888 2023-06-11 14:07:57.000000 circuitpython-mag-cal-1.3.0/mag_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-11 14:07:57.000000 circuitpython-mag-cal-1.3.0/mag_cal/lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-06-11 14:07:57.000000 circuitpython-mag-cal-1.3.0/mag_cal/nm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-11 14:07:57.000000 circuitpython-mag-cal-1.3.0/mag_cal/rbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-06-11 14:07:57.000000 circuitpython-mag-cal-1.3.0/mag_cal/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-11 14:07:57.000000 circuitpython-mag-cal-1.3.0/mag_cal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-11 14:07:57.000000 circuitpython-mag-cal-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 14:08:05.718836 circuitpython-mag-cal-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:08:05.710836 circuitpython-mag-cal-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 14:07:57.000000 circuitpython-mag-cal-1.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:08:05.702835 circuitpython-mag-cal-1.3.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:08:05.714836 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/ab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/ab.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/ai.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/ai.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/bh.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/bh.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/bi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/bi.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/ee.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/ee.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/fb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/fb.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/hj.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/hj.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/hj2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/hj2.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/jd.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-11 14:07:46.000000 circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/jd.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-11 14:07:57.000000 circuitpython-mag-cal-1.3.0/tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-11 14:07:57.000000 circuitpython-mag-cal-1.3.0/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-11 14:07:57.000000 circuitpython-mag-cal-1.3.0/tests/test_sensor.py
```

### Comparing `circuitpython-mag-cal-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-mag-cal-1.3.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/.gitignore` & `circuitpython-mag-cal-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/.pre-commit-config.yaml` & `circuitpython-mag-cal-1.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/.pylintrc` & `circuitpython-mag-cal-1.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/CODE_OF_CONDUCT.md` & `circuitpython-mag-cal-1.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/LICENSE` & `circuitpython-mag-cal-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/LICENSES/CC-BY-4.0.txt` & `circuitpython-mag-cal-1.3.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/LICENSES/MIT.txt` & `circuitpython-mag-cal-1.3.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/LICENSES/Unlicense.txt` & `circuitpython-mag-cal-1.3.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/PKG-INFO` & `circuitpython-mag-cal-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-mag-cal
-Version: 1.2.2
+Version: 1.3.0
 Summary: Calibrate magnetometer and accelerometer readings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_mag_cal
 Keywords: adafruit,blinka,circuitpython,micropython,mag_cal,magnetometer,accelerometer,compass,calibrate,calibration,gravity,magnetism,magnetic
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-mag-cal-1.2.2/README.rst` & `circuitpython-mag-cal-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/circuitpython_mag_cal.egg-info/PKG-INFO` & `circuitpython-mag-cal-1.3.0/circuitpython_mag_cal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-mag-cal
-Version: 1.2.2
+Version: 1.3.0
 Summary: Calibrate magnetometer and accelerometer readings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_mag_cal
 Keywords: adafruit,blinka,circuitpython,micropython,mag_cal,magnetometer,accelerometer,compass,calibrate,calibration,gravity,magnetism,magnetic
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-mag-cal-1.2.2/circuitpython_mag_cal.egg-info/SOURCES.txt` & `circuitpython-mag-cal-1.3.0/circuitpython_mag_cal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/docs/_static/favicon.ico` & `circuitpython-mag-cal-1.3.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/docs/conf.py` & `circuitpython-mag-cal-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/docs/howto.rst` & `circuitpython-mag-cal-1.3.0/docs/howto.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/docs/index.rst` & `circuitpython-mag-cal-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/examples/mag_cal_simpletest.py` & `circuitpython-mag-cal-1.3.0/examples/mag_cal_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/mag_cal/axes.py` & `circuitpython-mag-cal-1.3.0/mag_cal/axes.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/mag_cal/calibration.py` & `circuitpython-mag-cal-1.3.0/mag_cal/calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,35 @@
 #
 # SPDX-License-Identifier: MIT
 """
 Calibration class: main class to use
 """
 from . import nm
 from .rbf import RBF
-from .sensor import Sensor, DEFAULT_SIGMA
+from .sensor import Sensor, SensorError
 from .utils import normalise, solve_least_squares, cross
 
 try:
     from typing import Tuple, Dict
 except ImportError:
     # ignore if running in CircuitPython/MicroPython
     pass
 
 try:
     # work with normal numpy
     import numpy as np
+
+    arccos = np.arccos
 except ImportError:
     # or work with ulab if we are in CircuitPython
     from ulab import numpy as np
 
-__version__ = "1.2.2"
+    arccos = np.acos
+
+__version__ = "1.3.0"
 __repo__ = "https://github.com/furbrain/CircuitPython_mag_cal.git"
 
 
 def _vector_from_matrices(matrix: np.ndarray, i: int, j: int):
     return np.array([x[i, j] for x in matrix])
 
 
@@ -59,23 +63,30 @@
     Object representing a magnetometer and accelerometer calibration
     """
 
     MAGNETOMETER = 1
     ACCELEROMETER = 2
     BOTH = MAGNETOMETER | ACCELEROMETER
 
+    OFF = 0
+    SOFT = 1
+    HARD = 2
+
     ELLIPSOID = 0
     """Fit to Ellipsoid"""
     AXIS_CORRECTION = 1
     """Fit to ellipsoid then correct any axis misalignment"""
     NON_LINEAR = 2
     """as per `AXIS_CORRECTION` and then do correction for non-linear effects"""
     FAST_NON_LINEAR = 3
     """as per `AXIS_CORRECTION` and then do quick non-linear correction"""
 
+    _SOFT_SETTINGS = {"grav": 0.02, "mag": 0.05, "dip": 3}
+    _HARD_SETTINGS = {"grav": 0.01, "mag": 0.02, "dip": 1}
+
     def __init__(self, mag_axes: str = "+X+Y+Z", grav_axes: str = None):
         """
         Create an object representing the calibration coefficients for a combined
         magnetometer and accelerometer
 
         :param str mag_axes: A string representing how your magnetometer is mounted with respect to
           your device. For each axis XYZ of your device (see above for axis descriptions), state the
@@ -88,15 +99,14 @@
         """
         if grav_axes is None:
             grav_axes = mag_axes
         self.mag = Sensor(axes=mag_axes)
         self.grav = Sensor(axes=grav_axes)
         self.dip_avg: float = None
         self.dip_std: float = None
-        self.ready = False
 
     def calibrate(
         self,
         mag_data: np.ndarray,
         grav_data: np.ndarray,
         routine: int = FAST_NON_LINEAR,
     ):
@@ -163,30 +173,32 @@
 
         :return: The calibration as a dictionary
         :rtype: dict
         """
         dct = {
             "mag": self.mag.as_dict(),
             "grav": self.grav.as_dict(),
-            "ready": self.ready,
+            "dip_std": self.dip_std,
+            "dip_avg": self.dip_avg,
         }
         return dct
 
     @classmethod
     def from_dict(cls, dct: Dict) -> "Calibration":
         """
         Create a Calibration object based on a dict previously produced by `as_dict`
 
         :param dict dct: dict to instantiate
         :return: Calibration object
         """
         instance = cls()
         instance.mag = Sensor.from_dict(dct["mag"])
         instance.grav = Sensor.from_dict(dct["grav"])
-        instance.ready = dct["ready"]
+        instance.dip_std = dct["dip_std"]
+        instance.dip_avg = dct["dip_avg"]
         return instance
 
     def fit_ellipsoid(
         self, mag_data: np.ndarray, grav_data: np.ndarray
     ) -> Tuple[float, float]:
         """
         Take multiple sets of readings in various directions. You can then use this function
@@ -195,15 +207,14 @@
         :param np.ndarray mag_data: Numpy array of magnetic readings of shape (N,3)
         :param np.ndarray grav_data: Numpy array of gravity readings of shape (M,3)
         :return: (mag_accuracy, grav_accuracy) How well the calibrated model fits the data.
           Lower numbers are better
         """
         mag_accuracy = self.mag.fit_ellipsoid(mag_data)
         grav_accuracy = self.grav.fit_ellipsoid(grav_data)
-        self.ready = True
         return mag_accuracy, grav_accuracy
 
     def fit_to_axis(self, data, axis="Y") -> float:
         """
         Take multiple reading with the device pointing in the same direction, but rotated around
         ``axis``. You can repeat this with several directions. This function will take
         this data and ensure that your sensors aligned relative to each other. This function
@@ -604,15 +615,15 @@
         if len(normalised_gravs.shape) > 1:
             dot_products = [
                 np.dot(m, g) for m, g in zip(normalised_mags, normalised_gravs)
             ]
             dot_products = np.array(dot_products)
         else:
             dot_products = np.dot(normalised_mags, normalised_gravs)
-        dips = 90 - np.degrees(np.arccos(dot_products))
+        dips = 90 - np.degrees(arccos(dot_products))
         return dips
 
     def set_expected_mean_dip_and_std(self, mag, grav):
         """
         Store an expected dip and standard deviations. This will be used for
         magnetic and (gravitational!!) anomaly detection
 
@@ -636,28 +647,51 @@
           floats
         :return:
         """
         self.mag.set_expected_field_strengths(mag)
         self.grav.set_expected_field_strengths(grav)
         self.set_expected_mean_dip_and_std(mag, grav)
 
-    def raise_if_anomaly(self, mag, grav, sigma=DEFAULT_SIGMA):
+    def raise_if_anomaly(self, mag, grav, strictness: int = SOFT):
         """
         Raises an error if magnetic field strength and dip are not similar to during calibration
 
         :param numpy.ndarray mag: Magnetic readings, sequence of 3 floats
         :param numpy.ndarray grav: Gravity readings, sequence of 3 floats
-        :param sigma: number of standard deviations to accept, default is 3
+        :param int strictness: One of ``OFF``, ``SOFT``, ``HARD`` - these indicate how strictly
+          we check for deviations from field strength and dip
+
+          ========== ======= ======== ===
+          Strictness Gravity Magnetic Dip
+          ========== ======= ======== ===
+          ``OFF``    Off     Off      Off
+          ``SOFT``   ±2%     ±5%      3°
+          ``HARD``   ±1%     ±2%      1°
+          ========== ======= ======== ===
         :return: None
         :raises:
           * ``MagneticAnomalyError`` if magnetic field strength too big or small
           * ``GravityAnomalyError`` if gravity field strength too big or small - this should be rare
           * ``DipAnomalyError`` if magnetic field dip too big or small
         """
-        if self.mag.reading_is_anomalous(mag):
-            raise MagneticAnomalyError("Magnetic field strength out of limits")
-        if self.grav.reading_is_anomalous(grav):
-            raise GravityAnomalyError("Gravity field strength out of limits")
+        if strictness == self.OFF:
+            return
+        if strictness == self.SOFT:
+            settings = self._SOFT_SETTINGS
+        else:
+            settings = self._HARD_SETTINGS
+        try:
+            self.mag.raise_if_anomaly(mag, settings["mag"])
+        except SensorError as exc:
+            raise MagneticAnomalyError(exc.args) from exc
+        try:
+            self.grav.raise_if_anomaly(grav, settings["grav"])
+        except SensorError as exc:
+            raise GravityAnomalyError(exc.args) from exc
         dip = self.get_dips(mag, grav)
+        acceptable = max(3 * self.dip_std, settings["dip"])
         variation = abs(self.dip_avg - dip)
-        if variation > sigma * self.dip_std:
-            raise DipAnomalyError("Magnetic dip out of limits")
+        if variation > acceptable:
+            raise DipAnomalyError(
+                f"Magnetic dip {dip} out of limits {self.dip_avg-acceptable} - "
+                + f"{self.dip_avg+acceptable}"
+            )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `circuitpython-mag-cal-1.2.2/mag_cal/lstsq.py` & `circuitpython-mag-cal-1.3.0/mag_cal/lstsq.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/mag_cal/nm.py` & `circuitpython-mag-cal-1.3.0/mag_cal/nm.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/mag_cal/rbf.py` & `circuitpython-mag-cal-1.3.0/mag_cal/rbf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/mag_cal/sensor.py` & `circuitpython-mag-cal-1.3.0/mag_cal/sensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,19 @@
 except ImportError:
     from ulab import numpy as np
 
 from .axes import Axes
 from .utils import solve_least_squares, normalise, NotCalibrated, cross
 from .rbf import RBF
 
-DEFAULT_SIGMA = 3
+DEFAULT_TOLERANCE = 0.05
+
+
+class SensorError(Exception):
+    """Raised when sensor readings out of range"""
 
 
 class Sensor:
     """
     This represents the calibration coefficients for a single sensor
     """
 
@@ -257,17 +261,25 @@
         magnetic and (gravitational!!) anomaly detection
         :param numpy.ndarray data: Sensor readings, either as numpy array or sequence of 3 floats
         """
         strengths = self.get_field_strength(data)
         self.field_avg = np.mean(strengths)
         self.field_std = np.std(strengths)
 
-    def reading_is_anomalous(self, data, sigma=DEFAULT_SIGMA):
+    def raise_if_anomaly(self, data, tolerance=DEFAULT_TOLERANCE):
         """
-        Returns True if given reading is not within expected range
+        Raise SensorAnomaly if given reading is not within expected range
+
         :param data: sequence of 3 floats
-        :param sigma: NUmber of standard deviations that must be exceeded
-        :return: True if field strenght is greater than sigma standard deviations from the mean
+        :param tolerance: Amount if difference in field strength to accept
+        :raises: ``SensorError`` if field strength is greater than tolerance different from
+          the mean
         """
         strength = self.get_field_strength(data)
+        # set acceptable difference to be larger of 3 sigmas of standard deviation or tolerance
+        acceptable = max(self.field_std * 3, self.field_avg * tolerance)
         variation = abs(self.field_avg - strength)
-        return variation > sigma * self.field_std
+        if variation > acceptable:
+            raise SensorError(
+                f"Strength is {strength}, should be {self.field_avg-acceptable} - "
+                + f"{self.field_avg + acceptable}"
+            )
```

### Comparing `circuitpython-mag-cal-1.2.2/mag_cal/utils.py` & `circuitpython-mag-cal-1.3.0/mag_cal/utils.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/pyproject.toml` & `circuitpython-mag-cal-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-mag-cal"
 description = "Calibrate magnetometer and accelerometer readings"
-version = "1.2.2"
+version = "1.3.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/furbrain/CircuitPython_mag_cal"}
 keywords = [
     "adafruit",
```

### Comparing `circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/ab.json` & `circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/ab.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/ai.json` & `circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/ai.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/bh.json` & `circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/bh.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/bi.json` & `circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/bi.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/ee.json` & `circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/ee.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/fb.json` & `circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/fb.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/hj.json` & `circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/hj.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/hj2.json` & `circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/hj2.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/tests/fixtures/cal_data/jd.json` & `circuitpython-mag-cal-1.3.0/tests/fixtures/cal_data/jd.json`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/tests/test_axes.py` & `circuitpython-mag-cal-1.3.0/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mag-cal-1.2.2/tests/test_calibration.py` & `circuitpython-mag-cal-1.3.0/tests/test_calibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import unittest
 from pathlib import Path
 from unittest import TestCase
 from unittest.mock import patch
 
 import numpy as np
 
-from mag_cal.calibration import Calibration, CalibrationError
+from mag_cal.calibration import Calibration
 from mag_cal.utils import read_fixture
 
 
 class TestCalibration(TestCase):
     def setUp(self) -> None:
         np.set_printoptions(precision=4, suppress=True)
         self.fixtures = {}
@@ -139,17 +139,16 @@
                 calib.raise_if_anomaly(m, g)
 
     def test_calibration_readings_anomalous_with_low_sigma(self):
         # pylint: disable=invalid-name
         for mag, grav, _ in self.fixtures.values():
             calib = Calibration()
             calib.calibrate(mag, grav)
-            with self.assertRaises(CalibrationError):
-                for m, g in zip(mag, grav):
-                    calib.raise_if_anomaly(m, g, sigma=1)
+            for m, g in zip(mag, grav):
+                calib.raise_if_anomaly(m, g, Calibration.HARD)
 
     @unittest.skip
     def test_display_non_linear_maps(self):
         # pylint: disable=invalid-name,import-outside-toplevel,cell-var-from-loop
         import matplotlib.pyplot as plt
 
         mag, grav, aligned_data = list(self.fixtures.values())[3]
```

### Comparing `circuitpython-mag-cal-1.2.2/tests/test_sensor.py` & `circuitpython-mag-cal-1.3.0/tests/test_sensor.py`

 * *Files identical despite different names*

