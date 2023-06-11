# Comparing `tmp/fedcloudclient-1.3.1.tar.gz` & `tmp/fedcloudclient-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedcloudclient-1.3.1.tar", last modified: Tue Nov 22 12:48:42 2022, max compression
+gzip compressed data, was "fedcloudclient-1.4.0.tar", last modified: Sun Jun 11 18:15:56 2023, max compression
```

## Comparing `fedcloudclient-1.3.1.tar` & `fedcloudclient-1.4.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 12:48:42.524737 fedcloudclient-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 12:48:42.516738 fedcloudclient-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 12:48:42.520738 fedcloudclient-1.3.1/.github/linters/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/.github/linters/.flake8
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/.github/linters/.jscpd.json
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/.github/linters/.mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/.github/linters/mlc_config.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 12:48:42.520738 fedcloudclient-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/.github/workflows/check-links.yml
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/.github/workflows/publish_image.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/.github/workflows/sphinx-pages.yml
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-22 12:48:42.000000 fedcloudclient-1.3.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-22 12:48:42.000000 fedcloudclient-1.3.1/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8356 2022-11-22 12:48:42.524737 fedcloudclient-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7622 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 12:48:42.520738 fedcloudclient-1.3.1/config/
--rw-r--r--   0 runner    (1001) docker     (121)     3050 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/config/sites.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 12:48:42.520738 fedcloudclient-1.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/docs/FAQ.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/docs/cheat.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12755 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/docs/fedcloudclient-logo-non-transparent-small.png
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/docs/fedcloudclient.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2050 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2500 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3210 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/docs/scripts.rst
--rw-r--r--   0 runner    (1001) docker     (121)    19994 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 12:48:42.520738 fedcloudclient-1.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/examples/command_history.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/examples/demo.py
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/examples/fedcloud_bash_completion.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/examples/list-all-my-own-vms.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2791 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/examples/list-my-own-vms.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 12:48:42.524737 fedcloudclient-1.3.1/fedcloudclient/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/fedcloudclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6726 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/fedcloudclient/checkin.py
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/fedcloudclient/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     8007 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/fedcloudclient/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     6034 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/fedcloudclient/ec3.py
--rw-r--r--   0 runner    (1001) docker     (121)    12588 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/fedcloudclient/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     9636 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/fedcloudclient/openstack.py
--rw-r--r--   0 runner    (1001) docker     (121)     1904 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/fedcloudclient/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)    10242 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/fedcloudclient/secret.py
--rw-r--r--   0 runner    (1001) docker     (121)     7593 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/fedcloudclient/select.py
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/fedcloudclient/shell.py
--rw-r--r--   0 runner    (1001) docker     (121)    10664 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/fedcloudclient/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 12:48:42.524737 fedcloudclient-1.3.1/fedcloudclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8356 2022-11-22 12:48:42.000000 fedcloudclient-1.3.1/fedcloudclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-11-22 12:48:42.000000 fedcloudclient-1.3.1/fedcloudclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 12:48:42.000000 fedcloudclient-1.3.1/fedcloudclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-22 12:48:42.000000 fedcloudclient-1.3.1/fedcloudclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 12:48:42.000000 fedcloudclient-1.3.1/fedcloudclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-22 12:48:42.000000 fedcloudclient-1.3.1/fedcloudclient.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-11-22 12:48:42.000000 fedcloudclient-1.3.1/fedcloudclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-22 12:48:42.000000 fedcloudclient-1.3.1/fedcloudclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-11-22 12:48:42.524737 fedcloudclient-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 12:48:42.524737 fedcloudclient-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/tests/00_empty_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-11-22 12:48:26.000000 fedcloudclient-1.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:56.592853 fedcloudclient-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:56.588853 fedcloudclient-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:56.588853 fedcloudclient-1.4.0/.github/linters/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/.github/linters/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/.github/linters/.jscpd.json
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/.github/linters/.mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/.github/linters/mlc_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:56.588853 fedcloudclient-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/.github/workflows/check-links.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/.github/workflows/publish_image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/.github/workflows/sphinx-pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-11 18:15:56.000000 fedcloudclient-1.4.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-11 18:15:56.000000 fedcloudclient-1.4.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-06-11 18:15:56.592853 fedcloudclient-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:56.588853 fedcloudclient-1.4.0/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/config/sites.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:56.592853 fedcloudclient-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/docs/FAQ.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/docs/cheat.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12755 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/docs/fedcloudclient-logo-non-transparent-small.png
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/docs/fedcloudclient.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/docs/scripts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19994 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:56.592853 fedcloudclient-1.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/examples/command_history.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/examples/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/examples/fedcloud_bash_completion.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/examples/list-all-my-own-vms.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/examples/list-my-own-vms.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:56.592853 fedcloudclient-1.4.0/fedcloudclient/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/fedcloudclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/fedcloudclient/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/fedcloudclient/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/fedcloudclient/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/fedcloudclient/ec3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/fedcloudclient/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/fedcloudclient/openstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/fedcloudclient/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/fedcloudclient/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/fedcloudclient/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/fedcloudclient/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/fedcloudclient/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:56.592853 fedcloudclient-1.4.0/fedcloudclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-06-11 18:15:56.000000 fedcloudclient-1.4.0/fedcloudclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-11 18:15:56.000000 fedcloudclient-1.4.0/fedcloudclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:15:56.000000 fedcloudclient-1.4.0/fedcloudclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-11 18:15:56.000000 fedcloudclient-1.4.0/fedcloudclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:15:56.000000 fedcloudclient-1.4.0/fedcloudclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-11 18:15:56.000000 fedcloudclient-1.4.0/fedcloudclient.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-11 18:15:56.000000 fedcloudclient-1.4.0/fedcloudclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-11 18:15:56.000000 fedcloudclient-1.4.0/fedcloudclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-11 18:15:56.592853 fedcloudclient-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:56.592853 fedcloudclient-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/tests/00_empty_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-11 18:15:46.000000 fedcloudclient-1.4.0/tox.ini
```

### Comparing `fedcloudclient-1.3.1/.github/workflows/check-links.yml` & `fedcloudclient-1.4.0/.github/workflows/check-links.yml`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/.github/workflows/lint.yml` & `fedcloudclient-1.4.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/.github/workflows/publish_image.yml` & `fedcloudclient-1.4.0/.github/workflows/publish_image.yml`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/.github/workflows/python-package.yml` & `fedcloudclient-1.4.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/.github/workflows/python-publish.yml` & `fedcloudclient-1.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/.github/workflows/sphinx-pages.yml` & `fedcloudclient-1.4.0/.github/workflows/sphinx-pages.yml`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/CHANGELOG` & `fedcloudclient-1.4.0/CHANGELOG`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/Dockerfile` & `fedcloudclient-1.4.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/LICENSE` & `fedcloudclient-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/PKG-INFO` & `fedcloudclient-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedcloudclient
-Version: 1.3.1
+Version: 1.4.0
 Summary: EGI FedCloud client
 Home-page: https://fedcloudclient.fedcloud.eu/
 Author: Viet Tran, Enol Fernandez
 Author-email: tdviet@gmail.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fedcloudclient-1.3.1/README.md` & `fedcloudclient-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/config/sites.yaml` & `fedcloudclient-1.4.0/config/sites.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-# List of sites in https://github.com/EGI-Foundation/fedcloud-catchall-operations/tree/main/sites
+# List of sites in https://github.com/EGI-Federation/fedcloud-catchall-operations/tree/main/sites
 # As GitHub API has limited access rates, the list of sites is stored here for simple access
 
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/100IT.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/BIFI.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/CESGA.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/100IT.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/BIFI.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/CESGA.yaml"
 - "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/CESGA-CLOUD.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/CESNET-MCC.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/CETA-GRID.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/CLOUDIFIN.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/CYFRONET-CLOUD.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/DESY-CC.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/CESNET-MCC.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/CETA-GRID.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/CLOUDIFIN.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/CYFRONET-CLOUD.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/DESY-CC.yaml"
 - "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/GRNET-OPENSTACK.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/GSI-LCG2.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/IFCA-LCG2.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/IISAS-FedCloud-cloud.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/ILIFU-UCT.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/IN2P3-IRES.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/INFN-CATANIA-STACK.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/INFN-CLOUD-BARI.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/INFN-CLOUD-CNAF.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/INFN-PADOVA-STACK.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/NCG-INGRID-PT.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/SCAI.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/TR-FC1-ULAKBIM.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/UA-BITP.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/UNIV-LILLE.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/GSI-LCG2.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/IFCA-LCG2.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/IISAS-FedCloud-cloud.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/ILIFU-UCT.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/IN2P3-IRES.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/INFN-CLOUD-BARI.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/INFN-CLOUD-CNAF.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/INFN-PADOVA-STACK.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/NCG-INGRID-PT.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/SCAI.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/TR-FC1-ULAKBIM.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/UA-BITP.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/UNIV-LILLE.yaml"
 - "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/UPV-GRyCAP.yaml"
-- "https://raw.githubusercontent.com/EGI-Foundation/fedcloud-catchall-operations/main/sites/fedcloud.srce.hr.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/WALTON-CLOUD.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/fedcloud.srce.hr.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/EODC.yaml"
+- "https://raw.githubusercontent.com/EGI-Federation/fedcloud-catchall-operations/main/sites/ELKH-CLOUD.yaml"
+
```

### Comparing `fedcloudclient-1.3.1/docs/FAQ.rst` & `fedcloudclient-1.4.0/docs/FAQ.rst`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/docs/cheat.rst` & `fedcloudclient-1.4.0/docs/cheat.rst`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/docs/conf.py` & `fedcloudclient-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/docs/development.rst` & `fedcloudclient-1.4.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/docs/fedcloudclient-logo-non-transparent-small.png` & `fedcloudclient-1.4.0/docs/fedcloudclient-logo-non-transparent-small.png`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/docs/fedcloudclient.rst` & `fedcloudclient-1.4.0/docs/fedcloudclient.rst`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/docs/index.rst` & `fedcloudclient-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/docs/install.rst` & `fedcloudclient-1.4.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/docs/intro.rst` & `fedcloudclient-1.4.0/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/docs/quickstart.rst` & `fedcloudclient-1.4.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/docs/scripts.rst` & `fedcloudclient-1.4.0/docs/scripts.rst`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/docs/usage.rst` & `fedcloudclient-1.4.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/examples/demo.py` & `fedcloudclient-1.4.0/examples/demo.py`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/examples/fedcloud_bash_completion.sh` & `fedcloudclient-1.4.0/examples/fedcloud_bash_completion.sh`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/examples/list-all-my-own-vms.sh` & `fedcloudclient-1.4.0/examples/list-all-my-own-vms.sh`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/examples/list-my-own-vms.sh` & `fedcloudclient-1.4.0/examples/list-my-own-vms.sh`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/fedcloudclient/checkin.py` & `fedcloudclient-1.4.0/fedcloudclient/checkin.py`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/fedcloudclient/cli.py` & `fedcloudclient-1.4.0/fedcloudclient/cli.py`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/fedcloudclient/decorators.py` & `fedcloudclient-1.4.0/fedcloudclient/decorators.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,14 +30,23 @@
     "--site",
     help="Name of the site",
     required=True,
     envvar="EGI_SITE",
     metavar="site-name",
 )
 
+# Output format for secret module
+secret_output_params = click.option(
+    "--output-format",
+    "-f",
+    required=False,
+    help="Output format",
+    type=click.Choice(["text", "YAML", "JSON"], case_sensitive=False),
+)
+
 
 def all_site_params(func):
     """
     Decorator for all-sites options
     """
 
     @optgroup.group(
@@ -328,7 +337,75 @@
         default="JSON",
     )
     @wraps(func)
     def wrapper(*args, **kwargs):
         return func(*args, **kwargs)
 
     return wrapper
+
+
+def secret_token_params(func):
+    """
+    Decorator for secret token.
+    If locker token is not defined, get access token from oidc-* parameters
+    and replace them in the wrapper function
+    """
+
+    @optgroup.group("Token options", help="Choose one of options for providing token")
+    @optgroup.option(
+        "--locker-token",
+        help="Locker token",
+        envvar="FEDCLOUD_LOCKER_TOKEN",
+        metavar="locker_token",
+    )
+    @optgroup.option(
+        "--oidc-agent-account",
+        help="Account name in oidc-agent",
+        envvar="OIDC_AGENT_ACCOUNT",
+        metavar="account",
+    )
+    @optgroup.option(
+        "--oidc-access-token",
+        help="OIDC access token",
+        envvar="OIDC_ACCESS_TOKEN",
+        metavar="token",
+    )
+    @optgroup.option(
+        "--mytoken",
+        help="Mytoken string",
+        envvar="FEDCLOUD_MYTOKEN",
+        metavar="mytoken",
+    )
+    @optgroup.option(
+        "--mytoken-server",
+        help="Mytoken sever",
+        envvar="FEDCLOUD_MYTOKEN_SERVER",
+        default=DEFAULT_MYTOKEN_SERVER,
+        show_default=True,
+        metavar="mytoken-server",
+    )
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        from fedcloudclient.checkin import get_access_token
+
+        # If locker token is given, ignore OIDC token options
+        locker_token = kwargs.pop("locker_token")
+        if locker_token:
+            kwargs.pop("oidc_access_token")
+            kwargs.pop("oidc_agent_account")
+            kwargs.pop("mytoken")
+            kwargs.pop("mytoken_server")
+            kwargs["access_token"] = None
+            kwargs["locker_token"] = locker_token
+            return func(*args, **kwargs)
+
+        access_token = get_access_token(
+            kwargs.pop("oidc_access_token"),
+            kwargs.pop("oidc_agent_account"),
+            kwargs.pop("mytoken"),
+            kwargs.pop("mytoken_server"),
+        )
+        kwargs["access_token"] = access_token
+        kwargs["locker_token"] = None
+        return func(*args, **kwargs)
+
+    return wrapper
```

### Comparing `fedcloudclient-1.3.1/fedcloudclient/ec3.py` & `fedcloudclient-1.4.0/fedcloudclient/ec3.py`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/fedcloudclient/endpoint.py` & `fedcloudclient-1.4.0/fedcloudclient/endpoint.py`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/fedcloudclient/openstack.py` & `fedcloudclient-1.4.0/fedcloudclient/openstack.py`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/fedcloudclient/schema.json` & `fedcloudclient-1.4.0/fedcloudclient/schema.json`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/fedcloudclient/select.py` & `fedcloudclient-1.4.0/fedcloudclient/select.py`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/fedcloudclient/shell.py` & `fedcloudclient-1.4.0/fedcloudclient/shell.py`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/fedcloudclient/sites.py` & `fedcloudclient-1.4.0/fedcloudclient/sites.py`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/fedcloudclient.egg-info/PKG-INFO` & `fedcloudclient-1.4.0/fedcloudclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedcloudclient
-Version: 1.3.1
+Version: 1.4.0
 Summary: EGI FedCloud client
 Home-page: https://fedcloudclient.fedcloud.eu/
 Author: Viet Tran, Enol Fernandez
 Author-email: tdviet@gmail.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fedcloudclient-1.3.1/fedcloudclient.egg-info/SOURCES.txt` & `fedcloudclient-1.4.0/fedcloudclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/setup.cfg` & `fedcloudclient-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fedcloudclient-1.3.1/tox.ini` & `fedcloudclient-1.4.0/tox.ini`

 * *Files identical despite different names*

