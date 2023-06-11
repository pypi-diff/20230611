# Comparing `tmp/libauc-1.3.0rc1.tar.gz` & `tmp/libauc-1.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libauc-1.3.0rc1.tar", last modified: Sun Jun 11 05:06:48 2023, max compression
+gzip compressed data, was "libauc-1.3.0rc3.tar", last modified: Sun Jun 11 18:27:34 2023, max compression
```

## Comparing `libauc-1.3.0rc1.tar` & `libauc-1.3.0rc3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.078628 libauc-1.3.0rc1/
--rwx------   0 zhuoning   (501) staff       (20)    11357 2023-03-02 14:10:38.000000 libauc-1.3.0rc1/LICENSE
--rw-r--r--   0 zhuoning   (501) staff       (20)     4162 2023-06-11 05:06:48.078515 libauc-1.3.0rc1/PKG-INFO
--rw-r--r--   0 zhuoning   (501) staff       (20)     3676 2023-06-11 04:07:50.000000 libauc-1.3.0rc1/README.md
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.071776 libauc-1.3.0rc1/libauc/
--rwx------   0 zhuoning   (501) staff       (20)      112 2023-06-11 05:06:46.000000 libauc-1.3.0rc1/libauc/__init__.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.073787 libauc-1.3.0rc1/libauc/datasets/
--rwx------   0 zhuoning   (501) staff       (20)      245 2023-06-09 06:42:38.000000 libauc-1.3.0rc1/libauc/datasets/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)     2621 2023-06-10 17:15:47.000000 libauc-1.3.0rc1/libauc/datasets/breastcancer.py
--rwx------   0 zhuoning   (501) staff       (20)     2176 2023-06-10 17:15:53.000000 libauc-1.3.0rc1/libauc/datasets/cat_vs_dog.py
--rwx------   0 zhuoning   (501) staff       (20)     9859 2023-05-18 04:21:28.000000 libauc-1.3.0rc1/libauc/datasets/chexpert.py
--rwx------   0 zhuoning   (501) staff       (20)     6292 2023-05-24 19:24:50.000000 libauc-1.3.0rc1/libauc/datasets/cifar.py
--rwx------   0 zhuoning   (501) staff       (20)     1561 2023-06-09 06:42:09.000000 libauc-1.3.0rc1/libauc/datasets/dataset.py
--rwx------   0 zhuoning   (501) staff       (20)    12399 2023-03-09 21:50:47.000000 libauc-1.3.0rc1/libauc/datasets/folder.py
--rwx------   0 zhuoning   (501) staff       (20)     4854 2023-06-07 00:13:14.000000 libauc-1.3.0rc1/libauc/datasets/melanoma.py
--rwx------   0 zhuoning   (501) staff       (20)    13133 2023-06-07 00:16:53.000000 libauc-1.3.0rc1/libauc/datasets/movielens.py
--rwx------   0 zhuoning   (501) staff       (20)     1497 2023-06-09 07:05:10.000000 libauc-1.3.0rc1/libauc/datasets/musk2.py
--rwx------   0 zhuoning   (501) staff       (20)     2960 2023-03-02 14:10:38.000000 libauc-1.3.0rc1/libauc/datasets/stl10.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.075147 libauc-1.3.0rc1/libauc/losses/
--rwx------   0 zhuoning   (501) staff       (20)      117 2023-06-07 19:59:42.000000 libauc-1.3.0rc1/libauc/losses/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    49557 2023-06-10 17:45:01.000000 libauc-1.3.0rc1/libauc/losses/auc.py
--rwx------   0 zhuoning   (501) staff       (20)    23656 2023-06-08 21:47:59.000000 libauc-1.3.0rc1/libauc/losses/contrastive.py
--rwx------   0 zhuoning   (501) staff       (20)     2893 2023-06-08 21:37:05.000000 libauc-1.3.0rc1/libauc/losses/losses.py
--rwx------   0 zhuoning   (501) staff       (20)    15077 2023-06-10 06:44:38.000000 libauc-1.3.0rc1/libauc/losses/mil.py
--rwx------   0 zhuoning   (501) staff       (20)     3038 2023-06-11 04:06:56.000000 libauc-1.3.0rc1/libauc/losses/perf_at_top.py
--rwx------   0 zhuoning   (501) staff       (20)    12996 2023-06-11 04:07:47.000000 libauc-1.3.0rc1/libauc/losses/ranking.py
--rwx------   0 zhuoning   (501) staff       (20)     2618 2023-06-03 03:28:07.000000 libauc-1.3.0rc1/libauc/losses/surrogate.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.075359 libauc-1.3.0rc1/libauc/metrics/
--rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:29.000000 libauc-1.3.0rc1/libauc/metrics/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)     8479 2023-06-11 04:07:30.000000 libauc-1.3.0rc1/libauc/metrics/metrics.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.076106 libauc-1.3.0rc1/libauc/models/
--rwx------   0 zhuoning   (501) staff       (20)      153 2023-05-26 02:45:25.000000 libauc-1.3.0rc1/libauc/models/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    13913 2023-05-18 03:12:04.000000 libauc-1.3.0rc1/libauc/models/densenet.py
--rwx------   0 zhuoning   (501) staff       (20)     8626 2023-05-26 04:26:36.000000 libauc-1.3.0rc1/libauc/models/mil_models.py
--rwx------   0 zhuoning   (501) staff       (20)     3479 2023-06-07 00:10:14.000000 libauc-1.3.0rc1/libauc/models/neumf.py
--rwx------   0 zhuoning   (501) staff       (20)     1284 2023-06-07 00:11:49.000000 libauc-1.3.0rc1/libauc/models/perceptron.py
--rwx------   0 zhuoning   (501) staff       (20)    16352 2023-05-18 03:13:49.000000 libauc-1.3.0rc1/libauc/models/resnet.py
--rwx------   0 zhuoning   (501) staff       (20)     6836 2023-05-26 02:54:35.000000 libauc-1.3.0rc1/libauc/models/resnet_cifar.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.077772 libauc-1.3.0rc1/libauc/optimizers/
--rwx------   0 zhuoning   (501) staff       (20)      350 2023-06-01 06:26:46.000000 libauc-1.3.0rc1/libauc/optimizers/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)     8837 2023-06-03 23:34:47.000000 libauc-1.3.0rc1/libauc/optimizers/adam.py
--rwx------   0 zhuoning   (501) staff       (20)     8708 2023-06-03 23:34:51.000000 libauc-1.3.0rc1/libauc/optimizers/adamw.py
--rwx------   0 zhuoning   (501) staff       (20)    12516 2023-06-08 19:29:52.000000 libauc-1.3.0rc1/libauc/optimizers/isogclr.py
--rw-r--r--   0 zhuoning   (501) staff       (20)     1760 2023-06-02 02:43:22.000000 libauc-1.3.0rc1/libauc/optimizers/lars.py
--rwx------   0 zhuoning   (501) staff       (20)     8217 2023-06-08 21:20:22.000000 libauc-1.3.0rc1/libauc/optimizers/midam.py
--rwx------   0 zhuoning   (501) staff       (20)    11371 2023-06-10 01:13:32.000000 libauc-1.3.0rc1/libauc/optimizers/pdsca.py
--rwx------   0 zhuoning   (501) staff       (20)    14361 2023-06-08 19:11:26.000000 libauc-1.3.0rc1/libauc/optimizers/pesg.py
--rwx------   0 zhuoning   (501) staff       (20)     8075 2023-06-03 23:33:49.000000 libauc-1.3.0rc1/libauc/optimizers/sgd.py
--rwx------   0 zhuoning   (501) staff       (20)    13151 2023-06-03 23:34:03.000000 libauc-1.3.0rc1/libauc/optimizers/soap.py
--rwx------   0 zhuoning   (501) staff       (20)    11517 2023-06-08 19:11:51.000000 libauc-1.3.0rc1/libauc/optimizers/sogclr.py
--rwx------   0 zhuoning   (501) staff       (20)    12325 2023-06-10 02:57:39.000000 libauc-1.3.0rc1/libauc/optimizers/song.py
--rwx------   0 zhuoning   (501) staff       (20)    12831 2023-06-03 23:34:26.000000 libauc-1.3.0rc1/libauc/optimizers/sopa.py
--rwx------   0 zhuoning   (501) staff       (20)    12949 2023-06-06 02:37:46.000000 libauc-1.3.0rc1/libauc/optimizers/sopa_s.py
--rwx------   0 zhuoning   (501) staff       (20)    12710 2023-06-09 06:11:28.000000 libauc-1.3.0rc1/libauc/optimizers/sota_s.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.077991 libauc-1.3.0rc1/libauc/sampler/
--rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:26.000000 libauc-1.3.0rc1/libauc/sampler/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    20484 2023-06-07 02:18:39.000000 libauc-1.3.0rc1/libauc/sampler/sampler.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.078357 libauc-1.3.0rc1/libauc/utils/
--rwx------   0 zhuoning   (501) staff       (20)       50 2023-06-01 06:26:50.000000 libauc-1.3.0rc1/libauc/utils/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    20155 2023-06-10 17:58:55.000000 libauc-1.3.0rc1/libauc/utils/paper_utils.py
--rwx------   0 zhuoning   (501) staff       (20)     4706 2023-06-11 05:06:33.000000 libauc-1.3.0rc1/libauc/utils/utils.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.072419 libauc-1.3.0rc1/libauc.egg-info/
--rw-r--r--   0 zhuoning   (501) staff       (20)     4162 2023-06-11 05:06:48.000000 libauc-1.3.0rc1/libauc.egg-info/PKG-INFO
--rw-r--r--   0 zhuoning   (501) staff       (20)     1470 2023-06-11 05:06:48.000000 libauc-1.3.0rc1/libauc.egg-info/SOURCES.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)        1 2023-06-11 05:06:48.000000 libauc-1.3.0rc1/libauc.egg-info/dependency_links.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)       76 2023-06-11 05:06:48.000000 libauc-1.3.0rc1/libauc.egg-info/requires.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)        7 2023-06-11 05:06:48.000000 libauc-1.3.0rc1/libauc.egg-info/top_level.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)       38 2023-06-11 05:06:48.078664 libauc-1.3.0rc1/setup.cfg
--rw-r--r--   0 zhuoning   (501) staff       (20)      982 2023-06-11 05:06:45.000000 libauc-1.3.0rc1/setup.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 18:27:34.650484 libauc-1.3.0rc3/
+-rwx------   0 zhuoning   (501) staff       (20)    11357 2023-03-02 14:10:38.000000 libauc-1.3.0rc3/LICENSE
+-rw-r--r--   0 zhuoning   (501) staff       (20)     4162 2023-06-11 18:27:34.650370 libauc-1.3.0rc3/PKG-INFO
+-rw-r--r--   0 zhuoning   (501) staff       (20)     3676 2023-06-11 04:07:50.000000 libauc-1.3.0rc3/README.md
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 18:27:34.643924 libauc-1.3.0rc3/libauc/
+-rwx------   0 zhuoning   (501) staff       (20)      112 2023-06-11 18:26:47.000000 libauc-1.3.0rc3/libauc/__init__.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 18:27:34.646037 libauc-1.3.0rc3/libauc/datasets/
+-rwx------   0 zhuoning   (501) staff       (20)      245 2023-06-09 06:42:38.000000 libauc-1.3.0rc3/libauc/datasets/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)     2621 2023-06-10 17:15:47.000000 libauc-1.3.0rc3/libauc/datasets/breastcancer.py
+-rwx------   0 zhuoning   (501) staff       (20)     2176 2023-06-10 17:15:53.000000 libauc-1.3.0rc3/libauc/datasets/cat_vs_dog.py
+-rwx------   0 zhuoning   (501) staff       (20)     9859 2023-05-18 04:21:28.000000 libauc-1.3.0rc3/libauc/datasets/chexpert.py
+-rwx------   0 zhuoning   (501) staff       (20)     6292 2023-05-24 19:24:50.000000 libauc-1.3.0rc3/libauc/datasets/cifar.py
+-rwx------   0 zhuoning   (501) staff       (20)     1561 2023-06-09 06:42:09.000000 libauc-1.3.0rc3/libauc/datasets/dataset.py
+-rwx------   0 zhuoning   (501) staff       (20)    12399 2023-03-09 21:50:47.000000 libauc-1.3.0rc3/libauc/datasets/folder.py
+-rwx------   0 zhuoning   (501) staff       (20)     4854 2023-06-07 00:13:14.000000 libauc-1.3.0rc3/libauc/datasets/melanoma.py
+-rwx------   0 zhuoning   (501) staff       (20)    13133 2023-06-07 00:16:53.000000 libauc-1.3.0rc3/libauc/datasets/movielens.py
+-rwx------   0 zhuoning   (501) staff       (20)     1497 2023-06-09 07:05:10.000000 libauc-1.3.0rc3/libauc/datasets/musk2.py
+-rwx------   0 zhuoning   (501) staff       (20)     2960 2023-03-02 14:10:38.000000 libauc-1.3.0rc3/libauc/datasets/stl10.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 18:27:34.647010 libauc-1.3.0rc3/libauc/losses/
+-rwx------   0 zhuoning   (501) staff       (20)      117 2023-06-07 19:59:42.000000 libauc-1.3.0rc3/libauc/losses/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    49557 2023-06-10 17:45:01.000000 libauc-1.3.0rc3/libauc/losses/auc.py
+-rwx------   0 zhuoning   (501) staff       (20)    23656 2023-06-08 21:47:59.000000 libauc-1.3.0rc3/libauc/losses/contrastive.py
+-rwx------   0 zhuoning   (501) staff       (20)     2893 2023-06-08 21:37:05.000000 libauc-1.3.0rc3/libauc/losses/losses.py
+-rwx------   0 zhuoning   (501) staff       (20)    15077 2023-06-10 06:44:38.000000 libauc-1.3.0rc3/libauc/losses/mil.py
+-rwx------   0 zhuoning   (501) staff       (20)     3038 2023-06-11 04:06:56.000000 libauc-1.3.0rc3/libauc/losses/perf_at_top.py
+-rwx------   0 zhuoning   (501) staff       (20)    12996 2023-06-11 04:07:47.000000 libauc-1.3.0rc3/libauc/losses/ranking.py
+-rwx------   0 zhuoning   (501) staff       (20)     2618 2023-06-03 03:28:07.000000 libauc-1.3.0rc3/libauc/losses/surrogate.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 18:27:34.647263 libauc-1.3.0rc3/libauc/metrics/
+-rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:29.000000 libauc-1.3.0rc3/libauc/metrics/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)     8479 2023-06-11 04:07:30.000000 libauc-1.3.0rc3/libauc/metrics/metrics.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 18:27:34.648037 libauc-1.3.0rc3/libauc/models/
+-rwx------   0 zhuoning   (501) staff       (20)      153 2023-05-26 02:45:25.000000 libauc-1.3.0rc3/libauc/models/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    13913 2023-05-18 03:12:04.000000 libauc-1.3.0rc3/libauc/models/densenet.py
+-rwx------   0 zhuoning   (501) staff       (20)     8626 2023-05-26 04:26:36.000000 libauc-1.3.0rc3/libauc/models/mil_models.py
+-rwx------   0 zhuoning   (501) staff       (20)     3479 2023-06-07 00:10:14.000000 libauc-1.3.0rc3/libauc/models/neumf.py
+-rwx------   0 zhuoning   (501) staff       (20)     1284 2023-06-07 00:11:49.000000 libauc-1.3.0rc3/libauc/models/perceptron.py
+-rwx------   0 zhuoning   (501) staff       (20)    16352 2023-05-18 03:13:49.000000 libauc-1.3.0rc3/libauc/models/resnet.py
+-rwx------   0 zhuoning   (501) staff       (20)     6836 2023-05-26 02:54:35.000000 libauc-1.3.0rc3/libauc/models/resnet_cifar.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 18:27:34.649674 libauc-1.3.0rc3/libauc/optimizers/
+-rwx------   0 zhuoning   (501) staff       (20)      350 2023-06-01 06:26:46.000000 libauc-1.3.0rc3/libauc/optimizers/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)     8837 2023-06-03 23:34:47.000000 libauc-1.3.0rc3/libauc/optimizers/adam.py
+-rwx------   0 zhuoning   (501) staff       (20)     8708 2023-06-03 23:34:51.000000 libauc-1.3.0rc3/libauc/optimizers/adamw.py
+-rwx------   0 zhuoning   (501) staff       (20)    12516 2023-06-08 19:29:52.000000 libauc-1.3.0rc3/libauc/optimizers/isogclr.py
+-rw-r--r--   0 zhuoning   (501) staff       (20)     1760 2023-06-02 02:43:22.000000 libauc-1.3.0rc3/libauc/optimizers/lars.py
+-rwx------   0 zhuoning   (501) staff       (20)     8217 2023-06-08 21:20:22.000000 libauc-1.3.0rc3/libauc/optimizers/midam.py
+-rwx------   0 zhuoning   (501) staff       (20)    11371 2023-06-10 01:13:32.000000 libauc-1.3.0rc3/libauc/optimizers/pdsca.py
+-rwx------   0 zhuoning   (501) staff       (20)    14361 2023-06-08 19:11:26.000000 libauc-1.3.0rc3/libauc/optimizers/pesg.py
+-rwx------   0 zhuoning   (501) staff       (20)     8075 2023-06-03 23:33:49.000000 libauc-1.3.0rc3/libauc/optimizers/sgd.py
+-rwx------   0 zhuoning   (501) staff       (20)    13151 2023-06-03 23:34:03.000000 libauc-1.3.0rc3/libauc/optimizers/soap.py
+-rwx------   0 zhuoning   (501) staff       (20)    11517 2023-06-08 19:11:51.000000 libauc-1.3.0rc3/libauc/optimizers/sogclr.py
+-rwx------   0 zhuoning   (501) staff       (20)    12325 2023-06-10 02:57:39.000000 libauc-1.3.0rc3/libauc/optimizers/song.py
+-rwx------   0 zhuoning   (501) staff       (20)    12831 2023-06-03 23:34:26.000000 libauc-1.3.0rc3/libauc/optimizers/sopa.py
+-rwx------   0 zhuoning   (501) staff       (20)    12949 2023-06-06 02:37:46.000000 libauc-1.3.0rc3/libauc/optimizers/sopa_s.py
+-rwx------   0 zhuoning   (501) staff       (20)    12710 2023-06-09 06:11:28.000000 libauc-1.3.0rc3/libauc/optimizers/sota_s.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 18:27:34.649879 libauc-1.3.0rc3/libauc/sampler/
+-rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:26.000000 libauc-1.3.0rc3/libauc/sampler/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    20482 2023-06-11 18:24:26.000000 libauc-1.3.0rc3/libauc/sampler/sampler.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 18:27:34.650220 libauc-1.3.0rc3/libauc/utils/
+-rwx------   0 zhuoning   (501) staff       (20)       50 2023-06-01 06:26:50.000000 libauc-1.3.0rc3/libauc/utils/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    20155 2023-06-10 17:58:55.000000 libauc-1.3.0rc3/libauc/utils/paper_utils.py
+-rwx------   0 zhuoning   (501) staff       (20)     4706 2023-06-11 05:08:04.000000 libauc-1.3.0rc3/libauc/utils/utils.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 18:27:34.644589 libauc-1.3.0rc3/libauc.egg-info/
+-rw-r--r--   0 zhuoning   (501) staff       (20)     4162 2023-06-11 18:27:34.000000 libauc-1.3.0rc3/libauc.egg-info/PKG-INFO
+-rw-r--r--   0 zhuoning   (501) staff       (20)     1470 2023-06-11 18:27:34.000000 libauc-1.3.0rc3/libauc.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)        1 2023-06-11 18:27:34.000000 libauc-1.3.0rc3/libauc.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)       76 2023-06-11 18:27:34.000000 libauc-1.3.0rc3/libauc.egg-info/requires.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)        7 2023-06-11 18:27:34.000000 libauc-1.3.0rc3/libauc.egg-info/top_level.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)       38 2023-06-11 18:27:34.650521 libauc-1.3.0rc3/setup.cfg
+-rw-r--r--   0 zhuoning   (501) staff       (20)      982 2023-06-11 18:26:46.000000 libauc-1.3.0rc3/setup.py
```

### Comparing `libauc-1.3.0rc1/LICENSE` & `libauc-1.3.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/PKG-INFO` & `libauc-1.3.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libauc
-Version: 1.3.0rc1
+Version: 1.3.0rc3
 Summary: LibAUC: A Deep Learning Library for X-Risk Optimization
 Home-page: https://github.com/Optimization-AI/LibAUC
 Author: Zhuoning Yuan
 Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc1 Summary: LibAUC: A Deep
+Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc3 Summary: LibAUC: A Deep
 Learning Library for X-Risk Optimization Home-page: https://github.com/
 Optimization-AI/LibAUC Author: Zhuoning Yuan Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE LibAUC: A Deep Learning for X-Risk Optimization
 ---
```

### Comparing `libauc-1.3.0rc1/README.md` & `libauc-1.3.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/datasets/breastcancer.py` & `libauc-1.3.0rc3/libauc/datasets/breastcancer.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/datasets/cat_vs_dog.py` & `libauc-1.3.0rc3/libauc/datasets/cat_vs_dog.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/datasets/chexpert.py` & `libauc-1.3.0rc3/libauc/datasets/chexpert.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/datasets/cifar.py` & `libauc-1.3.0rc3/libauc/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/datasets/dataset.py` & `libauc-1.3.0rc3/libauc/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/datasets/folder.py` & `libauc-1.3.0rc3/libauc/datasets/folder.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/datasets/melanoma.py` & `libauc-1.3.0rc3/libauc/datasets/melanoma.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/datasets/movielens.py` & `libauc-1.3.0rc3/libauc/datasets/movielens.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/datasets/musk2.py` & `libauc-1.3.0rc3/libauc/datasets/musk2.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/datasets/stl10.py` & `libauc-1.3.0rc3/libauc/datasets/stl10.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/losses/auc.py` & `libauc-1.3.0rc3/libauc/losses/auc.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/losses/contrastive.py` & `libauc-1.3.0rc3/libauc/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/losses/losses.py` & `libauc-1.3.0rc3/libauc/losses/losses.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/losses/mil.py` & `libauc-1.3.0rc3/libauc/losses/mil.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/losses/perf_at_top.py` & `libauc-1.3.0rc3/libauc/losses/perf_at_top.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/losses/ranking.py` & `libauc-1.3.0rc3/libauc/losses/ranking.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/losses/surrogate.py` & `libauc-1.3.0rc3/libauc/losses/surrogate.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/metrics/metrics.py` & `libauc-1.3.0rc3/libauc/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/models/densenet.py` & `libauc-1.3.0rc3/libauc/models/densenet.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/models/mil_models.py` & `libauc-1.3.0rc3/libauc/models/mil_models.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/models/neumf.py` & `libauc-1.3.0rc3/libauc/models/neumf.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/models/perceptron.py` & `libauc-1.3.0rc3/libauc/models/perceptron.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/models/resnet.py` & `libauc-1.3.0rc3/libauc/models/resnet.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/models/resnet_cifar.py` & `libauc-1.3.0rc3/libauc/models/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/optimizers/adam.py` & `libauc-1.3.0rc3/libauc/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/optimizers/adamw.py` & `libauc-1.3.0rc3/libauc/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/optimizers/isogclr.py` & `libauc-1.3.0rc3/libauc/optimizers/isogclr.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/optimizers/lars.py` & `libauc-1.3.0rc3/libauc/optimizers/lars.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/optimizers/midam.py` & `libauc-1.3.0rc3/libauc/optimizers/midam.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/optimizers/pdsca.py` & `libauc-1.3.0rc3/libauc/optimizers/pdsca.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/optimizers/pesg.py` & `libauc-1.3.0rc3/libauc/optimizers/pesg.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/optimizers/sgd.py` & `libauc-1.3.0rc3/libauc/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/optimizers/soap.py` & `libauc-1.3.0rc3/libauc/optimizers/soap.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/optimizers/sogclr.py` & `libauc-1.3.0rc3/libauc/optimizers/sogclr.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/optimizers/song.py` & `libauc-1.3.0rc3/libauc/optimizers/song.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/optimizers/sopa.py` & `libauc-1.3.0rc3/libauc/optimizers/sopa.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/optimizers/sopa_s.py` & `libauc-1.3.0rc3/libauc/optimizers/sopa_s.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/optimizers/sota_s.py` & `libauc-1.3.0rc3/libauc/optimizers/sota_s.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/sampler/sampler.py` & `libauc-1.3.0rc3/libauc/sampler/sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,26 +112,26 @@
        dict = {}
        if num_sampled_task == 2: 
            task_id = 0   # binary data, i.e. num_sampled_task == 1
            dict[task_id] = (np.count_nonzero(labels == 1), np.count_nonzero(labels == 0) )
        else:
            task_ids = np.arange(num_sampled_task)              
            for task_id in task_ids:
-               dict[task_id] = (np.count_nonzero(labels[:, task_id] == 1), np.count_nonzero(labels[:, task_id] == 0) )
+               dict[task_id] = (np.count_nonzero(labels[:, task_id] > 0), np.count_nonzero(labels[:, task_id] == 0) )
        return dict
 
     def _get_sample_class_indices(self, labels, num_sampled_task=None):
         r"""Extract sample indices for postives and negatives per label (task)."""
         if not num_sampled_task:
            num_sampled_task = self._get_num_tasks(labels)
         num_sampled_task = num_sampled_task - 1 if num_sampled_task == 2 else num_sampled_task    
         pos_indices, neg_indices = {}, {}
         for task_id in range(num_sampled_task):
              label_t = labels[:, task_id] if num_sampled_task > 2 else labels
-             pos_idx = np.flatnonzero(label_t==1)
+             pos_idx = np.flatnonzero(label_t>0)
              neg_idx = np.flatnonzero(label_t==0)
              if self.shuffle:
                 np.random.shuffle(pos_idx), np.random.shuffle(neg_idx)
              pos_indices[task_id] = pos_idx
              neg_indices[task_id] = neg_idx
         return pos_indices, neg_indices
```

### Comparing `libauc-1.3.0rc1/libauc/utils/paper_utils.py` & `libauc-1.3.0rc3/libauc/utils/paper_utils.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc/utils/utils.py` & `libauc-1.3.0rc3/libauc/utils/utils.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/libauc.egg-info/PKG-INFO` & `libauc-1.3.0rc3/libauc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libauc
-Version: 1.3.0rc1
+Version: 1.3.0rc3
 Summary: LibAUC: A Deep Learning Library for X-Risk Optimization
 Home-page: https://github.com/Optimization-AI/LibAUC
 Author: Zhuoning Yuan
 Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc1 Summary: LibAUC: A Deep
+Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc3 Summary: LibAUC: A Deep
 Learning Library for X-Risk Optimization Home-page: https://github.com/
 Optimization-AI/LibAUC Author: Zhuoning Yuan Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE LibAUC: A Deep Learning for X-Risk Optimization
 ---
```

### Comparing `libauc-1.3.0rc1/libauc.egg-info/SOURCES.txt` & `libauc-1.3.0rc3/libauc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc1/setup.py` & `libauc-1.3.0rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
   
 setuptools.setup(
   name="libauc",
-  version="1.3.0rc1",
+  version="1.3.0rc3",
   author="Zhuoning Yuan",
   author_email="yzhuoning@gmail.com",
   description="LibAUC: A Deep Learning Library for X-Risk Optimization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/Optimization-AI/LibAUC",
   packages=setuptools.find_packages(),
```

