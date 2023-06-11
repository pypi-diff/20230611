# Comparing `tmp/alpaca_farm-0.1.2.tar.gz` & `tmp/alpaca_farm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_farm-0.1.2.tar", last modified: Sun Jun 11 20:31:51 2023, max compression
+gzip compressed data, was "alpaca_farm-0.1.3.tar", last modified: Sun Jun 11 21:49:21 2023, max compression
```

## Comparing `alpaca_farm-0.1.2.tar` & `alpaca_farm-0.1.3.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 20:31:51.098966 alpaca_farm-0.1.2/
--rw-r--r--   0 xuechenli   (501) staff       (20)    11410 2023-05-27 23:57:21.000000 alpaca_farm-0.1.2/LICENSE
--rw-r--r--   0 xuechenli   (501) staff       (20)       64 2023-06-11 03:50:42.000000 alpaca_farm-0.1.2/MANIFEST.in
--rw-r--r--   0 xuechenli   (501) staff       (20)    16097 2023-06-11 20:31:51.098680 alpaca_farm-0.1.2/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)    15496 2023-06-11 03:32:13.000000 alpaca_farm-0.1.2/README.md
--rw-r--r--   0 xuechenli   (501) staff       (20)       38 2023-06-11 20:31:51.099017 alpaca_farm-0.1.2/setup.cfg
--rw-r--r--   0 xuechenli   (501) staff       (20)     2524 2023-06-11 20:30:56.000000 alpaca_farm-0.1.2/setup.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 20:31:51.082500 alpaca_farm-0.1.2/src/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 20:31:51.087198 alpaca_farm-0.1.2/src/alpaca_farm/
--rw-r--r--   0 xuechenli   (501) staff       (20)      602 2023-06-11 20:30:39.000000 alpaca_farm-0.1.2/src/alpaca_farm/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1190 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/accelerate_patch.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 20:31:51.089221 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/
--rw-r--r--   0 xuechenli   (501) staff       (20)      634 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1894 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/analysis.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 20:31:51.082860 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 20:31:51.093996 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     1670 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6020 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5869 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     2605 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     2475 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3852 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3721 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3660 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3423 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7125 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6849 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7073 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6797 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6991 2023-06-10 06:22:43.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6969 2023-06-11 02:31:44.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     1057 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     1016 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     4067 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     3969 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     6289 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5932 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5559 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     5370 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 20:31:51.094560 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/
--rw-r--r--   0 xuechenli   (501) staff       (20)     7664 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)     7373 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      481 2023-06-11 02:31:44.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/configs.yaml
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 20:31:51.094829 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/test/
--rw-r--r--   0 xuechenli   (501) staff       (20)      426 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/test/configs.yaml
--rw-r--r--   0 xuechenli   (501) staff       (20)     4951 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/decoders.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4762 2023-06-11 03:32:13.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/eval.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    29607 2023-06-10 06:19:54.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/pairwise_annotators.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11403 2023-06-10 06:21:13.000000 alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13428 2023-06-11 04:26:11.000000 alpaca_farm-0.1.2/src/alpaca_farm/common.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2652 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/constants.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1369 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/data_postprocessor.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    18874 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/data_preprocessor.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3712 2023-06-11 20:27:00.000000 alpaca_farm-0.1.2/src/alpaca_farm/data_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2532 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/distributed_utils.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 20:31:51.095730 alpaca_farm-0.1.2/src/alpaca_farm/flash_models/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/flash_models/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1492 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/flash_models/apex_patch.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13316 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/flash_models/flash_llama.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11476 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/flash_models/flash_opt.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1741 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/flash_models/tensor_ops.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 20:31:51.096251 alpaca_farm-0.1.2/src/alpaca_farm/inference/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/inference/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    16267 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/inference/decode.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7147 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/inference/score.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3372 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/logging.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 20:31:51.096864 alpaca_farm-0.1.2/src/alpaca_farm/models/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/models/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2523 2023-06-11 04:26:11.000000 alpaca_farm-0.1.2/src/alpaca_farm/models/reward_model.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     8003 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/models/rl_models.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    11532 2023-06-10 06:21:02.000000 alpaca_farm-0.1.2/src/alpaca_farm/openai_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3208 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/reward_modeling_trainer.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 20:31:51.097900 alpaca_farm-0.1.2/src/alpaca_farm/rl/
--rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/rl/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2054 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/rl/kl_controller.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    22881 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/rl/ppo_trainer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7524 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/rl/ppo_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13765 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/rl/rl_trainer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3088 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/torch_ops.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3507 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/trainer_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1211 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/types.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     6141 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/src/alpaca_farm/utils.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 20:31:51.087864 alpaca_farm-0.1.2/src/alpaca_farm.egg-info/
--rw-r--r--   0 xuechenli   (501) staff       (20)    16097 2023-06-11 20:31:51.000000 alpaca_farm-0.1.2/src/alpaca_farm.egg-info/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)     4266 2023-06-11 20:31:51.000000 alpaca_farm-0.1.2/src/alpaca_farm.egg-info/SOURCES.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)        1 2023-06-11 20:31:51.000000 alpaca_farm-0.1.2/src/alpaca_farm.egg-info/dependency_links.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      295 2023-06-11 20:31:51.000000 alpaca_farm-0.1.2/src/alpaca_farm.egg-info/requires.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)       12 2023-06-11 20:31:51.000000 alpaca_farm-0.1.2/src/alpaca_farm.egg-info/top_level.txt
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 20:31:51.098418 alpaca_farm-0.1.2/tests/
--rw-r--r--   0 xuechenli   (501) staff       (20)    12263 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/tests/test_flash_llama.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     8351 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/tests/test_flash_opt.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      899 2023-05-23 16:11:47.000000 alpaca_farm-0.1.2/tests/test_torch_ops.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.996693 alpaca_farm-0.1.3/
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11410 2023-05-27 23:57:21.000000 alpaca_farm-0.1.3/LICENSE
+-rw-r--r--   0 xuechenli   (501) staff       (20)       64 2023-06-11 03:50:42.000000 alpaca_farm-0.1.3/MANIFEST.in
+-rw-r--r--   0 xuechenli   (501) staff       (20)    17050 2023-06-11 21:49:21.996528 alpaca_farm-0.1.3/PKG-INFO
+-rw-r--r--   0 xuechenli   (501) staff       (20)    16449 2023-06-11 21:47:42.000000 alpaca_farm-0.1.3/README.md
+-rw-r--r--   0 xuechenli   (501) staff       (20)       38 2023-06-11 21:49:21.996728 alpaca_farm-0.1.3/setup.cfg
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2524 2023-06-11 20:30:56.000000 alpaca_farm-0.1.3/setup.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.978016 alpaca_farm-0.1.3/src/
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.982857 alpaca_farm-0.1.3/src/alpaca_farm/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      602 2023-06-11 21:49:04.000000 alpaca_farm-0.1.3/src/alpaca_farm/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1190 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/accelerate_patch.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.985257 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      634 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1894 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/analysis.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.978375 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.990127 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1670 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6020 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5869 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2605 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2475 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3852 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3721 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3660 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3423 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7125 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6849 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7073 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6797 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6991 2023-06-10 06:22:43.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6700 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6969 2023-06-11 02:31:44.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1057 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1016 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4067 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3969 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6289 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5932 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5559 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5370 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.992740 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7664 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7373 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      481 2023-06-11 02:31:44.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/configs.yaml
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.992977 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/test/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      426 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/test/configs.yaml
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4951 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/decoders.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4762 2023-06-11 03:32:13.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/eval.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    29607 2023-06-10 06:19:54.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/pairwise_annotators.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11403 2023-06-10 06:21:13.000000 alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    13428 2023-06-11 04:26:11.000000 alpaca_farm-0.1.3/src/alpaca_farm/common.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2652 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/constants.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1369 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/data_postprocessor.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    18874 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/data_preprocessor.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4147 2023-06-11 21:47:42.000000 alpaca_farm-0.1.3/src/alpaca_farm/data_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2532 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/distributed_utils.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.993798 alpaca_farm-0.1.3/src/alpaca_farm/flash_models/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/flash_models/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1492 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/flash_models/apex_patch.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    13316 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/flash_models/flash_llama.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11476 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/flash_models/flash_opt.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1741 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/flash_models/tensor_ops.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.994611 alpaca_farm-0.1.3/src/alpaca_farm/inference/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/inference/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    16279 2023-06-11 21:47:42.000000 alpaca_farm-0.1.3/src/alpaca_farm/inference/decode.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7147 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/inference/score.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3372 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/logging.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.995137 alpaca_farm-0.1.3/src/alpaca_farm/models/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/models/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2523 2023-06-11 04:26:11.000000 alpaca_farm-0.1.3/src/alpaca_farm/models/reward_model.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     8003 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/models/rl_models.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    11532 2023-06-10 06:21:02.000000 alpaca_farm-0.1.3/src/alpaca_farm/openai_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3208 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/reward_modeling_trainer.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.995889 alpaca_farm-0.1.3/src/alpaca_farm/rl/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      579 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/rl/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2054 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/rl/kl_controller.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    22881 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/rl/ppo_trainer.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7524 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/rl/ppo_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    13765 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/rl/rl_trainer.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3088 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/torch_ops.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3507 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/trainer_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1211 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/types.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6141 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/src/alpaca_farm/utils.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.983733 alpaca_farm-0.1.3/src/alpaca_farm.egg-info/
+-rw-r--r--   0 xuechenli   (501) staff       (20)    17050 2023-06-11 21:49:21.000000 alpaca_farm-0.1.3/src/alpaca_farm.egg-info/PKG-INFO
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4266 2023-06-11 21:49:21.000000 alpaca_farm-0.1.3/src/alpaca_farm.egg-info/SOURCES.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)        1 2023-06-11 21:49:21.000000 alpaca_farm-0.1.3/src/alpaca_farm.egg-info/dependency_links.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      295 2023-06-11 21:49:21.000000 alpaca_farm-0.1.3/src/alpaca_farm.egg-info/requires.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)       12 2023-06-11 21:49:21.000000 alpaca_farm-0.1.3/src/alpaca_farm.egg-info/top_level.txt
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2023-06-11 21:49:21.996332 alpaca_farm-0.1.3/tests/
+-rw-r--r--   0 xuechenli   (501) staff       (20)    12263 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/tests/test_flash_llama.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     8351 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/tests/test_flash_opt.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      899 2023-05-23 16:11:47.000000 alpaca_farm-0.1.3/tests/test_torch_ops.py
```

### Comparing `alpaca_farm-0.1.2/LICENSE` & `alpaca_farm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/PKG-INFO` & `alpaca_farm-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_farm
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -63,15 +63,21 @@
 The goal of AlpacaFarm is to provide three key components that tackles steps 2 and 3:
 Low-cost simulation of pairwise feedback from API models (e.g. GPT-4, ChatGPT), automated evaluations for methods
 development, and reference implementations of
 learning algorithms for comparison and modification.
 
 ## Installation
 
-For basic installation, run
+To install the stable release, run
+
+```bash
+pip install alpaca-farm
+```
+
+To install from the latest commit on `main` branch, run
 
 ```bash
 pip install git+https://github.com/tatsu-lab/alpaca_farm.git
 ```
 
 To enable FlashAttention and other optimizations, install
 the [`flash-attn`](https://github.com/HazyResearch/flash-attention) and [`apex`](https://github.com/NVIDIA/apex)
@@ -154,15 +160,16 @@
 ```bash
 pip install git+https://github.com/tatsu-lab/alpaca_farm.git --no-deps
 pip install -r https://raw.githubusercontent.com/tatsu-lab/alpaca_farm/main/src/alpaca_farm/auto_annotations/requirements.txt
 ```
 
 </details>
 
-To get started, set the environment variable OPENAI_API_KEY to your OpenAI API key, and (optionally) OPENAI_ORG to the organization ID. You can do this by running
+To get started, set the environment variable OPENAI_API_KEY to your OpenAI API key, and (optionally) OPENAI_ORG to the
+organization ID. You can do this by running
 
 ```bash
 export OPENAI_API_KEY="sk..."
 ```
 
 The easiest to add your model to the Alpaca Leaderboard is to run the following code, which only requires having outputs
 for your model on our eval data.
@@ -277,42 +284,74 @@
   --tf32 True \
   --flash_attn True \
   --output_path <your_output_path_to_store_samples>
 ```
 
 You can then use the generated samples at `<your_output_path_to_store_samples>` directly with our automated evaluation.
 
+### Expert Iteration
+
+To replicate our expert iteration results for the AlpacaFarm evaluation suite, first produce best-of-n samples. Run
+
+```bash
+python examples/best_of_n.py \
+  --task "run_best_of_n" \
+  --decoder_name_or_path <your_output_dir_for_decoder> \  # SFT10k model.
+  --scorer_name_or_path <your_output_dir_for_reward_model> \
+  --num_return_sequences 16 \  # This is the n in best-of-n.
+  --per_device_batch_size 4 \  # Reduce this if you don't have enough memory.
+  --split "unlabeled" \
+  --mixed_precision "bf16" \
+  --tf32 True \
+  --flash_attn True \
+  --output_path '<your_output_dir_for_expiter_data>/best_of_n_samples.json'
+```
+
+Then perform supervised fine-tuning from the SFT10k checkpoint with the best-of-n samples
+
+```bash
+bash examples/scripts/expiter.sh \
+  <your_output_dir_for_expiter> \
+  <your_wandb_run_name> \
+  <your_output_dir_for_sft10k> \
+  <your_output_dir_for_expiter_data>
+```
+
 ### OpenAI models
 
 To run the OpenAI reference models with our prompts and decoding hyperparameters, run
 
 ```bash
 python examples/oai_baselines.py \
   --model_name <oai_model_name> \
   --save_path <save_path> 
 ```
 
 You can then use the generated samples at `<save_path>` directly with our automated evaluation.
 
 ## Downloading pre-tuned AlpacaFarm models
 
-We provide model checkpoints for reward models and all our reference methods, listed in Table 2 of our [paper](https://arxiv.org/abs/2305.14387). Concretely, we tune each reference method in AlpacaFarm simulation and on human preference data and release both versions. The current list of models (available [here](https://huggingface.co/tatsu-lab)) includes:
+We provide model checkpoints for reward models and all our reference methods, listed in Table 2 of
+our [paper](https://arxiv.org/abs/2305.14387). Concretely, we tune each reference method in AlpacaFarm simulation and on
+human preference data and release both versions. The current list of models (
+available [here](https://huggingface.co/tatsu-lab)) includes:
 
 - `sft10k`, the supervised learning base model that we collect preference data with.
 - `reward-model-sim`, the reward model trained on AlpacaFarm preference data.
 - `reward-model-human`, the reward model trained on human preference data.
 - `ppo-sim`, the best PPO checkpoint trained in simulation.
 - `ppo-human`, the best PPO checkpoint trained on human data.
 - `expiter-sim`, the best expert iteration checkpoint trained in simulation.
 - `expiter-human`, the best expert iteration checkpoint trained on human data.
 - `feedme-sim`, the FeedME method trained on simulated preferences.
 - `feedme-human`, the FeedME method trained on human preferences.
 - `reward-condition-sim`, the reward conditioning method trained on simulated preferences.
 
-To download these checkpoints, first make sure to have a LLaMA-7B checkpoint [converted into the huggingface format](https://huggingface.co/docs/transformers/main/model_doc/llama).
+To download these checkpoints, first make sure to have a LLaMA-7B
+checkpoint [converted into the huggingface format](https://huggingface.co/docs/transformers/main/model_doc/llama).
 Then, run the following to download all AlpacaFarm models:
 
 ```
 python -m pretrained_models.recover_model_weights \
   --llama-7b-hf-dir <your_path_to_hf_converted_llama_ckpt_and_tokenizer> \
   --alpaca-farm-model-name all
 ```
@@ -322,21 +361,21 @@
 ```
 python -m pretrained_models.recover_model_weights \
   --llama-7b-hf-dir <your_path_to_hf_converted_llama_ckpt_and_tokenizer> \
   --alpaca-farm-model-name <one_of_the_model_names_from_above> \
   --models-save-dir <dir_to_save_all_models>
 ```
 
-To download either of the reward models individually, you'll need to have `sft10k` downloaded first to `<dir_to_save_all_models>`.
+To download either of the reward models individually, you'll need to have `sft10k` downloaded first
+to `<dir_to_save_all_models>`.
 
 ## Coming soon
 
 - [ ] Quark implementation
-- [ ] Expert iteration implementation
-- [ ] Human evaluation of generated samples from leaderboard models
+- [ ] Direct Preference Optimization
 
 ## Citation
 
 Please consider citing our work if you use the data or code in this repo.
 
 ```
 @misc{dubois2023alpacafarm,
```

### Comparing `alpaca_farm-0.1.2/README.md` & `alpaca_farm-0.1.3/src/alpaca_farm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: alpaca-farm
+Version: 0.1.3
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: full
+Provides-Extra: dev
+License-File: LICENSE
+
 <p align="center" width="100%">
 <img src="assets/AlpacaFarm_big.png" alt="AlpacaFarm" style="width: 50%; min-width: 300px; display: block; margin: auto;">
 </p>
 
 # AlpacaFarm: A Simulation Framework for Methods that <br/>Learn from Human Feedback
 
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE)
@@ -46,15 +63,21 @@
 The goal of AlpacaFarm is to provide three key components that tackles steps 2 and 3:
 Low-cost simulation of pairwise feedback from API models (e.g. GPT-4, ChatGPT), automated evaluations for methods
 development, and reference implementations of
 learning algorithms for comparison and modification.
 
 ## Installation
 
-For basic installation, run
+To install the stable release, run
+
+```bash
+pip install alpaca-farm
+```
+
+To install from the latest commit on `main` branch, run
 
 ```bash
 pip install git+https://github.com/tatsu-lab/alpaca_farm.git
 ```
 
 To enable FlashAttention and other optimizations, install
 the [`flash-attn`](https://github.com/HazyResearch/flash-attention) and [`apex`](https://github.com/NVIDIA/apex)
@@ -137,15 +160,16 @@
 ```bash
 pip install git+https://github.com/tatsu-lab/alpaca_farm.git --no-deps
 pip install -r https://raw.githubusercontent.com/tatsu-lab/alpaca_farm/main/src/alpaca_farm/auto_annotations/requirements.txt
 ```
 
 </details>
 
-To get started, set the environment variable OPENAI_API_KEY to your OpenAI API key, and (optionally) OPENAI_ORG to the organization ID. You can do this by running
+To get started, set the environment variable OPENAI_API_KEY to your OpenAI API key, and (optionally) OPENAI_ORG to the
+organization ID. You can do this by running
 
 ```bash
 export OPENAI_API_KEY="sk..."
 ```
 
 The easiest to add your model to the Alpaca Leaderboard is to run the following code, which only requires having outputs
 for your model on our eval data.
@@ -260,42 +284,74 @@
   --tf32 True \
   --flash_attn True \
   --output_path <your_output_path_to_store_samples>
 ```
 
 You can then use the generated samples at `<your_output_path_to_store_samples>` directly with our automated evaluation.
 
+### Expert Iteration
+
+To replicate our expert iteration results for the AlpacaFarm evaluation suite, first produce best-of-n samples. Run
+
+```bash
+python examples/best_of_n.py \
+  --task "run_best_of_n" \
+  --decoder_name_or_path <your_output_dir_for_decoder> \  # SFT10k model.
+  --scorer_name_or_path <your_output_dir_for_reward_model> \
+  --num_return_sequences 16 \  # This is the n in best-of-n.
+  --per_device_batch_size 4 \  # Reduce this if you don't have enough memory.
+  --split "unlabeled" \
+  --mixed_precision "bf16" \
+  --tf32 True \
+  --flash_attn True \
+  --output_path '<your_output_dir_for_expiter_data>/best_of_n_samples.json'
+```
+
+Then perform supervised fine-tuning from the SFT10k checkpoint with the best-of-n samples
+
+```bash
+bash examples/scripts/expiter.sh \
+  <your_output_dir_for_expiter> \
+  <your_wandb_run_name> \
+  <your_output_dir_for_sft10k> \
+  <your_output_dir_for_expiter_data>
+```
+
 ### OpenAI models
 
 To run the OpenAI reference models with our prompts and decoding hyperparameters, run
 
 ```bash
 python examples/oai_baselines.py \
   --model_name <oai_model_name> \
   --save_path <save_path> 
 ```
 
 You can then use the generated samples at `<save_path>` directly with our automated evaluation.
 
 ## Downloading pre-tuned AlpacaFarm models
 
-We provide model checkpoints for reward models and all our reference methods, listed in Table 2 of our [paper](https://arxiv.org/abs/2305.14387). Concretely, we tune each reference method in AlpacaFarm simulation and on human preference data and release both versions. The current list of models (available [here](https://huggingface.co/tatsu-lab)) includes:
+We provide model checkpoints for reward models and all our reference methods, listed in Table 2 of
+our [paper](https://arxiv.org/abs/2305.14387). Concretely, we tune each reference method in AlpacaFarm simulation and on
+human preference data and release both versions. The current list of models (
+available [here](https://huggingface.co/tatsu-lab)) includes:
 
 - `sft10k`, the supervised learning base model that we collect preference data with.
 - `reward-model-sim`, the reward model trained on AlpacaFarm preference data.
 - `reward-model-human`, the reward model trained on human preference data.
 - `ppo-sim`, the best PPO checkpoint trained in simulation.
 - `ppo-human`, the best PPO checkpoint trained on human data.
 - `expiter-sim`, the best expert iteration checkpoint trained in simulation.
 - `expiter-human`, the best expert iteration checkpoint trained on human data.
 - `feedme-sim`, the FeedME method trained on simulated preferences.
 - `feedme-human`, the FeedME method trained on human preferences.
 - `reward-condition-sim`, the reward conditioning method trained on simulated preferences.
 
-To download these checkpoints, first make sure to have a LLaMA-7B checkpoint [converted into the huggingface format](https://huggingface.co/docs/transformers/main/model_doc/llama).
+To download these checkpoints, first make sure to have a LLaMA-7B
+checkpoint [converted into the huggingface format](https://huggingface.co/docs/transformers/main/model_doc/llama).
 Then, run the following to download all AlpacaFarm models:
 
 ```
 python -m pretrained_models.recover_model_weights \
   --llama-7b-hf-dir <your_path_to_hf_converted_llama_ckpt_and_tokenizer> \
   --alpaca-farm-model-name all
 ```
@@ -305,21 +361,21 @@
 ```
 python -m pretrained_models.recover_model_weights \
   --llama-7b-hf-dir <your_path_to_hf_converted_llama_ckpt_and_tokenizer> \
   --alpaca-farm-model-name <one_of_the_model_names_from_above> \
   --models-save-dir <dir_to_save_all_models>
 ```
 
-To download either of the reward models individually, you'll need to have `sft10k` downloaded first to `<dir_to_save_all_models>`.
+To download either of the reward models individually, you'll need to have `sft10k` downloaded first
+to `<dir_to_save_all_models>`.
 
 ## Coming soon
 
 - [ ] Quark implementation
-- [ ] Expert iteration implementation
-- [ ] Human evaluation of generated samples from leaderboard models
+- [ ] Direct Preference Optimization
 
 ## Citation
 
 Please consider citing our work if you use the data or code in this repo.
 
 ```
 @misc{dubois2023alpacafarm,
```

### Comparing `alpaca_farm-0.1.2/setup.py` & `alpaca_farm-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/__init__.py` & `alpaca_farm-0.1.3/src/alpaca_farm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/accelerate_patch.py` & `alpaca_farm-0.1.3/src/alpaca_farm/accelerate_patch.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/__init__.py` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/analysis.py` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/analysis.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/annotator_pool_v0/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_with_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/annotators/greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/decoders.py` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/decoders.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/eval.py` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/eval.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/pairwise_annotators.py` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/pairwise_annotators.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/auto_annotations/utils.py` & `alpaca_farm-0.1.3/src/alpaca_farm/auto_annotations/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/common.py` & `alpaca_farm-0.1.3/src/alpaca_farm/common.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/constants.py` & `alpaca_farm-0.1.3/src/alpaca_farm/constants.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/data_postprocessor.py` & `alpaca_farm-0.1.3/src/alpaca_farm/data_postprocessor.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/data_preprocessor.py` & `alpaca_farm-0.1.3/src/alpaca_farm/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/data_utils.py` & `alpaca_farm-0.1.3/src/alpaca_farm/data_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,47 +12,60 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datasets
 import pandas as pd
 import transformers
 
-from . import utils
+from . import utils, logging
 from .data_preprocessor import (
     BinaryRewardModelingDataset,
     DataCollatorForBinaryRewardModelingDataset,
     DataCollatorForQueryResponseDataset,
     DataCollatorForSFTDataset,
     QueryResponseDataset,
     SFTDataset,
     split_train_into_train_and_eval,
 )
 
+logger = logging.get_logger(__name__)
+
 
 def make_supervised_data_module(
     tokenizer: transformers.PreTrainedTokenizer,
     data_args,
     training_args,
 ):
     prompt_dict = utils.jload(data_args.prompt_dict_path)
 
     alpaca_instructions = datasets.load_dataset(data_args.dataset_path, data_args.dataset_name)
-    train_df = pd.concat([pd.DataFrame(alpaca_instructions[split]) for split in data_args.train_splits])
-    eval_df = pd.concat([pd.DataFrame(alpaca_instructions[split]) for split in data_args.eval_splits])
 
+    train_df = pd.concat([pd.DataFrame(alpaca_instructions[split]) for split in data_args.train_splits])
     train_dataset = SFTDataset(
         df=train_df,
         prompt_dict=prompt_dict,
         tokenizer=tokenizer,
     )
-    eval_dataset = SFTDataset(
-        df=eval_df,
-        prompt_dict=prompt_dict,
-        tokenizer=tokenizer,
-    )
+
+    eval_dataset = None
+    if data_args.eval_splits is not None:
+        found_splits = [
+            pd.DataFrame(alpaca_instructions[split]) for split in data_args.eval_splits if split in alpaca_instructions
+        ]
+        if len(found_splits) > 0:
+            eval_df = pd.concat(found_splits)
+            eval_dataset = SFTDataset(
+                df=eval_df,
+                prompt_dict=prompt_dict,
+                tokenizer=tokenizer,
+            )
+
+    if eval_dataset is None:
+        logger.warning("Didn't find evaluation dataset. Disabling evaluation.")
+        training_args.do_eval = False
 
     data_collator = DataCollatorForSFTDataset(tokenizer=tokenizer)
     return dict(train_dataset=train_dataset, eval_dataset=eval_dataset, data_collator=data_collator)
 
 
 def make_binary_reward_modeling_data_module(
     tokenizer: transformers.PreTrainedTokenizer,
```

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/distributed_utils.py` & `alpaca_farm-0.1.3/src/alpaca_farm/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/flash_models/__init__.py` & `alpaca_farm-0.1.3/src/alpaca_farm/flash_models/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/flash_models/apex_patch.py` & `alpaca_farm-0.1.3/src/alpaca_farm/flash_models/apex_patch.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/flash_models/flash_llama.py` & `alpaca_farm-0.1.3/src/alpaca_farm/flash_models/flash_llama.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/flash_models/flash_opt.py` & `alpaca_farm-0.1.3/src/alpaca_farm/flash_models/flash_opt.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/flash_models/tensor_ops.py` & `alpaca_farm-0.1.3/src/alpaca_farm/flash_models/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/inference/__init__.py` & `alpaca_farm-0.1.3/src/alpaca_farm/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/inference/decode.py` & `alpaca_farm-0.1.3/src/alpaca_farm/inference/decode.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,37 +46,38 @@
     resize_token_embeddings_if_mismatch=True,
 ) -> Tuple[transformers.PreTrainedModel, transformers.PreTrainedTokenizer]:
     """Load huggingface model and tokenizer from path or with name for inference.
 
     This function should only be used for decoding or reward scoring.
 
     Notes:
-        - This function is only guaranteed to work correctly when loading admissible model families, i.e., opt and llama.
-        - Loaded models are always in eval mode.
+        - This function is only guaranteed to work correctly when loading admissible model families,
+            i.e., opt and llama.
+        - Loaded models are in eval mode.
         - By default, this function internally shrinks the model embedding size to avoid generating out of vocab tokens.
             Models like OPT are by default created with embedding size that's divisible by 64, even though the vocab
             size is not. This is to help with training speed, but can be problematic when generating, i.e., there is
             a low probability of generating out of vocab ids (especially for untrained models).
         - By default, loaded models are on the device specified by LOCAL_RANK or cpu.
-            - This behavior can be overridden by passing device_map to model_kwargs.
-        - By default, loaded tokenizers are fast tokenizers in left padding mode.
-            - This behavior can be overridden by passing use_fast and padding_side to tokenizer_kwargs.
+            - This behavior can be overridden by passing `device_map` to model_kwargs.
+        - By default, loaded tokenizers are slow tokenizers in left padding mode.
+            - This behavior can be overridden by passing `use_fast` and `padding_side` to tokenizer_kwargs.
     """
     logger.warning(f"Loading model for inference: {model_name_or_path}")
 
     local_rank, world_size = distributed_utils.setup()
     device = torch.device("cuda", local_rank) if torch.cuda.is_available() else torch.device("cpu")
     default_model_kwargs = dict(low_cpu_mem_usage=True, device_map={"": device}, cache_dir=cache_dir)
     if model_kwargs is None:
         model_kwargs = default_model_kwargs
     else:
         default_model_kwargs.update(model_kwargs)  # Make possible overriding default_model_kwargs.
         model_kwargs = default_model_kwargs
 
-    default_tokenizer_kwargs = dict(padding_side="left", use_fast=True, cache_dir=cache_dir)
+    default_tokenizer_kwargs = dict(padding_side="left", use_fast=False, cache_dir=cache_dir)
     if tokenizer_kwargs is None:
         tokenizer_kwargs = default_tokenizer_kwargs
     else:
         default_tokenizer_kwargs.update(tokenizer_kwargs)
         tokenizer_kwargs = default_tokenizer_kwargs
 
     model = model_cls.from_pretrained(model_name_or_path, **model_kwargs).eval()
```

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/inference/score.py` & `alpaca_farm-0.1.3/src/alpaca_farm/inference/score.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/logging.py` & `alpaca_farm-0.1.3/src/alpaca_farm/logging.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/models/__init__.py` & `alpaca_farm-0.1.3/src/alpaca_farm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/models/reward_model.py` & `alpaca_farm-0.1.3/src/alpaca_farm/models/reward_model.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/models/rl_models.py` & `alpaca_farm-0.1.3/src/alpaca_farm/models/rl_models.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/openai_utils.py` & `alpaca_farm-0.1.3/src/alpaca_farm/openai_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/reward_modeling_trainer.py` & `alpaca_farm-0.1.3/src/alpaca_farm/reward_modeling_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/rl/__init__.py` & `alpaca_farm-0.1.3/src/alpaca_farm/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/rl/kl_controller.py` & `alpaca_farm-0.1.3/src/alpaca_farm/rl/kl_controller.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/rl/ppo_trainer.py` & `alpaca_farm-0.1.3/src/alpaca_farm/rl/ppo_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/rl/ppo_utils.py` & `alpaca_farm-0.1.3/src/alpaca_farm/rl/ppo_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/rl/rl_trainer.py` & `alpaca_farm-0.1.3/src/alpaca_farm/rl/rl_trainer.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/torch_ops.py` & `alpaca_farm-0.1.3/src/alpaca_farm/torch_ops.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/trainer_utils.py` & `alpaca_farm-0.1.3/src/alpaca_farm/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/types.py` & `alpaca_farm-0.1.3/src/alpaca_farm/types.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm/utils.py` & `alpaca_farm-0.1.3/src/alpaca_farm/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm.egg-info/PKG-INFO` & `alpaca_farm-0.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: alpaca-farm
-Version: 0.1.2
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: full
-Provides-Extra: dev
-License-File: LICENSE
-
 <p align="center" width="100%">
 <img src="assets/AlpacaFarm_big.png" alt="AlpacaFarm" style="width: 50%; min-width: 300px; display: block; margin: auto;">
 </p>
 
 # AlpacaFarm: A Simulation Framework for Methods that <br/>Learn from Human Feedback
 
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE)
@@ -63,15 +46,21 @@
 The goal of AlpacaFarm is to provide three key components that tackles steps 2 and 3:
 Low-cost simulation of pairwise feedback from API models (e.g. GPT-4, ChatGPT), automated evaluations for methods
 development, and reference implementations of
 learning algorithms for comparison and modification.
 
 ## Installation
 
-For basic installation, run
+To install the stable release, run
+
+```bash
+pip install alpaca-farm
+```
+
+To install from the latest commit on `main` branch, run
 
 ```bash
 pip install git+https://github.com/tatsu-lab/alpaca_farm.git
 ```
 
 To enable FlashAttention and other optimizations, install
 the [`flash-attn`](https://github.com/HazyResearch/flash-attention) and [`apex`](https://github.com/NVIDIA/apex)
@@ -154,15 +143,16 @@
 ```bash
 pip install git+https://github.com/tatsu-lab/alpaca_farm.git --no-deps
 pip install -r https://raw.githubusercontent.com/tatsu-lab/alpaca_farm/main/src/alpaca_farm/auto_annotations/requirements.txt
 ```
 
 </details>
 
-To get started, set the environment variable OPENAI_API_KEY to your OpenAI API key, and (optionally) OPENAI_ORG to the organization ID. You can do this by running
+To get started, set the environment variable OPENAI_API_KEY to your OpenAI API key, and (optionally) OPENAI_ORG to the
+organization ID. You can do this by running
 
 ```bash
 export OPENAI_API_KEY="sk..."
 ```
 
 The easiest to add your model to the Alpaca Leaderboard is to run the following code, which only requires having outputs
 for your model on our eval data.
@@ -277,42 +267,74 @@
   --tf32 True \
   --flash_attn True \
   --output_path <your_output_path_to_store_samples>
 ```
 
 You can then use the generated samples at `<your_output_path_to_store_samples>` directly with our automated evaluation.
 
+### Expert Iteration
+
+To replicate our expert iteration results for the AlpacaFarm evaluation suite, first produce best-of-n samples. Run
+
+```bash
+python examples/best_of_n.py \
+  --task "run_best_of_n" \
+  --decoder_name_or_path <your_output_dir_for_decoder> \  # SFT10k model.
+  --scorer_name_or_path <your_output_dir_for_reward_model> \
+  --num_return_sequences 16 \  # This is the n in best-of-n.
+  --per_device_batch_size 4 \  # Reduce this if you don't have enough memory.
+  --split "unlabeled" \
+  --mixed_precision "bf16" \
+  --tf32 True \
+  --flash_attn True \
+  --output_path '<your_output_dir_for_expiter_data>/best_of_n_samples.json'
+```
+
+Then perform supervised fine-tuning from the SFT10k checkpoint with the best-of-n samples
+
+```bash
+bash examples/scripts/expiter.sh \
+  <your_output_dir_for_expiter> \
+  <your_wandb_run_name> \
+  <your_output_dir_for_sft10k> \
+  <your_output_dir_for_expiter_data>
+```
+
 ### OpenAI models
 
 To run the OpenAI reference models with our prompts and decoding hyperparameters, run
 
 ```bash
 python examples/oai_baselines.py \
   --model_name <oai_model_name> \
   --save_path <save_path> 
 ```
 
 You can then use the generated samples at `<save_path>` directly with our automated evaluation.
 
 ## Downloading pre-tuned AlpacaFarm models
 
-We provide model checkpoints for reward models and all our reference methods, listed in Table 2 of our [paper](https://arxiv.org/abs/2305.14387). Concretely, we tune each reference method in AlpacaFarm simulation and on human preference data and release both versions. The current list of models (available [here](https://huggingface.co/tatsu-lab)) includes:
+We provide model checkpoints for reward models and all our reference methods, listed in Table 2 of
+our [paper](https://arxiv.org/abs/2305.14387). Concretely, we tune each reference method in AlpacaFarm simulation and on
+human preference data and release both versions. The current list of models (
+available [here](https://huggingface.co/tatsu-lab)) includes:
 
 - `sft10k`, the supervised learning base model that we collect preference data with.
 - `reward-model-sim`, the reward model trained on AlpacaFarm preference data.
 - `reward-model-human`, the reward model trained on human preference data.
 - `ppo-sim`, the best PPO checkpoint trained in simulation.
 - `ppo-human`, the best PPO checkpoint trained on human data.
 - `expiter-sim`, the best expert iteration checkpoint trained in simulation.
 - `expiter-human`, the best expert iteration checkpoint trained on human data.
 - `feedme-sim`, the FeedME method trained on simulated preferences.
 - `feedme-human`, the FeedME method trained on human preferences.
 - `reward-condition-sim`, the reward conditioning method trained on simulated preferences.
 
-To download these checkpoints, first make sure to have a LLaMA-7B checkpoint [converted into the huggingface format](https://huggingface.co/docs/transformers/main/model_doc/llama).
+To download these checkpoints, first make sure to have a LLaMA-7B
+checkpoint [converted into the huggingface format](https://huggingface.co/docs/transformers/main/model_doc/llama).
 Then, run the following to download all AlpacaFarm models:
 
 ```
 python -m pretrained_models.recover_model_weights \
   --llama-7b-hf-dir <your_path_to_hf_converted_llama_ckpt_and_tokenizer> \
   --alpaca-farm-model-name all
 ```
@@ -322,21 +344,21 @@
 ```
 python -m pretrained_models.recover_model_weights \
   --llama-7b-hf-dir <your_path_to_hf_converted_llama_ckpt_and_tokenizer> \
   --alpaca-farm-model-name <one_of_the_model_names_from_above> \
   --models-save-dir <dir_to_save_all_models>
 ```
 
-To download either of the reward models individually, you'll need to have `sft10k` downloaded first to `<dir_to_save_all_models>`.
+To download either of the reward models individually, you'll need to have `sft10k` downloaded first
+to `<dir_to_save_all_models>`.
 
 ## Coming soon
 
 - [ ] Quark implementation
-- [ ] Expert iteration implementation
-- [ ] Human evaluation of generated samples from leaderboard models
+- [ ] Direct Preference Optimization
 
 ## Citation
 
 Please consider citing our work if you use the data or code in this repo.
 
 ```
 @misc{dubois2023alpacafarm,
```

### Comparing `alpaca_farm-0.1.2/src/alpaca_farm.egg-info/SOURCES.txt` & `alpaca_farm-0.1.3/src/alpaca_farm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/tests/test_flash_llama.py` & `alpaca_farm-0.1.3/tests/test_flash_llama.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/tests/test_flash_opt.py` & `alpaca_farm-0.1.3/tests/test_flash_opt.py`

 * *Files identical despite different names*

### Comparing `alpaca_farm-0.1.2/tests/test_torch_ops.py` & `alpaca_farm-0.1.3/tests/test_torch_ops.py`

 * *Files identical despite different names*

