# Comparing `tmp/osmviz-4.1.0.tar.gz` & `tmp/osmviz-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osmviz-4.1.0.tar", last modified: Sat Jun  4 21:02:43 2022, max compression
+gzip compressed data, last modified: Sun Jun 11 07:59:04 2023, max compression
```

## Comparing `osmviz-4.1.0.tar` & `osmviz-4.2.0.tar`

### file list

```diff
@@ -1,94 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.469393 osmviz-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-06-04 21:02:17.000000 osmviz-4.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.461392 osmviz-4.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)     1878 2022-06-04 21:02:17.000000 osmviz-4.1.0/.github/labels.yml
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-06-04 21:02:17.000000 osmviz-4.1.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.461392 osmviz-4.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-06-04 21:02:17.000000 osmviz-4.1.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-06-04 21:02:17.000000 osmviz-4.1.0/.github/workflows/labels.yml
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-06-04 21:02:17.000000 osmviz-4.1.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-06-04 21:02:17.000000 osmviz-4.1.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-06-04 21:02:17.000000 osmviz-4.1.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-06-04 21:02:17.000000 osmviz-4.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-06-04 21:02:17.000000 osmviz-4.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-06-04 21:02:17.000000 osmviz-4.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-06-04 21:02:17.000000 osmviz-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-06-04 21:02:43.469393 osmviz-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-06-04 21:02:17.000000 osmviz-4.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-06-04 21:02:17.000000 osmviz-4.1.0/RELEASING.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.465392 osmviz-4.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-06-04 21:02:17.000000 osmviz-4.1.0/examples/README
--rw-r--r--   0 runner    (1001) docker     (121)     3851 2022-06-04 21:02:17.000000 osmviz-4.1.0/examples/custom_animations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.465392 osmviz-4.1.0/examples/images/
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-06-04 21:02:17.000000 osmviz-4.1.0/examples/images/train.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.465392 osmviz-4.1.0/examples/maptiles/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-04 21:02:17.000000 osmviz-4.1.0/examples/maptiles/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-06-04 21:02:17.000000 osmviz-4.1.0/examples/multiple_trackvizs.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-06-04 21:02:17.000000 osmviz-4.1.0/examples/pil_example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.465392 osmviz-4.1.0/html/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/contact.html
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/css.css
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/doc.html
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/download.html
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/examples.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.465392 osmviz-4.1.0/html/images/
--rw-r--r--   0 runner    (1001) docker     (121)    32032 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/images/buses_moving2.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   110128 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/images/custom_animations.png
--rw-r--r--   0 runner    (1001) docker     (121)     8103 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/images/custom_animations_small.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     2179 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/images/email.gif
--rw-r--r--   0 runner    (1001) docker     (121)   351283 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/images/multiple_trackvizs.png
--rw-r--r--   0 runner    (1001) docker     (121)    15953 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/images/multiple_trackvizs_small.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    63723 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/images/pil_example.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     9269 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/images/pil_example_small.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    15988 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/images/trainusa2.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     4540 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/nav.html
--rw-r--r--   0 runner    (1001) docker     (121)    25603 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/osmviz.animation.html
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/osmviz.html
--rw-r--r--   0 runner    (1001) docker     (121)    24898 2022-06-04 21:02:17.000000 osmviz-4.1.0/html/osmviz.manager.html
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-06-04 21:02:17.000000 osmviz-4.1.0/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     1536 2022-06-04 21:02:43.469393 osmviz-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-06-04 21:02:17.000000 osmviz-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.461392 osmviz-4.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.465392 osmviz-4.1.0/src/osmviz/
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2022-06-04 21:02:17.000000 osmviz-4.1.0/src/osmviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14575 2022-06-04 21:02:17.000000 osmviz-4.1.0/src/osmviz/animation.py
--rw-r--r--   0 runner    (1001) docker     (121)    14304 2022-06-04 21:02:17.000000 osmviz-4.1.0/src/osmviz/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.465392 osmviz-4.1.0/src/osmviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-06-04 21:02:42.000000 osmviz-4.1.0/src/osmviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-06-04 21:02:43.000000 osmviz-4.1.0/src/osmviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-04 21:02:42.000000 osmviz-4.1.0/src/osmviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-04 21:02:43.000000 osmviz-4.1.0/src/osmviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-04 21:02:43.000000 osmviz-4.1.0/src/osmviz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.461392 osmviz-4.1.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.465392 osmviz-4.1.0/test/functional/
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/functional/test_animation.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/functional/test_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.469393 osmviz-4.1.0/test/images/
--rw-r--r--   0 runner    (1001) docker     (121)     6148 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/E.gif
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/N.gif
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/NE.gif
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/NW.gif
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/S.gif
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/SE.gif
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/SW.gif
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/W.gif
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/bus.png
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/bus_small.png
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/bus_small_red.png
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/cable.png
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/drop.png
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/hybrid.png
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/onePxClear.gif
--rw-r--r--   0 runner    (1001) docker     (121)      721 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/service.png
--rw-r--r--   0 runner    (1001) docker     (121)     3208 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/spinner.gif
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/images/train.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.469393 osmviz-4.1.0/test/maptiles/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/maptiles/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 21:02:43.469393 osmviz-4.1.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/unit/test_image_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/unit/test_osm_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-06-04 21:02:17.000000 osmviz-4.1.0/test/unit/test_pil_image_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-06-04 21:02:17.000000 osmviz-4.1.0/tox.ini
+-rw-r--r--   0        0        0      277 2023-06-11 07:59:04.000000 osmviz-4.2.0/.coveragerc
+-rw-r--r--   0        0        0       30 2023-06-11 07:59:04.000000 osmviz-4.2.0/.flake8
+-rw-r--r--   0        0        0     1308 2023-06-11 07:59:04.000000 osmviz-4.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      786 2023-06-11 07:59:04.000000 osmviz-4.2.0/RELEASING.md
+-rw-r--r--   0        0        0      228 2023-06-11 07:59:04.000000 osmviz-4.2.0/index.html
+-rw-r--r--   0        0        0      542 2023-06-11 07:59:04.000000 osmviz-4.2.0/tox.ini
+-rw-r--r--   0        0        0     1785 2023-06-11 07:59:04.000000 osmviz-4.2.0/.github/labels.yml
+-rw-r--r--   0        0        0      900 2023-06-11 07:59:04.000000 osmviz-4.2.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      350 2023-06-11 07:59:04.000000 osmviz-4.2.0/.github/renovate.json
+-rw-r--r--   0        0        0     1755 2023-06-11 07:59:04.000000 osmviz-4.2.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      352 2023-06-11 07:59:04.000000 osmviz-4.2.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      298 2023-06-11 07:59:04.000000 osmviz-4.2.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2023-06-11 07:59:04.000000 osmviz-4.2.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      490 2023-06-11 07:59:04.000000 osmviz-4.2.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1171 2023-06-11 07:59:04.000000 osmviz-4.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       45 2023-06-11 07:59:04.000000 osmviz-4.2.0/examples/README
+-rw-r--r--   0        0        0     3852 2023-06-11 07:59:04.000000 osmviz-4.2.0/examples/custom_animations.py
+-rw-r--r--   0        0        0     1367 2023-06-11 07:59:04.000000 osmviz-4.2.0/examples/multiple_trackvizs.py
+-rw-r--r--   0        0        0      466 2023-06-11 07:59:04.000000 osmviz-4.2.0/examples/pil_example.py
+-rw-r--r--   0        0        0      763 2023-06-11 07:59:04.000000 osmviz-4.2.0/examples/images/train.png
+-rw-r--r--   0        0        0        6 2023-06-11 07:59:04.000000 osmviz-4.2.0/examples/maptiles/.gitignore
+-rw-r--r--   0        0        0      219 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/Makefile
+-rw-r--r--   0        0        0      474 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/contact.html
+-rw-r--r--   0        0        0     1489 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/css.css
+-rw-r--r--   0        0        0      793 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/doc.html
+-rw-r--r--   0        0        0      533 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/download.html
+-rw-r--r--   0        0        0     1479 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/examples.html
+-rw-r--r--   0        0        0     4540 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/index.html
+-rw-r--r--   0        0        0      594 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/nav.html
+-rw-r--r--   0        0        0    25603 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/osmviz.animation.html
+-rw-r--r--   0        0        0     1513 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/osmviz.html
+-rw-r--r--   0        0        0    24898 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/osmviz.manager.html
+-rw-r--r--   0        0        0    32032 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/images/buses_moving2.jpg
+-rw-r--r--   0        0        0   110128 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/images/custom_animations.png
+-rw-r--r--   0        0        0     8103 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/images/custom_animations_small.jpg
+-rw-r--r--   0        0        0     2179 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/images/email.gif
+-rw-r--r--   0        0        0   351283 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/images/multiple_trackvizs.png
+-rw-r--r--   0        0        0    15953 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/images/multiple_trackvizs_small.jpg
+-rw-r--r--   0        0        0    63723 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/images/pil_example.jpg
+-rw-r--r--   0        0        0     9269 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/images/pil_example_small.jpg
+-rw-r--r--   0        0        0    15988 2023-06-11 07:59:04.000000 osmviz-4.2.0/html/images/trainusa2.jpg
+-rw-r--r--   0        0        0     1123 2023-06-11 07:59:04.000000 osmviz-4.2.0/src/osmviz/__init__.py
+-rw-r--r--   0        0        0    14574 2023-06-11 07:59:04.000000 osmviz-4.2.0/src/osmviz/animation.py
+-rw-r--r--   0        0        0    14304 2023-06-11 07:59:04.000000 osmviz-4.2.0/src/osmviz/manager.py
+-rw-r--r--   0        0        0     1523 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/functional/test_animation.py
+-rw-r--r--   0        0        0      482 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/functional/test_manager.py
+-rw-r--r--   0        0        0     6148 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/.DS_Store
+-rw-r--r--   0        0        0      913 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/E.gif
+-rw-r--r--   0        0        0      917 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/N.gif
+-rw-r--r--   0        0        0      915 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/NE.gif
+-rw-r--r--   0        0        0      917 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/NW.gif
+-rw-r--r--   0        0        0      909 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/S.gif
+-rw-r--r--   0        0        0      915 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/SE.gif
+-rw-r--r--   0        0        0      917 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/SW.gif
+-rw-r--r--   0        0        0      910 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/W.gif
+-rw-r--r--   0        0        0      703 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/bus.png
+-rw-r--r--   0        0        0      414 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/bus_small.png
+-rw-r--r--   0        0        0      334 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/bus_small_red.png
+-rw-r--r--   0        0        0     1613 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/cable.png
+-rw-r--r--   0        0        0      664 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/drop.png
+-rw-r--r--   0        0        0     1339 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/hybrid.png
+-rw-r--r--   0        0        0       43 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/onePxClear.gif
+-rw-r--r--   0        0        0      721 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/service.png
+-rw-r--r--   0        0        0     3208 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/spinner.gif
+-rw-r--r--   0        0        0      763 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/images/train.png
+-rw-r--r--   0        0        0        6 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/maptiles/.gitignore
+-rw-r--r--   0        0        0      418 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/unit/test_image_manager.py
+-rw-r--r--   0        0        0     1937 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/unit/test_osm_manager.py
+-rw-r--r--   0        0        0     2339 2023-06-11 07:59:04.000000 osmviz-4.2.0/test/unit/test_pil_image_manager.py
+-rw-r--r--   0        0        0      716 2023-06-11 07:59:04.000000 osmviz-4.2.0/.gitignore
+-rw-r--r--   0        0        0     1073 2023-06-11 07:59:04.000000 osmviz-4.2.0/LICENSE
+-rw-r--r--   0        0        0     1795 2023-06-11 07:59:04.000000 osmviz-4.2.0/README.md
+-rw-r--r--   0        0        0     1643 2023-06-11 07:59:04.000000 osmviz-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3325 2023-06-11 07:59:04.000000 osmviz-4.2.0/PKG-INFO
```

### Comparing `osmviz-4.1.0/.github/labels.yml` & `osmviz-4.2.0/.github/labels.yml`

 * *Files 6% similar despite different names*

```diff
@@ -45,17 +45,14 @@
   description: "In case of vulnerabilities"
   name: "changelog: Security"
 - color: fbca04
   description: "Exclude PR from release draft"
   name: "changelog: skip"
 
 # Other labels
-- color: 2d18b2
-  description: "To automatically merge PRs that are ready"
-  name: automerge
 - color: 0366d6
   description: "For dependencies"
   name: dependencies
 - color: 0052cc
   description: "Documentation"
   name: docs
 - color: f4660e
```

### Comparing `osmviz-4.1.0/.github/release-drafter.yml` & `osmviz-4.2.0/.github/release-drafter.yml`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,19 @@
       - "bug"
   - title: "Security"
     label: "changelog: Security"
 
 exclude-labels:
   - "changelog: skip"
 
+autolabeler:
+  - label: "changelog: skip"
+    branch:
+      - "/pre-commit-ci-update-config/"
+
 template: |
   $CHANGES
 
 version-resolver:
   major:
     labels:
       - "changelog: Removed"
```

### Comparing `osmviz-4.1.0/.github/workflows/test.yml` & `osmviz-4.2.0/.github/workflows/test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -7,43 +7,44 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy-3.8", "3.7", "3.8", "3.9", "3.10", "3.11-dev"]
+        python-version: ["pypy3.9", "3.8", "3.9", "3.10", "3.11", "3.12"]
         os: [macos-latest, ubuntu-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
+          allow-prereleases: true
           cache: pip
-          cache-dependency-path: setup.cfg
+          cache-dependency-path: pyproject.toml
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U wheel
-          python -m pip install -U tox tox-gh-actions
+          python -m pip install -U tox
 
       - name: Tox tests
         run: |
           tox -e py
 
       - name: Upload coverage
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v3
         with:
           flags: ${{ matrix.os }}
           name: ${{ matrix.os }} Python ${{ matrix.python-version }}
 
   success:
     needs: test
     runs-on: ubuntu-latest
-    name: test successful
+    name: Test successful
     steps:
       - name: Success
         run: echo Test successful
```

### Comparing `osmviz-4.1.0/.gitignore` & `osmviz-4.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/LICENSE` & `osmviz-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/PKG-INFO` & `osmviz-4.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: osmviz
-Version: 4.1.0
+Version: 4.2.0
 Summary: OSMViz is a small set of Python tools for retrieving and using Mapnik tiles from a Slippy Map server (you may know these as OpenStreetMap images).
-Home-page: https://github.com/hugovk/osmviz
-Author: Colin Bick and Contributors
-Author-email: colin.bick@gmail.com
-Maintainer: Hugo van Kemenade
-License: MIT
+Project-URL: Changelog, https://github.com/hugovk/osmviz/releases
 Project-URL: Documentation, https://hugovk.github.io/osmviz/
+Project-URL: Homepage, https://github.com/hugovk/osmviz
 Project-URL: Source, https://github.com/hugovk/osmviz
+Author-email: Colin Bick and Contributors <colin.bick@gmail.com>
+Maintainer: Hugo van Kemenade
+License: MIT
+License-File: LICENSE
 Keywords: osm openstreetmap tiles visualization
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Documentation
-Requires: PyGame
-Requires: PIL
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Requires-Python: >=3.8
 Provides-Extra: tests
-License-File: LICENSE
+Requires-Dist: coverage; extra == 'tests'
+Requires-Dist: pillow>=9.1; extra == 'tests'
+Requires-Dist: pytest; extra == 'tests'
+Requires-Dist: pytest-cov; extra == 'tests'
+Description-Content-Type: text/markdown
 
 # OSMViz
 
 [![PyPI version](https://img.shields.io/pypi/v/osmviz.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/osmviz/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/osmviz.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/osmviz/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/osmviz.svg)](https://pypistats.org/packages/pypistats)
 [![GitHub Actions status](https://github.com/hugovk/osmviz/workflows/Test/badge.svg)](https://github.com/hugovk/osmviz/actions)
@@ -64,15 +66,15 @@
 
 OSMViz is a small set of Python tools for retrieving
 and using Mapnik tiles from a Slippy Map server
 (you may know these as OpenStreetMap images).
 
 ## Requirements
 
-* Python 3.7+
+* Python 3.8+
 * Pillow and/or Pygame
 
 ## Installation
 
 Either:
 
     pip install osmviz
```

### Comparing `osmviz-4.1.0/README.md` & `osmviz-4.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 OSMViz is a small set of Python tools for retrieving
 and using Mapnik tiles from a Slippy Map server
 (you may know these as OpenStreetMap images).
 
 ## Requirements
 
-* Python 3.7+
+* Python 3.8+
 * Pillow and/or Pygame
 
 ## Installation
 
 Either:
 
     pip install osmviz
```

### Comparing `osmviz-4.1.0/RELEASING.md` & `osmviz-4.2.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/examples/custom_animations.py` & `osmviz-4.2.0/examples/custom_animations.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,8 +117,8 @@
 
 
 denver = 39.756111, -104.994167
 train = TiedTrain(denver, 5.0, 5.0, 60, (0, 600), "Denver Bound")
 lasso = LassoViz(train.get_loc_at_time, lambda t: denver)
 
 sim = Simulation([train], [lasso], 0)
-sim.run(refresh_rate=0.01, speed=1, osmzoom=7)
+sim.run(refresh_rate=0.01, speed=1, osm_zoom=7)
```

### Comparing `osmviz-4.1.0/examples/images/train.png` & `osmviz-4.2.0/examples/images/train.png`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/examples/multiple_trackvizs.py` & `osmviz-4.2.0/examples/multiple_trackvizs.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,8 +53,8 @@
         1,
     )  # drawing order doesn't really matter here
 
     track_vizs.append(tviz)
 
 
 sim = Simulation(track_vizs, [], 0)
-sim.run(speed=1, refresh_rate=0.1, osmzoom=zoom)
+sim.run(speed=1, refresh_rate=0.1, osm_zoom=zoom)
```

### Comparing `osmviz-4.1.0/html/css.css` & `osmviz-4.2.0/html/css.css`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/doc.html` & `osmviz-4.2.0/html/doc.html`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/download.html` & `osmviz-4.2.0/html/download.html`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/examples.html` & `osmviz-4.2.0/html/examples.html`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/images/buses_moving2.jpg` & `osmviz-4.2.0/html/images/buses_moving2.jpg`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/images/custom_animations.png` & `osmviz-4.2.0/html/images/custom_animations.png`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/images/custom_animations_small.jpg` & `osmviz-4.2.0/html/images/custom_animations_small.jpg`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/images/email.gif` & `osmviz-4.2.0/html/images/email.gif`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/images/multiple_trackvizs.png` & `osmviz-4.2.0/html/images/multiple_trackvizs.png`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/images/multiple_trackvizs_small.jpg` & `osmviz-4.2.0/html/images/multiple_trackvizs_small.jpg`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/images/pil_example.jpg` & `osmviz-4.2.0/html/images/pil_example.jpg`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/images/pil_example_small.jpg` & `osmviz-4.2.0/html/images/pil_example_small.jpg`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/images/trainusa2.jpg` & `osmviz-4.2.0/html/images/trainusa2.jpg`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/index.html` & `osmviz-4.2.0/html/index.html`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/nav.html` & `osmviz-4.2.0/html/nav.html`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/osmviz.animation.html` & `osmviz-4.2.0/html/osmviz.animation.html`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/osmviz.html` & `osmviz-4.2.0/html/osmviz.html`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/html/osmviz.manager.html` & `osmviz-4.2.0/html/osmviz.manager.html`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/setup.cfg` & `osmviz-4.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,56 @@
-[metadata]
-name = osmviz
-description = OSMViz is a small set of Python tools for retrieving and using Mapnik tiles from a Slippy Map server (you may know these as OpenStreetMap images).
-long_description = file: README.md
-long_description_content_type = text/markdown
-url = https://github.com/hugovk/osmviz
-author = Colin Bick and Contributors
-author_email = colin.bick@gmail.com
-maintainer = Hugo van Kemenade
-license = MIT
-license_file = LICENSE
-classifiers = 
-	Intended Audience :: Developers
-	License :: OSI Approved :: MIT License
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.11
-	Programming Language :: Python :: Implementation :: CPython
-	Programming Language :: Python :: Implementation :: PyPy
-	Topic :: Software Development :: Documentation
-keywords = osm openstreetmap tiles visualization
-project_urls = 
-	Documentation=https://hugovk.github.io/osmviz/
-	Source=https://github.com/hugovk/osmviz
-requires = 
-	PyGame
-	PIL
+[build-system]
+build-backend = "hatchling.build"
+requires = [
+  "hatch-vcs",
+  "hatchling",
+]
+
+[project]
+name = "osmviz"
+description = "OSMViz is a small set of Python tools for retrieving and using Mapnik tiles from a Slippy Map server (you may know these as OpenStreetMap images)."
+readme = "README.md"
+keywords = [
+  "osm openstreetmap tiles visualization",
+]
+license = {text = "MIT"}
+maintainers = [{name = "Hugo van Kemenade"}]
+authors = [{name = "Colin Bick and Contributors", email = "colin.bick@gmail.com"}]
+requires-python = ">=3.8"
+classifiers = [
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
+  "Topic :: Software Development :: Documentation",
+]
+dynamic = [
+  "version",
+]
+[project.optional-dependencies]
+tests = [
+  "coverage",
+  "pillow>=9.1",
+  "pytest",
+  "pytest-cov",
+]
+[project.urls]
+Changelog = "https://github.com/hugovk/osmviz/releases"
+Documentation = "https://hugovk.github.io/osmviz/"
+Homepage = "https://github.com/hugovk/osmviz"
+Source = "https://github.com/hugovk/osmviz"
 
-[options]
-packages = find:
-python_requires = >=3.7
-include_package_data = True
-package_dir = =src
-setup_requires = 
-	setuptools-scm
+[tool.hatch]
+version.source = "vcs"
 
-[options.packages.find]
-where = src
-
-[options.extras_require]
-tests = 
-	coverage
-	pillow>=9.1.0
-	pytest
-	pytest-cov
-
-[flake8]
-max_line_length = 88
-
-[tool:pytest]
-addopts = 
-	-W error::DeprecationWarning
-
-[egg_info]
-tag_build = 
-tag_date = 0
+[tool.hatch.version.raw-options]
+local_scheme = "no-local-version"
 
+[tool.pytest.ini_options]
+addopts = "-W error::DeprecationWarning"
```

### Comparing `osmviz-4.1.0/src/osmviz/__init__.py` & `osmviz-4.2.0/src/osmviz/__init__.py`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/src/osmviz/animation.py` & `osmviz-4.2.0/src/osmviz/animation.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,14 @@
         def get_xy(lat, lon):
             return self.get_xy(lat, lon, new_bounds, window_size)
 
         # Main simulation loop #
 
         ready_to_exit = False
         while not ready_to_exit:
-
             # Check keyboard events
             for event in pygame.event.get():
                 if event.type == pygame.KEYDOWN and event.key == pygame.K_ESCAPE:
                     ready_to_exit = True
                 elif event.type == pygame.KEYDOWN and event.key == pygame.K_UP:
                     speed = max((speed + 1) * 1.4, (speed / 1.4) + 1)
                 elif event.type == pygame.KEYDOWN and event.key == pygame.K_DOWN:
```

### Comparing `osmviz-4.1.0/src/osmviz/manager.py` & `osmviz-4.2.0/src/osmviz/manager.py`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/functional/test_animation.py` & `osmviz-4.2.0/test/functional/test_animation.py`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/.DS_Store` & `osmviz-4.2.0/test/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/E.gif` & `osmviz-4.2.0/test/images/E.gif`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/N.gif` & `osmviz-4.2.0/test/images/N.gif`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/NE.gif` & `osmviz-4.2.0/test/images/NE.gif`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/NW.gif` & `osmviz-4.2.0/test/images/NW.gif`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/S.gif` & `osmviz-4.2.0/test/images/S.gif`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/SE.gif` & `osmviz-4.2.0/test/images/SE.gif`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/SW.gif` & `osmviz-4.2.0/test/images/SW.gif`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/W.gif` & `osmviz-4.2.0/test/images/W.gif`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/bus.png` & `osmviz-4.2.0/test/images/bus.png`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/cable.png` & `osmviz-4.2.0/test/images/cable.png`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/drop.png` & `osmviz-4.2.0/test/images/drop.png`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/hybrid.png` & `osmviz-4.2.0/test/images/hybrid.png`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/service.png` & `osmviz-4.2.0/test/images/service.png`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/spinner.gif` & `osmviz-4.2.0/test/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/images/train.png` & `osmviz-4.2.0/test/images/train.png`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/unit/test_osm_manager.py` & `osmviz-4.2.0/test/unit/test_osm_manager.py`

 * *Files identical despite different names*

### Comparing `osmviz-4.1.0/test/unit/test_pil_image_manager.py` & `osmviz-4.2.0/test/unit/test_pil_image_manager.py`

 * *Files identical despite different names*

