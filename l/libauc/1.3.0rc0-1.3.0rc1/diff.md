# Comparing `tmp/libauc-1.3.0rc0.tar.gz` & `tmp/libauc-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libauc-1.3.0rc0.tar", last modified: Sun Jun 11 04:14:37 2023, max compression
+gzip compressed data, was "libauc-1.3.0rc1.tar", last modified: Sun Jun 11 05:06:48 2023, max compression
```

## Comparing `libauc-1.3.0rc0.tar` & `libauc-1.3.0rc1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 04:14:37.882326 libauc-1.3.0rc0/
--rwx------   0 zhuoning   (501) staff       (20)    11357 2023-03-02 14:10:38.000000 libauc-1.3.0rc0/LICENSE
--rw-r--r--   0 zhuoning   (501) staff       (20)     4162 2023-06-11 04:14:37.882214 libauc-1.3.0rc0/PKG-INFO
--rw-r--r--   0 zhuoning   (501) staff       (20)     3676 2023-06-11 04:07:50.000000 libauc-1.3.0rc0/README.md
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 04:14:37.875684 libauc-1.3.0rc0/libauc/
--rwx------   0 zhuoning   (501) staff       (20)      112 2023-06-11 04:05:57.000000 libauc-1.3.0rc0/libauc/__init__.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 04:14:37.877754 libauc-1.3.0rc0/libauc/datasets/
--rwx------   0 zhuoning   (501) staff       (20)      245 2023-06-09 06:42:38.000000 libauc-1.3.0rc0/libauc/datasets/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)     2621 2023-06-10 17:15:47.000000 libauc-1.3.0rc0/libauc/datasets/breastcancer.py
--rwx------   0 zhuoning   (501) staff       (20)     2176 2023-06-10 17:15:53.000000 libauc-1.3.0rc0/libauc/datasets/cat_vs_dog.py
--rwx------   0 zhuoning   (501) staff       (20)     9859 2023-05-18 04:21:28.000000 libauc-1.3.0rc0/libauc/datasets/chexpert.py
--rwx------   0 zhuoning   (501) staff       (20)     6292 2023-05-24 19:24:50.000000 libauc-1.3.0rc0/libauc/datasets/cifar.py
--rwx------   0 zhuoning   (501) staff       (20)     1561 2023-06-09 06:42:09.000000 libauc-1.3.0rc0/libauc/datasets/dataset.py
--rwx------   0 zhuoning   (501) staff       (20)    12399 2023-03-09 21:50:47.000000 libauc-1.3.0rc0/libauc/datasets/folder.py
--rwx------   0 zhuoning   (501) staff       (20)     4854 2023-06-07 00:13:14.000000 libauc-1.3.0rc0/libauc/datasets/melanoma.py
--rwx------   0 zhuoning   (501) staff       (20)    13133 2023-06-07 00:16:53.000000 libauc-1.3.0rc0/libauc/datasets/movielens.py
--rwx------   0 zhuoning   (501) staff       (20)     1497 2023-06-09 07:05:10.000000 libauc-1.3.0rc0/libauc/datasets/musk2.py
--rwx------   0 zhuoning   (501) staff       (20)     2960 2023-03-02 14:10:38.000000 libauc-1.3.0rc0/libauc/datasets/stl10.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 04:14:37.878766 libauc-1.3.0rc0/libauc/losses/
--rwx------   0 zhuoning   (501) staff       (20)      117 2023-06-07 19:59:42.000000 libauc-1.3.0rc0/libauc/losses/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    49557 2023-06-10 17:45:01.000000 libauc-1.3.0rc0/libauc/losses/auc.py
--rwx------   0 zhuoning   (501) staff       (20)    23656 2023-06-08 21:47:59.000000 libauc-1.3.0rc0/libauc/losses/contrastive.py
--rwx------   0 zhuoning   (501) staff       (20)     2893 2023-06-08 21:37:05.000000 libauc-1.3.0rc0/libauc/losses/losses.py
--rwx------   0 zhuoning   (501) staff       (20)    15077 2023-06-10 06:44:38.000000 libauc-1.3.0rc0/libauc/losses/mil.py
--rwx------   0 zhuoning   (501) staff       (20)     3038 2023-06-11 04:06:56.000000 libauc-1.3.0rc0/libauc/losses/perf_at_top.py
--rwx------   0 zhuoning   (501) staff       (20)    12996 2023-06-11 04:07:47.000000 libauc-1.3.0rc0/libauc/losses/ranking.py
--rwx------   0 zhuoning   (501) staff       (20)     2618 2023-06-03 03:28:07.000000 libauc-1.3.0rc0/libauc/losses/surrogate.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 04:14:37.879005 libauc-1.3.0rc0/libauc/metrics/
--rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:29.000000 libauc-1.3.0rc0/libauc/metrics/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)     8479 2023-06-11 04:07:30.000000 libauc-1.3.0rc0/libauc/metrics/metrics.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 04:14:37.879827 libauc-1.3.0rc0/libauc/models/
--rwx------   0 zhuoning   (501) staff       (20)      153 2023-05-26 02:45:25.000000 libauc-1.3.0rc0/libauc/models/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    13913 2023-05-18 03:12:04.000000 libauc-1.3.0rc0/libauc/models/densenet.py
--rwx------   0 zhuoning   (501) staff       (20)     8626 2023-05-26 04:26:36.000000 libauc-1.3.0rc0/libauc/models/mil_models.py
--rwx------   0 zhuoning   (501) staff       (20)     3479 2023-06-07 00:10:14.000000 libauc-1.3.0rc0/libauc/models/neumf.py
--rwx------   0 zhuoning   (501) staff       (20)     1284 2023-06-07 00:11:49.000000 libauc-1.3.0rc0/libauc/models/perceptron.py
--rwx------   0 zhuoning   (501) staff       (20)    16352 2023-05-18 03:13:49.000000 libauc-1.3.0rc0/libauc/models/resnet.py
--rwx------   0 zhuoning   (501) staff       (20)     6836 2023-05-26 02:54:35.000000 libauc-1.3.0rc0/libauc/models/resnet_cifar.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 04:14:37.881474 libauc-1.3.0rc0/libauc/optimizers/
--rwx------   0 zhuoning   (501) staff       (20)      350 2023-06-01 06:26:46.000000 libauc-1.3.0rc0/libauc/optimizers/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)     8837 2023-06-03 23:34:47.000000 libauc-1.3.0rc0/libauc/optimizers/adam.py
--rwx------   0 zhuoning   (501) staff       (20)     8708 2023-06-03 23:34:51.000000 libauc-1.3.0rc0/libauc/optimizers/adamw.py
--rwx------   0 zhuoning   (501) staff       (20)    12516 2023-06-08 19:29:52.000000 libauc-1.3.0rc0/libauc/optimizers/isogclr.py
--rw-r--r--   0 zhuoning   (501) staff       (20)     1760 2023-06-02 02:43:22.000000 libauc-1.3.0rc0/libauc/optimizers/lars.py
--rwx------   0 zhuoning   (501) staff       (20)     8217 2023-06-08 21:20:22.000000 libauc-1.3.0rc0/libauc/optimizers/midam.py
--rwx------   0 zhuoning   (501) staff       (20)    11371 2023-06-10 01:13:32.000000 libauc-1.3.0rc0/libauc/optimizers/pdsca.py
--rwx------   0 zhuoning   (501) staff       (20)    14361 2023-06-08 19:11:26.000000 libauc-1.3.0rc0/libauc/optimizers/pesg.py
--rwx------   0 zhuoning   (501) staff       (20)     8075 2023-06-03 23:33:49.000000 libauc-1.3.0rc0/libauc/optimizers/sgd.py
--rwx------   0 zhuoning   (501) staff       (20)    13151 2023-06-03 23:34:03.000000 libauc-1.3.0rc0/libauc/optimizers/soap.py
--rwx------   0 zhuoning   (501) staff       (20)    11517 2023-06-08 19:11:51.000000 libauc-1.3.0rc0/libauc/optimizers/sogclr.py
--rwx------   0 zhuoning   (501) staff       (20)    12325 2023-06-10 02:57:39.000000 libauc-1.3.0rc0/libauc/optimizers/song.py
--rwx------   0 zhuoning   (501) staff       (20)    12831 2023-06-03 23:34:26.000000 libauc-1.3.0rc0/libauc/optimizers/sopa.py
--rwx------   0 zhuoning   (501) staff       (20)    12949 2023-06-06 02:37:46.000000 libauc-1.3.0rc0/libauc/optimizers/sopa_s.py
--rwx------   0 zhuoning   (501) staff       (20)    12710 2023-06-09 06:11:28.000000 libauc-1.3.0rc0/libauc/optimizers/sota_s.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 04:14:37.881681 libauc-1.3.0rc0/libauc/sampler/
--rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:26.000000 libauc-1.3.0rc0/libauc/sampler/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    20484 2023-06-07 02:18:39.000000 libauc-1.3.0rc0/libauc/sampler/sampler.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 04:14:37.882050 libauc-1.3.0rc0/libauc/utils/
--rwx------   0 zhuoning   (501) staff       (20)       50 2023-06-01 06:26:50.000000 libauc-1.3.0rc0/libauc/utils/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    20155 2023-06-10 17:58:55.000000 libauc-1.3.0rc0/libauc/utils/paper_utils.py
--rwx------   0 zhuoning   (501) staff       (20)     4657 2023-06-10 18:00:32.000000 libauc-1.3.0rc0/libauc/utils/utils.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 04:14:37.876370 libauc-1.3.0rc0/libauc.egg-info/
--rw-r--r--   0 zhuoning   (501) staff       (20)     4162 2023-06-11 04:14:37.000000 libauc-1.3.0rc0/libauc.egg-info/PKG-INFO
--rw-r--r--   0 zhuoning   (501) staff       (20)     1470 2023-06-11 04:14:37.000000 libauc-1.3.0rc0/libauc.egg-info/SOURCES.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)        1 2023-06-11 04:14:37.000000 libauc-1.3.0rc0/libauc.egg-info/dependency_links.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)       76 2023-06-11 04:14:37.000000 libauc-1.3.0rc0/libauc.egg-info/requires.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)        7 2023-06-11 04:14:37.000000 libauc-1.3.0rc0/libauc.egg-info/top_level.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)       38 2023-06-11 04:14:37.882364 libauc-1.3.0rc0/setup.cfg
--rw-r--r--   0 zhuoning   (501) staff       (20)      982 2023-06-11 04:07:49.000000 libauc-1.3.0rc0/setup.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.078628 libauc-1.3.0rc1/
+-rwx------   0 zhuoning   (501) staff       (20)    11357 2023-03-02 14:10:38.000000 libauc-1.3.0rc1/LICENSE
+-rw-r--r--   0 zhuoning   (501) staff       (20)     4162 2023-06-11 05:06:48.078515 libauc-1.3.0rc1/PKG-INFO
+-rw-r--r--   0 zhuoning   (501) staff       (20)     3676 2023-06-11 04:07:50.000000 libauc-1.3.0rc1/README.md
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.071776 libauc-1.3.0rc1/libauc/
+-rwx------   0 zhuoning   (501) staff       (20)      112 2023-06-11 05:06:46.000000 libauc-1.3.0rc1/libauc/__init__.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.073787 libauc-1.3.0rc1/libauc/datasets/
+-rwx------   0 zhuoning   (501) staff       (20)      245 2023-06-09 06:42:38.000000 libauc-1.3.0rc1/libauc/datasets/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)     2621 2023-06-10 17:15:47.000000 libauc-1.3.0rc1/libauc/datasets/breastcancer.py
+-rwx------   0 zhuoning   (501) staff       (20)     2176 2023-06-10 17:15:53.000000 libauc-1.3.0rc1/libauc/datasets/cat_vs_dog.py
+-rwx------   0 zhuoning   (501) staff       (20)     9859 2023-05-18 04:21:28.000000 libauc-1.3.0rc1/libauc/datasets/chexpert.py
+-rwx------   0 zhuoning   (501) staff       (20)     6292 2023-05-24 19:24:50.000000 libauc-1.3.0rc1/libauc/datasets/cifar.py
+-rwx------   0 zhuoning   (501) staff       (20)     1561 2023-06-09 06:42:09.000000 libauc-1.3.0rc1/libauc/datasets/dataset.py
+-rwx------   0 zhuoning   (501) staff       (20)    12399 2023-03-09 21:50:47.000000 libauc-1.3.0rc1/libauc/datasets/folder.py
+-rwx------   0 zhuoning   (501) staff       (20)     4854 2023-06-07 00:13:14.000000 libauc-1.3.0rc1/libauc/datasets/melanoma.py
+-rwx------   0 zhuoning   (501) staff       (20)    13133 2023-06-07 00:16:53.000000 libauc-1.3.0rc1/libauc/datasets/movielens.py
+-rwx------   0 zhuoning   (501) staff       (20)     1497 2023-06-09 07:05:10.000000 libauc-1.3.0rc1/libauc/datasets/musk2.py
+-rwx------   0 zhuoning   (501) staff       (20)     2960 2023-03-02 14:10:38.000000 libauc-1.3.0rc1/libauc/datasets/stl10.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.075147 libauc-1.3.0rc1/libauc/losses/
+-rwx------   0 zhuoning   (501) staff       (20)      117 2023-06-07 19:59:42.000000 libauc-1.3.0rc1/libauc/losses/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    49557 2023-06-10 17:45:01.000000 libauc-1.3.0rc1/libauc/losses/auc.py
+-rwx------   0 zhuoning   (501) staff       (20)    23656 2023-06-08 21:47:59.000000 libauc-1.3.0rc1/libauc/losses/contrastive.py
+-rwx------   0 zhuoning   (501) staff       (20)     2893 2023-06-08 21:37:05.000000 libauc-1.3.0rc1/libauc/losses/losses.py
+-rwx------   0 zhuoning   (501) staff       (20)    15077 2023-06-10 06:44:38.000000 libauc-1.3.0rc1/libauc/losses/mil.py
+-rwx------   0 zhuoning   (501) staff       (20)     3038 2023-06-11 04:06:56.000000 libauc-1.3.0rc1/libauc/losses/perf_at_top.py
+-rwx------   0 zhuoning   (501) staff       (20)    12996 2023-06-11 04:07:47.000000 libauc-1.3.0rc1/libauc/losses/ranking.py
+-rwx------   0 zhuoning   (501) staff       (20)     2618 2023-06-03 03:28:07.000000 libauc-1.3.0rc1/libauc/losses/surrogate.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.075359 libauc-1.3.0rc1/libauc/metrics/
+-rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:29.000000 libauc-1.3.0rc1/libauc/metrics/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)     8479 2023-06-11 04:07:30.000000 libauc-1.3.0rc1/libauc/metrics/metrics.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.076106 libauc-1.3.0rc1/libauc/models/
+-rwx------   0 zhuoning   (501) staff       (20)      153 2023-05-26 02:45:25.000000 libauc-1.3.0rc1/libauc/models/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    13913 2023-05-18 03:12:04.000000 libauc-1.3.0rc1/libauc/models/densenet.py
+-rwx------   0 zhuoning   (501) staff       (20)     8626 2023-05-26 04:26:36.000000 libauc-1.3.0rc1/libauc/models/mil_models.py
+-rwx------   0 zhuoning   (501) staff       (20)     3479 2023-06-07 00:10:14.000000 libauc-1.3.0rc1/libauc/models/neumf.py
+-rwx------   0 zhuoning   (501) staff       (20)     1284 2023-06-07 00:11:49.000000 libauc-1.3.0rc1/libauc/models/perceptron.py
+-rwx------   0 zhuoning   (501) staff       (20)    16352 2023-05-18 03:13:49.000000 libauc-1.3.0rc1/libauc/models/resnet.py
+-rwx------   0 zhuoning   (501) staff       (20)     6836 2023-05-26 02:54:35.000000 libauc-1.3.0rc1/libauc/models/resnet_cifar.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.077772 libauc-1.3.0rc1/libauc/optimizers/
+-rwx------   0 zhuoning   (501) staff       (20)      350 2023-06-01 06:26:46.000000 libauc-1.3.0rc1/libauc/optimizers/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)     8837 2023-06-03 23:34:47.000000 libauc-1.3.0rc1/libauc/optimizers/adam.py
+-rwx------   0 zhuoning   (501) staff       (20)     8708 2023-06-03 23:34:51.000000 libauc-1.3.0rc1/libauc/optimizers/adamw.py
+-rwx------   0 zhuoning   (501) staff       (20)    12516 2023-06-08 19:29:52.000000 libauc-1.3.0rc1/libauc/optimizers/isogclr.py
+-rw-r--r--   0 zhuoning   (501) staff       (20)     1760 2023-06-02 02:43:22.000000 libauc-1.3.0rc1/libauc/optimizers/lars.py
+-rwx------   0 zhuoning   (501) staff       (20)     8217 2023-06-08 21:20:22.000000 libauc-1.3.0rc1/libauc/optimizers/midam.py
+-rwx------   0 zhuoning   (501) staff       (20)    11371 2023-06-10 01:13:32.000000 libauc-1.3.0rc1/libauc/optimizers/pdsca.py
+-rwx------   0 zhuoning   (501) staff       (20)    14361 2023-06-08 19:11:26.000000 libauc-1.3.0rc1/libauc/optimizers/pesg.py
+-rwx------   0 zhuoning   (501) staff       (20)     8075 2023-06-03 23:33:49.000000 libauc-1.3.0rc1/libauc/optimizers/sgd.py
+-rwx------   0 zhuoning   (501) staff       (20)    13151 2023-06-03 23:34:03.000000 libauc-1.3.0rc1/libauc/optimizers/soap.py
+-rwx------   0 zhuoning   (501) staff       (20)    11517 2023-06-08 19:11:51.000000 libauc-1.3.0rc1/libauc/optimizers/sogclr.py
+-rwx------   0 zhuoning   (501) staff       (20)    12325 2023-06-10 02:57:39.000000 libauc-1.3.0rc1/libauc/optimizers/song.py
+-rwx------   0 zhuoning   (501) staff       (20)    12831 2023-06-03 23:34:26.000000 libauc-1.3.0rc1/libauc/optimizers/sopa.py
+-rwx------   0 zhuoning   (501) staff       (20)    12949 2023-06-06 02:37:46.000000 libauc-1.3.0rc1/libauc/optimizers/sopa_s.py
+-rwx------   0 zhuoning   (501) staff       (20)    12710 2023-06-09 06:11:28.000000 libauc-1.3.0rc1/libauc/optimizers/sota_s.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.077991 libauc-1.3.0rc1/libauc/sampler/
+-rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:26.000000 libauc-1.3.0rc1/libauc/sampler/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    20484 2023-06-07 02:18:39.000000 libauc-1.3.0rc1/libauc/sampler/sampler.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.078357 libauc-1.3.0rc1/libauc/utils/
+-rwx------   0 zhuoning   (501) staff       (20)       50 2023-06-01 06:26:50.000000 libauc-1.3.0rc1/libauc/utils/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    20155 2023-06-10 17:58:55.000000 libauc-1.3.0rc1/libauc/utils/paper_utils.py
+-rwx------   0 zhuoning   (501) staff       (20)     4706 2023-06-11 05:06:33.000000 libauc-1.3.0rc1/libauc/utils/utils.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 05:06:48.072419 libauc-1.3.0rc1/libauc.egg-info/
+-rw-r--r--   0 zhuoning   (501) staff       (20)     4162 2023-06-11 05:06:48.000000 libauc-1.3.0rc1/libauc.egg-info/PKG-INFO
+-rw-r--r--   0 zhuoning   (501) staff       (20)     1470 2023-06-11 05:06:48.000000 libauc-1.3.0rc1/libauc.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)        1 2023-06-11 05:06:48.000000 libauc-1.3.0rc1/libauc.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)       76 2023-06-11 05:06:48.000000 libauc-1.3.0rc1/libauc.egg-info/requires.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)        7 2023-06-11 05:06:48.000000 libauc-1.3.0rc1/libauc.egg-info/top_level.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)       38 2023-06-11 05:06:48.078664 libauc-1.3.0rc1/setup.cfg
+-rw-r--r--   0 zhuoning   (501) staff       (20)      982 2023-06-11 05:06:45.000000 libauc-1.3.0rc1/setup.py
```

### Comparing `libauc-1.3.0rc0/LICENSE` & `libauc-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/PKG-INFO` & `libauc-1.3.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libauc
-Version: 1.3.0rc0
+Version: 1.3.0rc1
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
-Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc0 Summary: LibAUC: A Deep
+Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc1 Summary: LibAUC: A Deep
 Learning Library for X-Risk Optimization Home-page: https://github.com/
 Optimization-AI/LibAUC Author: Zhuoning Yuan Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE LibAUC: A Deep Learning for X-Risk Optimization
 ---
```

### Comparing `libauc-1.3.0rc0/README.md` & `libauc-1.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/datasets/breastcancer.py` & `libauc-1.3.0rc1/libauc/datasets/breastcancer.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/datasets/cat_vs_dog.py` & `libauc-1.3.0rc1/libauc/datasets/cat_vs_dog.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/datasets/chexpert.py` & `libauc-1.3.0rc1/libauc/datasets/chexpert.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/datasets/cifar.py` & `libauc-1.3.0rc1/libauc/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/datasets/dataset.py` & `libauc-1.3.0rc1/libauc/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/datasets/folder.py` & `libauc-1.3.0rc1/libauc/datasets/folder.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/datasets/melanoma.py` & `libauc-1.3.0rc1/libauc/datasets/melanoma.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/datasets/movielens.py` & `libauc-1.3.0rc1/libauc/datasets/movielens.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/datasets/musk2.py` & `libauc-1.3.0rc1/libauc/datasets/musk2.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/datasets/stl10.py` & `libauc-1.3.0rc1/libauc/datasets/stl10.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/losses/auc.py` & `libauc-1.3.0rc1/libauc/losses/auc.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/losses/contrastive.py` & `libauc-1.3.0rc1/libauc/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/losses/losses.py` & `libauc-1.3.0rc1/libauc/losses/losses.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/losses/mil.py` & `libauc-1.3.0rc1/libauc/losses/mil.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/losses/perf_at_top.py` & `libauc-1.3.0rc1/libauc/losses/perf_at_top.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/losses/ranking.py` & `libauc-1.3.0rc1/libauc/losses/ranking.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/losses/surrogate.py` & `libauc-1.3.0rc1/libauc/losses/surrogate.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/metrics/metrics.py` & `libauc-1.3.0rc1/libauc/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/models/densenet.py` & `libauc-1.3.0rc1/libauc/models/densenet.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/models/mil_models.py` & `libauc-1.3.0rc1/libauc/models/mil_models.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/models/neumf.py` & `libauc-1.3.0rc1/libauc/models/neumf.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/models/perceptron.py` & `libauc-1.3.0rc1/libauc/models/perceptron.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/models/resnet.py` & `libauc-1.3.0rc1/libauc/models/resnet.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/models/resnet_cifar.py` & `libauc-1.3.0rc1/libauc/models/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/optimizers/adam.py` & `libauc-1.3.0rc1/libauc/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/optimizers/adamw.py` & `libauc-1.3.0rc1/libauc/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/optimizers/isogclr.py` & `libauc-1.3.0rc1/libauc/optimizers/isogclr.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/optimizers/lars.py` & `libauc-1.3.0rc1/libauc/optimizers/lars.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/optimizers/midam.py` & `libauc-1.3.0rc1/libauc/optimizers/midam.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/optimizers/pdsca.py` & `libauc-1.3.0rc1/libauc/optimizers/pdsca.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/optimizers/pesg.py` & `libauc-1.3.0rc1/libauc/optimizers/pesg.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/optimizers/sgd.py` & `libauc-1.3.0rc1/libauc/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/optimizers/soap.py` & `libauc-1.3.0rc1/libauc/optimizers/soap.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/optimizers/sogclr.py` & `libauc-1.3.0rc1/libauc/optimizers/sogclr.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/optimizers/song.py` & `libauc-1.3.0rc1/libauc/optimizers/song.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/optimizers/sopa.py` & `libauc-1.3.0rc1/libauc/optimizers/sopa.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/optimizers/sopa_s.py` & `libauc-1.3.0rc1/libauc/optimizers/sopa_s.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/optimizers/sota_s.py` & `libauc-1.3.0rc1/libauc/optimizers/sota_s.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/sampler/sampler.py` & `libauc-1.3.0rc1/libauc/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/utils/paper_utils.py` & `libauc-1.3.0rc1/libauc/utils/paper_utils.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/libauc/utils/utils.py` & `libauc-1.3.0rc1/libauc/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,16 +109,16 @@
         targets = np.maximum(targets, 0)
         if imratio is not None:
             self.imratio = imratio
         if self.imratio is None:
             raise ValueError("imratio is None.")
         assert self.imratio > 0 and self.imratio <= 0.5, 'imratio needs to be in (0, 0.5)!'
        
-        np.random.seed(self.random_seed)
         if self.shuffle:
+            np.random.seed(self.random_seed)
             idx = np.random.permutation(len(targets))
             data, targets = data[idx], targets[idx]
 
         num_classes = self._get_class_num(targets)
         split_index = self._get_split_index(num_classes)
         targets = np.where(targets <= split_index, 0, 1)
 
@@ -127,14 +127,15 @@
             pos_ids = np.where(targets == 1)[0]
             pos_ids = pos_ids[:int((self.imratio / (1 - self.imratio)) * len(neg_ids))]
             idx = np.concatenate([neg_ids, pos_ids])
             data, targets = data[idx], targets[idx]
             targets = targets.reshape(-1, 1).astype(np.float32)
 
         if self.shuffle:
+            np.random.seed(self.random_seed)
             idx = np.random.permutation(len(targets))
             data, targets = data[idx], targets[idx]
             
         if self.verbose:
             check_imbalance_ratio(targets)
 
         return data, targets
```

### Comparing `libauc-1.3.0rc0/libauc.egg-info/PKG-INFO` & `libauc-1.3.0rc1/libauc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libauc
-Version: 1.3.0rc0
+Version: 1.3.0rc1
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
-Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc0 Summary: LibAUC: A Deep
+Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc1 Summary: LibAUC: A Deep
 Learning Library for X-Risk Optimization Home-page: https://github.com/
 Optimization-AI/LibAUC Author: Zhuoning Yuan Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE LibAUC: A Deep Learning for X-Risk Optimization
 ---
```

### Comparing `libauc-1.3.0rc0/libauc.egg-info/SOURCES.txt` & `libauc-1.3.0rc1/libauc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc0/setup.py` & `libauc-1.3.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
   
 setuptools.setup(
   name="libauc",
-  version="1.3.0rc0",
+  version="1.3.0rc1",
   author="Zhuoning Yuan",
   author_email="yzhuoning@gmail.com",
   description="LibAUC: A Deep Learning Library for X-Risk Optimization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/Optimization-AI/LibAUC",
   packages=setuptools.find_packages(),
```

