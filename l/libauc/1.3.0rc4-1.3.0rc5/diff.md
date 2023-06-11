# Comparing `tmp/libauc-1.3.0rc4.tar.gz` & `tmp/libauc-1.3.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libauc-1.3.0rc4.tar", last modified: Sun Jun 11 19:57:09 2023, max compression
+gzip compressed data, was "libauc-1.3.0rc5.tar", last modified: Sun Jun 11 21:05:51 2023, max compression
```

## Comparing `libauc-1.3.0rc4.tar` & `libauc-1.3.0rc5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 19:57:09.446621 libauc-1.3.0rc4/
--rwx------   0 zhuoning   (501) staff       (20)    11357 2023-03-02 14:10:38.000000 libauc-1.3.0rc4/LICENSE
--rw-r--r--   0 zhuoning   (501) staff       (20)     4162 2023-06-11 19:57:09.446521 libauc-1.3.0rc4/PKG-INFO
--rw-r--r--   0 zhuoning   (501) staff       (20)     3676 2023-06-11 04:07:50.000000 libauc-1.3.0rc4/README.md
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 19:57:09.440160 libauc-1.3.0rc4/libauc/
--rwx------   0 zhuoning   (501) staff       (20)      112 2023-06-11 19:56:45.000000 libauc-1.3.0rc4/libauc/__init__.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 19:57:09.441988 libauc-1.3.0rc4/libauc/datasets/
--rwx------   0 zhuoning   (501) staff       (20)      245 2023-06-09 06:42:38.000000 libauc-1.3.0rc4/libauc/datasets/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)     2621 2023-06-10 17:15:47.000000 libauc-1.3.0rc4/libauc/datasets/breastcancer.py
--rwx------   0 zhuoning   (501) staff       (20)     2176 2023-06-10 17:15:53.000000 libauc-1.3.0rc4/libauc/datasets/cat_vs_dog.py
--rwx------   0 zhuoning   (501) staff       (20)     9859 2023-05-18 04:21:28.000000 libauc-1.3.0rc4/libauc/datasets/chexpert.py
--rwx------   0 zhuoning   (501) staff       (20)     6292 2023-05-24 19:24:50.000000 libauc-1.3.0rc4/libauc/datasets/cifar.py
--rwx------   0 zhuoning   (501) staff       (20)     1561 2023-06-09 06:42:09.000000 libauc-1.3.0rc4/libauc/datasets/dataset.py
--rwx------   0 zhuoning   (501) staff       (20)    12399 2023-03-09 21:50:47.000000 libauc-1.3.0rc4/libauc/datasets/folder.py
--rwx------   0 zhuoning   (501) staff       (20)     4854 2023-06-07 00:13:14.000000 libauc-1.3.0rc4/libauc/datasets/melanoma.py
--rwx------   0 zhuoning   (501) staff       (20)    13133 2023-06-11 19:11:48.000000 libauc-1.3.0rc4/libauc/datasets/movielens.py
--rwx------   0 zhuoning   (501) staff       (20)     1497 2023-06-09 07:05:10.000000 libauc-1.3.0rc4/libauc/datasets/musk2.py
--rwx------   0 zhuoning   (501) staff       (20)     2960 2023-03-02 14:10:38.000000 libauc-1.3.0rc4/libauc/datasets/stl10.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 19:57:09.443065 libauc-1.3.0rc4/libauc/losses/
--rwx------   0 zhuoning   (501) staff       (20)      117 2023-06-07 19:59:42.000000 libauc-1.3.0rc4/libauc/losses/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    49557 2023-06-10 17:45:01.000000 libauc-1.3.0rc4/libauc/losses/auc.py
--rwx------   0 zhuoning   (501) staff       (20)    23656 2023-06-08 21:47:59.000000 libauc-1.3.0rc4/libauc/losses/contrastive.py
--rwx------   0 zhuoning   (501) staff       (20)     2893 2023-06-08 21:37:05.000000 libauc-1.3.0rc4/libauc/losses/losses.py
--rwx------   0 zhuoning   (501) staff       (20)    15077 2023-06-10 06:44:38.000000 libauc-1.3.0rc4/libauc/losses/mil.py
--rwx------   0 zhuoning   (501) staff       (20)     3038 2023-06-11 04:06:56.000000 libauc-1.3.0rc4/libauc/losses/perf_at_top.py
--rwx------   0 zhuoning   (501) staff       (20)    12996 2023-06-11 04:07:47.000000 libauc-1.3.0rc4/libauc/losses/ranking.py
--rwx------   0 zhuoning   (501) staff       (20)     2618 2023-06-03 03:28:07.000000 libauc-1.3.0rc4/libauc/losses/surrogate.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 19:57:09.443269 libauc-1.3.0rc4/libauc/metrics/
--rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:29.000000 libauc-1.3.0rc4/libauc/metrics/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)     8479 2023-06-11 04:07:30.000000 libauc-1.3.0rc4/libauc/metrics/metrics.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 19:57:09.444020 libauc-1.3.0rc4/libauc/models/
--rwx------   0 zhuoning   (501) staff       (20)      153 2023-05-26 02:45:25.000000 libauc-1.3.0rc4/libauc/models/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    13913 2023-05-18 03:12:04.000000 libauc-1.3.0rc4/libauc/models/densenet.py
--rwx------   0 zhuoning   (501) staff       (20)     8626 2023-05-26 04:26:36.000000 libauc-1.3.0rc4/libauc/models/mil_models.py
--rwx------   0 zhuoning   (501) staff       (20)     3479 2023-06-07 00:10:14.000000 libauc-1.3.0rc4/libauc/models/neumf.py
--rwx------   0 zhuoning   (501) staff       (20)     1284 2023-06-07 00:11:49.000000 libauc-1.3.0rc4/libauc/models/perceptron.py
--rwx------   0 zhuoning   (501) staff       (20)    16352 2023-05-18 03:13:49.000000 libauc-1.3.0rc4/libauc/models/resnet.py
--rwx------   0 zhuoning   (501) staff       (20)     6836 2023-05-26 02:54:35.000000 libauc-1.3.0rc4/libauc/models/resnet_cifar.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 19:57:09.445691 libauc-1.3.0rc4/libauc/optimizers/
--rwx------   0 zhuoning   (501) staff       (20)      350 2023-06-01 06:26:46.000000 libauc-1.3.0rc4/libauc/optimizers/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)     8837 2023-06-03 23:34:47.000000 libauc-1.3.0rc4/libauc/optimizers/adam.py
--rwx------   0 zhuoning   (501) staff       (20)     8708 2023-06-03 23:34:51.000000 libauc-1.3.0rc4/libauc/optimizers/adamw.py
--rwx------   0 zhuoning   (501) staff       (20)    12516 2023-06-08 19:29:52.000000 libauc-1.3.0rc4/libauc/optimizers/isogclr.py
--rw-r--r--   0 zhuoning   (501) staff       (20)     1760 2023-06-02 02:43:22.000000 libauc-1.3.0rc4/libauc/optimizers/lars.py
--rwx------   0 zhuoning   (501) staff       (20)     8217 2023-06-08 21:20:22.000000 libauc-1.3.0rc4/libauc/optimizers/midam.py
--rwx------   0 zhuoning   (501) staff       (20)    11371 2023-06-10 01:13:32.000000 libauc-1.3.0rc4/libauc/optimizers/pdsca.py
--rwx------   0 zhuoning   (501) staff       (20)    14361 2023-06-08 19:11:26.000000 libauc-1.3.0rc4/libauc/optimizers/pesg.py
--rwx------   0 zhuoning   (501) staff       (20)     8075 2023-06-03 23:33:49.000000 libauc-1.3.0rc4/libauc/optimizers/sgd.py
--rwx------   0 zhuoning   (501) staff       (20)    13151 2023-06-03 23:34:03.000000 libauc-1.3.0rc4/libauc/optimizers/soap.py
--rwx------   0 zhuoning   (501) staff       (20)    11517 2023-06-08 19:11:51.000000 libauc-1.3.0rc4/libauc/optimizers/sogclr.py
--rwx------   0 zhuoning   (501) staff       (20)    12325 2023-06-10 02:57:39.000000 libauc-1.3.0rc4/libauc/optimizers/song.py
--rwx------   0 zhuoning   (501) staff       (20)    12831 2023-06-03 23:34:26.000000 libauc-1.3.0rc4/libauc/optimizers/sopa.py
--rwx------   0 zhuoning   (501) staff       (20)    12949 2023-06-06 02:37:46.000000 libauc-1.3.0rc4/libauc/optimizers/sopa_s.py
--rwx------   0 zhuoning   (501) staff       (20)    12710 2023-06-09 06:11:28.000000 libauc-1.3.0rc4/libauc/optimizers/sota_s.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 19:57:09.445994 libauc-1.3.0rc4/libauc/sampler/
--rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:26.000000 libauc-1.3.0rc4/libauc/sampler/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    20482 2023-06-11 19:54:36.000000 libauc-1.3.0rc4/libauc/sampler/sampler.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 19:57:09.446371 libauc-1.3.0rc4/libauc/utils/
--rwx------   0 zhuoning   (501) staff       (20)       50 2023-06-01 06:26:50.000000 libauc-1.3.0rc4/libauc/utils/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    20155 2023-06-10 17:58:55.000000 libauc-1.3.0rc4/libauc/utils/paper_utils.py
--rwx------   0 zhuoning   (501) staff       (20)     4706 2023-06-11 05:08:04.000000 libauc-1.3.0rc4/libauc/utils/utils.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 19:57:09.440761 libauc-1.3.0rc4/libauc.egg-info/
--rw-r--r--   0 zhuoning   (501) staff       (20)     4162 2023-06-11 19:57:09.000000 libauc-1.3.0rc4/libauc.egg-info/PKG-INFO
--rw-r--r--   0 zhuoning   (501) staff       (20)     1470 2023-06-11 19:57:09.000000 libauc-1.3.0rc4/libauc.egg-info/SOURCES.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)        1 2023-06-11 19:57:09.000000 libauc-1.3.0rc4/libauc.egg-info/dependency_links.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)       76 2023-06-11 19:57:09.000000 libauc-1.3.0rc4/libauc.egg-info/requires.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)        7 2023-06-11 19:57:09.000000 libauc-1.3.0rc4/libauc.egg-info/top_level.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)       38 2023-06-11 19:57:09.446654 libauc-1.3.0rc4/setup.cfg
--rw-r--r--   0 zhuoning   (501) staff       (20)      982 2023-06-11 19:56:53.000000 libauc-1.3.0rc4/setup.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:05:51.512474 libauc-1.3.0rc5/
+-rwx------   0 zhuoning   (501) staff       (20)    11357 2023-03-02 14:10:38.000000 libauc-1.3.0rc5/LICENSE
+-rw-r--r--   0 zhuoning   (501) staff       (20)     4143 2023-06-11 21:05:51.512348 libauc-1.3.0rc5/PKG-INFO
+-rw-r--r--   0 zhuoning   (501) staff       (20)     3657 2023-06-11 20:04:36.000000 libauc-1.3.0rc5/README.md
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:05:51.505933 libauc-1.3.0rc5/libauc/
+-rwx------   0 zhuoning   (501) staff       (20)      112 2023-06-11 21:05:49.000000 libauc-1.3.0rc5/libauc/__init__.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:05:51.507846 libauc-1.3.0rc5/libauc/datasets/
+-rwx------   0 zhuoning   (501) staff       (20)      245 2023-06-09 06:42:38.000000 libauc-1.3.0rc5/libauc/datasets/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)     2621 2023-06-10 17:15:47.000000 libauc-1.3.0rc5/libauc/datasets/breastcancer.py
+-rwx------   0 zhuoning   (501) staff       (20)     2176 2023-06-10 17:15:53.000000 libauc-1.3.0rc5/libauc/datasets/cat_vs_dog.py
+-rwx------   0 zhuoning   (501) staff       (20)     9859 2023-05-18 04:21:28.000000 libauc-1.3.0rc5/libauc/datasets/chexpert.py
+-rwx------   0 zhuoning   (501) staff       (20)     6292 2023-05-24 19:24:50.000000 libauc-1.3.0rc5/libauc/datasets/cifar.py
+-rwx------   0 zhuoning   (501) staff       (20)     1561 2023-06-09 06:42:09.000000 libauc-1.3.0rc5/libauc/datasets/dataset.py
+-rwx------   0 zhuoning   (501) staff       (20)    12399 2023-03-09 21:50:47.000000 libauc-1.3.0rc5/libauc/datasets/folder.py
+-rwx------   0 zhuoning   (501) staff       (20)     4854 2023-06-07 00:13:14.000000 libauc-1.3.0rc5/libauc/datasets/melanoma.py
+-rwx------   0 zhuoning   (501) staff       (20)    13133 2023-06-11 19:11:48.000000 libauc-1.3.0rc5/libauc/datasets/movielens.py
+-rwx------   0 zhuoning   (501) staff       (20)     1497 2023-06-09 07:05:10.000000 libauc-1.3.0rc5/libauc/datasets/musk2.py
+-rwx------   0 zhuoning   (501) staff       (20)     2960 2023-03-02 14:10:38.000000 libauc-1.3.0rc5/libauc/datasets/stl10.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:05:51.508787 libauc-1.3.0rc5/libauc/losses/
+-rwx------   0 zhuoning   (501) staff       (20)      117 2023-06-07 19:59:42.000000 libauc-1.3.0rc5/libauc/losses/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    49557 2023-06-10 17:45:01.000000 libauc-1.3.0rc5/libauc/losses/auc.py
+-rwx------   0 zhuoning   (501) staff       (20)    23656 2023-06-08 21:47:59.000000 libauc-1.3.0rc5/libauc/losses/contrastive.py
+-rwx------   0 zhuoning   (501) staff       (20)     2893 2023-06-08 21:37:05.000000 libauc-1.3.0rc5/libauc/losses/losses.py
+-rwx------   0 zhuoning   (501) staff       (20)    15077 2023-06-10 06:44:38.000000 libauc-1.3.0rc5/libauc/losses/mil.py
+-rwx------   0 zhuoning   (501) staff       (20)     3038 2023-06-11 04:06:56.000000 libauc-1.3.0rc5/libauc/losses/perf_at_top.py
+-rwx------   0 zhuoning   (501) staff       (20)    12996 2023-06-11 04:07:47.000000 libauc-1.3.0rc5/libauc/losses/ranking.py
+-rwx------   0 zhuoning   (501) staff       (20)     2618 2023-06-03 03:28:07.000000 libauc-1.3.0rc5/libauc/losses/surrogate.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:05:51.508988 libauc-1.3.0rc5/libauc/metrics/
+-rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:29.000000 libauc-1.3.0rc5/libauc/metrics/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)     8479 2023-06-11 04:07:30.000000 libauc-1.3.0rc5/libauc/metrics/metrics.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:05:51.509750 libauc-1.3.0rc5/libauc/models/
+-rwx------   0 zhuoning   (501) staff       (20)      153 2023-05-26 02:45:25.000000 libauc-1.3.0rc5/libauc/models/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    13913 2023-05-18 03:12:04.000000 libauc-1.3.0rc5/libauc/models/densenet.py
+-rwx------   0 zhuoning   (501) staff       (20)     8626 2023-05-26 04:26:36.000000 libauc-1.3.0rc5/libauc/models/mil_models.py
+-rwx------   0 zhuoning   (501) staff       (20)     3479 2023-06-07 00:10:14.000000 libauc-1.3.0rc5/libauc/models/neumf.py
+-rwx------   0 zhuoning   (501) staff       (20)     1284 2023-06-07 00:11:49.000000 libauc-1.3.0rc5/libauc/models/perceptron.py
+-rwx------   0 zhuoning   (501) staff       (20)    16352 2023-05-18 03:13:49.000000 libauc-1.3.0rc5/libauc/models/resnet.py
+-rwx------   0 zhuoning   (501) staff       (20)     6836 2023-05-26 02:54:35.000000 libauc-1.3.0rc5/libauc/models/resnet_cifar.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:05:51.511602 libauc-1.3.0rc5/libauc/optimizers/
+-rwx------   0 zhuoning   (501) staff       (20)      350 2023-06-01 06:26:46.000000 libauc-1.3.0rc5/libauc/optimizers/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)     9062 2023-06-11 20:55:33.000000 libauc-1.3.0rc5/libauc/optimizers/adam.py
+-rwx------   0 zhuoning   (501) staff       (20)     8911 2023-06-11 20:49:33.000000 libauc-1.3.0rc5/libauc/optimizers/adamw.py
+-rwx------   0 zhuoning   (501) staff       (20)    12775 2023-06-11 21:05:07.000000 libauc-1.3.0rc5/libauc/optimizers/isogclr.py
+-rw-r--r--   0 zhuoning   (501) staff       (20)     1760 2023-06-02 02:43:22.000000 libauc-1.3.0rc5/libauc/optimizers/lars.py
+-rwx------   0 zhuoning   (501) staff       (20)     8217 2023-06-08 21:20:22.000000 libauc-1.3.0rc5/libauc/optimizers/midam.py
+-rwx------   0 zhuoning   (501) staff       (20)    11591 2023-06-11 20:56:14.000000 libauc-1.3.0rc5/libauc/optimizers/pdsca.py
+-rwx------   0 zhuoning   (501) staff       (20)    14772 2023-06-11 20:57:02.000000 libauc-1.3.0rc5/libauc/optimizers/pesg.py
+-rwx------   0 zhuoning   (501) staff       (20)     8297 2023-06-11 20:57:22.000000 libauc-1.3.0rc5/libauc/optimizers/sgd.py
+-rwx------   0 zhuoning   (501) staff       (20)    13546 2023-06-11 21:01:55.000000 libauc-1.3.0rc5/libauc/optimizers/soap.py
+-rwx------   0 zhuoning   (501) staff       (20)    11774 2023-06-11 21:05:08.000000 libauc-1.3.0rc5/libauc/optimizers/sogclr.py
+-rwx------   0 zhuoning   (501) staff       (20)    12722 2023-06-11 20:51:48.000000 libauc-1.3.0rc5/libauc/optimizers/song.py
+-rwx------   0 zhuoning   (501) staff       (20)    13216 2023-06-11 20:53:19.000000 libauc-1.3.0rc5/libauc/optimizers/sopa.py
+-rwx------   0 zhuoning   (501) staff       (20)    13344 2023-06-11 20:52:35.000000 libauc-1.3.0rc5/libauc/optimizers/sopa_s.py
+-rwx------   0 zhuoning   (501) staff       (20)    12918 2023-06-11 20:54:05.000000 libauc-1.3.0rc5/libauc/optimizers/sota_s.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:05:51.511814 libauc-1.3.0rc5/libauc/sampler/
+-rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:26.000000 libauc-1.3.0rc5/libauc/sampler/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    20482 2023-06-11 19:54:36.000000 libauc-1.3.0rc5/libauc/sampler/sampler.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:05:51.512172 libauc-1.3.0rc5/libauc/utils/
+-rwx------   0 zhuoning   (501) staff       (20)       50 2023-06-01 06:26:50.000000 libauc-1.3.0rc5/libauc/utils/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    20155 2023-06-10 17:58:55.000000 libauc-1.3.0rc5/libauc/utils/paper_utils.py
+-rwx------   0 zhuoning   (501) staff       (20)     4706 2023-06-11 05:08:04.000000 libauc-1.3.0rc5/libauc/utils/utils.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:05:51.506540 libauc-1.3.0rc5/libauc.egg-info/
+-rw-r--r--   0 zhuoning   (501) staff       (20)     4143 2023-06-11 21:05:51.000000 libauc-1.3.0rc5/libauc.egg-info/PKG-INFO
+-rw-r--r--   0 zhuoning   (501) staff       (20)     1470 2023-06-11 21:05:51.000000 libauc-1.3.0rc5/libauc.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)        1 2023-06-11 21:05:51.000000 libauc-1.3.0rc5/libauc.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)       76 2023-06-11 21:05:51.000000 libauc-1.3.0rc5/libauc.egg-info/requires.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)        7 2023-06-11 21:05:51.000000 libauc-1.3.0rc5/libauc.egg-info/top_level.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)       38 2023-06-11 21:05:51.512513 libauc-1.3.0rc5/setup.cfg
+-rw-r--r--   0 zhuoning   (501) staff       (20)      982 2023-06-11 21:05:48.000000 libauc-1.3.0rc5/setup.py
```

### Comparing `libauc-1.3.0rc4/LICENSE` & `libauc-1.3.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/PKG-INFO` & `libauc-1.3.0rc5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libauc
-Version: 1.3.0rc4
+Version: 1.3.0rc5
 Summary: LibAUC: A Deep Learning Library for X-Risk Optimization
 Home-page: https://github.com/Optimization-AI/LibAUC
 Author: Zhuoning Yuan
 Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -41,17 +41,17 @@
 | [**Website**](https://libauc.org/)
 | [**Publication**](https://libauc.org/publications/)
 | [**Github**](https://github.com/Optimization-AI/LibAUC/) |
 
 
 Why LibAUC?
 ---
-LibAUC offers an easier way to directly optimize commonly-used performance measures and losses with user-friendly API. LibAUC has broad applications in AI for tackling both classic and emerging challenges, such as **Classification of Imbalanced Data (CID)**, **Learning to Rank (LTR)**, and **Contrastive Representation Learning (CLR)**.
+LibAUC offers an easier way to directly optimize commonly-used performance measures and losses with user-friendly API. LibAUC has broad applications in AI for tackling both classic and emerging challenges, such as **Classification of Imbalanced Data (CID)**, **Learning to Rank (LTR)**, and **Contrastive Learning of Representation (CLR)**.
 
-LibAUC provides a unified framework to abstract the optimization of many compositional loss functions, including surrogate losses for AUROC, AUPRC/AP, and partial AUROC that are suitable for CID, surrogate losses for NDCG, top-K NDCG, and listwise losses that are used in LTR, and global contrastive losses for CLR. Here’s an overview:
+LibAUC provides a unified framework to abstract the optimization of many compositional loss functions, including surrogate losses for AUROC, AUPRC/AP, and partial AUROC that are suitable for CID, surrogate losses for NDCG, top-K NDCG, and listwise losses that are used in LTR, and global contrastive losses for CLR.
 
 
 
 Installation
 --------------
 ```
 $ pip install -U libauc
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc4 Summary: LibAUC: A Deep
+Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc5 Summary: LibAUC: A Deep
 Learning Library for X-Risk Optimization Home-page: https://github.com/
 Optimization-AI/LibAUC Author: Zhuoning Yuan Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE LibAUC: A Deep Learning for X-Risk Optimization
 ---
@@ -11,20 +11,20 @@
 libauc.org/installation/) | [**Examples**](https://github.com/Optimization-AI/
 LibAUC/tree/main/examples) | [**Website**](https://libauc.org/) |
 [**Publication**](https://libauc.org/publications/) | [**Github**](https://
 github.com/Optimization-AI/LibAUC/) | Why LibAUC? --- LibAUC offers an easier
 way to directly optimize commonly-used performance measures and losses with
 user-friendly API. LibAUC has broad applications in AI for tackling both
 classic and emerging challenges, such as **Classification of Imbalanced Data
-(CID)**, **Learning to Rank (LTR)**, and **Contrastive Representation Learning
-(CLR)**. LibAUC provides a unified framework to abstract the optimization of
-many compositional loss functions, including surrogate losses for AUROC, AUPRC/
-AP, and partial AUROC that are suitable for CID, surrogate losses for NDCG,
-top-K NDCG, and listwise losses that are used in LTR, and global contrastive
-losses for CLR. Hereâs an overview: Installation -------------- ``` $ pip
+(CID)**, **Learning to Rank (LTR)**, and **Contrastive Learning of
+Representation (CLR)**. LibAUC provides a unified framework to abstract the
+optimization of many compositional loss functions, including surrogate losses
+for AUROC, AUPRC/AP, and partial AUROC that are suitable for CID, surrogate
+losses for NDCG, top-K NDCG, and listwise losses that are used in LTR, and
+global contrastive losses for CLR. Installation -------------- ``` $ pip
 install -U libauc ``` For more updates, please check the [release note](https:/
 /github.com/Optimization-AI/LibAUC/releases/). Usage --- #### Example training
 pipline for optimizing X-risk (e.g., AUROC) ```python >>> #import our loss and
 optimizer >>> from libauc.losses import AUCMLoss >>> from libauc.optimizers
 import PESG ... >>> #define loss & optimizer >>> Loss = AUCMLoss() >>>
 optimizer = PESG() ... >>> #training >>> model.train() >>> for data, targets in
 trainloader: >>> data, targets = data.cuda(), targets.cuda() logits = model
```

### Comparing `libauc-1.3.0rc4/README.md` & `libauc-1.3.0rc5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 | [**Website**](https://libauc.org/)
 | [**Publication**](https://libauc.org/publications/)
 | [**Github**](https://github.com/Optimization-AI/LibAUC/) |
 
 
 Why LibAUC?
 ---
-LibAUC offers an easier way to directly optimize commonly-used performance measures and losses with user-friendly API. LibAUC has broad applications in AI for tackling both classic and emerging challenges, such as **Classification of Imbalanced Data (CID)**, **Learning to Rank (LTR)**, and **Contrastive Representation Learning (CLR)**.
+LibAUC offers an easier way to directly optimize commonly-used performance measures and losses with user-friendly API. LibAUC has broad applications in AI for tackling both classic and emerging challenges, such as **Classification of Imbalanced Data (CID)**, **Learning to Rank (LTR)**, and **Contrastive Learning of Representation (CLR)**.
 
-LibAUC provides a unified framework to abstract the optimization of many compositional loss functions, including surrogate losses for AUROC, AUPRC/AP, and partial AUROC that are suitable for CID, surrogate losses for NDCG, top-K NDCG, and listwise losses that are used in LTR, and global contrastive losses for CLR. Here’s an overview:
+LibAUC provides a unified framework to abstract the optimization of many compositional loss functions, including surrogate losses for AUROC, AUPRC/AP, and partial AUROC that are suitable for CID, surrogate losses for NDCG, top-K NDCG, and listwise losses that are used in LTR, and global contrastive losses for CLR.
 
 
 
 Installation
 --------------
 ```
 $ pip install -U libauc
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -4,20 +4,20 @@
 libauc.org/installation/) | [**Examples**](https://github.com/Optimization-AI/
 LibAUC/tree/main/examples) | [**Website**](https://libauc.org/) |
 [**Publication**](https://libauc.org/publications/) | [**Github**](https://
 github.com/Optimization-AI/LibAUC/) | Why LibAUC? --- LibAUC offers an easier
 way to directly optimize commonly-used performance measures and losses with
 user-friendly API. LibAUC has broad applications in AI for tackling both
 classic and emerging challenges, such as **Classification of Imbalanced Data
-(CID)**, **Learning to Rank (LTR)**, and **Contrastive Representation Learning
-(CLR)**. LibAUC provides a unified framework to abstract the optimization of
-many compositional loss functions, including surrogate losses for AUROC, AUPRC/
-AP, and partial AUROC that are suitable for CID, surrogate losses for NDCG,
-top-K NDCG, and listwise losses that are used in LTR, and global contrastive
-losses for CLR. Hereâs an overview: Installation -------------- ``` $ pip
+(CID)**, **Learning to Rank (LTR)**, and **Contrastive Learning of
+Representation (CLR)**. LibAUC provides a unified framework to abstract the
+optimization of many compositional loss functions, including surrogate losses
+for AUROC, AUPRC/AP, and partial AUROC that are suitable for CID, surrogate
+losses for NDCG, top-K NDCG, and listwise losses that are used in LTR, and
+global contrastive losses for CLR. Installation -------------- ``` $ pip
 install -U libauc ``` For more updates, please check the [release note](https:/
 /github.com/Optimization-AI/LibAUC/releases/). Usage --- #### Example training
 pipline for optimizing X-risk (e.g., AUROC) ```python >>> #import our loss and
 optimizer >>> from libauc.losses import AUCMLoss >>> from libauc.optimizers
 import PESG ... >>> #define loss & optimizer >>> Loss = AUCMLoss() >>>
 optimizer = PESG() ... >>> #training >>> model.train() >>> for data, targets in
 trainloader: >>> data, targets = data.cuda(), targets.cuda() logits = model
```

### Comparing `libauc-1.3.0rc4/libauc/datasets/breastcancer.py` & `libauc-1.3.0rc5/libauc/datasets/breastcancer.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/datasets/cat_vs_dog.py` & `libauc-1.3.0rc5/libauc/datasets/cat_vs_dog.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/datasets/chexpert.py` & `libauc-1.3.0rc5/libauc/datasets/chexpert.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/datasets/cifar.py` & `libauc-1.3.0rc5/libauc/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/datasets/dataset.py` & `libauc-1.3.0rc5/libauc/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/datasets/folder.py` & `libauc-1.3.0rc5/libauc/datasets/folder.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/datasets/melanoma.py` & `libauc-1.3.0rc5/libauc/datasets/melanoma.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/datasets/movielens.py` & `libauc-1.3.0rc5/libauc/datasets/movielens.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/datasets/musk2.py` & `libauc-1.3.0rc5/libauc/datasets/musk2.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/datasets/stl10.py` & `libauc-1.3.0rc5/libauc/datasets/stl10.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/losses/auc.py` & `libauc-1.3.0rc5/libauc/losses/auc.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/losses/contrastive.py` & `libauc-1.3.0rc5/libauc/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/losses/losses.py` & `libauc-1.3.0rc5/libauc/losses/losses.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/losses/mil.py` & `libauc-1.3.0rc5/libauc/losses/mil.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/losses/perf_at_top.py` & `libauc-1.3.0rc5/libauc/losses/perf_at_top.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/losses/ranking.py` & `libauc-1.3.0rc5/libauc/losses/ranking.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/losses/surrogate.py` & `libauc-1.3.0rc5/libauc/losses/surrogate.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/metrics/metrics.py` & `libauc-1.3.0rc5/libauc/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/models/densenet.py` & `libauc-1.3.0rc5/libauc/models/densenet.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/models/mil_models.py` & `libauc-1.3.0rc5/libauc/models/mil_models.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/models/neumf.py` & `libauc-1.3.0rc5/libauc/models/neumf.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/models/perceptron.py` & `libauc-1.3.0rc5/libauc/models/perceptron.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/models/resnet.py` & `libauc-1.3.0rc5/libauc/models/resnet.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/models/resnet_cifar.py` & `libauc-1.3.0rc5/libauc/models/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/optimizers/adam.py` & `libauc-1.3.0rc5/libauc/optimizers/adam.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,16 @@
             raise ValueError("Invalid beta parameter at index 1: {}".format(betas[1]))
         if not 0.0 <= weight_decay:
             raise ValueError("Invalid weight_decay value: {}".format(weight_decay))
             
         self.params = list(params)
         self.lr = lr
 
-        self.model_ref = self.__init_model_ref__(self.params)
-        self.model_acc = self.__init_model_acc__(self.params)
+        self.model_ref = self.__init_model_ref__(self.params) if epoch_decay > 0 else None
+        self.model_acc = self.__init_model_acc__(self.params) if epoch_decay > 0 else None
 
         self.T = 0                # for epoch_decay
         self.steps = 0            # total optim steps
         self.verbose = verbose    # print updates for lr/regularizer
         
         defaults = dict(lr=lr, betas=betas, eps=eps,
                         weight_decay=weight_decay, epoch_decay=epoch_decay, amsgrad=amsgrad, 
@@ -116,15 +116,18 @@
             epoch_decay = group['epoch_decay']
             clip_value = group['clip_value']
             weight_decay = group['weight_decay']
     
             for i, p in enumerate(group['params']):
                 if p.grad is None:
                     continue
-                grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                if epoch_decay > 0:  
+                    grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                else:
+                    grad = torch.clamp(p.grad.data , -clip_value, clip_value) + weight_decay*p.data
                 if grad.is_sparse:
                     raise RuntimeError('Adam does not support sparse gradients, please consider SparseAdam instead')
                 amsgrad = group['amsgrad']
                 state = self.state[p]
 
                 # State initialization
                 if len(state) == 0:
```

### Comparing `libauc-1.3.0rc4/libauc/optimizers/adamw.py` & `libauc-1.3.0rc5/libauc/optimizers/adamw.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,16 @@
         if not 0.0 <= betas[1] < 1.0:
             raise ValueError("Invalid beta parameter at index 1: {}".format(betas[1]))
         if not 0.0 <= weight_decay:
             raise ValueError("Invalid weight_decay value: {}".format(weight_decay))
               
         self.params = list(params)
         self.lr = lr
-        self.model_ref = self.__init_model_ref__(self.params)
-        self.model_acc = self.__init_model_acc__(self.params)
+        self.model_ref = self.__init_model_ref__(self.params) if epoch_decay > 0 else None
+        self.model_acc = self.__init_model_acc__(self.params) if epoch_decay > 0 else None
         self.T = 0                # for epoch_decay
         self.steps = 0            # total optim steps
         self.verbose = verbose    # print updates for lr/regularizer
         
         defaults = dict(lr=lr, betas=betas, eps=eps,
                         weight_decay=weight_decay, epoch_decay=epoch_decay, amsgrad=amsgrad, 
                         clip_value=clip_value, model_ref=self.model_ref, model_acc=self.model_acc)
@@ -117,16 +117,19 @@
                 if p.grad is None:
                     continue
 
                 # Perform stepweight decay
                 p.mul_(1 - self.lr * group['weight_decay'])
 
                 # Perform optimization step
-                grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data)  #p.grad
-                
+                if epoch_decay > 0:
+                    grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data)  #p.grad
+                else:
+                    grad = torch.clamp(p.grad.data , -clip_value, clip_value) 
+                    
                 if grad.is_sparse:
                     raise RuntimeError('AdamW does not support sparse gradients')
                 amsgrad = group['amsgrad']
 
                 state = self.state[p]
 
                 # State initialization
```

### Comparing `libauc-1.3.0rc4/libauc/optimizers/isogclr.py` & `libauc-1.3.0rc5/libauc/optimizers/isogclr.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,29 +77,29 @@
             raise ValueError("Invalid weight_decay value: {}".format(weight_decay))
         if not isinstance(mode, str):
            raise ValueError("Invalid mode type: {}".format(mode))
                 
         self.params = list(params)
         self.lr = lr
         self.mode = mode.lower()
-        self.model_ref = self.__init_model_ref__(self.params)
-        self.model_acc = self.__init_model_acc__(self.params)
+        self.model_ref = self.__init_model_ref__(self.params) if epoch_decay > 0 else None
+        self.model_acc = self.__init_model_acc__(self.params) if epoch_decay > 0 else None
         self.T = 0                # for epoch_decay
         self.steps = 0            # total optimization steps
         self.verbose = verbose    # print updates for lr/regularizer
         assert self.mode in ['adamw', 'lars'], "Keyword is not found in [`adamw`, `lars`]!"
         
         defaults = dict(lr=lr, clip_value=clip_value, weight_decay=weight_decay, epoch_decay=epoch_decay, 
                         momentum=momentum, trust_coefficient=trust_coefficient,
                         betas=betas, eps=eps, amsgrad=amsgrad, model_ref=self.model_ref, model_acc=self.model_acc)
         
-        super(SogCLR, self).__init__(self.params, defaults)
+        super(iSogCLR, self).__init__(self.params, defaults)
             
     def __setstate__(self, state):
-        super(SogCLR, self).__setstate__(state)
+        super(iSogCLR, self).__setstate__(state)
         for group in self.param_groups:
             if self.mode == 'adamw':
                 group.setdefault('amsgrad', False)
 
 
     def __init_model_ref__(self, params):
          model_ref = []
@@ -144,16 +144,16 @@
 
                     if dp is None:
                         continue
 
                     if p.ndim > 1: # if not normalization gamma/beta or bias
                         dp = dp.add(p, alpha=group['weight_decay'])
                         # add epoch decay
-                        dp = dp +  epoch_decay*(p.data - model_ref[i].data)
-
+                        if epoch_decay > 0:
+                            dp = dp +  epoch_decay*(p.data - model_ref[i].data)
                         param_norm = torch.norm(p)
                         update_norm = torch.norm(dp)
                         one = torch.ones_like(param_norm)
                         q = torch.where(param_norm > 0.,
                                         torch.where(update_norm > 0,
                                         (group['trust_coefficient'] * param_norm / update_norm), one),
                                         one)
@@ -173,15 +173,18 @@
                     if p.grad is None:
                         continue
 
                     # Perform stepweight decay
                     p.mul_(1 - self.lr * group['weight_decay'])
 
                     # Perform optimization step
-                    grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data)  
+                    if epoch_decay > 0:
+                        grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data)  
+                    else:
+                        grad = torch.clamp(p.grad.data , -clip_value, clip_value)
 
                     if grad.is_sparse:
                         raise RuntimeError('AdamW does not support sparse gradients')
                     amsgrad = group['amsgrad']
 
                     state = self.state[p]
```

### Comparing `libauc-1.3.0rc4/libauc/optimizers/lars.py` & `libauc-1.3.0rc5/libauc/optimizers/lars.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/optimizers/midam.py` & `libauc-1.3.0rc5/libauc/optimizers/midam.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/optimizers/pdsca.py` & `libauc-1.3.0rc5/libauc/optimizers/pdsca.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,16 +87,16 @@
                 self.margin = loss_fn.margin
             except:
                 print('CompositionalAUCLoss is not found!')
         else:
             raise ValueError('No loss_fn found!')
 
             
-        self.model_ref = self.__init_model_ref__(self.params)
-        self.model_acc = self.__init_model_acc__(self.params)
+        self.model_ref = self.__init_model_ref__(self.params) if epoch_decay > 0 else None
+        self.model_acc = self.__init_model_acc__(self.params) if epoch_decay > 0 else None
         self.T = 0                # for epoch_decay
         self.steps = 0            # total optim steps
         self.verbose = verbose    # print updates for lr/regularizer
 
         # TODO: if I can use model.parameters and remove model as input (to simplify)
         if self.a is not None and self.b is not None:
            self.params = self.params + [self.a, self.b]
@@ -172,15 +172,18 @@
             a = group['a']
             b = group['b']
             alpha = group['alpha']
             
             for i, p in enumerate(group['params']):
                 if p.grad is None: 
                    continue
-                d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                if epoch_decay > 0:
+                    d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                else:
+                    d_p = torch.clamp(p.grad.data , -clip_value, clip_value)  + weight_decay*p.data
                 if alpha.grad is None: # sgd + moving g
                     p.data = p.data - group['lr0']*d_p 
                     if beta1!= 0: 
                         param_state = self.state[p]
                         if 'weight_buffer' not in param_state:
                             buf = param_state['weight_buffer'] = torch.clone(p).detach()
                         else:
```

### Comparing `libauc-1.3.0rc4/libauc/optimizers/pesg.py` & `libauc-1.3.0rc5/libauc/optimizers/pesg.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,16 +112,16 @@
             self.b = loss_fn.b 
             self.alpha = loss_fn.alpha 
             self.margin = loss_fn.margin
         except:
             print('AUCMLoss is not found!')
 
         # init 
-        self.model_ref = self.__init_model_ref__(self.params)
-        self.model_acc = self.__init_model_acc__(self.params)
+        self.model_ref = self.__init_model_ref__(self.params) if epoch_decay > 0 else None
+        self.model_acc = self.__init_model_acc__(self.params) if epoch_decay > 0 else None
         self.T = 0                # for epoch_decay
         self.steps = 0            # total optimization steps
         self.verbose = verbose    # print updates for lr/regularizer
     
         assert self.mode in ['adam', 'sgd'], "Keyword is not found in [`adam`, `sgd`]!"
        
         if self.a is not None and self.b is not None:
@@ -205,15 +205,18 @@
             alpha = group['alpha']
             
             if self.mode == 'sgd':
                 # updates
                 for i, p in enumerate(group['params']):
                     if p.grad is None:
                         continue
-                    d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                    if epoch_decay > 0:
+                        d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                    else:
+                        d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + weight_decay*p.data
                     if momentum != 0:
                         param_state = self.state[p]
                         if 'momentum_buffer' not in param_state:
                             buf = param_state['momentum_buffer'] = torch.clone(d_p).detach()
                         else:
                             buf = param_state['momentum_buffer']
                             buf.mul_(1-momentum).add_(d_p, alpha=momentum)
@@ -222,15 +225,18 @@
                     if epoch_decay > 0:
                        model_acc[i].data = model_acc[i].data + p.data
             elif self.mode == 'adam':
                 # updates
                 for i, p in enumerate(group['params']):
                     if p.grad is None:
                         continue
-                    grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                    if epoch_decay > 0:
+                        grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                    else:
+                        grad = torch.clamp(p.grad.data , -clip_value, clip_value) + weight_decay*p.data
                     amsgrad = group['amsgrad']
                     state = self.state[p]
 
                     # State initialization
                     if len(state) == 0:
                         state['step'] = 0
                         # Exponential moving average of gradient values
```

### Comparing `libauc-1.3.0rc4/libauc/optimizers/sgd.py` & `libauc-1.3.0rc5/libauc/optimizers/sgd.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,16 +75,16 @@
             raise ValueError("Invalid momentum value: {}".format(momentum))
         if weight_decay < 0.0:
             raise ValueError("Invalid weight_decay value: {}".format(weight_decay))
            
         self.params = list(params)
         self.lr = lr
 
-        self.model_ref = self.__init_model_ref__(self.params)
-        self.model_acc = self.__init_model_acc__(self.params)
+        self.model_ref = self.__init_model_ref__(self.params) if epoch_decay > 0 else None
+        self.model_acc = self.__init_model_acc__(self.params) if epoch_decay > 0 else None
 
         self.T = 0                # for epoch_decay
         self.steps = 0            # total optim steps
         self.verbose = verbose    # print updates for lr/regularizer
         
         defaults = dict(lr=lr, momentum=momentum, dampening=dampening,
                         weight_decay=weight_decay, epoch_decay=epoch_decay, nesterov=nesterov,
@@ -140,15 +140,18 @@
             weight_decay = group['weight_decay']
             model_ref = group['model_ref']
             model_acc = group['model_acc']
         
             for i, p in enumerate(group['params']):
                 if p.grad is None:
                     continue
-                d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                if epoch_decay > 0:
+                    d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                else:
+                    d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + weight_decay*p.data
                 if momentum != 0:
                     param_state = self.state[p]
                     if 'momentum_buffer' not in param_state:
                         buf = param_state['momentum_buffer'] = torch.clone(d_p).detach()
                     else:
                         buf = param_state['momentum_buffer']
                         buf.mul_(momentum).add_(d_p, alpha=1 - dampening)
```

### Comparing `libauc-1.3.0rc4/libauc/optimizers/soap.py` & `libauc-1.3.0rc5/libauc/optimizers/soap.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,16 +94,16 @@
             raise ValueError("Invalid epoch_decay value: {}".format(epoch_decay))        
         if not isinstance(mode, str):
            raise ValueError("Invalid mode type: {}".format(mode))
              
         self.params = list(params)
         self.lr = lr
         self.mode = mode.lower() 
-        self.model_ref = self.__init_model_ref__(self.params)
-        self.model_acc = self.__init_model_acc__(self.params)
+        self.model_ref = self.__init_model_ref__(self.params) if epoch_decay > 0 else None
+        self.model_acc = self.__init_model_acc__(self.params) if epoch_decay > 0 else None
         self.T = 0                # for epoch_decay
         self.steps = 0            # total optimization steps
         self.verbose = verbose    # print updates for lr/regularizer
         
         assert self.mode in ['adam', 'sgd'], "Keyword is not found in [`adam`, `sgd`]!"
 
         defaults = dict(lr=lr, weight_decay=weight_decay, epoch_decay=epoch_decay,
@@ -169,15 +169,18 @@
             model_acc = group['model_acc']
             self.lr = group['lr'] 
             
             if self.mode == 'sgd':
                for i, p in enumerate(group['params']):
                   if p.grad is None:
                       continue
-                  d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                  if epoch_decay > 0:
+                    d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                  else:
+                    d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + weight_decay*p.data
                   if momentum != 0:
                       param_state = self.state[p]
                       if 'momentum_buffer' not in param_state:
                           buf = param_state['momentum_buffer'] = torch.clone(d_p).detach()
                       else:
                           buf = param_state['momentum_buffer']
                           buf.mul_(momentum).add_(d_p, alpha=1 - dampening) 
@@ -189,15 +192,18 @@
                   if epoch_decay > 0:
                      model_acc[i].data = model_acc[i].data + p.data
 
             elif self.mode == 'adam':
                 for i, p in enumerate(group['params']):
                     if p.grad is None:
                         continue
-                    grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                    if epoch_decay > 0:
+                        grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                    else:
+                        grad = torch.clamp(p.grad.data , -clip_value, clip_value) + weight_decay*p.data
                     if grad.is_sparse:
                         raise RuntimeError('Adam does not support sparse gradients, please consider SparseAdam instead')
                     amsgrad = group['amsgrad']
                     state = self.state[p]
 
                     # State initialization
                     if len(state) == 0:
```

### Comparing `libauc-1.3.0rc4/libauc/optimizers/sogclr.py` & `libauc-1.3.0rc5/libauc/optimizers/sogclr.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,16 +70,16 @@
             raise ValueError("Invalid weight_decay value: {}".format(weight_decay))
         if not isinstance(mode, str):
            raise ValueError("Invalid mode type: {}".format(mode))
                 
         self.params = list(params)
         self.lr = lr
         self.mode = mode.lower()
-        self.model_ref = self.__init_model_ref__(self.params)
-        self.model_acc = self.__init_model_acc__(self.params)
+        self.model_ref = self.__init_model_ref__(self.params) if epoch_decay > 0 else None
+        self.model_acc = self.__init_model_acc__(self.params) if epoch_decay > 0 else None
         self.T = 0                # for epoch_decay
         self.steps = 0            # total optimization steps
         self.verbose = verbose    # print updates for lr/regularizer
         assert self.mode in ['adamw', 'lars'], "Keyword is not found in [`adamw`, `lars`]!"
         
         defaults = dict(lr=lr, clip_value=clip_value, weight_decay=weight_decay, epoch_decay=epoch_decay, 
                         momentum=momentum, trust_coefficient=trust_coefficient,
@@ -137,15 +137,16 @@
 
                     if dp is None:
                         continue
 
                     if p.ndim > 1: # if not normalization gamma/beta or bias
                         dp = dp.add(p, alpha=group['weight_decay'])
                         # add epoch decay
-                        dp = dp +  epoch_decay*(p.data - model_ref[i].data)
+                        if epoch_decay > 0:
+                            dp = dp +  epoch_decay*(p.data - model_ref[i].data)
 
                         param_norm = torch.norm(p)
                         update_norm = torch.norm(dp)
                         one = torch.ones_like(param_norm)
                         q = torch.where(param_norm > 0.,
                                         torch.where(update_norm > 0,
                                         (group['trust_coefficient'] * param_norm / update_norm), one),
@@ -166,16 +167,18 @@
                     if p.grad is None:
                         continue
 
                     # Perform stepweight decay
                     p.mul_(1 - self.lr * group['weight_decay'])
 
                     # Perform optimization step
-                    grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data)  
-
+                    if epoch_decay > 0:
+                        grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data)  
+                    else:
+                        grad = torch.clamp(p.grad.data , -clip_value, clip_value)
                     if grad.is_sparse:
                         raise RuntimeError('AdamW does not support sparse gradients')
                     amsgrad = group['amsgrad']
 
                     state = self.state[p]
 
                     # State initialization
```

### Comparing `libauc-1.3.0rc4/libauc/optimizers/song.py` & `libauc-1.3.0rc5/libauc/optimizers/song.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,16 +82,16 @@
             raise ValueError("Invalid weight_decay value: {}".format(weight_decay))
         if not isinstance(mode, str):
             raise ValueError("Invalid mode type: {}".format(mode))
         
         self.params = list(params) 
         self.lr = lr
         self.mode = mode.lower() 
-        self.model_ref = self.__init_model_ref__(self.params)
-        self.model_acc = self.__init_model_acc__(self.params)
+        self.model_ref = self.__init_model_ref__(self.params) if epoch_decay > 0 else None
+        self.model_acc = self.__init_model_acc__(self.params) if epoch_decay > 0 else None
         self.T = 0                # for epoch_decay
         self.steps = 0            # total optimization steps
         self.verbose = verbose    # print updates for lr/regularizer
         self.epoch_decay = epoch_decay
 
         assert self.mode in ['adam', 'sgd'], "Keyword is not found in [`adam`, `sgd`]!"
 
@@ -162,15 +162,18 @@
             model_ref = group['model_ref']
             model_acc = group['model_acc']
                
             if self.mode == 'sgd':
                for i, p in enumerate(group['params']):
                   if p.grad is None:
                       continue
-                  d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                  if epoch_decay > 0:
+                     d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                  else:
+                     d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + weight_decay*p.data
                   if momentum != 0:
                       param_state = self.state[p]
                       if 'momentum_buffer' not in param_state:
                           buf = param_state['momentum_buffer'] = torch.clone(d_p).detach()
                       else:
                           buf = param_state['momentum_buffer']
                           buf.mul_(momentum).add_(d_p, alpha=1 - dampening) 
@@ -183,15 +186,18 @@
                      model_acc[i].data = model_acc[i].data + p.data
 
             elif self.mode == 'adam':
                 for i, p in enumerate(group['params']):
                     if p.grad is None:
                         continue
                     #grad = p.grad
-                    grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                    if epoch_decay > 0:
+                        grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                    else:
+                        grad = torch.clamp(p.grad.data , -clip_value, clip_value) + weight_decay*p.data
                     if grad.is_sparse:
                         raise RuntimeError('Adam does not support sparse gradients, please consider SparseAdam instead')
                     amsgrad = group['amsgrad']
                     state = self.state[p]
 
                     # State initialization
                     if len(state) == 0:
```

### Comparing `libauc-1.3.0rc4/libauc/optimizers/sopa.py` & `libauc-1.3.0rc5/libauc/optimizers/sopa.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,16 +87,16 @@
             raise ValueError("Invalid epoch_decay value: {}".format(epoch_decay))  
         if not isinstance(mode, str):
            raise ValueError("Invalid mode type: {}".format(mode))
                 
         self.params = list(params) # support optimizing partial parameters of models
         self.lr = lr
         self.mode = mode.lower()
-        self.model_ref = self.__init_model_ref__(self.params)
-        self.model_acc = self.__init_model_acc__(self.params)
+        self.model_ref = self.__init_model_ref__(self.params) if epoch_decay > 0 else None
+        self.model_acc = self.__init_model_acc__(self.params) if epoch_decay > 0 else None
         self.T = 0                # for epoch_decay
         self.steps = 0            # total optimization steps
         self.verbose = verbose    # print updates for lr/regularizer
         self.epoch_decay = epoch_decay
 
         assert self.mode in ['adam', 'sgd'], "Keyword is not found in [`adam`, `sgd`]!"
    
@@ -163,15 +163,18 @@
             
             if self.mode == 'adam':
 
               for i, p in enumerate(group['params']):
                   if p.grad is None:
                       continue
                   #grad = p.grad
-                  grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                  if epoch_decay > 0:
+                    grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                  else:
+                    grad = torch.clamp(p.grad.data , -clip_value, clip_value) + weight_decay*p.data
                   if grad.is_sparse:
                       raise RuntimeError('Adam does not support sparse gradients, please consider SparseAdam instead')
                   amsgrad = group['amsgrad']
                   state = self.state[p]
                   # State initialization
                   if len(state) == 0:
                       state['step'] = 0
@@ -206,15 +209,18 @@
                      model_acc[i].data = model_acc[i].data + p.data
                   
             elif self.mode == 'sgd':
               for i, p in enumerate(group['params']):
                   if p.grad is None:
                       continue
                   #d_p = p.grad
-                  d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                  if epoch_decay > 0:
+                    d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                  else:
+                    d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + weight_decay*p.data
                   if momentum != 0:
                       param_state = self.state[p]
                       if 'momentum_buffer' not in param_state:
                           buf = param_state['momentum_buffer'] = torch.clone(d_p).detach()
                       else:
                           buf = param_state['momentum_buffer']
                           buf.mul_(momentum).add_(d_p, alpha=1 - dampening)
```

### Comparing `libauc-1.3.0rc4/libauc/optimizers/sopa_s.py` & `libauc-1.3.0rc5/libauc/optimizers/sopa_s.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,16 @@
             raise ValueError("Invalid epoch_decay value: {}".format(epoch_decay))  
         if not isinstance(mode, str):
            raise ValueError("Invalid mode type: {}".format(mode))
            
         self.params = list(params) # support optimizing partial parameters of models
         self.lr = lr
         self.mode = mode.lower()
-        self.model_ref = self.__init_model_ref__(self.params)
-        self.model_acc = self.__init_model_acc__(self.params)
+        self.model_ref = self.__init_model_ref__(self.params) if epoch_decay > 0 else None
+        self.model_acc = self.__init_model_acc__(self.params) if epoch_decay > 0 else None
         self.T = 0                # for epoch_decay
         self.steps = 0            # total optimization steps
         self.verbose = verbose    # print updates for lr/regularizer
         self.steps = 0
         self.epoch_decay = epoch_decay
 
         assert self.mode in ['adam', 'sgd'], "Keyword is not found in [`adam`, `sgd`]!"
@@ -166,15 +166,18 @@
             model_acc = group['model_acc']
              
             if self.mode == 'sgd':
                for i, p in enumerate(group['params']):
                   if p.grad is None:
                       print(p.shape)
                       continue
-                  d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                  if epoch_decay > 0:
+                    d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                  else:
+                    d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + weight_decay*p.data
                   if momentum != 0:
                       param_state = self.state[p]
                       if 'momentum_buffer' not in param_state:
                           buf = param_state['momentum_buffer'] = torch.clone(d_p).detach()
                       else:
                           buf = param_state['momentum_buffer']
                           buf.mul_(momentum).add_(d_p, alpha=1 - dampening)
@@ -186,15 +189,18 @@
                   if epoch_decay > 0:
                      model_acc[i].data = model_acc[i].data + p.data
 
             elif self.mode == 'adam':
                 for i, p in enumerate(group['params']):
                     if p.grad is None:
                         continue
-                    grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                    if epoch_decay > 0:
+                        grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                    else:
+                        grad = torch.clamp(p.grad.data , -clip_value, clip_value) + weight_decay*p.data
                     if grad.is_sparse:
                         raise RuntimeError('Adam does not support sparse gradients, please consider SparseAdam instead')
                     amsgrad = group['amsgrad']
                     state = self.state[p]
 
                     # State initialization
                     if len(state) == 0:
```

### Comparing `libauc-1.3.0rc4/libauc/optimizers/sota_s.py` & `libauc-1.3.0rc5/libauc/optimizers/sota_s.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,16 @@
             raise ValueError("Invalid beta parameter at index 1: {}".format(betas[1]))
         if not 0.0 <= weight_decay:
             raise ValueError("Invalid weight_decay value: {}".format(weight_decay))
             
         self.params = list(params) # support optimizing partial parameters of models
         self.lr = lr
 
-        self.model_ref = self.__init_model_ref__(self.params)
-        self.model_acc = self.__init_model_acc__(self.params)
+        self.model_ref = self.__init_model_ref__(self.params) if epoch_decay > 0 else None
+        self.model_acc = self.__init_model_acc__(self.params) if epoch_decay > 0 else None
         self.T = 0                # for epoch_decay
         self.steps = 0            # total optimization steps
         self.verbose = verbose    # print updates for lr/regularizer
 
         self.epoch_decay = epoch_decay
         self.mode = mode.lower()
         assert self.mode in ['adam', 'sgd'], "Keyword is not found in [`adam`, `sgd`]!"
@@ -157,16 +157,18 @@
             clip_value = group['clip_value']
             weight_decay = group['weight_decay']
             
             if self.mode == 'adam':
               for i, p in enumerate(group['params']):
                   if p.grad is None:
                       continue
-             
-                  grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                  if epoch_decay > 0:
+                    grad = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                  else:
+                    grad = torch.clamp(p.grad.data , -clip_value, clip_value) + weight_decay*p.data
                   if grad.is_sparse:
                       raise RuntimeError('Adam does not support sparse gradients, please consider SparseAdam instead')
                   amsgrad = group['amsgrad']
                   state = self.state[p]
                   # State initialization
                   if len(state) == 0:
                       state['step'] = 0
```

### Comparing `libauc-1.3.0rc4/libauc/sampler/sampler.py` & `libauc-1.3.0rc5/libauc/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/utils/paper_utils.py` & `libauc-1.3.0rc5/libauc/utils/paper_utils.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc/utils/utils.py` & `libauc-1.3.0rc5/libauc/utils/utils.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/libauc.egg-info/PKG-INFO` & `libauc-1.3.0rc5/libauc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libauc
-Version: 1.3.0rc4
+Version: 1.3.0rc5
 Summary: LibAUC: A Deep Learning Library for X-Risk Optimization
 Home-page: https://github.com/Optimization-AI/LibAUC
 Author: Zhuoning Yuan
 Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -41,17 +41,17 @@
 | [**Website**](https://libauc.org/)
 | [**Publication**](https://libauc.org/publications/)
 | [**Github**](https://github.com/Optimization-AI/LibAUC/) |
 
 
 Why LibAUC?
 ---
-LibAUC offers an easier way to directly optimize commonly-used performance measures and losses with user-friendly API. LibAUC has broad applications in AI for tackling both classic and emerging challenges, such as **Classification of Imbalanced Data (CID)**, **Learning to Rank (LTR)**, and **Contrastive Representation Learning (CLR)**.
+LibAUC offers an easier way to directly optimize commonly-used performance measures and losses with user-friendly API. LibAUC has broad applications in AI for tackling both classic and emerging challenges, such as **Classification of Imbalanced Data (CID)**, **Learning to Rank (LTR)**, and **Contrastive Learning of Representation (CLR)**.
 
-LibAUC provides a unified framework to abstract the optimization of many compositional loss functions, including surrogate losses for AUROC, AUPRC/AP, and partial AUROC that are suitable for CID, surrogate losses for NDCG, top-K NDCG, and listwise losses that are used in LTR, and global contrastive losses for CLR. Here’s an overview:
+LibAUC provides a unified framework to abstract the optimization of many compositional loss functions, including surrogate losses for AUROC, AUPRC/AP, and partial AUROC that are suitable for CID, surrogate losses for NDCG, top-K NDCG, and listwise losses that are used in LTR, and global contrastive losses for CLR.
 
 
 
 Installation
 --------------
 ```
 $ pip install -U libauc
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc4 Summary: LibAUC: A Deep
+Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc5 Summary: LibAUC: A Deep
 Learning Library for X-Risk Optimization Home-page: https://github.com/
 Optimization-AI/LibAUC Author: Zhuoning Yuan Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE LibAUC: A Deep Learning for X-Risk Optimization
 ---
@@ -11,20 +11,20 @@
 libauc.org/installation/) | [**Examples**](https://github.com/Optimization-AI/
 LibAUC/tree/main/examples) | [**Website**](https://libauc.org/) |
 [**Publication**](https://libauc.org/publications/) | [**Github**](https://
 github.com/Optimization-AI/LibAUC/) | Why LibAUC? --- LibAUC offers an easier
 way to directly optimize commonly-used performance measures and losses with
 user-friendly API. LibAUC has broad applications in AI for tackling both
 classic and emerging challenges, such as **Classification of Imbalanced Data
-(CID)**, **Learning to Rank (LTR)**, and **Contrastive Representation Learning
-(CLR)**. LibAUC provides a unified framework to abstract the optimization of
-many compositional loss functions, including surrogate losses for AUROC, AUPRC/
-AP, and partial AUROC that are suitable for CID, surrogate losses for NDCG,
-top-K NDCG, and listwise losses that are used in LTR, and global contrastive
-losses for CLR. Hereâs an overview: Installation -------------- ``` $ pip
+(CID)**, **Learning to Rank (LTR)**, and **Contrastive Learning of
+Representation (CLR)**. LibAUC provides a unified framework to abstract the
+optimization of many compositional loss functions, including surrogate losses
+for AUROC, AUPRC/AP, and partial AUROC that are suitable for CID, surrogate
+losses for NDCG, top-K NDCG, and listwise losses that are used in LTR, and
+global contrastive losses for CLR. Installation -------------- ``` $ pip
 install -U libauc ``` For more updates, please check the [release note](https:/
 /github.com/Optimization-AI/LibAUC/releases/). Usage --- #### Example training
 pipline for optimizing X-risk (e.g., AUROC) ```python >>> #import our loss and
 optimizer >>> from libauc.losses import AUCMLoss >>> from libauc.optimizers
 import PESG ... >>> #define loss & optimizer >>> Loss = AUCMLoss() >>>
 optimizer = PESG() ... >>> #training >>> model.train() >>> for data, targets in
 trainloader: >>> data, targets = data.cuda(), targets.cuda() logits = model
```

### Comparing `libauc-1.3.0rc4/libauc.egg-info/SOURCES.txt` & `libauc-1.3.0rc5/libauc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc4/setup.py` & `libauc-1.3.0rc5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
   
 setuptools.setup(
   name="libauc",
-  version="1.3.0rc4",
+  version="1.3.0rc5",
   author="Zhuoning Yuan",
   author_email="yzhuoning@gmail.com",
   description="LibAUC: A Deep Learning Library for X-Risk Optimization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/Optimization-AI/LibAUC",
   packages=setuptools.find_packages(),
```

