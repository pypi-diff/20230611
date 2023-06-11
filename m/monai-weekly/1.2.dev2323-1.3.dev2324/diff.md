# Comparing `tmp/monai-weekly-1.2.dev2323.tar.gz` & `tmp/monai-weekly-1.3.dev2324.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monai-weekly-1.2.dev2323.tar", last modified: Sun Jun  4 02:36:52 2023, max compression
+gzip compressed data, was "monai-weekly-1.3.dev2324.tar", last modified: Sun Jun 11 02:35:37 2023, max compression
```

## Comparing `monai-weekly-1.2.dev2323.tar` & `monai-weekly-1.3.dev2324.tar`

### file list

```diff
@@ -1,1137 +1,1140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.552636 monai-weekly-1.2.dev2323/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-04 02:36:52.552636 monai-weekly-1.2.dev2323/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.552636 monai-weekly-1.2.dev2323/monai/
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-04 02:34:54.000000 monai-weekly-1.2.dev2323/monai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.088628 monai-weekly-1.2.dev2323/monai/_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.088628 monai-weekly-1.2.dev2323/monai/_extensions/gmm/
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/_extensions/gmm/gmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/_extensions/gmm/gmm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/_extensions/gmm/gmm_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/_extensions/gmm/gmm_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/_extensions/gmm/gmm_cuda_linalg.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/_extensions/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-04 02:36:52.552636 monai-weekly-1.2.dev2323/monai/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.092629 monai-weekly-1.2.dev2323/monai/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.096629 monai-weekly-1.2.dev2323/monai/apps/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/auto3dseg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37030 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/auto3dseg/auto_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/auto3dseg/bundle_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/auto3dseg/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27929 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/auto3dseg/ensemble_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/auto3dseg/hpo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/auto3dseg/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/auto3dseg/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.096629 monai-weekly-1.2.dev2323/monai/apps/deepedit/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/deepedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/deepedit/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/deepedit/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.096629 monai-weekly-1.2.dev2323/monai/apps/deepgrow/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/deepgrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/deepgrow/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/deepgrow/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    42011 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/deepgrow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.096629 monai-weekly-1.2.dev2323/monai/apps/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.100629 monai-weekly-1.2.dev2323/monai/apps/detection/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/metrics/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/metrics/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.100629 monai-weekly-1.2.dev2323/monai/apps/detection/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53640 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/networks/retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/networks/retinanet_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.104629 monai-weekly-1.2.dev2323/monai/apps/detection/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/transforms/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    69282 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.108629 monai-weekly-1.2.dev2323/monai/apps/detection/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/utils/ATSS_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/utils/anchor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/utils/box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/utils/box_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/utils/detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/utils/hard_negative_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/detection/utils/predict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.108629 monai-weekly-1.2.dev2323/monai/apps/mmars/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/mmars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/mmars/mmars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/mmars/model_desc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.108629 monai-weekly-1.2.dev2323/monai/apps/nnunet/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/nnunet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/nnunet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48597 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/nnunet/nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/nnunet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.112629 monai-weekly-1.2.dev2323/monai/apps/nuclick/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/nuclick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/nuclick/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.112629 monai-weekly-1.2.dev2323/monai/apps/pathology/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.112629 monai-weekly-1.2.dev2323/monai/apps/pathology/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/engines/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.112629 monai-weekly-1.2.dev2323/monai/apps/pathology/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/handlers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.112629 monai-weekly-1.2.dev2323/monai/apps/pathology/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/inferers/inferer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.112629 monai-weekly-1.2.dev2323/monai/apps/pathology/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/losses/hovernet_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.116629 monai-weekly-1.2.dev2323/monai/apps/pathology/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/metrics/lesion_froc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.116629 monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.116629 monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37322 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.116629 monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/stain/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/stain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/stain/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/stain/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/pathology/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.120629 monai-weekly-1.2.dev2323/monai/apps/reconstruction/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/mri_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.120629 monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.120629 monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/blocks/varnetblock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.120629 monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/nets/complex_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/nets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/nets/varnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.124629 monai-weekly-1.2.dev2323/monai/apps/reconstruction/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/reconstruction/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.124629 monai-weekly-1.2.dev2323/monai/apps/tcia/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/tcia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/tcia/label_desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/tcia/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.124629 monai-weekly-1.2.dev2323/monai/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/auto3dseg/algo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/auto3dseg/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/auto3dseg/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/auto3dseg/seg_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/auto3dseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.128629 monai-weekly-1.2.dev2323/monai/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/bundle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/bundle/config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    22360 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/bundle/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/bundle/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/bundle/reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    64632 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/bundle/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/bundle/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19141 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/bundle/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.132629 monai-weekly-1.2.dev2323/monai/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/config/deviceconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/config/type_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.144629 monai-weekly-1.2.dev2323/monai/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    68927 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    60619 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/image_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/meta_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    27511 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/test_time_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65095 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/video_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/wsi_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    49510 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/data/wsi_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.144629 monai-weekly-1.2.dev2323/monai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/engines/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/engines/multi_gpu_supervised_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/engines/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/engines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/engines/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.148630 monai-weekly-1.2.dev2323/monai/fl/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/fl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.148630 monai-weekly-1.2.dev2323/monai/fl/client/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/fl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/fl/client/client_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/fl/client/monai_algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.148630 monai-weekly-1.2.dev2323/monai/fl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/fl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/fl/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/fl/utils/exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/fl/utils/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.160630 monai-weekly-1.2.dev2323/monai/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/clearml_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/earlystop_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/logfile_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/lr_schedule_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/metrics_reloaded_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/nvtx_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/probability_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/smartcache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/stats_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/tensorboard_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/handlers/validation_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.164630 monai-weekly-1.2.dev2323/monai/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/inferers/inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/inferers/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/inferers/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/inferers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.168630 monai-weekly-1.2.dev2323/monai/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/losses/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/losses/deform.py
--rw-r--r--   0 runner    (1001) docker     (123)    46326 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/losses/ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/losses/giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/losses/image_dissimilarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/losses/multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/losses/spatial_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/losses/ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/losses/tversky.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/losses/unified_focal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.176630 monai-weekly-1.2.dev2323/monai/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/active_learning_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/f_beta_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/metrics/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.176630 monai-weekly-1.2.dev2323/monai/networks/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.188630 monai-weekly-1.2.dev2323/monai/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/acti_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/backbone_fpn_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/crf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/dints_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/feature_pyramid_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/fft_utils_t.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/squeeze_and_excitation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/blocks/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.196630 monai-weekly-1.2.dev2323/monai/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/layers/convutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/layers/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/layers/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/layers/gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/layers/simplelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/layers/spatial_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/layers/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.212630 monai-weekly-1.2.dev2323/monai/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/dints.py
--rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    40643 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/netadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/torchvision_fc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/nets/vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    47132 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.212630 monai-weekly-1.2.dev2323/monai/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/optimizers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/optimizers/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/optimizers/novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/optimizers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.216631 monai-weekly-1.2.dev2323/monai/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    37090 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.220631 monai-weekly-1.2.dev2323/monai/transforms/croppad/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/croppad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    74947 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/croppad/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/croppad/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    60872 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/croppad/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/croppad/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.224631 monai-weekly-1.2.dev2323/monai/transforms/intensity/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98613 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/intensity/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    76501 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/intensity/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    18233 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/inverse_batch_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.224631 monai-weekly-1.2.dev2323/monai/transforms/io/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25430 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/io/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/io/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.228631 monai-weekly-1.2.dev2323/monai/transforms/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/lazy/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/lazy/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/lazy/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/lazy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.228631 monai-weekly-1.2.dev2323/monai/transforms/meta_utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/meta_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/meta_utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/nvtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.228631 monai-weekly-1.2.dev2323/monai/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.232631 monai-weekly-1.2.dev2323/monai/transforms/signal/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/signal/array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.232631 monai-weekly-1.2.dev2323/monai/transforms/smooth_field/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/smooth_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/smooth_field/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/smooth_field/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.236631 monai-weekly-1.2.dev2323/monai/transforms/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   178852 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/spatial/array.py
--rw-r--r--   0 runner    (1001) docker     (123)   127396 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/spatial/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    31305 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/spatial/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.236631 monai-weekly-1.2.dev2323/monai/transforms/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70847 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/utility/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    76330 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    81124 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/utils_create_transform_ims.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/transforms/utils_pytorch_numpy_unification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.244631 monai-weekly-1.2.dev2323/monai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/utils/deprecate_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/utils/jupyter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28184 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/utils/nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/utils/state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/utils/type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.248631 monai-weekly-1.2.dev2323/monai/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/visualize/class_activation_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/visualize/gradient_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/visualize/img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/visualize/occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/visualize/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/monai/visualize/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.252631 monai-weekly-1.2.dev2323/monai_weekly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-04 02:36:52.000000 monai-weekly-1.2.dev2323/monai_weekly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34012 2023-06-04 02:36:52.000000 monai-weekly-1.2.dev2323/monai_weekly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 02:36:52.000000 monai-weekly-1.2.dev2323/monai_weekly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 02:36:52.000000 monai-weekly-1.2.dev2323/monai_weekly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-04 02:36:52.000000 monai-weekly-1.2.dev2323/monai_weekly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 02:36:52.000000 monai-weekly-1.2.dev2323/monai_weekly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-04 02:36:52.552636 monai-weekly-1.2.dev2323/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:36:52.552636 monai-weekly-1.2.dev2323/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_acn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_activationsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_add_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_add_coordinate_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_add_coordinate_channelsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_add_extreme_points_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_add_extreme_points_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_adn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_affine_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_anchor_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_apply_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_arraydataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_as_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_as_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_as_channel_last.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_as_channel_lastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_as_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_as_discreted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_atss_box_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_auto3dseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_auto3dseg_bundlegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_auto3dseg_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_auto3dseg_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bending_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bilateral_approx_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bilateral_approx_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bilateral_precise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_blend_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_border_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_border_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bounding_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bounding_rectd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_box_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bundle_ckpt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bundle_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bundle_get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bundle_init_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bundle_onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bundle_trt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bundle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bundle_verify_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bundle_verify_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_bundle_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_cachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_cachedataset_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_cachedataset_persistent_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_cachentransdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_call_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_cast_to_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_cast_to_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_center_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_center_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_center_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_center_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_channel_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_check_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_check_missing_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_classes_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_component_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25127 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_compose_get_number_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_compute_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_compute_f_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_compute_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_compute_generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_compute_ho_ver_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_compute_ho_ver_maps_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_compute_meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_compute_meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_compute_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_compute_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_compute_roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_compute_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_concat_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_contrastive_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_convert_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_convert_to_multi_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_convert_to_multi_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_convert_to_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_convert_to_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_convert_to_trt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_copy_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_copy_model_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_correct_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_create_cross_validation_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_create_grid_and_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_crf_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_crf_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_crop_foreground.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_crop_foregroundd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_csv_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_cumulative_average_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_cv2_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_data_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_data_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_dataset_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_decathlondataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_decollate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_deepedit_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_deepedit_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_deepgrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_deepgrow_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_deepgrow_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_delete_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_detect_envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_detection_coco_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_detector_boxselector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_dev_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_dice_ce_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_dints_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_dints_mixop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_dints_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_divisible_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_divisible_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_download_and_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_downsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_dvf2ddf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_ensure_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_ensure_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_ensure_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_ensure_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_ensure_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_enum_bound_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_eval_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_evenly_divisible_all_gather_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_factorized_increase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_factorized_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_fg_bg_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_fg_bg_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_file_basename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_fill_holes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_fill_holesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_fl_exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_fl_monai_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_fl_monai_algo_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_fl_monai_algo_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_flatten_sub_keysd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_foreground_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_foreground_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_fpn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_from_engine_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_gaussian_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generalized_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generalized_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generalized_wasserstein_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_distance_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_distance_mapd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_instance_border.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_instance_borderd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_instance_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_instance_centroidd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_instance_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_instance_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_instance_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_label_classes_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_param_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_pos_neg_label_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_spatial_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_succinct_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_succinct_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_watershed_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_watershed_markersd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_watershed_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generate_watershed_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_get_equivalent_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_get_extreme_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_get_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_get_package_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_get_unique_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_global_mutual_information_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_globalnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_grid_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_grid_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_grid_splitd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_classification_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_clearml_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_clearml_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_confusion_matrix_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_early_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_logfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_metrics_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_prob_map_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_regression_metrics_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_rocauc_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_smartcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_tb_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_tb_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_hardnegsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_header_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_hilbert_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_histogram_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_histogram_normalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_hovernet_instance_map_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_hovernet_instance_map_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_hovernet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_hovernet_nuclear_type_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_hovernet_nuclear_type_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_identityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_image_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_image_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_init_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_autorunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_bundle_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_classification_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_fast_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_gpu_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_lazy_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_segmentation_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_sliding_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_stn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_unet_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_integration_workflows_gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_intensity_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_intensity_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_inverse_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_inverse_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_invert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_invertd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_is_supported_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_itk_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_keep_largest_connected_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_keep_largest_connected_componentd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_kspace_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_label_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_label_filterd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_label_quality_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_label_to_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_label_to_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_label_to_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_label_to_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_lesion_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_list_data_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_list_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_lltm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_lmdbdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_lmdbdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_load_decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_load_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_load_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_load_spacing_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_loader_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_local_normalized_cross_correlation_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_localnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_look_up_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_make_nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_map_binary_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_map_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_map_label_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_map_label_valued.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_mask_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_mask_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_masked_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_masked_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_masked_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_matshow3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_mean_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_median_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_median_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_median_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_mednistdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_meta_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23538 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_metatensor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_mmar_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_module_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_monai_env_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_monai_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_mri_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_net_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_network_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_nifti_endianness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_nifti_header_revise.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_nifti_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_normalize_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_npzdictitemdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_nrrd_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_nuclick_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_numpy_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_nvtx_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_nvtx_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_one_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_optim_novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_optional_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_ori_ras_lps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_orientationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_p3d_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_pad_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_pad_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_parallel_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_parallel_execution_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_partition_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_partition_dataset_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_patch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_patch_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_pathology_he_stain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_pathology_he_stain_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_pathology_prob_nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_persistentdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_persistentdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_phl_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_phl_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_pil_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_plot_2d_or_3d_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_png_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_polyval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_prepare_batch_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_prepare_batch_default_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_prepare_batch_extra_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_prepare_batch_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_preset_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_print_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_print_transform_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_probnms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_probnmsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_pytorch_version_after.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_query_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_axis_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_axis_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_bias_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_bias_fieldd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_coarse_dropoutd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_coarse_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_coarse_shuffled.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_crop_by_label_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_crop_by_label_classesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_crop_by_pos_neg_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_crop_by_pos_neg_labeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_deform_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_elastic_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_elastic_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_elasticd_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_elasticd_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_gaussian_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_histogram_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_histogram_shiftd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_rician_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_rician_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_spatial_crop_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_spatial_crop_samplesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_weighted_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_weighted_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rand_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_randidentity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_random_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_randomizable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_randomizable_transform_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_randtorchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rankfilter_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_recon_net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_reference_based_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_reference_based_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_reg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_remove_repeated_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_remove_repeated_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_remove_small_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_repeat_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_repeat_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_replace_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_require_pkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_resample_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_resample_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_resample_to_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_resample_to_matchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_resize_with_pad_or_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_resize_with_pad_or_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_resized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_retinanet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_retinanet_predict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_safe_dtype_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_saliency_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_sample_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_save_classificationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_save_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_save_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_save_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_savitzky_golay_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_savitzky_golay_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_savitzky_golay_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_scale_intensity_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_scale_intensity_range_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_scale_intensity_range_percentilesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_scale_intensity_ranged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_se_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_se_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_seg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_select_cross_validation_folds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_select_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_senet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_separable_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_set_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_set_visible_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_shuffle_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_signal_continuouswavelet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_signal_fillempty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_signal_rand_add_gaussiannoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_signal_rand_add_sine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_signal_rand_add_sine_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_signal_rand_add_squarepulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_signal_rand_add_squarepulse_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_signal_rand_drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_signal_rand_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_signal_rand_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_signal_remove_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_simple_aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_simulatedelay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_simulatedelayd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_skip_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_slice_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_sliding_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_sliding_window_hovernet_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_sliding_window_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_smartcachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_smooth_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_sobel_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_sobel_gradientd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_some_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_spacingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_spatial_combine_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_spatial_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_spatial_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_spatial_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_spatial_resampled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_split_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_split_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_splitdim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_splitdimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_squeezedim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_squeezedimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_ssim_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_str2bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_str2list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_subpixel_upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    21649 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_tciadataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_testtimeaugmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_text_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_threadcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_threshold_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_threshold_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_timedcall_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_to_cupy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_to_cupyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_to_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_to_deviced.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_to_from_meta_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_to_numpyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_to_onehot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_to_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_to_pild.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_to_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_to_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_torchvision_fc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_torchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_traceable_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_train_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_trainable_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_trainable_joint_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_transposed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_tversky_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_unified_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_upsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_utils_pytorch_numpy_unification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_varnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_version_leq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_video_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_vis_cam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_vis_gradbased.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_vis_gradcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_vote_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_vote_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_warp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_watershed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_watershedd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_weighted_random_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_with_allow_missing_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_write_metrics_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_wsi_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_wsireader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_zipdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_zoom_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/tests/test_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-06-04 02:34:51.000000 monai-weekly-1.2.dev2323/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.419405 monai-weekly-1.3.dev2324/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-11 02:35:37.419405 monai-weekly-1.3.dev2324/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.423405 monai-weekly-1.3.dev2324/monai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-11 02:33:41.000000 monai-weekly-1.3.dev2324/monai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.815365 monai-weekly-1.3.dev2324/monai/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.819365 monai-weekly-1.3.dev2324/monai/_extensions/gmm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/_extensions/gmm/gmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/_extensions/gmm/gmm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/_extensions/gmm/gmm_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/_extensions/gmm/gmm_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/_extensions/gmm/gmm_cuda_linalg.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/_extensions/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-11 02:35:37.423405 monai-weekly-1.3.dev2324/monai/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.823366 monai-weekly-1.3.dev2324/monai/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.831366 monai-weekly-1.3.dev2324/monai/apps/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/auto3dseg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37173 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/auto3dseg/auto_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/auto3dseg/bundle_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/auto3dseg/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27796 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/auto3dseg/ensemble_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/auto3dseg/hpo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/auto3dseg/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/auto3dseg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.831366 monai-weekly-1.3.dev2324/monai/apps/deepedit/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/deepedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/deepedit/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/deepedit/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.835366 monai-weekly-1.3.dev2324/monai/apps/deepgrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/deepgrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/deepgrow/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/deepgrow/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42011 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/deepgrow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.835366 monai-weekly-1.3.dev2324/monai/apps/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.835366 monai-weekly-1.3.dev2324/monai/apps/detection/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/metrics/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/metrics/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.839367 monai-weekly-1.3.dev2324/monai/apps/detection/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53640 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/networks/retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/networks/retinanet_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.839367 monai-weekly-1.3.dev2324/monai/apps/detection/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/transforms/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69282 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.847367 monai-weekly-1.3.dev2324/monai/apps/detection/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/utils/ATSS_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/utils/anchor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/utils/box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/utils/box_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/utils/detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/utils/hard_negative_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/detection/utils/predict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.847367 monai-weekly-1.3.dev2324/monai/apps/mmars/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/mmars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/mmars/mmars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/mmars/model_desc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.851367 monai-weekly-1.3.dev2324/monai/apps/nnunet/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/nnunet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/nnunet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48597 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/nnunet/nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/nnunet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.851367 monai-weekly-1.3.dev2324/monai/apps/nuclick/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/nuclick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/nuclick/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.851367 monai-weekly-1.3.dev2324/monai/apps/pathology/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.851367 monai-weekly-1.3.dev2324/monai/apps/pathology/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/engines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.855368 monai-weekly-1.3.dev2324/monai/apps/pathology/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/handlers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.855368 monai-weekly-1.3.dev2324/monai/apps/pathology/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/inferers/inferer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.855368 monai-weekly-1.3.dev2324/monai/apps/pathology/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/losses/hovernet_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.855368 monai-weekly-1.3.dev2324/monai/apps/pathology/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/metrics/lesion_froc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.859368 monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.859368 monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37322 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.859368 monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/stain/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/stain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/stain/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/stain/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/pathology/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.863368 monai-weekly-1.3.dev2324/monai/apps/reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/mri_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.863368 monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.863368 monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/blocks/varnetblock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.867368 monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/nets/complex_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/nets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/nets/varnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.867368 monai-weekly-1.3.dev2324/monai/apps/reconstruction/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/reconstruction/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.871369 monai-weekly-1.3.dev2324/monai/apps/tcia/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/tcia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/tcia/label_desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/tcia/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.875369 monai-weekly-1.3.dev2324/monai/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/auto3dseg/algo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/auto3dseg/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/auto3dseg/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/auto3dseg/seg_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/auto3dseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.879369 monai-weekly-1.3.dev2324/monai/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/bundle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/bundle/config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22360 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/bundle/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/bundle/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/bundle/reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64632 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/bundle/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/bundle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19141 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/bundle/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.883370 monai-weekly-1.3.dev2324/monai/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/config/deviceconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/config/type_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.903371 monai-weekly-1.3.dev2324/monai/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68912 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60619 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/image_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/meta_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27511 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/test_time_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65095 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/video_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/wsi_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49510 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/data/wsi_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.907371 monai-weekly-1.3.dev2324/monai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/engines/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/engines/multi_gpu_supervised_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/engines/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/engines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/engines/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.907371 monai-weekly-1.3.dev2324/monai/fl/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/fl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.907371 monai-weekly-1.3.dev2324/monai/fl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/fl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/fl/client/client_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/fl/client/monai_algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.911371 monai-weekly-1.3.dev2324/monai/fl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/fl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/fl/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/fl/utils/exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/fl/utils/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.931373 monai-weekly-1.3.dev2324/monai/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/clearml_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/earlystop_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/logfile_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/lr_schedule_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/metrics_reloaded_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/nvtx_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/probability_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/smartcache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/stats_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/tensorboard_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/handlers/validation_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.935373 monai-weekly-1.3.dev2324/monai/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/inferers/inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/inferers/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/inferers/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/inferers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.939373 monai-weekly-1.3.dev2324/monai/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/losses/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/losses/deform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46326 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/losses/ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/losses/giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/losses/image_dissimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/losses/multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/losses/spatial_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/losses/ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/losses/tversky.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/losses/unified_focal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.951374 monai-weekly-1.3.dev2324/monai/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/active_learning_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/f_beta_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/metrics/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.955374 monai-weekly-1.3.dev2324/monai/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.967375 monai-weekly-1.3.dev2324/monai/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/acti_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/backbone_fpn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/crf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/dints_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/feature_pyramid_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/fft_utils_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/squeeze_and_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/blocks/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.975376 monai-weekly-1.3.dev2324/monai/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/layers/convutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/layers/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/layers/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/layers/gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/layers/simplelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/layers/spatial_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/layers/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.995377 monai-weekly-1.3.dev2324/monai/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/dints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40643 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/netadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/torchvision_fc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/nets/vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47132 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:36.999377 monai-weekly-1.3.dev2324/monai/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/optimizers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/optimizers/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/optimizers/novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/optimizers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.003377 monai-weekly-1.3.dev2324/monai/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37090 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.011378 monai-weekly-1.3.dev2324/monai/transforms/croppad/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/croppad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74891 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/croppad/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/croppad/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60872 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/croppad/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/croppad/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.011378 monai-weekly-1.3.dev2324/monai/transforms/intensity/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107801 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/intensity/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82230 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/intensity/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18233 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/inverse_batch_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.015378 monai-weekly-1.3.dev2324/monai/transforms/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25374 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/io/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/io/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.015378 monai-weekly-1.3.dev2324/monai/transforms/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/lazy/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/lazy/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/lazy/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/lazy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.019379 monai-weekly-1.3.dev2324/monai/transforms/meta_utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/meta_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/meta_utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/nvtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.019379 monai-weekly-1.3.dev2324/monai/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40802 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.019379 monai-weekly-1.3.dev2324/monai/transforms/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/signal/array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.023379 monai-weekly-1.3.dev2324/monai/transforms/smooth_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/smooth_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/smooth_field/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/smooth_field/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.027379 monai-weekly-1.3.dev2324/monai/transforms/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   178796 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/spatial/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127396 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/spatial/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/spatial/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.027379 monai-weekly-1.3.dev2324/monai/transforms/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70307 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/utility/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76161 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81124 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/utils_create_transform_ims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/transforms/utils_pytorch_numpy_unification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.035380 monai-weekly-1.3.dev2324/monai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/utils/deprecate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/utils/jupyter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28184 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/utils/nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/utils/state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/utils/type_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.039380 monai-weekly-1.3.dev2324/monai/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/visualize/class_activation_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/visualize/gradient_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/visualize/img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/visualize/occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/visualize/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/monai/visualize/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.043380 monai-weekly-1.3.dev2324/monai_weekly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-11 02:35:36.000000 monai-weekly-1.3.dev2324/monai_weekly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34146 2023-06-11 02:35:36.000000 monai-weekly-1.3.dev2324/monai_weekly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 02:35:36.000000 monai-weekly-1.3.dev2324/monai_weekly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 02:35:36.000000 monai-weekly-1.3.dev2324/monai_weekly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-11 02:35:36.000000 monai-weekly-1.3.dev2324/monai_weekly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 02:35:36.000000 monai-weekly-1.3.dev2324/monai_weekly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-11 02:35:37.423405 monai-weekly-1.3.dev2324/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 02:35:37.419405 monai-weekly-1.3.dev2324/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_acn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_activationsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_add_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_add_coordinate_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_add_coordinate_channelsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_add_extreme_points_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_add_extreme_points_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_adn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_affine_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_anchor_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_apply_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_arraydataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_as_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_as_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_as_channel_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_as_channel_lastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_as_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_as_discreted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_atss_box_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_auto3dseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_auto3dseg_bundlegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_auto3dseg_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_auto3dseg_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bending_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bilateral_approx_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bilateral_approx_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bilateral_precise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_blend_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_border_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_border_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bounding_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bounding_rectd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_box_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bundle_ckpt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bundle_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bundle_get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bundle_init_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bundle_onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bundle_trt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bundle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bundle_verify_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bundle_verify_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_bundle_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_cachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_cachedataset_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_cachedataset_persistent_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_cachentransdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_call_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_cast_to_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_cast_to_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_center_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_center_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_center_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_center_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_channel_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_check_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_check_missing_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_classes_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_component_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25175 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_compose_get_number_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_compute_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_compute_f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_compute_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_compute_generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_compute_ho_ver_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_compute_ho_ver_maps_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_compute_meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_compute_meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_compute_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_compute_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_compute_roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_compute_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_concat_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_contrastive_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_convert_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_convert_to_multi_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_convert_to_multi_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_convert_to_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_convert_to_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_convert_to_trt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_copy_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_copy_model_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_correct_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_create_cross_validation_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_create_grid_and_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_crf_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_crf_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_crop_foreground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_crop_foregroundd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_csv_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_cumulative_average_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_cv2_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_data_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_dataset_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_decathlondataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_decollate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_deepedit_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_deepedit_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_deepgrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_deepgrow_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_deepgrow_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_delete_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_detect_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_detection_coco_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_detector_boxselector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_dev_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_dice_ce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_dints_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_dints_mixop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_dints_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_divisible_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_divisible_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_download_and_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_downsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_dvf2ddf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_ensure_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_ensure_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_ensure_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_ensure_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_ensure_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_enum_bound_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_eval_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_evenly_divisible_all_gather_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_factorized_increase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_factorized_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_fg_bg_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_fg_bg_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_file_basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_fill_holes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_fill_holesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_fl_exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_fl_monai_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_fl_monai_algo_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_fl_monai_algo_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_flatten_sub_keysd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_foreground_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_foreground_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_fpn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_from_engine_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_gaussian_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generalized_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generalized_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generalized_wasserstein_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_distance_mapd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_instance_border.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_instance_borderd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_instance_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_instance_centroidd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_instance_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_instance_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_instance_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_label_classes_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_param_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_pos_neg_label_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_spatial_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_succinct_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_succinct_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_watershed_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_watershed_markersd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_watershed_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generate_watershed_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_get_equivalent_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_get_extreme_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_get_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_get_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_get_unique_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_global_mutual_information_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_globalnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_grid_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_grid_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_grid_splitd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_classification_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_clearml_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_clearml_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_confusion_matrix_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_early_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_logfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_metrics_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_prob_map_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_regression_metrics_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_rocauc_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_smartcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_tb_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_tb_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_hardnegsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_header_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_hilbert_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_histogram_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_histogram_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_hovernet_instance_map_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_hovernet_instance_map_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_hovernet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_hovernet_nuclear_type_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_hovernet_nuclear_type_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_identityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_image_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_image_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_init_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_autorunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_bundle_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_classification_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_fast_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_gpu_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_lazy_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_sliding_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_unet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_integration_workflows_gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_intensity_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_intensity_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18993 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_inverse_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_inverse_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_invert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_invertd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_is_supported_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_itk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_keep_largest_connected_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_keep_largest_connected_componentd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_kspace_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_label_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_label_filterd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_label_quality_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_label_to_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_label_to_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_label_to_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_label_to_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_lesion_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_list_data_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_list_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_lltm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_lmdbdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_lmdbdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_load_decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_load_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_load_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_load_spacing_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_loader_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_local_normalized_cross_correlation_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_localnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_look_up_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_make_nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_map_binary_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_map_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_map_label_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_map_label_valued.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_mask_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_mask_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_masked_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_masked_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_masked_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_matshow3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_mean_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_median_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_median_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_median_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_mednistdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_meta_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23538 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_metatensor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_mmar_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_monai_env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_monai_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_mri_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_net_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_network_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_nifti_endianness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_nifti_header_revise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_nifti_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_normalize_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_npzdictitemdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_nrrd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_nuclick_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_numpy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_nvtx_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_nvtx_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_optim_novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_optional_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_ori_ras_lps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_orientationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_p3d_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_pad_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_pad_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_parallel_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_parallel_execution_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_partition_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_partition_dataset_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_patch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_patch_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_pathology_he_stain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_pathology_he_stain_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_pathology_prob_nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_persistentdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_persistentdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_phl_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_phl_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_pil_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_plot_2d_or_3d_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_png_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_polyval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_prepare_batch_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_prepare_batch_default_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_prepare_batch_extra_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_prepare_batch_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_preset_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_print_transform_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_probnms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_probnmsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_pytorch_version_after.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_query_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_axis_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_axis_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_bias_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_bias_fieldd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_coarse_dropoutd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_coarse_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_coarse_shuffled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_crop_by_label_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_crop_by_label_classesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_crop_by_pos_neg_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_crop_by_pos_neg_labeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_deform_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_elastic_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_elastic_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_elasticd_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_elasticd_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_gaussian_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_histogram_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_histogram_shiftd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_rician_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_rician_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_scale_intensity_fixed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_scale_intensity_fixed_meand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_spatial_crop_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_spatial_crop_samplesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_weighted_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_weighted_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rand_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_randidentity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_random_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_randomizable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_randomizable_transform_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_randtorchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rankfilter_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_recon_net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_reference_based_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_reference_based_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_reg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_remove_repeated_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_remove_repeated_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_remove_small_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_repeat_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_repeat_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_replace_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_require_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_resample_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_resample_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_resample_to_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_resample_to_matchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_resize_with_pad_or_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_resize_with_pad_or_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_resized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_retinanet_predict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_safe_dtype_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_saliency_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_sample_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_save_classificationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_save_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_save_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_save_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_savitzky_golay_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_savitzky_golay_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_savitzky_golay_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_scale_intensity_fixed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_scale_intensity_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_scale_intensity_range_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_scale_intensity_range_percentilesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_scale_intensity_ranged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_se_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_se_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_seg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_select_cross_validation_folds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_select_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_separable_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_set_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_set_visible_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_shuffle_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_signal_continuouswavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_signal_fillempty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_signal_rand_add_gaussiannoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_signal_rand_add_sine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_signal_rand_add_sine_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_signal_rand_add_squarepulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_signal_rand_add_squarepulse_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_signal_rand_drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_signal_rand_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_signal_rand_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_signal_remove_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_simple_aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_simulatedelay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_simulatedelayd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_skip_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_slice_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_sliding_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_sliding_window_hovernet_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_sliding_window_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_smartcachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_smooth_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_sobel_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_sobel_gradientd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_some_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_spacingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_spatial_combine_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_spatial_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_spatial_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_spatial_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_spatial_resampled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_split_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_split_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_splitdim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_splitdimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_squeezedim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_squeezedimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_ssim_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_str2bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_str2list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_subpixel_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21649 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_tciadataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_testtimeaugmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_text_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_threadcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_threshold_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_threshold_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_timedcall_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_to_cupy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_to_cupyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_to_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_to_deviced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_to_from_meta_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_to_numpyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_to_onehot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_to_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_to_pild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_to_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_to_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_torchvision_fc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_torchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_traceable_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_train_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_trainable_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_trainable_joint_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_transposed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_tversky_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_unified_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_upsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_utils_pytorch_numpy_unification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_varnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_version_leq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_video_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_vis_cam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_vis_gradbased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_vis_gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_vote_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_vote_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_watershed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_watershedd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_weighted_random_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_with_allow_missing_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_write_metrics_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_wsi_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_wsireader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_zipdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_zoom_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/tests/test_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-06-11 02:33:38.000000 monai-weekly-1.3.dev2324/versioneer.py
```

### Comparing `monai-weekly-1.2.dev2323/LICENSE` & `monai-weekly-1.3.dev2324/LICENSE`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/PKG-INFO` & `monai-weekly-1.3.dev2324/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.2.dev2323
+Version: 1.3.dev2324
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
@@ -90,15 +90,15 @@
 ## Features
 > _Please see [the technical highlights](https://docs.monai.io/en/latest/highlights.html) and [What's New](https://docs.monai.io/en/latest/whatsnew.html) of the milestone releases._
 
 - flexible pre-processing for multi-dimensional medical imaging data;
 - compositional & portable APIs for ease of integration in existing workflows;
 - domain-specific implementations for networks, losses, evaluation metrics and more;
 - customizable design for varying user expertise;
-- multi-GPU data parallelism support.
+- multi-GPU multi-node data parallelism support.
 
 
 ## Installation
 
 To install [the current release](https://pypi.org/project/monai/), you can simply run:
 
 ```bash
```

### Comparing `monai-weekly-1.2.dev2323/README.md` & `monai-weekly-1.3.dev2324/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ## Features
 > _Please see [the technical highlights](https://docs.monai.io/en/latest/highlights.html) and [What's New](https://docs.monai.io/en/latest/whatsnew.html) of the milestone releases._
 
 - flexible pre-processing for multi-dimensional medical imaging data;
 - compositional & portable APIs for ease of integration in existing workflows;
 - domain-specific implementations for networks, losses, evaluation metrics and more;
 - customizable design for varying user expertise;
-- multi-GPU data parallelism support.
+- multi-GPU multi-node data parallelism support.
 
 
 ## Installation
 
 To install [the current release](https://pypi.org/project/monai/), you can simply run:
 
 ```bash
```

### Comparing `monai-weekly-1.2.dev2323/monai/__init__.py` & `monai-weekly-1.3.dev2324/monai/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,8 +74,8 @@
     "metrics",
     "networks",
     "optimizers",
     "transforms",
     "utils",
     "visualize",
 ]
-__commit_id__ = "00376799a2ae0e6b84fb1efe1ef9ff6d8cbedc19"
+__commit_id__ = "858b86cf3af36e17efac8661533e3aa642dff5be"
```

### Comparing `monai-weekly-1.2.dev2323/monai/_extensions/__init__.py` & `monai-weekly-1.3.dev2324/monai/_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/_extensions/gmm/gmm.cpp` & `monai-weekly-1.3.dev2324/monai/_extensions/gmm/gmm.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/_extensions/gmm/gmm.h` & `monai-weekly-1.3.dev2324/monai/_extensions/gmm/gmm.h`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/_extensions/gmm/gmm_cpu.cpp` & `monai-weekly-1.3.dev2324/monai/_extensions/gmm/gmm_cpu.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/_extensions/gmm/gmm_cuda.cu` & `monai-weekly-1.3.dev2324/monai/_extensions/gmm/gmm_cuda.cu`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/_extensions/gmm/gmm_cuda_linalg.cuh` & `monai-weekly-1.3.dev2324/monai/_extensions/gmm/gmm_cuda_linalg.cuh`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/_extensions/loader.py` & `monai-weekly-1.3.dev2324/monai/_extensions/loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/auto3dseg/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/auto3dseg/__main__.py` & `monai-weekly-1.3.dev2324/monai/apps/auto3dseg/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/auto3dseg/auto_runner.py` & `monai-weekly-1.3.dev2324/monai/apps/auto3dseg/auto_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,14 +288,17 @@
         if hpo_backend.lower() != "nni":
             raise NotImplementedError("HPOGen backend only supports NNI")
         self.hpo = hpo and has_nni
         self.set_hpo_params()
         self.search_space: dict[str, dict[str, Any]] = {}
         self.hpo_tasks = 0
 
+        if "sigmoid" not in self.kwargs and "sigmoid" in self.data_src_cfg:
+            self.kwargs["sigmoid"] = self.data_src_cfg["sigmoid"]
+
     def read_cache(self):
         """
         Check if the intermediate result is cached after each step in the current working directory
 
         Returns:
             a dict of cache results. If not_use_cache is set to True, or there is no cache file in the
             working directory, the result will be ``empty_cache`` in which all ``has_cache`` keys are
```

### Comparing `monai-weekly-1.2.dev2323/monai/apps/auto3dseg/bundle_gen.py` & `monai-weekly-1.3.dev2324/monai/apps/auto3dseg/bundle_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from monai.auto3dseg.utils import algo_to_pickle
 from monai.bundle.config_parser import ConfigParser
 from monai.config import PathLike
 from monai.utils import ensure_tuple
 from monai.utils.enums import AlgoKeys
 
 logger = get_logger(module_name=__name__)
-ALGO_HASH = os.environ.get("MONAI_ALGO_HASH", "58af562")
+ALGO_HASH = os.environ.get("MONAI_ALGO_HASH", "b5c01d4")
 
 __all__ = ["BundleAlgo", "BundleGen"]
 
 
 class BundleAlgo(Algo):
     """
     An algorithm represented by a set of bundle configurations and scripts.
@@ -533,15 +533,15 @@
         Args:
             output_folder: the output folder to save each algorithm.
             num_fold: the number of cross validation fold.
             gpu_customization: the switch to determine automatically customize/optimize bundle script/config
                 parameters for each bundleAlgo based on gpus. Custom parameters are obtained through dummy
                 training to simulate the actual model training process and hyperparameter optimization (HPO)
                 experiments.
-            gpu_customization_specs (optinal): the dictionary to enable users overwrite the HPO settings. user can
+            gpu_customization_specs: the dictionary to enable users overwrite the HPO settings. user can
                 overwrite part of variables as follows or all of them. The structure is as follows.
             allow_skip: a switch to determine if some Algo in the default templates can be skipped based on the
                 analysis on the dataset from Auto3DSeg DataAnalyzer.
 
                 .. code-block:: python
 
                     gpu_customization_specs = {
```

### Comparing `monai-weekly-1.2.dev2323/monai/apps/auto3dseg/data_analyzer.py` & `monai-weekly-1.3.dev2324/monai/apps/auto3dseg/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/auto3dseg/ensemble_builder.py` & `monai-weekly-1.3.dev2324/monai/apps/auto3dseg/ensemble_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
                 The first group contains:
 
                     - ``"infer_files"``: file paths to the images to read in a list.
                     - ``"files_slices"``: a value type of `slice`. The files_slices will slice the ``"infer_files"`` and
                       only make prediction on the infer_files[file_slices].
                     - ``"mode"``: ensemble mode. Currently "mean" and "vote" (majority voting) schemes are supported.
                     - ``"image_save_func"``: a dictionary used to instantiate the ``SaveImage`` transform. When specified,
-                      the ensemble prediction will save the prediciton files, instead of keeping the files in the memory.
+                      the ensemble prediction will save the prediction files, instead of keeping the files in the memory.
                       Example: `{"_target_": "SaveImage", "output_dir": "./"}`
                     - ``"sigmoid"``: use the sigmoid function (e.g. x > 0.5) to convert the prediction probability map
                       to the label class prediction, otherwise argmax(x) is used.
                     - ``"algo_spec_params"``: a dictionary to add pred_params that are specific to a model.
                       The dict has a format of {"<name of algo>": "<pred_params for that algo>"}.
 
                 The parameters in the second group is defined in the ``config`` of each Algo templates. Please check:
@@ -548,15 +548,15 @@
         """
 
         if num_fold <= 0:
             raise ValueError(f"num_fold is expected to be an integer greater than zero. Now it gets {num_fold}")
         self.num_fold = num_fold
 
     def ensemble(self):
-        if self.mgpu:  # torch.cuda.device_count() is not used because env is not set by autorruner
+        if self.mgpu:  # torch.cuda.device_count() is not used because env is not set by autorunner
             # init multiprocessing and update infer_files
             dist.init_process_group(backend="nccl", init_method="env://")
             self.world_size = dist.get_world_size()
             self.rank = dist.get_rank()
             logger.addFilter(RankFilter())
         # set params after init_process_group to know the rank
         self.set_num_fold(num_fold=self.num_fold)
@@ -582,22 +582,18 @@
         builder.set_ensemble_method(self.ensemble_method)
         self.ensembler = builder.get_ensemble()
         infer_files = self.ensembler.infer_files
         if len(infer_files) < self.world_size:
             if len(infer_files) == 0:
                 logger.info("No testing files for inference is provided. Ensembler ending.")
                 return
-            infer_files = (
-                partition_dataset(data=infer_files, shuffle=False, num_partitions=len(infer_files))[self.rank]
-                if self.rank < len(infer_files)
-                else []
-            )
+            infer_files = [infer_files[self.rank]] if self.rank < len(infer_files) else []
         else:
             infer_files = partition_dataset(
-                data=infer_files, shuffle=False, num_partitions=self.world_size, even_divisible=True
+                data=infer_files, shuffle=False, num_partitions=self.world_size, even_divisible=False
             )[self.rank]
 
         # TO DO: Add some function in ensembler for infer_files update?
         self.ensembler.infer_files = infer_files
         # add rank to pred_params
         self.kwargs["rank"] = self.rank
         self.kwargs["image_save_func"] = save_image
```

### Comparing `monai-weekly-1.2.dev2323/monai/apps/auto3dseg/hpo_gen.py` & `monai-weekly-1.3.dev2324/monai/apps/auto3dseg/hpo_gen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/auto3dseg/transforms.py` & `monai-weekly-1.3.dev2324/monai/apps/auto3dseg/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/auto3dseg/utils.py` & `monai-weekly-1.3.dev2324/monai/apps/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/datasets.py` & `monai-weekly-1.3.dev2324/monai/apps/datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/deepedit/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/deepedit/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/deepedit/interaction.py` & `monai-weekly-1.3.dev2324/monai/apps/deepedit/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/deepedit/transforms.py` & `monai-weekly-1.3.dev2324/monai/apps/deepedit/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/deepgrow/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/deepgrow/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/deepgrow/dataset.py` & `monai-weekly-1.3.dev2324/monai/apps/deepgrow/dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/deepgrow/interaction.py` & `monai-weekly-1.3.dev2324/monai/apps/deepgrow/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/deepgrow/transforms.py` & `monai-weekly-1.3.dev2324/monai/apps/deepgrow/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/metrics/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/metrics/coco.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/metrics/coco.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/metrics/matching.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/metrics/matching.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/networks/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/networks/retinanet_detector.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/networks/retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/networks/retinanet_network.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/networks/retinanet_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/transforms/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/transforms/array.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/transforms/box_ops.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/transforms/box_ops.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/transforms/dictionary.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/utils/ATSS_matcher.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/utils/ATSS_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/utils/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/utils/anchor_utils.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/utils/anchor_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/utils/box_coder.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/utils/box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/utils/box_selector.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/utils/box_selector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/utils/detector_utils.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/utils/detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/utils/hard_negative_sampler.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/utils/hard_negative_sampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/detection/utils/predict_utils.py` & `monai-weekly-1.3.dev2324/monai/apps/detection/utils/predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/mmars/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/mmars/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/mmars/mmars.py` & `monai-weekly-1.3.dev2324/monai/apps/mmars/mmars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/mmars/model_desc.py` & `monai-weekly-1.3.dev2324/monai/apps/mmars/model_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/nnunet/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/nnunet/__main__.py` & `monai-weekly-1.3.dev2324/monai/apps/nnunet/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/nnunet/nnunetv2_runner.py` & `monai-weekly-1.3.dev2324/monai/apps/nnunet/nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/nnunet/utils.py` & `monai-weekly-1.3.dev2324/monai/apps/nnunet/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/nuclick/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/nuclick/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/nuclick/transforms.py` & `monai-weekly-1.3.dev2324/monai/apps/nuclick/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/engines/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/engines/utils.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/handlers/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/handlers/utils.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/handlers/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 def from_engine_hovernet(keys: KeysCollection, nested_key: str) -> Callable[[Any], Any]:
     """
     Since the output of HoVerNet is a dictionary, this function is to extend `monai.handlers.from_engine`
     to work with HoVerNet.
 
-    If data is a list of nestes dictionaries after decollating, extract nested value with expected keys and
+    If data is a list of nested dictionaries after decollating, extract nested value with expected keys and
     construct lists respectively, for example,
     if data is `[{"A": {"C": 1, "D": 2}, "B": {"C": 2, "D": 2}}, {"A":  {"C": 3, "D": 2}, "B":  {"C": 4, "D": 2}}]`,
     from_engine_hovernet(["A", "B"], "C"): `([1, 3], [2, 4])`.
 
     Here is a simple example::
 
         from monai.handlers import MeanDice, from_engine_hovernet
```

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/inferers/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/inferers/inferer.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/losses/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/losses/hovernet_loss.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/losses/hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/metrics/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/metrics/lesion_froc.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/metrics/lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/post/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/post/array.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/post/dictionary.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/stain/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/stain/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/stain/array.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/stain/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/transforms/stain/dictionary.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/transforms/stain/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/pathology/utils.py` & `monai-weekly-1.3.dev2324/monai/apps/pathology/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/complex_utils.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/fastmri_reader.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/mri_utils.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/blocks/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/blocks/varnetblock.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/blocks/varnetblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/nets/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/nets/complex_unet.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/nets/complex_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/nets/utils.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/nets/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/networks/nets/varnet.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/networks/nets/varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/transforms/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/transforms/array.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/reconstruction/transforms/dictionary.py` & `monai-weekly-1.3.dev2324/monai/apps/reconstruction/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/tcia/__init__.py` & `monai-weekly-1.3.dev2324/monai/apps/tcia/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/tcia/label_desc.py` & `monai-weekly-1.3.dev2324/monai/apps/tcia/label_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/tcia/utils.py` & `monai-weekly-1.3.dev2324/monai/apps/tcia/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/apps/utils.py` & `monai-weekly-1.3.dev2324/monai/apps/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/auto3dseg/__init__.py` & `monai-weekly-1.3.dev2324/monai/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/auto3dseg/algo_gen.py` & `monai-weekly-1.3.dev2324/monai/auto3dseg/algo_gen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/auto3dseg/analyzer.py` & `monai-weekly-1.3.dev2324/monai/auto3dseg/analyzer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/auto3dseg/operations.py` & `monai-weekly-1.3.dev2324/monai/auto3dseg/operations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/auto3dseg/seg_summarizer.py` & `monai-weekly-1.3.dev2324/monai/auto3dseg/seg_summarizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/auto3dseg/utils.py` & `monai-weekly-1.3.dev2324/monai/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/bundle/__init__.py` & `monai-weekly-1.3.dev2324/monai/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/bundle/__main__.py` & `monai-weekly-1.3.dev2324/monai/bundle/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/bundle/config_item.py` & `monai-weekly-1.3.dev2324/monai/bundle/config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/bundle/config_parser.py` & `monai-weekly-1.3.dev2324/monai/bundle/config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/bundle/properties.py` & `monai-weekly-1.3.dev2324/monai/bundle/properties.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/bundle/reference_resolver.py` & `monai-weekly-1.3.dev2324/monai/bundle/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/bundle/scripts.py` & `monai-weekly-1.3.dev2324/monai/bundle/scripts.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/bundle/utils.py` & `monai-weekly-1.3.dev2324/monai/bundle/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/bundle/workflows.py` & `monai-weekly-1.3.dev2324/monai/bundle/workflows.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/config/__init__.py` & `monai-weekly-1.3.dev2324/monai/config/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/config/deviceconfig.py` & `monai-weekly-1.3.dev2324/monai/config/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/config/type_definitions.py` & `monai-weekly-1.3.dev2324/monai/config/type_definitions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/__init__.py` & `monai-weekly-1.3.dev2324/monai/data/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/box_utils.py` & `monai-weekly-1.3.dev2324/monai/data/box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/csv_saver.py` & `monai-weekly-1.3.dev2324/monai/data/csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/dataloader.py` & `monai-weekly-1.3.dev2324/monai/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/dataset.py` & `monai-weekly-1.3.dev2324/monai/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -562,15 +562,15 @@
             db_name: lmdb database file name. Defaults to "monai_cache".
             progress: whether to display a progress bar.
             pickle_protocol: pickle protocol version. Defaults to pickle.HIGHEST_PROTOCOL.
                 https://docs.python.org/3/library/pickle.html#pickle-protocols
             hash_transform: a callable to compute hash from the transform information when caching.
                 This may reduce errors due to transforms changing during experiments. Default to None (no hash).
                 Other options are `pickle_hashing` and `json_hashing` functions from `monai.data.utils`.
-            reset_ops_id: whether to set `TraceKeys.ID` to ``Tracekys.NONE``, defaults to ``True``.
+            reset_ops_id: whether to set `TraceKeys.ID` to ``Tracekeys.NONE``, defaults to ``True``.
                 When this is enabled, the traced transform instance IDs will be removed from the cached MetaTensors.
                 This is useful for skipping the transform instance checks when inverting applied operations
                 using the cached content and with re-created transform instances.
             lmdb_kwargs: additional keyword arguments to the lmdb environment.
                 for more details please visit: https://lmdb.readthedocs.io/en/release/#environment-class
         """
         super().__init__(
@@ -937,15 +937,15 @@
     transform sequence before being fed to GPU. At the same time, another thread is preparing replacement
     items by applying the transform sequence to items not in cache. Once one epoch is completed, Smart
     Cache replaces the same number of items with replacement items.
     Smart Cache uses a simple `running window` algorithm to determine the cache content and replacement items.
     Let N be the configured number of objects in cache; and R be the number of replacement objects (R = ceil(N * r),
     where r is the configured replace rate).
     For more details, please refer to:
-    https://docs.nvidia.com/clara/tlt-mi/clara-train-sdk-v3.0/nvmidl/additional_features/smart_cache.html#smart-cache
+    https://docs.nvidia.com/clara/clara-train-archive/3.1/nvmidl/additional_features/smart_cache.html
     If passing slicing indices, will return a PyTorch Subset, for example: `data: Subset = dataset[1:4]`,
     for more details, please check: https://pytorch.org/docs/stable/data.html#torch.utils.data.Subset
 
     For example, if we have 5 images: `[image1, image2, image3, image4, image5]`, and `cache_num=4`, `replace_rate=0.25`.
     so the actual training images cached and replaced for every epoch are as below::
 
         epoch 1: [image1, image2, image3, image4]
```

### Comparing `monai-weekly-1.2.dev2323/monai/data/dataset_summary.py` & `monai-weekly-1.3.dev2324/monai/data/dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/decathlon_datalist.py` & `monai-weekly-1.3.dev2324/monai/data/decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/fft_utils.py` & `monai-weekly-1.3.dev2324/monai/data/fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/folder_layout.py` & `monai-weekly-1.3.dev2324/monai/data/folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/grid_dataset.py` & `monai-weekly-1.3.dev2324/monai/data/grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/image_dataset.py` & `monai-weekly-1.3.dev2324/monai/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/image_reader.py` & `monai-weekly-1.3.dev2324/monai/data/image_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/image_writer.py` & `monai-weekly-1.3.dev2324/monai/data/image_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/iterable_dataset.py` & `monai-weekly-1.3.dev2324/monai/data/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/itk_torch_bridge.py` & `monai-weekly-1.3.dev2324/monai/data/itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/meta_obj.py` & `monai-weekly-1.3.dev2324/monai/data/meta_obj.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/meta_tensor.py` & `monai-weekly-1.3.dev2324/monai/data/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/samplers.py` & `monai-weekly-1.3.dev2324/monai/data/samplers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/synthetic.py` & `monai-weekly-1.3.dev2324/monai/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/test_time_augmentation.py` & `monai-weekly-1.3.dev2324/monai/data/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/thread_buffer.py` & `monai-weekly-1.3.dev2324/monai/data/thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/torchscript_utils.py` & `monai-weekly-1.3.dev2324/monai/data/torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/utils.py` & `monai-weekly-1.3.dev2324/monai/data/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/video_dataset.py` & `monai-weekly-1.3.dev2324/monai/data/video_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/wsi_datasets.py` & `monai-weekly-1.3.dev2324/monai/data/wsi_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/data/wsi_reader.py` & `monai-weekly-1.3.dev2324/monai/data/wsi_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/engines/__init__.py` & `monai-weekly-1.3.dev2324/monai/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/engines/evaluator.py` & `monai-weekly-1.3.dev2324/monai/engines/evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/engines/multi_gpu_supervised_trainer.py` & `monai-weekly-1.3.dev2324/monai/engines/multi_gpu_supervised_trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/engines/trainer.py` & `monai-weekly-1.3.dev2324/monai/engines/trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/engines/utils.py` & `monai-weekly-1.3.dev2324/monai/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/engines/workflow.py` & `monai-weekly-1.3.dev2324/monai/engines/workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/fl/__init__.py` & `monai-weekly-1.3.dev2324/monai/fl/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/fl/client/__init__.py` & `monai-weekly-1.3.dev2324/monai/fl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/fl/client/client_algo.py` & `monai-weekly-1.3.dev2324/monai/fl/client/client_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/fl/client/monai_algo.py` & `monai-weekly-1.3.dev2324/monai/fl/client/monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/fl/utils/__init__.py` & `monai-weekly-1.3.dev2324/monai/fl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/fl/utils/constants.py` & `monai-weekly-1.3.dev2324/monai/fl/utils/constants.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/fl/utils/exchange_object.py` & `monai-weekly-1.3.dev2324/monai/fl/utils/exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/fl/utils/filters.py` & `monai-weekly-1.3.dev2324/monai/fl/utils/filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/__init__.py` & `monai-weekly-1.3.dev2324/monai/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/checkpoint_loader.py` & `monai-weekly-1.3.dev2324/monai/handlers/checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/checkpoint_saver.py` & `monai-weekly-1.3.dev2324/monai/handlers/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/classification_saver.py` & `monai-weekly-1.3.dev2324/monai/handlers/classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/clearml_handlers.py` & `monai-weekly-1.3.dev2324/monai/handlers/clearml_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/confusion_matrix.py` & `monai-weekly-1.3.dev2324/monai/handlers/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/decollate_batch.py` & `monai-weekly-1.3.dev2324/monai/handlers/decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/earlystop_handler.py` & `monai-weekly-1.3.dev2324/monai/handlers/earlystop_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/garbage_collector.py` & `monai-weekly-1.3.dev2324/monai/handlers/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/hausdorff_distance.py` & `monai-weekly-1.3.dev2324/monai/handlers/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/ignite_metric.py` & `monai-weekly-1.3.dev2324/monai/handlers/ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/logfile_handler.py` & `monai-weekly-1.3.dev2324/monai/handlers/logfile_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/lr_schedule_handler.py` & `monai-weekly-1.3.dev2324/monai/handlers/lr_schedule_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/mean_dice.py` & `monai-weekly-1.3.dev2324/monai/handlers/mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/mean_iou.py` & `monai-weekly-1.3.dev2324/monai/handlers/mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/metric_logger.py` & `monai-weekly-1.3.dev2324/monai/handlers/metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/metrics_reloaded_handler.py` & `monai-weekly-1.3.dev2324/monai/handlers/metrics_reloaded_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/metrics_saver.py` & `monai-weekly-1.3.dev2324/monai/handlers/metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/mlflow_handler.py` & `monai-weekly-1.3.dev2324/monai/handlers/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/nvtx_handlers.py` & `monai-weekly-1.3.dev2324/monai/handlers/nvtx_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/panoptic_quality.py` & `monai-weekly-1.3.dev2324/monai/handlers/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/parameter_scheduler.py` & `monai-weekly-1.3.dev2324/monai/handlers/parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/postprocessing.py` & `monai-weekly-1.3.dev2324/monai/handlers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/probability_maps.py` & `monai-weekly-1.3.dev2324/monai/handlers/probability_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/regression_metrics.py` & `monai-weekly-1.3.dev2324/monai/handlers/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/roc_auc.py` & `monai-weekly-1.3.dev2324/monai/handlers/roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/smartcache_handler.py` & `monai-weekly-1.3.dev2324/monai/handlers/smartcache_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/stats_handler.py` & `monai-weekly-1.3.dev2324/monai/handlers/stats_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/surface_distance.py` & `monai-weekly-1.3.dev2324/monai/handlers/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/tensorboard_handlers.py` & `monai-weekly-1.3.dev2324/monai/handlers/tensorboard_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/utils.py` & `monai-weekly-1.3.dev2324/monai/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/handlers/validation_handler.py` & `monai-weekly-1.3.dev2324/monai/handlers/validation_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/inferers/__init__.py` & `monai-weekly-1.3.dev2324/monai/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/inferers/inferer.py` & `monai-weekly-1.3.dev2324/monai/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/inferers/merger.py` & `monai-weekly-1.3.dev2324/monai/inferers/merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/inferers/splitter.py` & `monai-weekly-1.3.dev2324/monai/inferers/splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/inferers/utils.py` & `monai-weekly-1.3.dev2324/monai/inferers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/losses/__init__.py` & `monai-weekly-1.3.dev2324/monai/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/losses/contrastive.py` & `monai-weekly-1.3.dev2324/monai/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/losses/deform.py` & `monai-weekly-1.3.dev2324/monai/losses/deform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/losses/dice.py` & `monai-weekly-1.3.dev2324/monai/losses/dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/losses/ds_loss.py` & `monai-weekly-1.3.dev2324/monai/losses/ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/losses/focal_loss.py` & `monai-weekly-1.3.dev2324/monai/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/losses/giou_loss.py` & `monai-weekly-1.3.dev2324/monai/losses/giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/losses/image_dissimilarity.py` & `monai-weekly-1.3.dev2324/monai/losses/image_dissimilarity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/losses/multi_scale.py` & `monai-weekly-1.3.dev2324/monai/losses/multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/losses/spatial_mask.py` & `monai-weekly-1.3.dev2324/monai/losses/spatial_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/losses/ssim_loss.py` & `monai-weekly-1.3.dev2324/monai/losses/ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/losses/tversky.py` & `monai-weekly-1.3.dev2324/monai/losses/tversky.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/losses/unified_focal_loss.py` & `monai-weekly-1.3.dev2324/monai/losses/unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/__init__.py` & `monai-weekly-1.3.dev2324/monai/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/active_learning_metrics.py` & `monai-weekly-1.3.dev2324/monai/metrics/active_learning_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/confusion_matrix.py` & `monai-weekly-1.3.dev2324/monai/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/cumulative_average.py` & `monai-weekly-1.3.dev2324/monai/metrics/cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/f_beta_score.py` & `monai-weekly-1.3.dev2324/monai/metrics/f_beta_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/froc.py` & `monai-weekly-1.3.dev2324/monai/metrics/froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/generalized_dice.py` & `monai-weekly-1.3.dev2324/monai/metrics/generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/hausdorff_distance.py` & `monai-weekly-1.3.dev2324/monai/metrics/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/loss_metric.py` & `monai-weekly-1.3.dev2324/monai/metrics/loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/meandice.py` & `monai-weekly-1.3.dev2324/monai/metrics/meandice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/meaniou.py` & `monai-weekly-1.3.dev2324/monai/metrics/meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/metric.py` & `monai-weekly-1.3.dev2324/monai/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/panoptic_quality.py` & `monai-weekly-1.3.dev2324/monai/metrics/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/regression.py` & `monai-weekly-1.3.dev2324/monai/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/rocauc.py` & `monai-weekly-1.3.dev2324/monai/metrics/rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/surface_dice.py` & `monai-weekly-1.3.dev2324/monai/metrics/surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/surface_distance.py` & `monai-weekly-1.3.dev2324/monai/metrics/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/utils.py` & `monai-weekly-1.3.dev2324/monai/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/metrics/wrapper.py` & `monai-weekly-1.3.dev2324/monai/metrics/wrapper.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/__init__.py` & `monai-weekly-1.3.dev2324/monai/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/__init__.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/acti_norm.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/acti_norm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/activation.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/activation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/aspp.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/backbone_fpn_utils.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/backbone_fpn_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/convolutions.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/crf.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/crf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/denseblock.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/dints_block.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/dints_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/downsample.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/downsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/dynunet_block.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/encoder.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/encoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/fcn.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/fcn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/feature_pyramid_network.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/feature_pyramid_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/fft_utils_t.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/fft_utils_t.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/localnet_block.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/mlp.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/patchembedding.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/regunet_block.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/segresnet_block.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/selfattention.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/squeeze_and_excitation.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/text_embedding.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/text_embedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/transformerblock.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/unetr_block.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/upsample.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/blocks/warp.py` & `monai-weekly-1.3.dev2324/monai/networks/blocks/warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/layers/__init__.py` & `monai-weekly-1.3.dev2324/monai/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/layers/convutils.py` & `monai-weekly-1.3.dev2324/monai/networks/layers/convutils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/layers/drop_path.py` & `monai-weekly-1.3.dev2324/monai/networks/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/layers/factories.py` & `monai-weekly-1.3.dev2324/monai/networks/layers/factories.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/layers/filtering.py` & `monai-weekly-1.3.dev2324/monai/networks/layers/filtering.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/layers/gmm.py` & `monai-weekly-1.3.dev2324/monai/networks/layers/gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/layers/simplelayers.py` & `monai-weekly-1.3.dev2324/monai/networks/layers/simplelayers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/layers/spatial_transforms.py` & `monai-weekly-1.3.dev2324/monai/networks/layers/spatial_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/layers/utils.py` & `monai-weekly-1.3.dev2324/monai/networks/layers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/layers/weight_init.py` & `monai-weekly-1.3.dev2324/monai/networks/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/__init__.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/ahnet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/attentionunet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/autoencoder.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/basic_unet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/basic_unetplusplus.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/classifier.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/classifier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/densenet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/dints.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/dints.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/dynunet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/dynunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/efficientnet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/flexible_unet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/fullyconnectednet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/generator.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/highresnet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/hovernet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/milmodel.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/netadapter.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/netadapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/regressor.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/regressor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/regunet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/resnet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/segresnet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/segresnet_ds.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/senet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/swin_unetr.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/torchvision_fc.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/torchvision_fc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/transchex.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/unet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/unetr.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/varautoencoder.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/vit.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/vit.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/vitautoenc.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/nets/vnet.py` & `monai-weekly-1.3.dev2324/monai/networks/nets/vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/networks/utils.py` & `monai-weekly-1.3.dev2324/monai/networks/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/optimizers/__init__.py` & `monai-weekly-1.3.dev2324/monai/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/optimizers/lr_finder.py` & `monai-weekly-1.3.dev2324/monai/optimizers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/optimizers/lr_scheduler.py` & `monai-weekly-1.3.dev2324/monai/optimizers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/optimizers/novograd.py` & `monai-weekly-1.3.dev2324/monai/optimizers/novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/optimizers/utils.py` & `monai-weekly-1.3.dev2324/monai/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/__init__.py` & `monai-weekly-1.3.dev2324/monai/transforms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,18 +114,20 @@
     RandGaussianSmooth,
     RandGibbsNoise,
     RandHistogramShift,
     RandIntensityRemap,
     RandKSpaceSpikeNoise,
     RandRicianNoise,
     RandScaleIntensity,
+    RandScaleIntensityFixedMean,
     RandShiftIntensity,
     RandStdShiftIntensity,
     SavitzkyGolaySmooth,
     ScaleIntensity,
+    ScaleIntensityFixedMean,
     ScaleIntensityRange,
     ScaleIntensityRangePercentiles,
     ShiftIntensity,
     StdShiftIntensity,
     ThresholdIntensity,
 )
 from .intensity.dictionary import (
@@ -194,14 +196,17 @@
     RandKSpaceSpikeNoiseDict,
     RandRicianNoised,
     RandRicianNoiseD,
     RandRicianNoiseDict,
     RandScaleIntensityd,
     RandScaleIntensityD,
     RandScaleIntensityDict,
+    RandScaleIntensityFixedMeand,
+    RandScaleIntensityFixedMeanD,
+    RandScaleIntensityFixedMeanDict,
     RandShiftIntensityd,
     RandShiftIntensityD,
     RandShiftIntensityDict,
     RandStdShiftIntensityd,
     RandStdShiftIntensityD,
     RandStdShiftIntensityDict,
     SavitzkyGolaySmoothd,
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/adaptors.py` & `monai-weekly-1.3.dev2324/monai/transforms/adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/compose.py` & `monai-weekly-1.3.dev2324/monai/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/croppad/__init__.py` & `monai-weekly-1.3.dev2324/monai/transforms/croppad/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/croppad/array.py` & `monai-weekly-1.3.dev2324/monai/transforms/croppad/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-A collection of "vanilla" transforms for crop and pad operations
-https://github.com/Project-MONAI/MONAI/wiki/MONAI_Design
+A collection of "vanilla" transforms for crop and pad operations.
 """
 
 from __future__ import annotations
 
 import warnings
 from collections.abc import Callable, Sequence
 from itertools import chain
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/croppad/batch.py` & `monai-weekly-1.3.dev2324/monai/transforms/croppad/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-A collection of "vanilla" transforms for crop and pad operations acting on batches of data
-https://github.com/Project-MONAI/MONAI/wiki/MONAI_Design
+A collection of "vanilla" transforms for crop and pad operations acting on batches of data.
 """
 
 from __future__ import annotations
 
 from collections.abc import Hashable, Mapping
 from typing import Any
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/croppad/dictionary.py` & `monai-weekly-1.3.dev2324/monai/transforms/croppad/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/croppad/functional.py` & `monai-weekly-1.3.dev2324/monai/transforms/croppad/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-A collection of "functional" transforms for spatial operations
-https://github.com/Project-MONAI/MONAI/wiki/MONAI_Design
+A collection of "functional" transforms for spatial operations.
 """
 
 from __future__ import annotations
 
 import warnings
 
 import numpy as np
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/intensity/__init__.py` & `monai-weekly-1.3.dev2324/monai/transforms/intensity/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/intensity/array.py` & `monai-weekly-1.3.dev2324/monai/transforms/intensity/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-A collection of "vanilla" transforms for intensity adjustment
-https://github.com/Project-MONAI/MONAI/wiki/MONAI_Design
+A collection of "vanilla" transforms for intensity adjustment.
 """
 
 from __future__ import annotations
 
 from abc import abstractmethod
 from collections.abc import Callable, Iterable, Sequence
 from functools import partial
@@ -45,14 +44,16 @@
     "ShiftIntensity",
     "RandShiftIntensity",
     "StdShiftIntensity",
     "RandStdShiftIntensity",
     "RandBiasField",
     "ScaleIntensity",
     "RandScaleIntensity",
+    "ScaleIntensityFixedMean",
+    "RandScaleIntensityFixedMean",
     "NormalizeIntensity",
     "ThresholdIntensity",
     "ScaleIntensityRange",
     "AdjustContrast",
     "RandAdjustContrast",
     "ScaleIntensityRangePercentiles",
     "MaskIntensity",
@@ -463,14 +464,169 @@
                 ret = rescale_array(img_t, self.minv, self.maxv, dtype=self.dtype)
         else:
             ret = (img_t * (1 + self.factor)) if self.factor is not None else img_t
         ret = convert_to_dst_type(ret, dst=img, dtype=self.dtype or img_t.dtype)[0]
         return ret
 
 
+class ScaleIntensityFixedMean(Transform):
+    """
+    Scale the intensity of input image by ``v = v * (1 + factor)``, then shift the output so that the output image has the
+    same mean as the input.
+    """
+
+    backend = [TransformBackends.TORCH, TransformBackends.NUMPY]
+
+    def __init__(
+        self,
+        factor: float = 0,
+        preserve_range: bool = False,
+        fixed_mean: bool = True,
+        channel_wise: bool = False,
+        dtype: DtypeLike = np.float32,
+    ) -> None:
+        """
+        Args:
+            factor: factor scale by ``v = v * (1 + factor)``.
+            preserve_range: clips the output array/tensor to the range of the input array/tensor
+            fixed_mean: subtract the mean intensity before scaling with `factor`, then add the same value after scaling
+                to ensure that the output has the same mean as the input.
+            channel_wise: if True, scale on each channel separately. `preserve_range` and `fixed_mean` are also applied
+            on each channel separately if `channel_wise` is True. Please ensure that the first dimension represents the
+            channel of the image if True.
+            dtype: output data type, if None, same as input image. defaults to float32.
+        """
+        self.factor = factor
+        self.preserve_range = preserve_range
+        self.fixed_mean = fixed_mean
+        self.channel_wise = channel_wise
+        self.dtype = dtype
+
+    def __call__(self, img: NdarrayOrTensor, factor=None) -> NdarrayOrTensor:
+        """
+        Apply the transform to `img`.
+        Args:
+            img: the input tensor/array
+            factor: factor scale by ``v = v * (1 + factor)``
+
+        """
+
+        factor = factor if factor is not None else self.factor
+
+        img = convert_to_tensor(img, track_meta=get_track_meta())
+        img_t = convert_to_tensor(img, track_meta=False)
+        ret: NdarrayOrTensor
+        if self.channel_wise:
+            out = []
+            for d in img_t:
+                if self.preserve_range:
+                    clip_min = d.min()
+                    clip_max = d.max()
+
+                if self.fixed_mean:
+                    mn = d.mean()
+                    d = d - mn
+
+                out_channel = d * (1 + factor)
+
+                if self.fixed_mean:
+                    out_channel = out_channel + mn
+
+                if self.preserve_range:
+                    out_channel = clip(out_channel, clip_min, clip_max)
+
+                out.append(out_channel)
+            ret = torch.stack(out)  # type: ignore
+        else:
+            if self.preserve_range:
+                clip_min = img_t.min()
+                clip_max = img_t.max()
+
+            if self.fixed_mean:
+                mn = img_t.mean()
+                img_t = img_t - mn
+
+            ret = img_t * (1 + factor)
+
+            if self.fixed_mean:
+                ret = ret + mn
+
+            if self.preserve_range:
+                ret = clip(ret, clip_min, clip_max)
+
+        ret = convert_to_dst_type(ret, dst=img, dtype=self.dtype or img_t.dtype)[0]
+        return ret
+
+
+class RandScaleIntensityFixedMean(RandomizableTransform):
+    """
+    Randomly scale the intensity of input image by ``v = v * (1 + factor)`` where the `factor`
+    is randomly picked. Subtract the mean intensity before scaling with `factor`, then add the same value after scaling
+    to ensure that the output has the same mean as the input.
+    """
+
+    backend = ScaleIntensityFixedMean.backend
+
+    def __init__(
+        self,
+        prob: float = 0.1,
+        factors: Sequence[float] | float = 0,
+        fixed_mean: bool = True,
+        preserve_range: bool = False,
+        dtype: DtypeLike = np.float32,
+    ) -> None:
+        """
+        Args:
+            factors: factor range to randomly scale by ``v = v * (1 + factor)``.
+                if single number, factor value is picked from (-factors, factors).
+            preserve_range: clips the output array/tensor to the range of the input array/tensor
+            fixed_mean: subtract the mean intensity before scaling with `factor`, then add the same value after scaling
+                to ensure that the output has the same mean as the input.
+            channel_wise: if True, scale on each channel separately. `preserve_range` and `fixed_mean` are also applied
+            on each channel separately if `channel_wise` is True. Please ensure that the first dimension represents the
+            channel of the image if True.
+            dtype: output data type, if None, same as input image. defaults to float32.
+
+        """
+        RandomizableTransform.__init__(self, prob)
+        if isinstance(factors, (int, float)):
+            self.factors = (min(-factors, factors), max(-factors, factors))
+        elif len(factors) != 2:
+            raise ValueError("factors should be a number or pair of numbers.")
+        else:
+            self.factors = (min(factors), max(factors))
+        self.factor = self.factors[0]
+        self.fixed_mean = fixed_mean
+        self.preserve_range = preserve_range
+        self.dtype = dtype
+
+        self.scaler = ScaleIntensityFixedMean(
+            factor=self.factor, fixed_mean=self.fixed_mean, preserve_range=self.preserve_range, dtype=self.dtype
+        )
+
+    def randomize(self, data: Any | None = None) -> None:
+        super().randomize(None)
+        if not self._do_transform:
+            return None
+        self.factor = self.R.uniform(low=self.factors[0], high=self.factors[1])
+
+    def __call__(self, img: NdarrayOrTensor, randomize: bool = True) -> NdarrayOrTensor:
+        """
+        Apply the transform to `img`.
+        """
+        img = convert_to_tensor(img, track_meta=get_track_meta())
+        if randomize:
+            self.randomize()
+
+        if not self._do_transform:
+            return convert_data_type(img, dtype=self.dtype)[0]
+
+        return self.scaler(img, self.factor)
+
+
 class RandScaleIntensity(RandomizableTransform):
     """
     Randomly scale the intensity of input image by ``v = v * (1 + factor)`` where the `factor`
     is randomly picked.
     """
 
     backend = ScaleIntensity.backend
@@ -796,70 +952,127 @@
         ret: NdarrayOrTensor = convert_data_type(img, dtype=dtype)[0]
 
         return ret
 
 
 class AdjustContrast(Transform):
     """
-    Changes image intensity by gamma. Each pixel/voxel intensity is updated as::
+    Changes image intensity with gamma transform. Each pixel/voxel intensity is updated as::
 
         x = ((x - min) / intensity_range) ^ gamma * intensity_range + min
 
     Args:
         gamma: gamma value to adjust the contrast as function.
+        invert_image: whether to invert the image before applying gamma augmentation. If True, multiply all intensity
+            values with -1 before the gamma transform and again after the gamma transform. This behaviour is mimicked
+            from `nnU-Net <https://www.nature.com/articles/s41592-020-01008-z>`_, specifically `this
+            <https://github.com/MIC-DKFZ/batchgenerators/blob/7fb802b28b045b21346b197735d64f12fbb070aa/batchgenerators/augmentations/color_augmentations.py#L107>`_
+            function.
+        retain_stats: if True, applies a scaling factor and an offset to all intensity values after gamma transform to
+            ensure that the output intensity distribution has the same mean and standard deviation as the intensity
+            distribution of the input. This behaviour is mimicked from `nnU-Net
+            <https://www.nature.com/articles/s41592-020-01008-z>`_, specifically `this
+            <https://github.com/MIC-DKFZ/batchgenerators/blob/7fb802b28b045b21346b197735d64f12fbb070aa/batchgenerators/augmentations/color_augmentations.py#L107>`_
+            function.
     """
 
     backend = [TransformBackends.TORCH, TransformBackends.NUMPY]
 
-    def __init__(self, gamma: float) -> None:
+    def __init__(self, gamma: float, invert_image: bool = False, retain_stats: bool = False) -> None:
         if not isinstance(gamma, (int, float)):
             raise ValueError(f"gamma must be a float or int number, got {type(gamma)} {gamma}.")
         self.gamma = gamma
+        self.invert_image = invert_image
+        self.retain_stats = retain_stats
 
-    def __call__(self, img: NdarrayOrTensor) -> NdarrayOrTensor:
+    def __call__(self, img: NdarrayOrTensor, gamma=None) -> NdarrayOrTensor:
         """
         Apply the transform to `img`.
+        gamma: gamma value to adjust the contrast as function.
         """
         img = convert_to_tensor(img, track_meta=get_track_meta())
+        gamma = gamma if gamma is not None else self.gamma
+
+        if self.invert_image:
+            img = -img
+
+        if self.retain_stats:
+            mn = img.mean()
+            sd = img.std()
+
         epsilon = 1e-7
         img_min = img.min()
         img_range = img.max() - img_min
-        ret: NdarrayOrTensor = ((img - img_min) / float(img_range + epsilon)) ** self.gamma * img_range + img_min
+        ret: NdarrayOrTensor = ((img - img_min) / float(img_range + epsilon)) ** gamma * img_range + img_min
+
+        if self.retain_stats:
+            # zero mean and normalize
+            ret = ret - ret.mean()
+            ret = ret / (ret.std() + 1e-8)
+            # restore old mean and standard deviation
+            ret = sd * ret + mn
+
+        if self.invert_image:
+            ret = -ret
+
         return ret
 
 
 class RandAdjustContrast(RandomizableTransform):
     """
-    Randomly changes image intensity by gamma. Each pixel/voxel intensity is updated as::
+    Randomly changes image intensity with gamma transform. Each pixel/voxel intensity is updated as:
 
         x = ((x - min) / intensity_range) ^ gamma * intensity_range + min
 
     Args:
         prob: Probability of adjustment.
         gamma: Range of gamma values.
             If single number, value is picked from (0.5, gamma), default is (0.5, 4.5).
+        invert_image: whether to invert the image before applying gamma augmentation. If True, multiply all intensity
+            values with -1 before the gamma transform and again after the gamma transform. This behaviour is mimicked
+            from `nnU-Net <https://www.nature.com/articles/s41592-020-01008-z>`_, specifically `this
+            <https://github.com/MIC-DKFZ/batchgenerators/blob/7fb802b28b045b21346b197735d64f12fbb070aa/batchgenerators/augmentations/color_augmentations.py#L107>`_
+            function.
+        retain_stats: if True, applies a scaling factor and an offset to all intensity values after gamma transform to
+            ensure that the output intensity distribution has the same mean and standard deviation as the intensity
+            distribution of the input. This behaviour is mimicked from `nnU-Net
+            <https://www.nature.com/articles/s41592-020-01008-z>`_, specifically `this
+            <https://github.com/MIC-DKFZ/batchgenerators/blob/7fb802b28b045b21346b197735d64f12fbb070aa/batchgenerators/augmentations/color_augmentations.py#L107>`_
+            function.
     """
 
     backend = AdjustContrast.backend
 
-    def __init__(self, prob: float = 0.1, gamma: Sequence[float] | float = (0.5, 4.5)) -> None:
+    def __init__(
+        self,
+        prob: float = 0.1,
+        gamma: Sequence[float] | float = (0.5, 4.5),
+        invert_image: bool = False,
+        retain_stats: bool = False,
+    ) -> None:
         RandomizableTransform.__init__(self, prob)
 
         if isinstance(gamma, (int, float)):
             if gamma <= 0.5:
                 raise ValueError(
                     f"if gamma is a number, must greater than 0.5 and value is picked from (0.5, gamma), got {gamma}"
                 )
             self.gamma = (0.5, gamma)
         elif len(gamma) != 2:
             raise ValueError("gamma should be a number or pair of numbers.")
         else:
             self.gamma = (min(gamma), max(gamma))
 
-        self.gamma_value: float | None = None
+        self.gamma_value: float = 1.0
+        self.invert_image: bool = invert_image
+        self.retain_stats: bool = retain_stats
+
+        self.adjust_contrast = AdjustContrast(
+            self.gamma_value, invert_image=self.invert_image, retain_stats=self.retain_stats
+        )
 
     def randomize(self, data: Any | None = None) -> None:
         super().randomize(None)
         if not self._do_transform:
             return None
         self.gamma_value = self.R.uniform(low=self.gamma[0], high=self.gamma[1])
 
@@ -872,15 +1085,16 @@
             self.randomize()
 
         if not self._do_transform:
             return img
 
         if self.gamma_value is None:
             raise RuntimeError("gamma_value is not set, please call `randomize` function first.")
-        return AdjustContrast(self.gamma_value)(img)
+
+        return self.adjust_contrast(img, self.gamma_value)
 
 
 class ScaleIntensityRangePercentiles(Transform):
     """
     Apply range scaling to a numpy array based on the intensity distribution of the input.
 
     By default this transform will scale from [lower_intensity_percentile, upper_intensity_percentile] to
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/intensity/dictionary.py` & `monai-weekly-1.3.dev2324/monai/transforms/intensity/dictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     RandGaussianSharpen,
     RandGaussianSmooth,
     RandGibbsNoise,
     RandHistogramShift,
     RandKSpaceSpikeNoise,
     RandRicianNoise,
     RandScaleIntensity,
+    RandScaleIntensityFixedMean,
     RandShiftIntensity,
     RandStdShiftIntensity,
     SavitzkyGolaySmooth,
     ScaleIntensity,
     ScaleIntensityRange,
     ScaleIntensityRangePercentiles,
     ShiftIntensity,
@@ -104,14 +105,17 @@
     "RandShiftIntensityDict",
     "ScaleIntensityD",
     "ScaleIntensityDict",
     "StdShiftIntensityD",
     "StdShiftIntensityDict",
     "RandScaleIntensityD",
     "RandScaleIntensityDict",
+    "RandScaleIntensityFixedMeand",
+    "RandScaleIntensityFixedMeanDict",
+    "RandScaleIntensityFixedMeanD",
     "RandStdShiftIntensityD",
     "RandStdShiftIntensityDict",
     "RandBiasFieldD",
     "RandBiasFieldDict",
     "NormalizeIntensityD",
     "NormalizeIntensityDict",
     "ThresholdIntensityD",
@@ -619,14 +623,79 @@
         # all the keys share the same random scale factor
         self.scaler.randomize(None)
         for key in self.key_iterator(d):
             d[key] = self.scaler(d[key], randomize=False)
         return d
 
 
+class RandScaleIntensityFixedMeand(RandomizableTransform, MapTransform):
+    """
+    Dictionary-based version :py:class:`monai.transforms.RandScaleIntensity`.
+    Subtract the mean intensity before scaling with `factor`, then add the same value after scaling
+    to ensure that the output has the same mean as the input.
+    """
+
+    backend = RandScaleIntensityFixedMean.backend
+
+    def __init__(
+        self,
+        keys: KeysCollection,
+        factors: Sequence[float] | float,
+        fixed_mean: bool = True,
+        preserve_range: bool = False,
+        prob: float = 0.1,
+        dtype: DtypeLike = np.float32,
+        allow_missing_keys: bool = False,
+    ) -> None:
+        """
+        Args:
+            keys: keys of the corresponding items to be transformed.
+                See also: :py:class:`monai.transforms.compose.MapTransform`
+            factors: factor range to randomly scale by ``v = v * (1 + factor)``.
+                if single number, factor value is picked from (-factors, factors).
+            preserve_range: clips the output array/tensor to the range of the input array/tensor
+            fixed_mean: subtract the mean intensity before scaling with `factor`, then add the same value after scaling
+                to ensure that the output has the same mean as the input.
+            channel_wise: if True, scale on each channel separately. `preserve_range` and `fixed_mean` are also applied
+            on each channel separately if `channel_wise` is True. Please ensure that the first dimension represents the
+            channel of the image if True.
+            dtype: output data type, if None, same as input image. defaults to float32.
+            allow_missing_keys: don't raise exception if key is missing.
+
+        """
+        MapTransform.__init__(self, keys, allow_missing_keys)
+        RandomizableTransform.__init__(self, prob)
+        self.fixed_mean = fixed_mean
+        self.preserve_range = preserve_range
+        self.scaler = RandScaleIntensityFixedMean(
+            factors=factors, fixed_mean=self.fixed_mean, preserve_range=preserve_range, dtype=dtype, prob=1.0
+        )
+
+    def set_random_state(
+        self, seed: int | None = None, state: np.random.RandomState | None = None
+    ) -> RandScaleIntensityFixedMeand:
+        super().set_random_state(seed, state)
+        self.scaler.set_random_state(seed, state)
+        return self
+
+    def __call__(self, data: Mapping[Hashable, NdarrayOrTensor]) -> dict[Hashable, NdarrayOrTensor]:
+        d = dict(data)
+        self.randomize(None)
+        if not self._do_transform:
+            for key in self.key_iterator(d):
+                d[key] = convert_to_tensor(d[key], track_meta=get_track_meta())
+            return d
+
+        # all the keys share the same random scale factor
+        self.scaler.randomize(None)
+        for key in self.key_iterator(d):
+            d[key] = self.scaler(d[key], randomize=False)
+        return d
+
+
 class RandBiasFieldd(RandomizableTransform, MapTransform):
     """
     Dictionary-based version :py:class:`monai.transforms.RandBiasField`.
     """
 
     backend = RandBiasField.backend
 
@@ -794,66 +863,98 @@
             d[key] = self.scaler(d[key])
         return d
 
 
 class AdjustContrastd(MapTransform):
     """
     Dictionary-based wrapper of :py:class:`monai.transforms.AdjustContrast`.
-    Changes image intensity by gamma. Each pixel/voxel intensity is updated as:
+    Changes image intensity with gamma transform. Each pixel/voxel intensity is updated as:
 
         `x = ((x - min) / intensity_range) ^ gamma * intensity_range + min`
 
     Args:
         keys: keys of the corresponding items to be transformed.
             See also: monai.transforms.MapTransform
         gamma: gamma value to adjust the contrast as function.
+        invert_image: whether to invert the image before applying gamma augmentation. If True, multiply all intensity
+            values with -1 before the gamma transform and again after the gamma transform. This behaviour is mimicked
+            from `nnU-Net <https://www.nature.com/articles/s41592-020-01008-z>`_, specifically `this
+            <https://github.com/MIC-DKFZ/batchgenerators/blob/7fb802b28b045b21346b197735d64f12fbb070aa/batchgenerators/augmentations/color_augmentations.py#L107>`_
+            function.
+        retain_stats: if True, applies a scaling factor and an offset to all intensity values after gamma transform to
+            ensure that the output intensity distribution has the same mean and standard deviation as the intensity
+            distribution of the input. This behaviour is mimicked from `nnU-Net
+            <https://www.nature.com/articles/s41592-020-01008-z>`_, specifically `this
+            <https://github.com/MIC-DKFZ/batchgenerators/blob/7fb802b28b045b21346b197735d64f12fbb070aa/batchgenerators/augmentations/color_augmentations.py#L107>`_
+            function.
         allow_missing_keys: don't raise exception if key is missing.
     """
 
     backend = AdjustContrast.backend
 
-    def __init__(self, keys: KeysCollection, gamma: float, allow_missing_keys: bool = False) -> None:
+    def __init__(
+        self,
+        keys: KeysCollection,
+        gamma: float,
+        invert_image: bool = False,
+        retain_stats: bool = False,
+        allow_missing_keys: bool = False,
+    ) -> None:
         super().__init__(keys, allow_missing_keys)
-        self.adjuster = AdjustContrast(gamma)
+        self.adjuster = AdjustContrast(gamma, invert_image, retain_stats)
 
     def __call__(self, data: Mapping[Hashable, NdarrayOrTensor]) -> dict[Hashable, NdarrayOrTensor]:
         d = dict(data)
         for key in self.key_iterator(d):
             d[key] = self.adjuster(d[key])
         return d
 
 
 class RandAdjustContrastd(RandomizableTransform, MapTransform):
     """
     Dictionary-based version :py:class:`monai.transforms.RandAdjustContrast`.
-    Randomly changes image intensity by gamma. Each pixel/voxel intensity is updated as:
+    Randomly changes image intensity with gamma transform. Each pixel/voxel intensity is updated as:
 
         `x = ((x - min) / intensity_range) ^ gamma * intensity_range + min`
 
     Args:
         keys: keys of the corresponding items to be transformed.
             See also: monai.transforms.MapTransform
         prob: Probability of adjustment.
         gamma: Range of gamma values.
             If single number, value is picked from (0.5, gamma), default is (0.5, 4.5).
+        invert_image: whether to invert the image before applying gamma augmentation. If True, multiply all intensity
+            values with -1 before the gamma transform and again after the gamma transform. This behaviour is mimicked
+            from `nnU-Net <https://www.nature.com/articles/s41592-020-01008-z>`_, specifically `this
+            <https://github.com/MIC-DKFZ/batchgenerators/blob/7fb802b28b045b21346b197735d64f12fbb070aa/batchgenerators/augmentations/color_augmentations.py#L107>`_
+            function.
+        retain_stats: if True, applies a scaling factor and an offset to all intensity values after gamma transform to
+            ensure that the output intensity distribution has the same mean and standard deviation as the intensity
+            distribution of the input. This behaviour is mimicked from `nnU-Net
+            <https://www.nature.com/articles/s41592-020-01008-z>`_, specifically `this
+            <https://github.com/MIC-DKFZ/batchgenerators/blob/7fb802b28b045b21346b197735d64f12fbb070aa/batchgenerators/augmentations/color_augmentations.py#L107>`_
+            function.
         allow_missing_keys: don't raise exception if key is missing.
     """
 
     backend = RandAdjustContrast.backend
 
     def __init__(
         self,
         keys: KeysCollection,
         prob: float = 0.1,
         gamma: tuple[float, float] | float = (0.5, 4.5),
+        invert_image: bool = False,
+        retain_stats: bool = False,
         allow_missing_keys: bool = False,
     ) -> None:
         MapTransform.__init__(self, keys, allow_missing_keys)
         RandomizableTransform.__init__(self, prob)
-        self.adjuster = RandAdjustContrast(gamma=gamma, prob=1.0)
+        self.adjuster = RandAdjustContrast(gamma=gamma, prob=1.0, invert_image=invert_image, retain_stats=retain_stats)
+        self.invert_image = invert_image
 
     def set_random_state(
         self, seed: int | None = None, state: np.random.RandomState | None = None
     ) -> RandAdjustContrastd:
         super().set_random_state(seed, state)
         self.adjuster.set_random_state(seed, state)
         return self
@@ -1797,14 +1898,15 @@
 ShiftIntensityD = ShiftIntensityDict = ShiftIntensityd
 RandShiftIntensityD = RandShiftIntensityDict = RandShiftIntensityd
 StdShiftIntensityD = StdShiftIntensityDict = StdShiftIntensityd
 RandStdShiftIntensityD = RandStdShiftIntensityDict = RandStdShiftIntensityd
 RandBiasFieldD = RandBiasFieldDict = RandBiasFieldd
 ScaleIntensityD = ScaleIntensityDict = ScaleIntensityd
 RandScaleIntensityD = RandScaleIntensityDict = RandScaleIntensityd
+RandScaleIntensityFixedMeanD = RandScaleIntensityFixedMeanDict = RandScaleIntensityFixedMeand
 NormalizeIntensityD = NormalizeIntensityDict = NormalizeIntensityd
 ThresholdIntensityD = ThresholdIntensityDict = ThresholdIntensityd
 ScaleIntensityRangeD = ScaleIntensityRangeDict = ScaleIntensityRanged
 AdjustContrastD = AdjustContrastDict = AdjustContrastd
 RandAdjustContrastD = RandAdjustContrastDict = RandAdjustContrastd
 ScaleIntensityRangePercentilesD = ScaleIntensityRangePercentilesDict = ScaleIntensityRangePercentilesd
 MaskIntensityD = MaskIntensityDict = MaskIntensityd
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/inverse.py` & `monai-weekly-1.3.dev2324/monai/transforms/inverse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/inverse_batch_transform.py` & `monai-weekly-1.3.dev2324/monai/transforms/inverse_batch_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/io/__init__.py` & `monai-weekly-1.3.dev2324/monai/transforms/io/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/io/array.py` & `monai-weekly-1.3.dev2324/monai/transforms/io/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-A collection of "vanilla" transforms for IO functions
-https://github.com/Project-MONAI/MONAI/wiki/MONAI_Design
+A collection of "vanilla" transforms for IO functions.
 """
 
 from __future__ import annotations
 
 import inspect
 import logging
 import sys
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/io/dictionary.py` & `monai-weekly-1.3.dev2324/monai/transforms/io/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/lazy/__init__.py` & `monai-weekly-1.3.dev2324/monai/transforms/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/lazy/array.py` & `monai-weekly-1.3.dev2324/monai/transforms/lazy/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/lazy/dictionary.py` & `monai-weekly-1.3.dev2324/monai/transforms/lazy/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/lazy/functional.py` & `monai-weekly-1.3.dev2324/monai/transforms/lazy/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/lazy/utils.py` & `monai-weekly-1.3.dev2324/monai/transforms/lazy/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/meta_utility/__init__.py` & `monai-weekly-1.3.dev2324/monai/transforms/meta_utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/meta_utility/dictionary.py` & `monai-weekly-1.3.dev2324/monai/transforms/meta_utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/nvtx.py` & `monai-weekly-1.3.dev2324/monai/transforms/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/post/__init__.py` & `monai-weekly-1.3.dev2324/monai/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/post/array.py` & `monai-weekly-1.3.dev2324/monai/transforms/post/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-A collection of "vanilla" transforms for the model output tensors
-https://github.com/Project-MONAI/MONAI/wiki/MONAI_Design
+A collection of "vanilla" transforms for the model output tensors.
 """
 
 from __future__ import annotations
 
 import warnings
 from collections.abc import Callable, Iterable, Sequence
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/post/dictionary.py` & `monai-weekly-1.3.dev2324/monai/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/signal/__init__.py` & `monai-weekly-1.3.dev2324/monai/transforms/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/signal/array.py` & `monai-weekly-1.3.dev2324/monai/transforms/signal/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-A collection of transforms for signal operations
-https://github.com/Project-MONAI/MONAI/wiki/MONAI_Design
+A collection of transforms for signal operations.
 """
 
 from __future__ import annotations
 
 import warnings
 from collections.abc import Sequence
 from typing import Any
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/smooth_field/__init__.py` & `monai-weekly-1.3.dev2324/monai/transforms/smooth_field/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/smooth_field/array.py` & `monai-weekly-1.3.dev2324/monai/transforms/smooth_field/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/smooth_field/dictionary.py` & `monai-weekly-1.3.dev2324/monai/transforms/smooth_field/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/spatial/__init__.py` & `monai-weekly-1.3.dev2324/monai/transforms/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/spatial/array.py` & `monai-weekly-1.3.dev2324/monai/transforms/spatial/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-A collection of "vanilla" transforms for spatial operations
-https://github.com/Project-MONAI/MONAI/wiki/MONAI_Design
+A collection of "vanilla" transforms for spatial operations.
 """
 
 from __future__ import annotations
 
 import warnings
 from collections.abc import Callable
 from copy import deepcopy
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/spatial/dictionary.py` & `monai-weekly-1.3.dev2324/monai/transforms/spatial/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/spatial/functional.py` & `monai-weekly-1.3.dev2324/monai/transforms/spatial/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-A collection of "functional" transforms for spatial operations
-https://github.com/Project-MONAI/MONAI/wiki/MONAI_Design
+A collection of "functional" transforms for spatial operations.
 """
 
 from __future__ import annotations
 
 import math
 import warnings
 from enum import Enum
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/traits.py` & `monai-weekly-1.3.dev2324/monai/transforms/traits.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/transform.py` & `monai-weekly-1.3.dev2324/monai/transforms/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,16 +271,15 @@
         To simplify the input validations, most of the transforms assume that
 
         - ``data`` is a Numpy ndarray, PyTorch Tensor or string,
         - the data shape can be:
 
           #. string data without shape, `LoadImage` transform expects file paths,
           #. most of the pre-/post-processing transforms expect: ``(num_channels, spatial_dim_1[, spatial_dim_2, ...])``,
-             except for example: `AddChannel` expects (spatial_dim_1[, spatial_dim_2, ...]) and
-             `AsChannelFirst` expects (spatial_dim_1[, spatial_dim_2, ...], num_channels),
+             except for example: `AddChannel` expects (spatial_dim_1[, spatial_dim_2, ...])
 
         - the channel dimension is often not omitted even if number of channels is one.
 
         This method can optionally take additional arguments to help execute transformation operation.
 
         Raises:
             NotImplementedError: When the subclass does not override this method.
@@ -437,16 +436,15 @@
 
         - ``data`` is a Python dictionary,
         - ``data[key]`` is a Numpy ndarray, PyTorch Tensor or string, where ``key`` is an element
           of ``self.keys``, the data shape can be:
 
           #. string data without shape, `LoadImaged` transform expects file paths,
           #. most of the pre-/post-processing transforms expect: ``(num_channels, spatial_dim_1[, spatial_dim_2, ...])``,
-             except for example: `AddChanneld` expects (spatial_dim_1[, spatial_dim_2, ...]) and
-             `AsChannelFirstd` expects (spatial_dim_1[, spatial_dim_2, ...], num_channels)
+             except for example: `AddChanneld` expects (spatial_dim_1[, spatial_dim_2, ...])
 
         - the channel dimension is often not omitted even if number of channels is one.
 
         Raises:
             NotImplementedError: When the subclass does not override this method.
 
         returns:
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/utility/__init__.py` & `monai-weekly-1.3.dev2324/monai/transforms/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/utility/array.py` & `monai-weekly-1.3.dev2324/monai/transforms/utility/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-A collection of "vanilla" transforms for utility functions
-https://github.com/Project-MONAI/MONAI/wiki/MONAI_Design
+A collection of "vanilla" transforms for utility functions.
 """
 
 from __future__ import annotations
 
 import logging
 import sys
 import time
@@ -138,46 +137,14 @@
 
     backend = [TransformBackends.TORCH, TransformBackends.NUMPY]
 
     def __call__(self, data: Any) -> Any:
         return data
 
 
-@deprecated(since="0.8", msg_suffix="please use MetaTensor data type and monai.transforms.EnsureChannelFirst instead.")
-class AsChannelFirst(Transform):
-    """
-    Change the channel dimension of the image to the first dimension.
-
-    Most of the image transformations in ``monai.transforms``
-    assume the input image is in the channel-first format, which has the shape
-    (num_channels, spatial_dim_1[, spatial_dim_2, ...]).
-
-    This transform could be used to convert, for example, a channel-last image array in shape
-    (spatial_dim_1[, spatial_dim_2, ...], num_channels) into the channel-first format,
-    so that the multidimensional image array can be correctly interpreted by the other transforms.
-
-    Args:
-        channel_dim: which dimension of input image is the channel, default is the last dimension.
-    """
-
-    backend = [TransformBackends.TORCH, TransformBackends.NUMPY]
-
-    def __init__(self, channel_dim: int = -1) -> None:
-        if not (isinstance(channel_dim, int) and channel_dim >= -1):
-            raise ValueError(f"invalid channel dimension ({channel_dim}).")
-        self.channel_dim = channel_dim
-
-    def __call__(self, img: NdarrayOrTensor) -> NdarrayOrTensor:
-        """
-        Apply the transform to `img`.
-        """
-        out: NdarrayOrTensor = convert_to_tensor(moveaxis(img, self.channel_dim, 0), track_meta=get_track_meta())
-        return out
-
-
 class AsChannelLast(Transform):
     """
     Change the channel dimension of the image to the last dimension.
 
     Some of other 3rd party transforms assume the input image is in the channel-last format with shape
     (spatial_dim_1[, spatial_dim_2, ...], num_channels).
 
@@ -200,39 +167,14 @@
         """
         Apply the transform to `img`.
         """
         out: NdarrayOrTensor = convert_to_tensor(moveaxis(img, self.channel_dim, -1), track_meta=get_track_meta())
         return out
 
 
-@deprecated(since="0.8", msg_suffix="please use MetaTensor data type and monai.transforms.EnsureChannelFirst instead.")
-class AddChannel(Transform):
-    """
-    Adds a 1-length channel dimension to the input image.
-
-    Most of the image transformations in ``monai.transforms``
-    assumes the input image is in the channel-first format, which has the shape
-    (num_channels, spatial_dim_1[, spatial_dim_2, ...]).
-
-    This transform could be used, for example, to convert a (spatial_dim_1[, spatial_dim_2, ...])
-    spatial image into the channel-first format so that the
-    multidimensional image array can be correctly interpreted by the other
-    transforms.
-    """
-
-    backend = [TransformBackends.TORCH, TransformBackends.NUMPY]
-
-    def __call__(self, img: NdarrayOrTensor) -> NdarrayOrTensor:
-        """
-        Apply the transform to `img`.
-        """
-        out: NdarrayOrTensor = convert_to_tensor(img[None], track_meta=get_track_meta())
-        return out
-
-
 class EnsureChannelFirst(Transform):
     """
     Adjust or add the channel dimension of input data to ensure `channel_first` shape.
 
     This extracts the `original_channel_dim` info from provided meta_data dictionary or MetaTensor input. This value
     should state which dimension is the channel dimension so that it can be moved forward, or contain "no_channel" to
     state no dimension is the channel and so a 1-size first dimension is to be added.
@@ -287,14 +229,62 @@
             result = img[None]
         else:
             result = moveaxis(img, int(channel_dim), 0)  # type: ignore
 
         return convert_to_tensor(result, track_meta=get_track_meta())  # type: ignore
 
 
+@deprecated(
+    since="0.8",
+    removed="1.3",
+    msg_suffix="please use MetaTensor data type and monai.transforms.EnsureChannelFirst instead.",
+)
+class AsChannelFirst(EnsureChannelFirst):
+    """
+    Change the channel dimension of the image to the first dimension.
+    Most of the image transformations in ``monai.transforms``
+    assume the input image is in the channel-first format, which has the shape
+    (num_channels, spatial_dim_1[, spatial_dim_2, ...]).
+    This transform could be used to convert, for example, a channel-last image array in shape
+    (spatial_dim_1[, spatial_dim_2, ...], num_channels) into the channel-first format,
+    so that the multidimensional image array can be correctly interpreted by the other transforms.
+    Args:
+        channel_dim: which dimension of input image is the channel, default is the last dimension.
+    """
+
+    def __init__(self, channel_dim: int = -1) -> None:
+        super().__init__(channel_dim=channel_dim)
+
+
+@deprecated(
+    since="0.8",
+    removed="1.3",
+    msg_suffix="please use MetaTensor data type and monai.transforms.EnsureChannelFirst instead"
+    " with `channel_dim='no_channel'`.",
+)
+class AddChannel(EnsureChannelFirst):
+    """
+    Adds a 1-length channel dimension to the input image.
+
+    Most of the image transformations in ``monai.transforms``
+    assumes the input image is in the channel-first format, which has the shape
+    (num_channels, spatial_dim_1[, spatial_dim_2, ...]).
+
+    This transform could be used, for example, to convert a (spatial_dim_1[, spatial_dim_2, ...])
+    spatial image into the channel-first format so that the
+    multidimensional image array can be correctly interpreted by the other
+    transforms.
+    """
+
+    backend = [TransformBackends.TORCH, TransformBackends.NUMPY]
+
+    def __init__(self) -> None:
+        super().__init__(channel_dim="no_channel")
+
+
 class RepeatChannel(Transform):
     """
     Repeat channel data to construct expected input shape for models.
     The `repeats` count includes the origin data, for example:
     ``RepeatChannel(repeats=2)([[1, 2], [3, 4]])`` generates: ``[[1, 2], [1, 2], [3, 4], [3, 4]]``
 
     Args:
@@ -387,15 +377,15 @@
                 ndim = len(item.affine)
                 shift = torch.eye(ndim, device=item.affine.device, dtype=item.affine.dtype)
                 shift[self.dim - 1, -1] = idx
                 item.affine = item.affine @ shift
         return outputs
 
 
-@deprecated(since="0.8", msg_suffix="please use `SplitDim` instead.")
+@deprecated(since="0.8", removed="1.3", msg_suffix="please use `SplitDim` instead.")
 class SplitChannel(SplitDim):
     """
     Split Numpy array or PyTorch Tensor data according to the channel dim.
     It can help applying different following transforms to different channels.
 
     Note: `torch.split`/`np.split` is used, so the outputs are views of the input (shallow copy).
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/utility/dictionary.py` & `monai-weekly-1.3.dev2324/monai/transforms/utility/dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,18 +29,16 @@
 from monai.config.type_definitions import NdarrayOrTensor
 from monai.data.meta_tensor import MetaObj, MetaTensor
 from monai.data.utils import no_collation
 from monai.transforms.inverse import InvertibleTransform
 from monai.transforms.traits import MultiSampleTrait, RandomizableTrait
 from monai.transforms.transform import MapTransform, Randomizable, RandomizableTransform
 from monai.transforms.utility.array import (
-    AddChannel,
     AddCoordinateChannels,
     AddExtremePointsChannel,
-    AsChannelFirst,
     AsChannelLast,
     CastToType,
     ClassesToIndices,
     ConvertToMultiChannelBasedOnBratsClasses,
     CuCIM,
     DataStats,
     EnsureChannelFirst,
@@ -217,39 +215,14 @@
     def __call__(self, data: Mapping[Hashable, NdarrayOrTensor]) -> dict[Hashable, NdarrayOrTensor]:
         d = dict(data)
         for key in self.key_iterator(d):
             d[key] = self.identity(d[key])
         return d
 
 
-class AsChannelFirstd(MapTransform):
-    """
-    Dictionary-based wrapper of :py:class:`monai.transforms.AsChannelFirst`.
-    """
-
-    backend = AsChannelFirst.backend
-
-    def __init__(self, keys: KeysCollection, channel_dim: int = -1, allow_missing_keys: bool = False) -> None:
-        """
-        Args:
-            keys: keys of the corresponding items to be transformed.
-                See also: :py:class:`monai.transforms.compose.MapTransform`
-            channel_dim: which dimension of input image is the channel, default is the last dimension.
-            allow_missing_keys: don't raise exception if key is missing.
-        """
-        super().__init__(keys, allow_missing_keys)
-        self.converter = AsChannelFirst(channel_dim=channel_dim)
-
-    def __call__(self, data: Mapping[Hashable, NdarrayOrTensor]) -> dict[Hashable, NdarrayOrTensor]:
-        d = dict(data)
-        for key in self.key_iterator(d):
-            d[key] = self.converter(d[key])
-        return d
-
-
 class AsChannelLastd(MapTransform):
     """
     Dictionary-based wrapper of :py:class:`monai.transforms.AsChannelLast`.
     """
 
     backend = AsChannelLast.backend
 
@@ -267,38 +240,14 @@
     def __call__(self, data: Mapping[Hashable, NdarrayOrTensor]) -> dict[Hashable, NdarrayOrTensor]:
         d = dict(data)
         for key in self.key_iterator(d):
             d[key] = self.converter(d[key])
         return d
 
 
-class AddChanneld(MapTransform):
-    """
-    Dictionary-based wrapper of :py:class:`monai.transforms.AddChannel`.
-    """
-
-    backend = AddChannel.backend
-
-    def __init__(self, keys: KeysCollection, allow_missing_keys: bool = False) -> None:
-        """
-        Args:
-            keys: keys of the corresponding items to be transformed.
-                See also: :py:class:`monai.transforms.compose.MapTransform`
-            allow_missing_keys: don't raise exception if key is missing.
-        """
-        super().__init__(keys, allow_missing_keys)
-        self.adder = AddChannel()
-
-    def __call__(self, data: Mapping[Hashable, NdarrayOrTensor]) -> dict[Hashable, NdarrayOrTensor]:
-        d = dict(data)
-        for key in self.key_iterator(d):
-            d[key] = self.adder(d[key])
-        return d
-
-
 class EnsureChannelFirstd(MapTransform):
     """
     Dictionary-based wrapper of :py:class:`monai.transforms.EnsureChannelFirst`.
     """
 
     backend = EnsureChannelFirst.backend
 
@@ -332,14 +281,58 @@
     def __call__(self, data: Mapping[Hashable, torch.Tensor]) -> dict[Hashable, torch.Tensor]:
         d = dict(data)
         for key, meta_key, meta_key_postfix in self.key_iterator(d, self.meta_keys, self.meta_key_postfix):
             d[key] = self.adjuster(d[key], d.get(meta_key or f"{key}_{meta_key_postfix}"))  # type: ignore
         return d
 
 
+@deprecated(
+    since="0.8",
+    removed="1.3",
+    msg_suffix="please use MetaTensor data type and monai.transforms.EnsureChannelFirstd instead.",
+)
+class AsChannelFirstd(EnsureChannelFirstd):
+    """
+    Dictionary-based wrapper of :py:class:`monai.transforms.AsChannelFirst`.
+    """
+
+    def __init__(self, keys: KeysCollection, channel_dim: int = -1, allow_missing_keys: bool = False) -> None:
+        """
+        Args:
+            keys: keys of the corresponding items to be transformed.
+                See also: :py:class:`monai.transforms.compose.MapTransform`
+            channel_dim: which dimension of input image is the channel, default is the last dimension.
+            allow_missing_keys: don't raise exception if key is missing.
+        """
+        super().__init__(keys=keys, channel_dim=channel_dim, allow_missing_keys=allow_missing_keys)
+
+
+@deprecated(
+    since="0.8",
+    removed="1.3",
+    msg_suffix="please use MetaTensor data type and monai.transforms.EnsureChannelFirstd instead"
+    " with `channel_dim='no_channel'`.",
+)
+class AddChanneld(EnsureChannelFirstd):
+    """
+    Dictionary-based wrapper of :py:class:`monai.transforms.AddChannel`.
+    """
+
+    backend = EnsureChannelFirstd.backend
+
+    def __init__(self, keys: KeysCollection, allow_missing_keys: bool = False) -> None:
+        """
+        Args:
+            keys: keys of the corresponding items to be transformed.
+                See also: :py:class:`monai.transforms.compose.MapTransform`
+            allow_missing_keys: don't raise exception if key is missing.
+        """
+        super().__init__(keys, allow_missing_keys, channel_dim="no_channel")
+
+
 class RepeatChanneld(MapTransform):
     """
     Dictionary-based wrapper of :py:class:`monai.transforms.RepeatChannel`.
     """
 
     backend = RepeatChannel.backend
 
@@ -448,15 +441,15 @@
                 split_key = f"{key}_{postfixes[i]}"
                 if split_key in d:
                     raise RuntimeError(f"input data already contains key {split_key}.")
                 d[split_key] = r
         return d
 
 
-@deprecated(since="0.8", msg_suffix="please use `SplitDimd` instead.")
+@deprecated(since="0.8", removed="1.3", msg_suffix="please use `SplitDimd` instead.")
 class SplitChanneld(SplitDimd):
     """
     Dictionary-based wrapper of :py:class:`monai.transforms.SplitChannel`.
     All the input specified by `keys` should be split into same count of data.
     """
 
     def __init__(
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/utils.py` & `monai-weekly-1.3.dev2324/monai/transforms/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1662,15 +1662,15 @@
             n_uncategorized += 1
         print_table_column(k, v[0], v[1], color=color)
 
     print("Total number of transforms:", n_total)
     print_color(f"Number transforms allowing both torch and numpy: {n_t_or_np}", Colors.green)
     print_color(f"Number of TorchTransform: {n_t}", Colors.green)
     print_color(f"Number of NumpyTransform: {n_np}", Colors.yellow)
-    print_color(f"Number of uncategorised: {n_uncategorized}", Colors.red)
+    print_color(f"Number of uncategorized: {n_uncategorized}", Colors.red)
 
 
 def convert_pad_mode(dst: NdarrayOrTensor, mode: str | None):
     """
     Utility to convert padding mode between numpy array and PyTorch Tensor.
 
     Args:
```

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/utils_create_transform_ims.py` & `monai-weekly-1.3.dev2324/monai/transforms/utils_create_transform_ims.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/transforms/utils_pytorch_numpy_unification.py` & `monai-weekly-1.3.dev2324/monai/transforms/utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/utils/__init__.py` & `monai-weekly-1.3.dev2324/monai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/utils/aliases.py` & `monai-weekly-1.3.dev2324/monai/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/utils/decorators.py` & `monai-weekly-1.3.dev2324/monai/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/utils/deprecate_utils.py` & `monai-weekly-1.3.dev2324/monai/utils/deprecate_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/utils/dist.py` & `monai-weekly-1.3.dev2324/monai/utils/dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/utils/enums.py` & `monai-weekly-1.3.dev2324/monai/utils/enums.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/utils/jupyter_utils.py` & `monai-weekly-1.3.dev2324/monai/utils/jupyter_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/utils/misc.py` & `monai-weekly-1.3.dev2324/monai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/utils/module.py` & `monai-weekly-1.3.dev2324/monai/utils/module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/utils/nvtx.py` & `monai-weekly-1.3.dev2324/monai/utils/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/utils/profiling.py` & `monai-weekly-1.3.dev2324/monai/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/utils/state_cacher.py` & `monai-weekly-1.3.dev2324/monai/utils/state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/utils/type_conversion.py` & `monai-weekly-1.3.dev2324/monai/utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/visualize/__init__.py` & `monai-weekly-1.3.dev2324/monai/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/visualize/class_activation_maps.py` & `monai-weekly-1.3.dev2324/monai/visualize/class_activation_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/visualize/gradient_based.py` & `monai-weekly-1.3.dev2324/monai/visualize/gradient_based.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/visualize/img2tensorboard.py` & `monai-weekly-1.3.dev2324/monai/visualize/img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/visualize/occlusion_sensitivity.py` & `monai-weekly-1.3.dev2324/monai/visualize/occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/visualize/utils.py` & `monai-weekly-1.3.dev2324/monai/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai/visualize/visualizer.py` & `monai-weekly-1.3.dev2324/monai/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/monai_weekly.egg-info/PKG-INFO` & `monai-weekly-1.3.dev2324/monai_weekly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.2.dev2323
+Version: 1.3.dev2324
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
@@ -90,15 +90,15 @@
 ## Features
 > _Please see [the technical highlights](https://docs.monai.io/en/latest/highlights.html) and [What's New](https://docs.monai.io/en/latest/whatsnew.html) of the milestone releases._
 
 - flexible pre-processing for multi-dimensional medical imaging data;
 - compositional & portable APIs for ease of integration in existing workflows;
 - domain-specific implementations for networks, losses, evaluation metrics and more;
 - customizable design for varying user expertise;
-- multi-GPU data parallelism support.
+- multi-GPU multi-node data parallelism support.
 
 
 ## Installation
 
 To install [the current release](https://pypi.org/project/monai/), you can simply run:
 
 ```bash
```

### Comparing `monai-weekly-1.2.dev2323/monai_weekly.egg-info/SOURCES.txt` & `monai-weekly-1.3.dev2324/monai_weekly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -865,14 +865,16 @@
 tests/test_rand_rotate.py
 tests/test_rand_rotate90.py
 tests/test_rand_rotate90d.py
 tests/test_rand_rotated.py
 tests/test_rand_scale_crop.py
 tests/test_rand_scale_cropd.py
 tests/test_rand_scale_intensity.py
+tests/test_rand_scale_intensity_fixed_mean.py
+tests/test_rand_scale_intensity_fixed_meand.py
 tests/test_rand_scale_intensityd.py
 tests/test_rand_shift_intensity.py
 tests/test_rand_shift_intensityd.py
 tests/test_rand_spatial_crop.py
 tests/test_rand_spatial_crop_samples.py
 tests/test_rand_spatial_crop_samplesd.py
 tests/test_rand_spatial_cropd.py
@@ -928,14 +930,15 @@
 tests/test_save_image.py
 tests/test_save_imaged.py
 tests/test_save_state.py
 tests/test_savitzky_golay_filter.py
 tests/test_savitzky_golay_smooth.py
 tests/test_savitzky_golay_smoothd.py
 tests/test_scale_intensity.py
+tests/test_scale_intensity_fixed_mean.py
 tests/test_scale_intensity_range.py
 tests/test_scale_intensity_range_percentiles.py
 tests/test_scale_intensity_range_percentilesd.py
 tests/test_scale_intensity_ranged.py
 tests/test_scale_intensityd.py
 tests/test_se_block.py
 tests/test_se_blocks.py
```

### Comparing `monai-weekly-1.2.dev2323/monai_weekly.egg-info/requires.txt` & `monai-weekly-1.3.dev2324/monai_weekly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/pyproject.toml` & `monai-weekly-1.3.dev2324/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/setup.cfg` & `monai-weekly-1.3.dev2324/setup.cfg`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/setup.py` & `monai-weekly-1.3.dev2324/setup.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_acn_block.py` & `monai-weekly-1.3.dev2324/tests/test_acn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_activations.py` & `monai-weekly-1.3.dev2324/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_activationsd.py` & `monai-weekly-1.3.dev2324/tests/test_activationsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_adaptors.py` & `monai-weekly-1.3.dev2324/tests/test_adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_add_channeld.py` & `monai-weekly-1.3.dev2324/tests/test_add_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_add_coordinate_channels.py` & `monai-weekly-1.3.dev2324/tests/test_add_coordinate_channels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_add_coordinate_channelsd.py` & `monai-weekly-1.3.dev2324/tests/test_add_coordinate_channelsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_add_extreme_points_channel.py` & `monai-weekly-1.3.dev2324/tests/test_add_extreme_points_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_add_extreme_points_channeld.py` & `monai-weekly-1.3.dev2324/tests/test_add_extreme_points_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_adjust_contrast.py` & `monai-weekly-1.3.dev2324/tests/test_rand_adjust_contrastd.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,37 +12,33 @@
 from __future__ import annotations
 
 import unittest
 
 import numpy as np
 from parameterized import parameterized
 
-from monai.transforms import AdjustContrast
+from monai.transforms import RandAdjustContrastd
 from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D, assert_allclose
 
-TEST_CASE_1 = [1.0]
+TEST_CASE_1 = [(0.5, 4.5)]
 
-TEST_CASE_2 = [0.5]
+TEST_CASE_2 = [1.5]
 
-TEST_CASE_3 = [4.5]
 
-
-class TestAdjustContrast(NumpyImageTestCase2D):
-    @parameterized.expand([TEST_CASE_1, TEST_CASE_2, TEST_CASE_3])
+class TestRandAdjustContrastd(NumpyImageTestCase2D):
+    @parameterized.expand([TEST_CASE_1, TEST_CASE_2])
     def test_correct_results(self, gamma):
-        adjuster = AdjustContrast(gamma=gamma)
+        adjuster = RandAdjustContrastd("img", prob=1.0, gamma=gamma)
         for p in TEST_NDARRAYS:
-            im = p(self.imt)
-            result = adjuster(im)
-            self.assertTrue(type(im), type(result))
-            if gamma == 1.0:
-                expected = self.imt
-            else:
-                epsilon = 1e-7
-                img_min = self.imt.min()
-                img_range = self.imt.max() - img_min
-                expected = np.power(((self.imt - img_min) / float(img_range + epsilon)), gamma) * img_range + img_min
-            assert_allclose(result, expected, rtol=1e-05, type_test="tensor")
+            result = adjuster({"img": p(self.imt)})
+            epsilon = 1e-7
+            img_min = self.imt.min()
+            img_range = self.imt.max() - img_min
+            expected = (
+                np.power(((self.imt - img_min) / float(img_range + epsilon)), adjuster.adjuster.gamma_value) * img_range
+                + img_min
+            )
+            assert_allclose(result["img"], expected, rtol=1e-05, type_test="tensor")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_adjust_contrastd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_adjust_contrast.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,35 +12,34 @@
 from __future__ import annotations
 
 import unittest
 
 import numpy as np
 from parameterized import parameterized
 
-from monai.transforms import AdjustContrastd
+from monai.transforms import RandAdjustContrast
 from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D, assert_allclose
 
-TEST_CASE_1 = [1.0]
+TEST_CASE_1 = [(0.5, 4.5)]
 
-TEST_CASE_2 = [0.5]
+TEST_CASE_2 = [1.5]
 
-TEST_CASE_3 = [4.5]
 
-
-class TestAdjustContrastd(NumpyImageTestCase2D):
-    @parameterized.expand([TEST_CASE_1, TEST_CASE_2, TEST_CASE_3])
+class TestRandAdjustContrast(NumpyImageTestCase2D):
+    @parameterized.expand([TEST_CASE_1, TEST_CASE_2])
     def test_correct_results(self, gamma):
-        adjuster = AdjustContrastd("img", gamma=gamma)
+        adjuster = RandAdjustContrast(prob=1.0, gamma=gamma)
         for p in TEST_NDARRAYS:
-            result = adjuster({"img": p(self.imt)})
-            if gamma == 1.0:
-                expected = self.imt
-            else:
-                epsilon = 1e-7
-                img_min = self.imt.min()
-                img_range = self.imt.max() - img_min
-                expected = np.power(((self.imt - img_min) / float(img_range + epsilon)), gamma) * img_range + img_min
-            assert_allclose(result["img"], expected, rtol=1e-05, type_test="tensor")
+            im = p(self.imt)
+            result = adjuster(im)
+            epsilon = 1e-7
+            img_min = self.imt.min()
+            img_range = self.imt.max() - img_min
+            expected = (
+                np.power(((self.imt - img_min) / float(img_range + epsilon)), adjuster.gamma_value) * img_range
+                + img_min
+            )
+            assert_allclose(result, expected, rtol=1e-05, type_test=False)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_adn.py` & `monai-weekly-1.3.dev2324/tests/test_adn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_affine.py` & `monai-weekly-1.3.dev2324/tests/test_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_affine_grid.py` & `monai-weekly-1.3.dev2324/tests/test_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_affine_transform.py` & `monai-weekly-1.3.dev2324/tests/test_affine_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_affined.py` & `monai-weekly-1.3.dev2324/tests/test_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_ahnet.py` & `monai-weekly-1.3.dev2324/tests/test_ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_alias.py` & `monai-weekly-1.3.dev2324/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_anchor_box.py` & `monai-weekly-1.3.dev2324/tests/test_anchor_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_apply.py` & `monai-weekly-1.3.dev2324/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_apply_filter.py` & `monai-weekly-1.3.dev2324/tests/test_apply_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_arraydataset.py` & `monai-weekly-1.3.dev2324/tests/test_arraydataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,26 +18,26 @@
 
 import nibabel as nib
 import numpy as np
 from parameterized import parameterized
 from torch.utils.data import DataLoader
 
 from monai.data import ArrayDataset
-from monai.transforms import AddChannel, Compose, LoadImage, RandAdjustContrast, RandGaussianNoise, Spacing
+from monai.transforms import Compose, EnsureChannelFirst, LoadImage, RandAdjustContrast, RandGaussianNoise, Spacing
 
 TEST_CASE_1 = [
-    Compose([LoadImage(image_only=True), AddChannel(), RandGaussianNoise(prob=1.0)]),
-    Compose([LoadImage(image_only=True), AddChannel(), RandGaussianNoise(prob=1.0)]),
+    Compose([LoadImage(image_only=True), EnsureChannelFirst(channel_dim="no_channel"), RandGaussianNoise(prob=1.0)]),
+    Compose([LoadImage(image_only=True), EnsureChannelFirst(channel_dim="no_channel"), RandGaussianNoise(prob=1.0)]),
     (0, 1),
     (1, 128, 128, 128),
 ]
 
 TEST_CASE_2 = [
-    Compose([LoadImage(image_only=True), AddChannel(), RandAdjustContrast(prob=1.0)]),
-    Compose([LoadImage(image_only=True), AddChannel(), RandAdjustContrast(prob=1.0)]),
+    Compose([LoadImage(image_only=True), EnsureChannelFirst(channel_dim="no_channel"), RandAdjustContrast(prob=1.0)]),
+    Compose([LoadImage(image_only=True), EnsureChannelFirst(channel_dim="no_channel"), RandAdjustContrast(prob=1.0)]),
     (0, 1),
     (1, 128, 128, 128),
 ]
 
 
 class TestCompose(Compose):
     def __call__(self, input_):
@@ -46,21 +46,38 @@
         img = self.transforms[1](img)
         img = self.transforms[2](img, metadata["affine"])
         metadata = img.meta
         return self.transforms[3](img), metadata
 
 
 TEST_CASE_3 = [
-    TestCompose([LoadImage(image_only=True), AddChannel(), Spacing(pixdim=(2, 2, 4)), RandAdjustContrast(prob=1.0)]),
-    TestCompose([LoadImage(image_only=True), AddChannel(), Spacing(pixdim=(2, 2, 4)), RandAdjustContrast(prob=1.0)]),
+    TestCompose(
+        [
+            LoadImage(image_only=True),
+            EnsureChannelFirst(channel_dim="no_channel"),
+            Spacing(pixdim=(2, 2, 4)),
+            RandAdjustContrast(prob=1.0),
+        ]
+    ),
+    TestCompose(
+        [
+            LoadImage(image_only=True),
+            EnsureChannelFirst(channel_dim="no_channel"),
+            Spacing(pixdim=(2, 2, 4)),
+            RandAdjustContrast(prob=1.0),
+        ]
+    ),
     (0, 2),
     (1, 64, 64, 33),
 ]
 
-TEST_CASE_4 = [Compose([LoadImage(image_only=True), AddChannel(), RandGaussianNoise(prob=1.0)]), (1, 128, 128, 128)]
+TEST_CASE_4 = [
+    Compose([LoadImage(image_only=True), EnsureChannelFirst(channel_dim="no_channel"), RandGaussianNoise(prob=1.0)]),
+    (1, 128, 128, 128),
+]
 
 
 class TestArrayDataset(unittest.TestCase):
     @parameterized.expand([TEST_CASE_1, TEST_CASE_2, TEST_CASE_3])
     def test_shape(self, img_transform, label_transform, indices, expected_shape):
         test_image = nib.Nifti1Image(np.random.randint(0, 2, size=(128, 128, 128)).astype(float), np.eye(4))
         with tempfile.TemporaryDirectory() as tempdir:
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_as_channel_first.py` & `monai-weekly-1.3.dev2324/tests/test_as_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_as_channel_firstd.py` & `monai-weekly-1.3.dev2324/tests/test_as_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_as_channel_last.py` & `monai-weekly-1.3.dev2324/tests/test_as_channel_last.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_as_channel_lastd.py` & `monai-weekly-1.3.dev2324/tests/test_as_channel_lastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_as_discrete.py` & `monai-weekly-1.3.dev2324/tests/test_as_discrete.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_as_discreted.py` & `monai-weekly-1.3.dev2324/tests/test_as_discreted.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_atss_box_matcher.py` & `monai-weekly-1.3.dev2324/tests/test_atss_box_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_attentionunet.py` & `monai-weekly-1.3.dev2324/tests/test_attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_auto3dseg.py` & `monai-weekly-1.3.dev2324/tests/test_auto3dseg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_auto3dseg_bundlegen.py` & `monai-weekly-1.3.dev2324/tests/test_auto3dseg_bundlegen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_auto3dseg_ensemble.py` & `monai-weekly-1.3.dev2324/tests/test_auto3dseg_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_auto3dseg_hpo.py` & `monai-weekly-1.3.dev2324/tests/test_auto3dseg_hpo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_autoencoder.py` & `monai-weekly-1.3.dev2324/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_avg_merger.py` & `monai-weekly-1.3.dev2324/tests/test_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_basic_unet.py` & `monai-weekly-1.3.dev2324/tests/test_basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_basic_unetplusplus.py` & `monai-weekly-1.3.dev2324/tests/test_basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bending_energy.py` & `monai-weekly-1.3.dev2324/tests/test_bending_energy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bilateral_approx_cpu.py` & `monai-weekly-1.3.dev2324/tests/test_bilateral_approx_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bilateral_approx_cuda.py` & `monai-weekly-1.3.dev2324/tests/test_bilateral_approx_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bilateral_precise.py` & `monai-weekly-1.3.dev2324/tests/test_bilateral_precise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_blend_images.py` & `monai-weekly-1.3.dev2324/tests/test_blend_images.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_border_pad.py` & `monai-weekly-1.3.dev2324/tests/test_border_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_border_padd.py` & `monai-weekly-1.3.dev2324/tests/test_border_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bounding_rect.py` & `monai-weekly-1.3.dev2324/tests/test_bounding_rect.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bounding_rectd.py` & `monai-weekly-1.3.dev2324/tests/test_bounding_rectd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_box_coder.py` & `monai-weekly-1.3.dev2324/tests/test_box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_box_transform.py` & `monai-weekly-1.3.dev2324/tests/test_box_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_box_utils.py` & `monai-weekly-1.3.dev2324/tests/test_box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bundle_ckpt_export.py` & `monai-weekly-1.3.dev2324/tests/test_bundle_ckpt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bundle_download.py` & `monai-weekly-1.3.dev2324/tests/test_bundle_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bundle_get_data.py` & `monai-weekly-1.3.dev2324/tests/test_bundle_get_data.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bundle_init_bundle.py` & `monai-weekly-1.3.dev2324/tests/test_bundle_init_bundle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bundle_onnx_export.py` & `monai-weekly-1.3.dev2324/tests/test_bundle_onnx_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bundle_trt_export.py` & `monai-weekly-1.3.dev2324/tests/test_bundle_trt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bundle_utils.py` & `monai-weekly-1.3.dev2324/tests/test_bundle_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bundle_verify_metadata.py` & `monai-weekly-1.3.dev2324/tests/test_bundle_verify_metadata.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bundle_verify_net.py` & `monai-weekly-1.3.dev2324/tests/test_bundle_verify_net.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_bundle_workflow.py` & `monai-weekly-1.3.dev2324/tests/test_bundle_workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_cachedataset.py` & `monai-weekly-1.3.dev2324/tests/test_cachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_cachedataset_parallel.py` & `monai-weekly-1.3.dev2324/tests/test_cachedataset_parallel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_cachedataset_persistent_workers.py` & `monai-weekly-1.3.dev2324/tests/test_cachedataset_persistent_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_cachentransdataset.py` & `monai-weekly-1.3.dev2324/tests/test_cachentransdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_call_dist.py` & `monai-weekly-1.3.dev2324/tests/test_call_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_cast_to_type.py` & `monai-weekly-1.3.dev2324/tests/test_cast_to_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_cast_to_typed.py` & `monai-weekly-1.3.dev2324/tests/test_cast_to_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_center_scale_crop.py` & `monai-weekly-1.3.dev2324/tests/test_center_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_center_scale_cropd.py` & `monai-weekly-1.3.dev2324/tests/test_center_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_center_spatial_crop.py` & `monai-weekly-1.3.dev2324/tests/test_center_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_center_spatial_cropd.py` & `monai-weekly-1.3.dev2324/tests/test_center_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_channel_pad.py` & `monai-weekly-1.3.dev2324/tests/test_channel_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_check_hash.py` & `monai-weekly-1.3.dev2324/tests/test_check_hash.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_check_missing_files.py` & `monai-weekly-1.3.dev2324/tests/test_check_missing_files.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_classes_to_indices.py` & `monai-weekly-1.3.dev2324/tests/test_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_classes_to_indicesd.py` & `monai-weekly-1.3.dev2324/tests/test_classes_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_complex_utils.py` & `monai-weekly-1.3.dev2324/tests/test_complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_component_locator.py` & `monai-weekly-1.3.dev2324/tests/test_component_locator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_compose.py` & `monai-weekly-1.3.dev2324/tests/test_compose.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,16 +190,16 @@
                 pass
 
         c = mt.Compose([_RandomClass(), _RandomClass()])
         with self.assertWarns(Warning):
             c.randomize()
 
     def test_err_msg(self):
-        transforms = mt.Compose([abs, mt.AddChannel(), round])
-        with self.assertRaisesRegex(Exception, "AddChannel"):
+        transforms = mt.Compose([abs, mt.EnsureChannelFirst(), round])
+        with self.assertRaisesRegex(Exception, "EnsureChannelFirst"):
             transforms(42.1)
 
     def test_data_loader(self):
         xform_1 = mt.Compose([_RandXform()])
         train_ds = Dataset([1], transform=xform_1)
 
         xform_1.set_random_state(123)
@@ -240,15 +240,15 @@
 
             train_loader = DataLoader(train_ds, num_workers=2)
             out_1 = next(iter(train_loader))
             self.assertAlmostEqual(out_1.cpu().item(), 0.28602141572)
         set_determinism(None)
 
     def test_flatten_and_len(self):
-        x = mt.AddChannel()
+        x = mt.EnsureChannelFirst(channel_dim="no_channel")
         t1 = mt.Compose([x, x, x, x, mt.Compose([mt.Compose([x, x]), x, x])])
 
         t2 = t1.flatten()
         for t in t2.transforms:
             self.assertNotIsInstance(t, mt.Compose)
 
         # test len
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_compose_get_number_conversions.py` & `monai-weekly-1.3.dev2324/tests/test_compose_get_number_conversions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_compute_confusion_matrix.py` & `monai-weekly-1.3.dev2324/tests/test_compute_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_compute_f_beta.py` & `monai-weekly-1.3.dev2324/tests/test_compute_f_beta.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_compute_froc.py` & `monai-weekly-1.3.dev2324/tests/test_compute_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_compute_generalized_dice.py` & `monai-weekly-1.3.dev2324/tests/test_compute_generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_compute_ho_ver_maps.py` & `monai-weekly-1.3.dev2324/tests/test_compute_ho_ver_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_compute_ho_ver_maps_d.py` & `monai-weekly-1.3.dev2324/tests/test_compute_ho_ver_maps_d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_compute_meandice.py` & `monai-weekly-1.3.dev2324/tests/test_compute_meandice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_compute_meaniou.py` & `monai-weekly-1.3.dev2324/tests/test_compute_meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_compute_panoptic_quality.py` & `monai-weekly-1.3.dev2324/tests/test_compute_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_compute_regression_metrics.py` & `monai-weekly-1.3.dev2324/tests/test_compute_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_compute_roc_auc.py` & `monai-weekly-1.3.dev2324/tests/test_compute_roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_compute_variance.py` & `monai-weekly-1.3.dev2324/tests/test_compute_variance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_concat_itemsd.py` & `monai-weekly-1.3.dev2324/tests/test_concat_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_config_item.py` & `monai-weekly-1.3.dev2324/tests/test_config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_config_parser.py` & `monai-weekly-1.3.dev2324/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_contrastive_loss.py` & `monai-weekly-1.3.dev2324/tests/test_contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_convert_data_type.py` & `monai-weekly-1.3.dev2324/tests/test_convert_data_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_convert_to_multi_channel.py` & `monai-weekly-1.3.dev2324/tests/test_convert_to_multi_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_convert_to_multi_channeld.py` & `monai-weekly-1.3.dev2324/tests/test_convert_to_multi_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_convert_to_onnx.py` & `monai-weekly-1.3.dev2324/tests/test_convert_to_onnx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_convert_to_torchscript.py` & `monai-weekly-1.3.dev2324/tests/test_convert_to_torchscript.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_convert_to_trt.py` & `monai-weekly-1.3.dev2324/tests/test_convert_to_trt.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_convolutions.py` & `monai-weekly-1.3.dev2324/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_copy_itemsd.py` & `monai-weekly-1.3.dev2324/tests/test_copy_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_copy_model_state.py` & `monai-weekly-1.3.dev2324/tests/test_copy_model_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_correct_crop_centers.py` & `monai-weekly-1.3.dev2324/tests/test_correct_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_create_cross_validation_datalist.py` & `monai-weekly-1.3.dev2324/tests/test_create_cross_validation_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_create_grid_and_affine.py` & `monai-weekly-1.3.dev2324/tests/test_create_grid_and_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_crf_cpu.py` & `monai-weekly-1.3.dev2324/tests/test_crf_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_crf_cuda.py` & `monai-weekly-1.3.dev2324/tests/test_crf_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_crop_foreground.py` & `monai-weekly-1.3.dev2324/tests/test_crop_foreground.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_crop_foregroundd.py` & `monai-weekly-1.3.dev2324/tests/test_crop_foregroundd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_cross_validation.py` & `monai-weekly-1.3.dev2324/tests/test_cross_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,28 @@
 from __future__ import annotations
 
 import os
 import unittest
 
 from monai.apps import CrossValidation, DecathlonDataset
 from monai.data import MetaTensor
-from monai.transforms import AddChanneld, Compose, LoadImaged, ScaleIntensityd
+from monai.transforms import Compose, EnsureChannelFirstd, LoadImaged, ScaleIntensityd
 from tests.utils import skip_if_downloading_fails, skip_if_quick
 
 
 class TestCrossValidation(unittest.TestCase):
     @skip_if_quick
     def test_values(self):
         testing_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "testing_data")
         train_transform = Compose(
-            [LoadImaged(keys=["image", "label"]), AddChanneld(keys=["image", "label"]), ScaleIntensityd(keys="image")]
+            [
+                LoadImaged(keys=["image", "label"]),
+                EnsureChannelFirstd(keys=["image", "label"], channel_dim="no_channel"),
+                ScaleIntensityd(keys="image"),
+            ]
         )
         val_transform = LoadImaged(keys=["image", "label"])
 
         def _test_dataset(dataset):
             self.assertEqual(len(dataset), 52)
             self.assertTrue("image" in dataset[0])
             self.assertTrue("label" in dataset[0])
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_csv_dataset.py` & `monai-weekly-1.3.dev2324/tests/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_csv_iterable_dataset.py` & `monai-weekly-1.3.dev2324/tests/test_csv_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_csv_saver.py` & `monai-weekly-1.3.dev2324/tests/test_csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_cucim_dict_transform.py` & `monai-weekly-1.3.dev2324/tests/test_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_cucim_transform.py` & `monai-weekly-1.3.dev2324/tests/test_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_cumulative.py` & `monai-weekly-1.3.dev2324/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_cumulative_average.py` & `monai-weekly-1.3.dev2324/tests/test_cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_cumulative_average_dist.py` & `monai-weekly-1.3.dev2324/tests/test_cumulative_average_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_cv2_dist.py` & `monai-weekly-1.3.dev2324/tests/test_cv2_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_data_stats.py` & `monai-weekly-1.3.dev2324/tests/test_data_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_data_statsd.py` & `monai-weekly-1.3.dev2324/tests/test_data_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_dataloader.py` & `monai-weekly-1.3.dev2324/tests/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_dataset.py` & `monai-weekly-1.3.dev2324/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_dataset_func.py` & `monai-weekly-1.3.dev2324/tests/test_dataset_func.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_dataset_summary.py` & `monai-weekly-1.3.dev2324/tests/test_dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_decathlondataset.py` & `monai-weekly-1.3.dev2324/tests/test_decathlondataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,24 +14,28 @@
 import os
 import shutil
 import unittest
 from pathlib import Path
 
 from monai.apps import DecathlonDataset
 from monai.data import MetaTensor
-from monai.transforms import AddChanneld, Compose, LoadImaged, ScaleIntensityd
+from monai.transforms import Compose, EnsureChannelFirstd, LoadImaged, ScaleIntensityd
 from tests.utils import skip_if_downloading_fails, skip_if_quick
 
 
 class TestDecathlonDataset(unittest.TestCase):
     @skip_if_quick
     def test_values(self):
         testing_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "testing_data")
         transform = Compose(
-            [LoadImaged(keys=["image", "label"]), AddChanneld(keys=["image", "label"]), ScaleIntensityd(keys="image")]
+            [
+                LoadImaged(keys=["image", "label"]),
+                EnsureChannelFirstd(keys=["image", "label"], channel_dim="no_channel"),
+                ScaleIntensityd(keys="image"),
+            ]
         )
 
         def _test_dataset(dataset):
             self.assertEqual(len(dataset), 52)
             self.assertTrue("image" in dataset[0])
             self.assertTrue("label" in dataset[0])
             self.assertTrue(isinstance(dataset[0]["image"], MetaTensor))
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_decollate.py` & `monai-weekly-1.3.dev2324/tests/test_decollate.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import numpy as np
 import torch
 from parameterized import parameterized
 
 from monai.data import CacheDataset, DataLoader, Dataset, create_test_image_2d
 from monai.data.utils import decollate_batch
 from monai.transforms import (
-    AddChannel,
-    AddChanneld,
     Compose,
+    EnsureChannelFirst,
+    EnsureChannelFirstd,
     LoadImage,
     LoadImaged,
     RandAffine,
     RandFlip,
     RandFlipd,
     RandRotate90,
     SpatialPad,
@@ -125,35 +125,35 @@
 
             for decollated in [decollated_1, decollated_2]:
                 for i, d in enumerate(decollated):
                     self.check_match(dataset[b * batch_size + i], d)
 
     @parameterized.expand(TESTS_DICT)
     def test_decollation_dict(self, *transforms):
-        t_compose = Compose([AddChanneld(KEYS), Compose(transforms), ToTensord(KEYS)])
+        t_compose = Compose([EnsureChannelFirstd(KEYS, channel_dim="no_channel"), Compose(transforms), ToTensord(KEYS)])
         # If nibabel present, read from disk
         if has_nib:
             t_compose = Compose([LoadImaged("image", image_only=True), t_compose])
 
         dataset = CacheDataset(self.data_dict, t_compose, progress=False)
         self.check_decollate(dataset=dataset)
 
     @parameterized.expand(TESTS_LIST)
     def test_decollation_tensor(self, *transforms):
-        t_compose = Compose([AddChannel(), Compose(transforms), ToTensor()])
+        t_compose = Compose([EnsureChannelFirst(channel_dim="no_channel"), Compose(transforms), ToTensor()])
         # If nibabel present, read from disk
         if has_nib:
             t_compose = Compose([LoadImage(image_only=True), t_compose])
 
         dataset = Dataset(self.data_list, t_compose)
         self.check_decollate(dataset=dataset)
 
     @parameterized.expand(TESTS_LIST)
     def test_decollation_list(self, *transforms):
-        t_compose = Compose([AddChannel(), Compose(transforms), ToTensor()])
+        t_compose = Compose([EnsureChannelFirst(channel_dim="no_channel"), Compose(transforms), ToTensor()])
         # If nibabel present, read from disk
         if has_nib:
             t_compose = Compose([LoadImage(image_only=True), t_compose])
 
         dataset = Dataset(self.data_list, t_compose)
         self.check_decollate(dataset=dataset)
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_deepedit_interaction.py` & `monai-weekly-1.3.dev2324/tests/test_deepedit_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_deepedit_transforms.py` & `monai-weekly-1.3.dev2324/tests/test_deepedit_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_deepgrow_dataset.py` & `monai-weekly-1.3.dev2324/tests/test_deepgrow_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_deepgrow_interaction.py` & `monai-weekly-1.3.dev2324/tests/test_deepgrow_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_deepgrow_transforms.py` & `monai-weekly-1.3.dev2324/tests/test_deepgrow_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_delete_itemsd.py` & `monai-weekly-1.3.dev2324/tests/test_delete_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_denseblock.py` & `monai-weekly-1.3.dev2324/tests/test_denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_densenet.py` & `monai-weekly-1.3.dev2324/tests/test_densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_deprecated.py` & `monai-weekly-1.3.dev2324/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_detect_envelope.py` & `monai-weekly-1.3.dev2324/tests/test_detect_envelope.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_detection_coco_metrics.py` & `monai-weekly-1.3.dev2324/tests/test_detection_coco_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_detector_boxselector.py` & `monai-weekly-1.3.dev2324/tests/test_detector_boxselector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_detector_utils.py` & `monai-weekly-1.3.dev2324/tests/test_detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_dev_collate.py` & `monai-weekly-1.3.dev2324/tests/test_dev_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_dice_ce_loss.py` & `monai-weekly-1.3.dev2324/tests/test_dice_ce_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_dice_focal_loss.py` & `monai-weekly-1.3.dev2324/tests/test_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_dice_loss.py` & `monai-weekly-1.3.dev2324/tests/test_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_dints_cell.py` & `monai-weekly-1.3.dev2324/tests/test_dints_cell.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_dints_mixop.py` & `monai-weekly-1.3.dev2324/tests/test_dints_mixop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_dints_network.py` & `monai-weekly-1.3.dev2324/tests/test_dints_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_discriminator.py` & `monai-weekly-1.3.dev2324/tests/test_discriminator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_divisible_pad.py` & `monai-weekly-1.3.dev2324/tests/test_divisible_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_divisible_padd.py` & `monai-weekly-1.3.dev2324/tests/test_divisible_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_download_and_extract.py` & `monai-weekly-1.3.dev2324/tests/test_download_and_extract.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_downsample_block.py` & `monai-weekly-1.3.dev2324/tests/test_downsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_drop_path.py` & `monai-weekly-1.3.dev2324/tests/test_drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_ds_loss.py` & `monai-weekly-1.3.dev2324/tests/test_ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_dvf2ddf.py` & `monai-weekly-1.3.dev2324/tests/test_dvf2ddf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_dynunet.py` & `monai-weekly-1.3.dev2324/tests/test_dynunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_dynunet_block.py` & `monai-weekly-1.3.dev2324/tests/test_dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_efficientnet.py` & `monai-weekly-1.3.dev2324/tests/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_ensemble_evaluator.py` & `monai-weekly-1.3.dev2324/tests/test_ensemble_evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_ensure_channel_first.py` & `monai-weekly-1.3.dev2324/tests/test_ensure_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_ensure_channel_firstd.py` & `monai-weekly-1.3.dev2324/tests/test_ensure_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_ensure_tuple.py` & `monai-weekly-1.3.dev2324/tests/test_ensure_tuple.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_ensure_type.py` & `monai-weekly-1.3.dev2324/tests/test_ensure_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_ensure_typed.py` & `monai-weekly-1.3.dev2324/tests/test_ensure_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_enum_bound_interp.py` & `monai-weekly-1.3.dev2324/tests/test_enum_bound_interp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_eval_mode.py` & `monai-weekly-1.3.dev2324/tests/test_eval_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_evenly_divisible_all_gather_dist.py` & `monai-weekly-1.3.dev2324/tests/test_evenly_divisible_all_gather_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_factorized_increase.py` & `monai-weekly-1.3.dev2324/tests/test_factorized_increase.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_factorized_reduce.py` & `monai-weekly-1.3.dev2324/tests/test_factorized_reduce.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_fastmri_reader.py` & `monai-weekly-1.3.dev2324/tests/test_fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_fft_utils.py` & `monai-weekly-1.3.dev2324/tests/test_fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_fg_bg_to_indices.py` & `monai-weekly-1.3.dev2324/tests/test_fg_bg_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_fg_bg_to_indicesd.py` & `monai-weekly-1.3.dev2324/tests/test_fg_bg_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_file_basename.py` & `monai-weekly-1.3.dev2324/tests/test_file_basename.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_fill_holes.py` & `monai-weekly-1.3.dev2324/tests/test_fill_holes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_fill_holesd.py` & `monai-weekly-1.3.dev2324/tests/test_fill_holesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_fl_exchange_object.py` & `monai-weekly-1.3.dev2324/tests/test_fl_exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_fl_monai_algo.py` & `monai-weekly-1.3.dev2324/tests/test_fl_monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_fl_monai_algo_dist.py` & `monai-weekly-1.3.dev2324/tests/test_fl_monai_algo_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_fl_monai_algo_stats.py` & `monai-weekly-1.3.dev2324/tests/test_fl_monai_algo_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_flatten_sub_keysd.py` & `monai-weekly-1.3.dev2324/tests/test_flatten_sub_keysd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_flexible_unet.py` & `monai-weekly-1.3.dev2324/tests/test_flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_flip.py` & `monai-weekly-1.3.dev2324/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_flipd.py` & `monai-weekly-1.3.dev2324/tests/test_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_focal_loss.py` & `monai-weekly-1.3.dev2324/tests/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_folder_layout.py` & `monai-weekly-1.3.dev2324/tests/test_folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_foreground_mask.py` & `monai-weekly-1.3.dev2324/tests/test_foreground_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_foreground_maskd.py` & `monai-weekly-1.3.dev2324/tests/test_foreground_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_fourier.py` & `monai-weekly-1.3.dev2324/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_fpn_block.py` & `monai-weekly-1.3.dev2324/tests/test_fpn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_from_engine_hovernet.py` & `monai-weekly-1.3.dev2324/tests/test_from_engine_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_fullyconnectednet.py` & `monai-weekly-1.3.dev2324/tests/test_fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_gaussian.py` & `monai-weekly-1.3.dev2324/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_gaussian_filter.py` & `monai-weekly-1.3.dev2324/tests/test_gaussian_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_gaussian_sharpen.py` & `monai-weekly-1.3.dev2324/tests/test_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_gaussian_sharpend.py` & `monai-weekly-1.3.dev2324/tests/test_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_gaussian_smooth.py` & `monai-weekly-1.3.dev2324/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_gaussian_smoothd.py` & `monai-weekly-1.3.dev2324/tests/test_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generalized_dice_focal_loss.py` & `monai-weekly-1.3.dev2324/tests/test_generalized_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generalized_dice_loss.py` & `monai-weekly-1.3.dev2324/tests/test_generalized_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generalized_wasserstein_dice_loss.py` & `monai-weekly-1.3.dev2324/tests/test_generalized_wasserstein_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_distance_map.py` & `monai-weekly-1.3.dev2324/tests/test_generate_distance_map.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_distance_mapd.py` & `monai-weekly-1.3.dev2324/tests/test_generate_distance_mapd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_instance_border.py` & `monai-weekly-1.3.dev2324/tests/test_generate_instance_border.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_instance_borderd.py` & `monai-weekly-1.3.dev2324/tests/test_generate_instance_borderd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_instance_centroid.py` & `monai-weekly-1.3.dev2324/tests/test_generate_instance_centroid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_instance_centroidd.py` & `monai-weekly-1.3.dev2324/tests/test_generate_instance_centroidd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_instance_contour.py` & `monai-weekly-1.3.dev2324/tests/test_generate_instance_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_instance_contourd.py` & `monai-weekly-1.3.dev2324/tests/test_generate_instance_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_instance_type.py` & `monai-weekly-1.3.dev2324/tests/test_generate_instance_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_instance_typed.py` & `monai-weekly-1.3.dev2324/tests/test_generate_instance_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_label_classes_crop_centers.py` & `monai-weekly-1.3.dev2324/tests/test_generate_label_classes_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_param_groups.py` & `monai-weekly-1.3.dev2324/tests/test_generate_param_groups.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_pos_neg_label_crop_centers.py` & `monai-weekly-1.3.dev2324/tests/test_generate_pos_neg_label_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_spatial_bounding_box.py` & `monai-weekly-1.3.dev2324/tests/test_generate_spatial_bounding_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_succinct_contour.py` & `monai-weekly-1.3.dev2324/tests/test_generate_succinct_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_succinct_contourd.py` & `monai-weekly-1.3.dev2324/tests/test_generate_succinct_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_watershed_markers.py` & `monai-weekly-1.3.dev2324/tests/test_generate_watershed_markers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_watershed_markersd.py` & `monai-weekly-1.3.dev2324/tests/test_generate_watershed_markersd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_watershed_mask.py` & `monai-weekly-1.3.dev2324/tests/test_generate_watershed_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generate_watershed_maskd.py` & `monai-weekly-1.3.dev2324/tests/test_generate_watershed_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_generator.py` & `monai-weekly-1.3.dev2324/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_get_equivalent_dtype.py` & `monai-weekly-1.3.dev2324/tests/test_get_equivalent_dtype.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_get_extreme_points.py` & `monai-weekly-1.3.dev2324/tests/test_get_extreme_points.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_get_layers.py` & `monai-weekly-1.3.dev2324/tests/test_get_layers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_get_package_version.py` & `monai-weekly-1.3.dev2324/tests/test_get_package_version.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_get_unique_labels.py` & `monai-weekly-1.3.dev2324/tests/test_get_unique_labels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_gibbs_noise.py` & `monai-weekly-1.3.dev2324/tests/test_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_gibbs_noised.py` & `monai-weekly-1.3.dev2324/tests/test_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_giou_loss.py` & `monai-weekly-1.3.dev2324/tests/test_giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_global_mutual_information_loss.py` & `monai-weekly-1.3.dev2324/tests/test_global_mutual_information_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_globalnet.py` & `monai-weekly-1.3.dev2324/tests/test_globalnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_gmm.py` & `monai-weekly-1.3.dev2324/tests/test_gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_grid_dataset.py` & `monai-weekly-1.3.dev2324/tests/test_grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_grid_distortion.py` & `monai-weekly-1.3.dev2324/tests/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_grid_distortiond.py` & `monai-weekly-1.3.dev2324/tests/test_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_grid_patch.py` & `monai-weekly-1.3.dev2324/tests/test_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_grid_patchd.py` & `monai-weekly-1.3.dev2324/tests/test_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_grid_pull.py` & `monai-weekly-1.3.dev2324/tests/test_grid_pull.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_grid_split.py` & `monai-weekly-1.3.dev2324/tests/test_grid_split.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_grid_splitd.py` & `monai-weekly-1.3.dev2324/tests/test_grid_splitd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_checkpoint_loader.py` & `monai-weekly-1.3.dev2324/tests/test_handler_checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_checkpoint_saver.py` & `monai-weekly-1.3.dev2324/tests/test_handler_checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_classification_saver.py` & `monai-weekly-1.3.dev2324/tests/test_handler_classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_classification_saver_dist.py` & `monai-weekly-1.3.dev2324/tests/test_handler_classification_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_clearml_image.py` & `monai-weekly-1.3.dev2324/tests/test_handler_clearml_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_clearml_stats.py` & `monai-weekly-1.3.dev2324/tests/test_handler_clearml_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_confusion_matrix.py` & `monai-weekly-1.3.dev2324/tests/test_handler_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_confusion_matrix_dist.py` & `monai-weekly-1.3.dev2324/tests/test_handler_confusion_matrix_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_decollate_batch.py` & `monai-weekly-1.3.dev2324/tests/test_handler_decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_early_stop.py` & `monai-weekly-1.3.dev2324/tests/test_handler_early_stop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_garbage_collector.py` & `monai-weekly-1.3.dev2324/tests/test_handler_garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_hausdorff_distance.py` & `monai-weekly-1.3.dev2324/tests/test_handler_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_logfile.py` & `monai-weekly-1.3.dev2324/tests/test_handler_logfile.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_lr_scheduler.py` & `monai-weekly-1.3.dev2324/tests/test_handler_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_mean_dice.py` & `monai-weekly-1.3.dev2324/tests/test_handler_mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_mean_iou.py` & `monai-weekly-1.3.dev2324/tests/test_handler_mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_metric_logger.py` & `monai-weekly-1.3.dev2324/tests/test_handler_metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_metrics_reloaded.py` & `monai-weekly-1.3.dev2324/tests/test_handler_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_metrics_saver.py` & `monai-weekly-1.3.dev2324/tests/test_handler_metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_metrics_saver_dist.py` & `monai-weekly-1.3.dev2324/tests/test_handler_metrics_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_mlflow.py` & `monai-weekly-1.3.dev2324/tests/test_handler_mlflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_nvtx.py` & `monai-weekly-1.3.dev2324/tests/test_handler_nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_panoptic_quality.py` & `monai-weekly-1.3.dev2324/tests/test_handler_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_parameter_scheduler.py` & `monai-weekly-1.3.dev2324/tests/test_handler_parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_post_processing.py` & `monai-weekly-1.3.dev2324/tests/test_handler_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_prob_map_producer.py` & `monai-weekly-1.3.dev2324/tests/test_handler_prob_map_producer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_regression_metrics.py` & `monai-weekly-1.3.dev2324/tests/test_handler_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_regression_metrics_dist.py` & `monai-weekly-1.3.dev2324/tests/test_handler_regression_metrics_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_rocauc.py` & `monai-weekly-1.3.dev2324/tests/test_handler_rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_rocauc_dist.py` & `monai-weekly-1.3.dev2324/tests/test_handler_rocauc_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_smartcache.py` & `monai-weekly-1.3.dev2324/tests/test_handler_smartcache.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_stats.py` & `monai-weekly-1.3.dev2324/tests/test_handler_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_surface_distance.py` & `monai-weekly-1.3.dev2324/tests/test_handler_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_tb_image.py` & `monai-weekly-1.3.dev2324/tests/test_handler_tb_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_tb_stats.py` & `monai-weekly-1.3.dev2324/tests/test_handler_tb_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_handler_validation.py` & `monai-weekly-1.3.dev2324/tests/test_handler_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_hardnegsampler.py` & `monai-weekly-1.3.dev2324/tests/test_hardnegsampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_hashing.py` & `monai-weekly-1.3.dev2324/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_hausdorff_distance.py` & `monai-weekly-1.3.dev2324/tests/test_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_header_correct.py` & `monai-weekly-1.3.dev2324/tests/test_header_correct.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_highresnet.py` & `monai-weekly-1.3.dev2324/tests/test_highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_hilbert_transform.py` & `monai-weekly-1.3.dev2324/tests/test_hilbert_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_histogram_normalize.py` & `monai-weekly-1.3.dev2324/tests/test_histogram_normalize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_histogram_normalized.py` & `monai-weekly-1.3.dev2324/tests/test_histogram_normalized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_hovernet.py` & `monai-weekly-1.3.dev2324/tests/test_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_hovernet_instance_map_post_processing.py` & `monai-weekly-1.3.dev2324/tests/test_hovernet_instance_map_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_hovernet_instance_map_post_processingd.py` & `monai-weekly-1.3.dev2324/tests/test_hovernet_instance_map_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_hovernet_loss.py` & `monai-weekly-1.3.dev2324/tests/test_hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_hovernet_nuclear_type_post_processing.py` & `monai-weekly-1.3.dev2324/tests/test_hovernet_nuclear_type_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_hovernet_nuclear_type_post_processingd.py` & `monai-weekly-1.3.dev2324/tests/test_hovernet_nuclear_type_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_identity.py` & `monai-weekly-1.3.dev2324/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_identityd.py` & `monai-weekly-1.3.dev2324/tests/test_identityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_image_dataset.py` & `monai-weekly-1.3.dev2324/tests/test_image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_image_filter.py` & `monai-weekly-1.3.dev2324/tests/test_image_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_image_rw.py` & `monai-weekly-1.3.dev2324/tests/test_image_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_img2tensorboard.py` & `monai-weekly-1.3.dev2324/tests/test_img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_init_reader.py` & `monai-weekly-1.3.dev2324/tests/test_init_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_autorunner.py` & `monai-weekly-1.3.dev2324/tests/test_integration_autorunner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_bundle_run.py` & `monai-weekly-1.3.dev2324/tests/test_integration_bundle_run.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_classification_2d.py` & `monai-weekly-1.3.dev2324/tests/test_integration_classification_2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 from monai.apps import download_and_extract
 from monai.data import decollate_batch
 from monai.metrics import ROCAUCMetric
 from monai.networks import eval_mode
 from monai.networks.nets import DenseNet121
 from monai.transforms import (
     Activations,
-    AddChannel,
     AsDiscrete,
     Compose,
+    EnsureChannelFirst,
     LoadImage,
     RandFlip,
     RandRotate,
     RandZoom,
     ScaleIntensity,
     Transpose,
 )
@@ -59,25 +59,30 @@
 
 def run_training_test(root_dir, train_x, train_y, val_x, val_y, device="cuda:0", num_workers=10):
     monai.config.print_config()
     # define transforms for image and classification
     train_transforms = Compose(
         [
             LoadImage(image_only=True, simple_keys=True),
-            AddChannel(),
+            EnsureChannelFirst(channel_dim="no_channel"),
             Transpose(indices=[0, 2, 1]),
             ScaleIntensity(),
             RandRotate(range_x=np.pi / 12, prob=0.5, keep_size=True, dtype=np.float64),
             RandFlip(spatial_axis=0, prob=0.5),
             RandZoom(min_zoom=0.9, max_zoom=1.1, prob=0.5),
         ]
     )
     train_transforms.set_random_state(1234)
     val_transforms = Compose(
-        [LoadImage(image_only=True, simple_keys=True), AddChannel(), Transpose(indices=[0, 2, 1]), ScaleIntensity()]
+        [
+            LoadImage(image_only=True, simple_keys=True),
+            EnsureChannelFirst(channel_dim="no_channel"),
+            Transpose(indices=[0, 2, 1]),
+            ScaleIntensity(),
+        ]
     )
     y_pred_trans = Compose([Activations(softmax=True)])
     y_trans = AsDiscrete(to_onehot=len(np.unique(train_y)))
     auc_metric = ROCAUCMetric()
 
     # create train, val data loaders
     train_ds = MedNISTDataset(train_x, train_y, train_transforms)
@@ -148,15 +153,17 @@
                 )
     print(f"train completed, best_metric: {best_metric:0.4f}  at epoch: {best_metric_epoch}")
     return epoch_loss_values, best_metric, best_metric_epoch
 
 
 def run_inference_test(root_dir, test_x, test_y, device="cuda:0", num_workers=10):
     # define transforms for image and classification
-    val_transforms = Compose([LoadImage(image_only=True), AddChannel(), ScaleIntensity()])
+    val_transforms = Compose(
+        [LoadImage(image_only=True), EnsureChannelFirst(channel_dim="no_channel"), ScaleIntensity()]
+    )
     val_ds = MedNISTDataset(test_x, test_y, val_transforms)
     val_loader = DataLoader(val_ds, batch_size=300, num_workers=num_workers)
 
     model = DenseNet121(spatial_dims=2, in_channels=1, out_channels=len(np.unique(test_y))).to(device)
 
     model_filename = os.path.join(root_dir, "best_metric_model.pth")
     model.load_state_dict(torch.load(model_filename))
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_determinism.py` & `monai-weekly-1.3.dev2324/tests/test_integration_determinism.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import numpy as np
 import torch
 from torch.utils.data import DataLoader, Dataset
 
 from monai.data import create_test_image_2d
 from monai.losses import DiceLoss
 from monai.networks.nets import UNet
-from monai.transforms import AddChannel, Compose, RandRotate90, RandSpatialCrop, ScaleIntensity
+from monai.transforms import Compose, EnsureChannelFirst, RandRotate90, RandSpatialCrop, ScaleIntensity
 from monai.utils import set_determinism
 from tests.utils import DistTestCase, TimedCall
 
 
 def run_test(batch_size=64, train_steps=200, device="cuda:0"):
     class _TestBatch(Dataset):
         def __init__(self, transforms):
@@ -45,15 +45,20 @@
     net = UNet(
         spatial_dims=2, in_channels=1, out_channels=1, channels=(4, 8, 16, 32), strides=(2, 2, 2), num_res_units=2
     ).to(device)
 
     loss = DiceLoss(sigmoid=True)
     opt = torch.optim.Adam(net.parameters(), 1e-2)
     train_transforms = Compose(
-        [AddChannel(), ScaleIntensity(), RandSpatialCrop((96, 96), random_size=False), RandRotate90()]
+        [
+            EnsureChannelFirst(channel_dim="no_channel"),
+            ScaleIntensity(),
+            RandSpatialCrop((96, 96), random_size=False),
+            RandRotate90(),
+        ]
     )
 
     src = DataLoader(_TestBatch(train_transforms), batch_size=batch_size, shuffle=True)
 
     net.train()
     epoch_loss = 0
     step = 0
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_fast_train.py` & `monai-weekly-1.3.dev2324/tests/test_integration_fast_train.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_gpu_customization.py` & `monai-weekly-1.3.dev2324/tests/test_integration_gpu_customization.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_lazy_samples.py` & `monai-weekly-1.3.dev2324/tests/test_integration_lazy_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_nnunetv2_runner.py` & `monai-weekly-1.3.dev2324/tests/test_integration_nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_segmentation_3d.py` & `monai-weekly-1.3.dev2324/tests/test_integration_segmentation_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_sliding_window.py` & `monai-weekly-1.3.dev2324/tests/test_integration_sliding_window.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,21 +21,27 @@
 from ignite.engine import Engine, Events
 from torch.utils.data import DataLoader
 
 from monai.data import ImageDataset, create_test_image_3d
 from monai.inferers import sliding_window_inference
 from monai.networks import eval_mode, predict_segmentation
 from monai.networks.nets import UNet
-from monai.transforms import AddChannel, SaveImage
+from monai.transforms import EnsureChannelFirst, SaveImage
 from monai.utils import pytorch_after, set_determinism
 from tests.utils import DistTestCase, TimedCall, make_nifti_image, skip_if_quick
 
 
 def run_test(batch_size, img_name, seg_name, output_dir, device="cuda:0"):
-    ds = ImageDataset([img_name], [seg_name], transform=AddChannel(), seg_transform=AddChannel(), image_only=True)
+    ds = ImageDataset(
+        [img_name],
+        [seg_name],
+        transform=EnsureChannelFirst(channel_dim="no_channel"),
+        seg_transform=EnsureChannelFirst(channel_dim="no_channel"),
+        image_only=True,
+    )
     loader = DataLoader(ds, batch_size=1, pin_memory=torch.cuda.is_available())
 
     net = UNet(
         spatial_dims=3, in_channels=1, out_channels=1, channels=(4, 8, 16, 32), strides=(2, 2, 2), num_res_units=2
     ).to(device)
     roi_size = (16, 32, 48)
     sw_batch_size = batch_size
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_stn.py` & `monai-weekly-1.3.dev2324/tests/test_integration_stn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_unet_2d.py` & `monai-weekly-1.3.dev2324/tests/test_integration_unet_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_workers.py` & `monai-weekly-1.3.dev2324/tests/test_integration_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_workflows.py` & `monai-weekly-1.3.dev2324/tests/test_integration_workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
     TensorBoardStatsHandler,
     ValidationHandler,
     from_engine,
 )
 from monai.inferers import SimpleInferer, SlidingWindowInferer
 from monai.transforms import (
     Activationsd,
-    AsChannelFirstd,
     AsDiscreted,
     Compose,
+    EnsureChannelFirstd,
     KeepLargestConnectedComponentd,
     LoadImaged,
     RandCropByPosNegLabeld,
     RandRotate90d,
     SaveImage,
     SaveImaged,
     ScaleIntensityd,
@@ -67,26 +67,26 @@
     train_files = [{"image": img, "label": seg} for img, seg in zip(images[:20], segs[:20])]
     val_files = [{"image": img, "label": seg} for img, seg in zip(images[-20:], segs[-20:])]
 
     # define transforms for image and segmentation
     train_transforms = Compose(
         [
             LoadImaged(keys=["image", "label"]),
-            AsChannelFirstd(keys=["image", "label"], channel_dim=-1),
+            EnsureChannelFirstd(keys=["image", "label"], channel_dim=-1),
             ScaleIntensityd(keys=["image", "label"]),
             RandCropByPosNegLabeld(
                 keys=["image", "label"], label_key="label", spatial_size=[96, 96, 96], pos=1, neg=1, num_samples=4
             ),
             RandRotate90d(keys=["image", "label"], prob=0.5, spatial_axes=[0, 2]),
         ]
     )
     val_transforms = Compose(
         [
             LoadImaged(keys=["image", "label"]),
-            AsChannelFirstd(keys=["image", "label"], channel_dim=-1),
+            EnsureChannelFirstd(keys=["image", "label"], channel_dim=-1),
             ScaleIntensityd(keys=["image", "label"]),
         ]
     )
 
     # create a training data loader
     train_ds = monai.data.CacheDataset(data=train_files, transform=train_transforms, cache_rate=0.5)
     # use batch_size=2 to load images and use RandCropByPosNegLabeld to generate 2 x 4 images for network training
@@ -220,15 +220,15 @@
     segs = sorted(glob(os.path.join(root_dir, "seg*.nii.gz")))
     val_files = [{"image": img, "label": seg} for img, seg in zip(images, segs)]
 
     # define transforms for image and segmentation
     val_transforms = Compose(
         [
             LoadImaged(keys=["image", "label"]),
-            AsChannelFirstd(keys=["image", "label"], channel_dim=-1),
+            EnsureChannelFirstd(keys=["image", "label"], channel_dim=-1),
             ScaleIntensityd(keys=["image", "label"]),
         ]
     )
 
     # create a validation data loader
     val_ds = monai.data.Dataset(data=val_files, transform=val_transforms)
     val_loader = monai.data.DataLoader(val_ds, batch_size=1, num_workers=num_workers)
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_integration_workflows_gan.py` & `monai-weekly-1.3.dev2324/tests/test_integration_workflows_gan.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,29 +23,29 @@
 
 import monai
 from monai.data import create_test_image_2d
 from monai.engines import GanTrainer
 from monai.handlers import CheckpointSaver, StatsHandler, TensorBoardStatsHandler
 from monai.networks import normal_init
 from monai.networks.nets import Discriminator, Generator
-from monai.transforms import AsChannelFirstd, Compose, LoadImaged, RandFlipd, ScaleIntensityd
+from monai.transforms import Compose, EnsureChannelFirstd, LoadImaged, RandFlipd, ScaleIntensityd
 from monai.utils import GanKeys as Keys
 from monai.utils import set_determinism
 from tests.utils import DistTestCase, TimedCall, skip_if_quick
 
 
 def run_training_test(root_dir, device="cuda:0"):
     real_images = sorted(glob(os.path.join(root_dir, "img*.nii.gz")))
     train_files = [{"reals": img} for img in zip(real_images)]
 
     # prepare real data
     train_transforms = Compose(
         [
             LoadImaged(keys=["reals"]),
-            AsChannelFirstd(keys=["reals"]),
+            EnsureChannelFirstd(keys=["reals"], channel_dim=-1),
             ScaleIntensityd(keys=["reals"]),
             RandFlipd(keys=["reals"], prob=0.5),
         ]
     )
     train_ds = monai.data.CacheDataset(data=train_files, transform=train_transforms, cache_rate=0.5)
     train_loader = monai.data.DataLoader(train_ds, batch_size=2, shuffle=True, num_workers=4)
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_intensity_stats.py` & `monai-weekly-1.3.dev2324/tests/test_intensity_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_intensity_statsd.py` & `monai-weekly-1.3.dev2324/tests/test_intensity_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_inverse.py` & `monai-weekly-1.3.dev2324/tests/test_inverse.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 import numpy as np
 import torch
 from parameterized import parameterized
 
 from monai.data import CacheDataset, DataLoader, MetaTensor, create_test_image_2d, create_test_image_3d, decollate_batch
 from monai.networks.nets import UNet
 from monai.transforms import (
-    AddChanneld,
     Affined,
     BorderPadd,
     CenterScaleCropd,
     CenterSpatialCropd,
     Compose,
     CropForegroundd,
     DivisiblePadd,
+    EnsureChannelFirstd,
     Flipd,
     FromMetaTensord,
     InvertibleTransform,
     Lambdad,
     LoadImaged,
     Orientationd,
     RandAffined,
@@ -384,15 +384,17 @@
                 "label": torch.as_tensor(np.array(im_1d, copy=True)),
                 "other": torch.as_tensor(np.array(im_1d, copy=True)),
             }
 
         im_2d_fname, seg_2d_fname = (make_nifti_image(i) for i in create_test_image_2d(101, 100))
         im_3d_fname, seg_3d_fname = (make_nifti_image(i, affine) for i in create_test_image_3d(100, 101, 107))
 
-        load_ims = Compose([LoadImaged(KEYS), AddChanneld(KEYS), FromMetaTensord(KEYS)])
+        load_ims = Compose(
+            [LoadImaged(KEYS), EnsureChannelFirstd(KEYS, channel_dim="no_channel"), FromMetaTensord(KEYS)]
+        )
         self.all_data["2D"] = load_ims({"image": im_2d_fname, "label": seg_2d_fname})
         self.all_data["3D"] = load_ims({"image": im_3d_fname, "label": seg_3d_fname})
 
     def tearDown(self):
         set_determinism(seed=None)
 
     def check_inverse(self, name, keys, orig_d, fwd_bck_d, unmodified_d, acceptable_diff):
@@ -467,15 +469,17 @@
         for _ in range(20):
             image, label = create_test_image_2d(100, 101)
             test_data.append({"image": image, "label": label.astype(np.float32)})
 
         batch_size = 10
         # num workers = 0 for mac
         num_workers = 2 if sys.platform == "linux" else 0
-        transforms = Compose([AddChanneld(KEYS), SpatialPadd(KEYS, (150, 153)), extra_transform])
+        transforms = Compose(
+            [EnsureChannelFirstd(KEYS, channel_dim="no_channel"), SpatialPadd(KEYS, (150, 153)), extra_transform]
+        )
 
         dataset = CacheDataset(test_data, transform=transforms, progress=False)
         loader = DataLoader(dataset, batch_size=batch_size, shuffle=False, num_workers=num_workers)
 
         device = "cuda" if torch.cuda.is_available() else "cpu"
         model = UNet(spatial_dims=2, in_channels=1, out_channels=1, channels=(2, 4), strides=(1,)).to(device)
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_inverse_array.py` & `monai-weekly-1.3.dev2324/tests/test_inverse_array.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import unittest
 
 import torch
 from parameterized import parameterized
 
 from monai.data import MetaTensor
-from monai.transforms import AddChannel, Compose, Flip, Orientation, Spacing
+from monai.transforms import Compose, EnsureChannelFirst, Flip, Orientation, Spacing
 from monai.transforms.inverse import InvertibleTransform
 from monai.utils import optional_import
 from tests.utils import TEST_DEVICES
 
 _, has_nib = optional_import("nibabel")
 
 TESTS = []
@@ -38,15 +38,22 @@
         affine = torch.tensor([[0, 0, 1, 0], [-1, 0, 0, 0], [0, 10, 0, 0], [0, 0, 0, 1]]).to(dtype).to(device)
         img = torch.rand((15, 16, 17)).to(dtype).to(device)
         return MetaTensor(img, affine=affine)
 
     @parameterized.expand(TESTS)
     def test_inverse_array(self, use_compose: bool, dtype: torch.dtype, device: torch.device):
         img: MetaTensor
-        tr = Compose([AddChannel(), Orientation("RAS"), Flip(1), Spacing([1.0, 1.2, 0.9], align_corners=False)])
+        tr = Compose(
+            [
+                EnsureChannelFirst(channel_dim="no_channel"),
+                Orientation("RAS"),
+                Flip(1),
+                Spacing([1.0, 1.2, 0.9], align_corners=False),
+            ]
+        )
         num_invertible = len([i for i in tr.transforms if isinstance(i, InvertibleTransform)])
 
         # forward
         img = tr(self.get_image(dtype, device))
         self.assertEqual(len(img.applied_operations), num_invertible)
 
         # inverse with Compose
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_inverse_collation.py` & `monai-weekly-1.3.dev2324/tests/test_inverse_collation.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     MetaTensor,
     create_test_image_2d,
     create_test_image_3d,
     decollate_batch,
     pad_list_data_collate,
 )
 from monai.transforms import (
-    AddChanneld,
     Compose,
+    EnsureChannelFirstd,
     Flipd,
     LoadImaged,
     RandAffined,
     RandAxisFlipd,
     RandFlipd,
     RandRotate90d,
     RandRotated,
@@ -94,20 +94,20 @@
         if not has_nib:
             self.skipTest("nibabel required for test_inverse")
 
         set_determinism(seed=0)
 
         b_size = 11
         im_fname, seg_fname = (make_nifti_image(i) for i in create_test_image_3d(101, 100, 107))
-        load_ims = Compose([LoadImaged(KEYS), AddChanneld(KEYS)])
+        load_ims = Compose([LoadImaged(KEYS), EnsureChannelFirstd(KEYS, channel_dim="no_channel")])
         self.data_3d = [load_ims({"image": im_fname, "label": seg_fname}) for _ in range(b_size)]
 
         b_size = 8
         im_fname, seg_fname = (make_nifti_image(i) for i in create_test_image_2d(62, 37, rad_max=10))
-        load_ims = Compose([LoadImaged(KEYS), AddChanneld(KEYS)])
+        load_ims = Compose([LoadImaged(KEYS), EnsureChannelFirstd(KEYS, channel_dim="no_channel")])
         self.data_2d = [load_ims({"image": im_fname, "label": seg_fname}) for _ in range(b_size)]
 
         self.batch_size = 7
 
     def tearDown(self):
         set_determinism(seed=None)
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_invert.py` & `monai-weekly-1.3.dev2324/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_invertd.py` & `monai-weekly-1.3.dev2324/tests/test_invertd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_is_supported_format.py` & `monai-weekly-1.3.dev2324/tests/test_is_supported_format.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_iterable_dataset.py` & `monai-weekly-1.3.dev2324/tests/test_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_itk_torch_bridge.py` & `monai-weekly-1.3.dev2324/tests/test_itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_itk_writer.py` & `monai-weekly-1.3.dev2324/tests/test_itk_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_k_space_spike_noise.py` & `monai-weekly-1.3.dev2324/tests/test_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_k_space_spike_noised.py` & `monai-weekly-1.3.dev2324/tests/test_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_keep_largest_connected_component.py` & `monai-weekly-1.3.dev2324/tests/test_keep_largest_connected_component.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_keep_largest_connected_componentd.py` & `monai-weekly-1.3.dev2324/tests/test_keep_largest_connected_componentd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_kspace_mask.py` & `monai-weekly-1.3.dev2324/tests/test_kspace_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_label_filter.py` & `monai-weekly-1.3.dev2324/tests/test_label_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_label_filterd.py` & `monai-weekly-1.3.dev2324/tests/test_label_filterd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_label_quality_score.py` & `monai-weekly-1.3.dev2324/tests/test_label_quality_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_label_to_contour.py` & `monai-weekly-1.3.dev2324/tests/test_label_to_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_label_to_contourd.py` & `monai-weekly-1.3.dev2324/tests/test_label_to_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_label_to_mask.py` & `monai-weekly-1.3.dev2324/tests/test_label_to_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_label_to_maskd.py` & `monai-weekly-1.3.dev2324/tests/test_label_to_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_lambda.py` & `monai-weekly-1.3.dev2324/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_lambdad.py` & `monai-weekly-1.3.dev2324/tests/test_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_lesion_froc.py` & `monai-weekly-1.3.dev2324/tests/test_lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_list_data_collate.py` & `monai-weekly-1.3.dev2324/tests/test_list_data_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_list_to_dict.py` & `monai-weekly-1.3.dev2324/tests/test_list_to_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_lltm.py` & `monai-weekly-1.3.dev2324/tests/test_lltm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_lmdbdataset.py` & `monai-weekly-1.3.dev2324/tests/test_lmdbdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_lmdbdataset_dist.py` & `monai-weekly-1.3.dev2324/tests/test_lmdbdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_load_decathlon_datalist.py` & `monai-weekly-1.3.dev2324/tests/test_load_decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_load_image.py` & `monai-weekly-1.3.dev2324/tests/test_load_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_load_imaged.py` & `monai-weekly-1.3.dev2324/tests/test_load_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_load_spacing_orientation.py` & `monai-weekly-1.3.dev2324/tests/test_load_spacing_orientation.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 
 import nibabel
 import numpy as np
 import torch
 from nibabel.processing import resample_to_output
 from parameterized import parameterized
 
-from monai.transforms import AddChanneld, Compose, LoadImaged, Orientationd, Spacingd
+from monai.transforms import Compose, EnsureChannelFirstd, LoadImaged, Orientationd, Spacingd
 
 FILES = tuple(
     os.path.join(os.path.dirname(__file__), "testing_data", filename)
     for filename in ("anatomical.nii", "reoriented_anat_moved.nii")
 )
 
 
 class TestLoadSpacingOrientation(unittest.TestCase):
     @staticmethod
     def load_image(filename):
         data = {"image": filename}
-        t = Compose([LoadImaged(keys="image"), AddChanneld(keys="image")])
+        t = Compose([LoadImaged(keys="image"), EnsureChannelFirstd(keys="image", channel_dim="no_channel")])
         return t(data)
 
     @parameterized.expand(FILES)
     def test_load_spacingd(self, filename):
         data_dict = self.load_image(filename)
         t = time.time()
         res_dict = Spacingd(keys="image", pixdim=(1, 0.2, 1), diagonal=True, padding_mode="zeros")(data_dict)
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_loader_semaphore.py` & `monai-weekly-1.3.dev2324/tests/test_loader_semaphore.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_local_normalized_cross_correlation_loss.py` & `monai-weekly-1.3.dev2324/tests/test_local_normalized_cross_correlation_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_localnet.py` & `monai-weekly-1.3.dev2324/tests/test_localnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_localnet_block.py` & `monai-weekly-1.3.dev2324/tests/test_localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_look_up_option.py` & `monai-weekly-1.3.dev2324/tests/test_look_up_option.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_loss_metric.py` & `monai-weekly-1.3.dev2324/tests/test_loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_lr_finder.py` & `monai-weekly-1.3.dev2324/tests/test_lr_finder.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import torch
 from torch.utils.data import DataLoader
 
 from monai.apps import MedNISTDataset
 from monai.networks.nets import DenseNet
 from monai.optimizers import LearningRateFinder
-from monai.transforms import AddChanneld, Compose, LoadImaged, ScaleIntensityd, ToTensord
+from monai.transforms import Compose, EnsureChannelFirstd, LoadImaged, ScaleIntensityd, ToTensord
 from monai.utils import optional_import, set_determinism
 from monai.utils.misc import MONAIEnvVars
 from tests.utils import skip_if_downloading_fails
 
 if TYPE_CHECKING:
     import matplotlib.pyplot as plt
 
@@ -52,15 +52,15 @@
         self.root_dir = MONAIEnvVars.data_dir()
         if not self.root_dir:
             self.root_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "testing_data")
 
         self.transforms = Compose(
             [
                 LoadImaged(keys="image"),
-                AddChanneld(keys="image"),
+                EnsureChannelFirstd(keys="image", channel_dim="no_channel"),
                 ScaleIntensityd(keys="image"),
                 ToTensord(keys="image"),
             ]
         )
 
     def test_lr_finder(self):
         # 0.001 gives 54 examples
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_lr_scheduler.py` & `monai-weekly-1.3.dev2324/tests/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_make_nifti.py` & `monai-weekly-1.3.dev2324/tests/test_make_nifti.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_map_binary_to_indices.py` & `monai-weekly-1.3.dev2324/tests/test_map_binary_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_map_classes_to_indices.py` & `monai-weekly-1.3.dev2324/tests/test_map_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_map_label_value.py` & `monai-weekly-1.3.dev2324/tests/test_map_label_value.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_map_label_valued.py` & `monai-weekly-1.3.dev2324/tests/test_map_label_valued.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_map_transform.py` & `monai-weekly-1.3.dev2324/tests/test_map_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_mask_intensity.py` & `monai-weekly-1.3.dev2324/tests/test_mask_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_mask_intensityd.py` & `monai-weekly-1.3.dev2324/tests/test_mask_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_masked_dice_loss.py` & `monai-weekly-1.3.dev2324/tests/test_masked_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_masked_loss.py` & `monai-weekly-1.3.dev2324/tests/test_masked_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_masked_patch_wsi_dataset.py` & `monai-weekly-1.3.dev2324/tests/test_masked_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_matshow3d.py` & `monai-weekly-1.3.dev2324/tests/test_matshow3d.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,29 +13,42 @@
 
 import os
 import tempfile
 import unittest
 
 import numpy as np
 
-from monai.transforms import AddChanneld, Compose, LoadImaged, RandSpatialCropSamplesd, RepeatChanneld, ScaleIntensityd
+from monai.transforms import (
+    Compose,
+    EnsureChannelFirstd,
+    LoadImaged,
+    RandSpatialCropSamplesd,
+    RepeatChanneld,
+    ScaleIntensityd,
+)
 from monai.utils import optional_import
 from monai.visualize.utils import matshow3d
 from tests.utils import SkipIfNoModule
 
 compare_images, _ = optional_import("matplotlib.testing.compare", name="compare_images")
 pyplot, has_pyplot = optional_import("matplotlib", name="pyplot")
 
 
 @SkipIfNoModule("matplotlib")
 class TestMatshow3d(unittest.TestCase):
     def test_3d(self):
         testing_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "testing_data")
         keys = "image"
-        xforms = Compose([LoadImaged(keys=keys), AddChanneld(keys=keys), ScaleIntensityd(keys=keys)])
+        xforms = Compose(
+            [
+                LoadImaged(keys=keys),
+                EnsureChannelFirstd(keys=keys, channel_dim="no_channel"),
+                ScaleIntensityd(keys=keys),
+            ]
+        )
         image_path = os.path.join(testing_dir, "anatomical.nii")
         ims = xforms({keys: image_path})
 
         fig = pyplot.figure()  # external figure
         fig, _ = matshow3d(ims[keys], fig=fig, figsize=(2, 2), frames_per_row=5, every_n=2, frame_dim=-1, show=False)
 
         with tempfile.TemporaryDirectory() as tempdir:
@@ -49,15 +62,15 @@
 
     def test_samples(self):
         testing_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "testing_data")
         keys = "image"
         xforms = Compose(
             [
                 LoadImaged(keys=keys),
-                AddChanneld(keys=keys),
+                EnsureChannelFirstd(keys=keys),
                 ScaleIntensityd(keys=keys),
                 RandSpatialCropSamplesd(keys=keys, roi_size=(8, 8, 5), random_size=True, num_samples=10),
             ]
         )
         image_path = os.path.join(testing_dir, "anatomical.nii")
         xforms.set_random_state(0)
         ims = xforms({keys: image_path})
@@ -78,15 +91,15 @@
 
     def test_3d_rgb(self):
         testing_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "testing_data")
         keys = "image"
         xforms = Compose(
             [
                 LoadImaged(keys=keys),
-                AddChanneld(keys=keys),
+                EnsureChannelFirstd(keys=keys, channel_dim="no_channel"),
                 ScaleIntensityd(keys=keys),
                 # change to RGB color image
                 RepeatChanneld(keys=keys, repeats=3),
             ]
         )
         image_path = os.path.join(testing_dir, "anatomical.nii")
         ims = xforms({keys: image_path})
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_mean_ensemble.py` & `monai-weekly-1.3.dev2324/tests/test_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_mean_ensembled.py` & `monai-weekly-1.3.dev2324/tests/test_mean_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_median_filter.py` & `monai-weekly-1.3.dev2324/tests/test_median_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_median_smooth.py` & `monai-weekly-1.3.dev2324/tests/test_median_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_median_smoothd.py` & `monai-weekly-1.3.dev2324/tests/test_median_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_mednistdataset.py` & `monai-weekly-1.3.dev2324/tests/test_mednistdataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,25 +14,31 @@
 import os
 import shutil
 import unittest
 from pathlib import Path
 
 from monai.apps import MedNISTDataset
 from monai.data import MetaTensor
-from monai.transforms import AddChanneld, Compose, LoadImaged, ScaleIntensityd
+from monai.transforms import Compose, EnsureChannelFirstd, LoadImaged, ScaleIntensityd
 from tests.utils import skip_if_downloading_fails, skip_if_quick
 
 MEDNIST_FULL_DATASET_LENGTH = 58954
 
 
 class TestMedNISTDataset(unittest.TestCase):
     @skip_if_quick
     def test_values(self):
         testing_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "testing_data")
-        transform = Compose([LoadImaged(keys="image"), AddChanneld(keys="image"), ScaleIntensityd(keys="image")])
+        transform = Compose(
+            [
+                LoadImaged(keys="image"),
+                EnsureChannelFirstd(keys="image", channel_dim="no_channel"),
+                ScaleIntensityd(keys="image"),
+            ]
+        )
 
         def _test_dataset(dataset):
             self.assertEqual(len(dataset), int(MEDNIST_FULL_DATASET_LENGTH * dataset.test_frac))
             self.assertTrue("image" in dataset[0])
             self.assertTrue("label" in dataset[0])
             self.assertTrue(isinstance(dataset[0]["image"], MetaTensor))
             self.assertTupleEqual(dataset[0]["image"].shape, (1, 64, 64))
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_meta_affine.py` & `monai-weekly-1.3.dev2324/tests/test_meta_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_meta_tensor.py` & `monai-weekly-1.3.dev2324/tests/test_meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_metatensor_integration.py` & `monai-weekly-1.3.dev2324/tests/test_metatensor_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_metrics_reloaded.py` & `monai-weekly-1.3.dev2324/tests/test_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_milmodel.py` & `monai-weekly-1.3.dev2324/tests/test_milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_mlp.py` & `monai-weekly-1.3.dev2324/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_mmar_download.py` & `monai-weekly-1.3.dev2324/tests/test_mmar_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_module_list.py` & `monai-weekly-1.3.dev2324/tests/test_module_list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_monai_env_vars.py` & `monai-weekly-1.3.dev2324/tests/test_monai_env_vars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_monai_utils_misc.py` & `monai-weekly-1.3.dev2324/tests/test_monai_utils_misc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_mri_utils.py` & `monai-weekly-1.3.dev2324/tests/test_mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_multi_scale.py` & `monai-weekly-1.3.dev2324/tests/test_multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_net_adapter.py` & `monai-weekly-1.3.dev2324/tests/test_net_adapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_network_consistency.py` & `monai-weekly-1.3.dev2324/tests/test_network_consistency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_nifti_endianness.py` & `monai-weekly-1.3.dev2324/tests/test_nifti_endianness.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_nifti_header_revise.py` & `monai-weekly-1.3.dev2324/tests/test_nifti_header_revise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_nifti_rw.py` & `monai-weekly-1.3.dev2324/tests/test_nifti_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_normalize_intensity.py` & `monai-weekly-1.3.dev2324/tests/test_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_normalize_intensityd.py` & `monai-weekly-1.3.dev2324/tests/test_normalize_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_npzdictitemdataset.py` & `monai-weekly-1.3.dev2324/tests/test_npzdictitemdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_nrrd_reader.py` & `monai-weekly-1.3.dev2324/tests/test_nrrd_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_nuclick_transforms.py` & `monai-weekly-1.3.dev2324/tests/test_nuclick_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_numpy_reader.py` & `monai-weekly-1.3.dev2324/tests/test_numpy_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_nvtx_decorator.py` & `monai-weekly-1.3.dev2324/tests/test_nvtx_decorator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_nvtx_transform.py` & `monai-weekly-1.3.dev2324/tests/test_nvtx_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_occlusion_sensitivity.py` & `monai-weekly-1.3.dev2324/tests/test_occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_one_of.py` & `monai-weekly-1.3.dev2324/tests/test_one_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_optim_novograd.py` & `monai-weekly-1.3.dev2324/tests/test_optim_novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_optional_import.py` & `monai-weekly-1.3.dev2324/tests/test_optional_import.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_ori_ras_lps.py` & `monai-weekly-1.3.dev2324/tests/test_ori_ras_lps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_orientation.py` & `monai-weekly-1.3.dev2324/tests/test_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_orientationd.py` & `monai-weekly-1.3.dev2324/tests/test_orientationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_p3d_block.py` & `monai-weekly-1.3.dev2324/tests/test_p3d_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_pad_collation.py` & `monai-weekly-1.3.dev2324/tests/test_pad_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_pad_mode.py` & `monai-weekly-1.3.dev2324/tests/test_pad_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_parallel_execution.py` & `monai-weekly-1.3.dev2324/tests/test_parallel_execution.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_parallel_execution_dist.py` & `monai-weekly-1.3.dev2324/tests/test_parallel_execution_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_partition_dataset.py` & `monai-weekly-1.3.dev2324/tests/test_partition_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_partition_dataset_classes.py` & `monai-weekly-1.3.dev2324/tests/test_partition_dataset_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_patch_dataset.py` & `monai-weekly-1.3.dev2324/tests/test_patch_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_patch_inferer.py` & `monai-weekly-1.3.dev2324/tests/test_patch_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_patch_wsi_dataset.py` & `monai-weekly-1.3.dev2324/tests/test_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_patchembedding.py` & `monai-weekly-1.3.dev2324/tests/test_patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_pathology_he_stain.py` & `monai-weekly-1.3.dev2324/tests/test_pathology_he_stain.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_pathology_he_stain_dict.py` & `monai-weekly-1.3.dev2324/tests/test_pathology_he_stain_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_pathology_prob_nms.py` & `monai-weekly-1.3.dev2324/tests/test_pathology_prob_nms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_persistentdataset.py` & `monai-weekly-1.3.dev2324/tests/test_persistentdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_persistentdataset_dist.py` & `monai-weekly-1.3.dev2324/tests/test_persistentdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_phl_cpu.py` & `monai-weekly-1.3.dev2324/tests/test_phl_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_phl_cuda.py` & `monai-weekly-1.3.dev2324/tests/test_phl_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_pil_reader.py` & `monai-weekly-1.3.dev2324/tests/test_pil_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_plot_2d_or_3d_image.py` & `monai-weekly-1.3.dev2324/tests/test_plot_2d_or_3d_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_png_rw.py` & `monai-weekly-1.3.dev2324/tests/test_png_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_polyval.py` & `monai-weekly-1.3.dev2324/tests/test_polyval.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_prepare_batch_default.py` & `monai-weekly-1.3.dev2324/tests/test_prepare_batch_default.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_prepare_batch_default_dist.py` & `monai-weekly-1.3.dev2324/tests/test_prepare_batch_default_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_prepare_batch_extra_input.py` & `monai-weekly-1.3.dev2324/tests/test_prepare_batch_extra_input.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_prepare_batch_hovernet.py` & `monai-weekly-1.3.dev2324/tests/test_prepare_batch_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_preset_filters.py` & `monai-weekly-1.3.dev2324/tests/test_preset_filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_print_info.py` & `monai-weekly-1.3.dev2324/tests/test_print_info.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_print_transform_backends.py` & `monai-weekly-1.3.dev2324/tests/test_print_transform_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_probnms.py` & `monai-weekly-1.3.dev2324/tests/test_probnms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_probnmsd.py` & `monai-weekly-1.3.dev2324/tests/test_probnmsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_profiling.py` & `monai-weekly-1.3.dev2324/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_pytorch_version_after.py` & `monai-weekly-1.3.dev2324/tests/test_pytorch_version_after.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_query_memory.py` & `monai-weekly-1.3.dev2324/tests/test_query_memory.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_adjust_contrastd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_std_shift_intensity.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,35 +10,34 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import unittest
 
 import numpy as np
+import torch
 from parameterized import parameterized
 
-from monai.transforms import RandAdjustContrastd
+from monai.transforms import RandStdShiftIntensity
 from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D, assert_allclose
 
-TEST_CASE_1 = [(0.5, 4.5)]
 
-TEST_CASE_2 = [1.5]
-
-
-class TestRandAdjustContrastd(NumpyImageTestCase2D):
-    @parameterized.expand([TEST_CASE_1, TEST_CASE_2])
-    def test_correct_results(self, gamma):
-        adjuster = RandAdjustContrastd("img", prob=1.0, gamma=gamma)
-        for p in TEST_NDARRAYS:
-            result = adjuster({"img": p(self.imt)})
-            epsilon = 1e-7
-            img_min = self.imt.min()
-            img_range = self.imt.max() - img_min
-            expected = (
-                np.power(((self.imt - img_min) / float(img_range + epsilon)), adjuster.adjuster.gamma_value) * img_range
-                + img_min
-            )
-            assert_allclose(result["img"], expected, rtol=1e-05, type_test="tensor")
+class TestRandStdShiftIntensity(NumpyImageTestCase2D):
+    @parameterized.expand([[p] for p in TEST_NDARRAYS])
+    def test_value(self, p):
+        np.random.seed(0)
+        # simulate the randomize() of transform
+        np.random.random()
+        factor = np.random.uniform(low=-1.0, high=1.0)
+        offset = factor * np.std(self.imt)
+        expected = p(self.imt + offset)
+        shifter = RandStdShiftIntensity(factors=1.0, prob=1.0)
+        shifter.set_random_state(seed=0)
+        _imt = p(self.imt)
+        result = shifter(_imt)
+        if isinstance(_imt, torch.Tensor):
+            self.assertEqual(result.dtype, _imt.dtype)
+        assert_allclose(result, expected, atol=0, rtol=1e-5, type_test="tensor")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_affine.py` & `monai-weekly-1.3.dev2324/tests/test_rand_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_affine_grid.py` & `monai-weekly-1.3.dev2324/tests/test_rand_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_affined.py` & `monai-weekly-1.3.dev2324/tests/test_rand_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_axis_flip.py` & `monai-weekly-1.3.dev2324/tests/test_rand_axis_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_axis_flipd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_axis_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_bias_field.py` & `monai-weekly-1.3.dev2324/tests/test_rand_bias_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_bias_fieldd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_bias_fieldd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_coarse_dropout.py` & `monai-weekly-1.3.dev2324/tests/test_rand_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_coarse_dropoutd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_coarse_dropoutd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_coarse_shuffle.py` & `monai-weekly-1.3.dev2324/tests/test_rand_coarse_shuffle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_coarse_shuffled.py` & `monai-weekly-1.3.dev2324/tests/test_rand_coarse_shuffled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_crop_by_label_classes.py` & `monai-weekly-1.3.dev2324/tests/test_rand_crop_by_label_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_crop_by_label_classesd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_crop_by_label_classesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_crop_by_pos_neg_label.py` & `monai-weekly-1.3.dev2324/tests/test_rand_crop_by_pos_neg_label.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_crop_by_pos_neg_labeld.py` & `monai-weekly-1.3.dev2324/tests/test_rand_crop_by_pos_neg_labeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_cucim_dict_transform.py` & `monai-weekly-1.3.dev2324/tests/test_rand_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_cucim_transform.py` & `monai-weekly-1.3.dev2324/tests/test_rand_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_deform_grid.py` & `monai-weekly-1.3.dev2324/tests/test_rand_deform_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_elastic_2d.py` & `monai-weekly-1.3.dev2324/tests/test_rand_elastic_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_elastic_3d.py` & `monai-weekly-1.3.dev2324/tests/test_rand_elastic_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_elasticd_2d.py` & `monai-weekly-1.3.dev2324/tests/test_rand_elasticd_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_elasticd_3d.py` & `monai-weekly-1.3.dev2324/tests/test_rand_elasticd_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_flip.py` & `monai-weekly-1.3.dev2324/tests/test_rand_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_flipd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_gaussian_noise.py` & `monai-weekly-1.3.dev2324/tests/test_rand_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_gaussian_noised.py` & `monai-weekly-1.3.dev2324/tests/test_rand_gaussian_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_gaussian_sharpen.py` & `monai-weekly-1.3.dev2324/tests/test_rand_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_gaussian_sharpend.py` & `monai-weekly-1.3.dev2324/tests/test_rand_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_gaussian_smooth.py` & `monai-weekly-1.3.dev2324/tests/test_rand_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_gaussian_smoothd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_gibbs_noise.py` & `monai-weekly-1.3.dev2324/tests/test_rand_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_gibbs_noised.py` & `monai-weekly-1.3.dev2324/tests/test_rand_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_grid_distortion.py` & `monai-weekly-1.3.dev2324/tests/test_rand_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_grid_distortiond.py` & `monai-weekly-1.3.dev2324/tests/test_rand_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_grid_patch.py` & `monai-weekly-1.3.dev2324/tests/test_rand_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_grid_patchd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_histogram_shift.py` & `monai-weekly-1.3.dev2324/tests/test_rand_histogram_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_histogram_shiftd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_histogram_shiftd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_k_space_spike_noise.py` & `monai-weekly-1.3.dev2324/tests/test_rand_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_k_space_spike_noised.py` & `monai-weekly-1.3.dev2324/tests/test_rand_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_lambda.py` & `monai-weekly-1.3.dev2324/tests/test_rand_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_lambdad.py` & `monai-weekly-1.3.dev2324/tests/test_rand_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_rician_noise.py` & `monai-weekly-1.3.dev2324/tests/test_rand_rician_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_rician_noised.py` & `monai-weekly-1.3.dev2324/tests/test_rand_rician_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_rotate.py` & `monai-weekly-1.3.dev2324/tests/test_rand_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_rotate90.py` & `monai-weekly-1.3.dev2324/tests/test_rand_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_rotate90d.py` & `monai-weekly-1.3.dev2324/tests/test_rand_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_rotated.py` & `monai-weekly-1.3.dev2324/tests/test_rand_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_scale_crop.py` & `monai-weekly-1.3.dev2324/tests/test_rand_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_scale_cropd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_scale_intensity.py` & `monai-weekly-1.3.dev2324/tests/test_rand_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_scale_intensityd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_shift_intensity.py` & `monai-weekly-1.3.dev2324/tests/test_rand_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_shift_intensityd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_spatial_crop.py` & `monai-weekly-1.3.dev2324/tests/test_rand_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_spatial_crop_samples.py` & `monai-weekly-1.3.dev2324/tests/test_rand_spatial_crop_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_spatial_crop_samplesd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_spatial_crop_samplesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_spatial_cropd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_std_shift_intensity.py` & `monai-weekly-1.3.dev2324/tests/test_rand_scale_intensity_fixed_mean.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,34 +10,32 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import unittest
 
 import numpy as np
-import torch
 from parameterized import parameterized
 
-from monai.transforms import RandStdShiftIntensity
+from monai.transforms import RandScaleIntensityFixedMean
 from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D, assert_allclose
 
 
-class TestRandStdShiftIntensity(NumpyImageTestCase2D):
+class TestRandScaleIntensity(NumpyImageTestCase2D):
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_value(self, p):
+        scaler = RandScaleIntensityFixedMean(prob=1.0, factors=0.5)
+        scaler.set_random_state(seed=0)
+        im = p(self.imt)
+        result = scaler(im)
         np.random.seed(0)
         # simulate the randomize() of transform
         np.random.random()
-        factor = np.random.uniform(low=-1.0, high=1.0)
-        offset = factor * np.std(self.imt)
-        expected = p(self.imt + offset)
-        shifter = RandStdShiftIntensity(factors=1.0, prob=1.0)
-        shifter.set_random_state(seed=0)
-        _imt = p(self.imt)
-        result = shifter(_imt)
-        if isinstance(_imt, torch.Tensor):
-            self.assertEqual(result.dtype, _imt.dtype)
-        assert_allclose(result, expected, atol=0, rtol=1e-5, type_test="tensor")
+        mn = im.mean()
+        im = im - mn
+        expected = (1 + np.random.uniform(low=-0.5, high=0.5)) * im
+        expected = expected + mn
+        assert_allclose(result, expected, type_test="tensor", atol=1e-7)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_std_shift_intensityd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_weighted_crop.py` & `monai-weekly-1.3.dev2324/tests/test_rand_weighted_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_weighted_cropd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_weighted_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_zoom.py` & `monai-weekly-1.3.dev2324/tests/test_rand_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rand_zoomd.py` & `monai-weekly-1.3.dev2324/tests/test_rand_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_randidentity.py` & `monai-weekly-1.3.dev2324/tests/test_randidentity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_random_order.py` & `monai-weekly-1.3.dev2324/tests/test_random_order.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_randomizable.py` & `monai-weekly-1.3.dev2324/tests/test_randomizable.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_randomizable_transform_type.py` & `monai-weekly-1.3.dev2324/tests/test_randomizable_transform_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_randtorchvisiond.py` & `monai-weekly-1.3.dev2324/tests/test_randtorchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rankfilter_dist.py` & `monai-weekly-1.3.dev2324/tests/test_rankfilter_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_recon_net_utils.py` & `monai-weekly-1.3.dev2324/tests/test_recon_net_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_reference_based_normalize_intensity.py` & `monai-weekly-1.3.dev2324/tests/test_reference_based_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_reference_based_spatial_cropd.py` & `monai-weekly-1.3.dev2324/tests/test_reference_based_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_reference_resolver.py` & `monai-weekly-1.3.dev2324/tests/test_reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_reg_loss_integration.py` & `monai-weekly-1.3.dev2324/tests/test_reg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_regunet.py` & `monai-weekly-1.3.dev2324/tests/test_regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_regunet_block.py` & `monai-weekly-1.3.dev2324/tests/test_regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_remove_repeated_channel.py` & `monai-weekly-1.3.dev2324/tests/test_remove_repeated_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_remove_repeated_channeld.py` & `monai-weekly-1.3.dev2324/tests/test_remove_repeated_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_remove_small_objects.py` & `monai-weekly-1.3.dev2324/tests/test_remove_small_objects.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_repeat_channel.py` & `monai-weekly-1.3.dev2324/tests/test_repeat_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_repeat_channeld.py` & `monai-weekly-1.3.dev2324/tests/test_repeat_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_replace_module.py` & `monai-weekly-1.3.dev2324/tests/test_replace_module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_require_pkg.py` & `monai-weekly-1.3.dev2324/tests/test_require_pkg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_resample.py` & `monai-weekly-1.3.dev2324/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_resample_backends.py` & `monai-weekly-1.3.dev2324/tests/test_resample_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_resample_datalist.py` & `monai-weekly-1.3.dev2324/tests/test_resample_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_resample_to_match.py` & `monai-weekly-1.3.dev2324/tests/test_resample_to_match.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_resample_to_matchd.py` & `monai-weekly-1.3.dev2324/tests/test_resample_to_matchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_resampler.py` & `monai-weekly-1.3.dev2324/tests/test_resampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_resize.py` & `monai-weekly-1.3.dev2324/tests/test_resize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_resize_with_pad_or_crop.py` & `monai-weekly-1.3.dev2324/tests/test_resize_with_pad_or_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_resize_with_pad_or_cropd.py` & `monai-weekly-1.3.dev2324/tests/test_resize_with_pad_or_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_resized.py` & `monai-weekly-1.3.dev2324/tests/test_resized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_resnet.py` & `monai-weekly-1.3.dev2324/tests/test_resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_retinanet.py` & `monai-weekly-1.3.dev2324/tests/test_retinanet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_retinanet_detector.py` & `monai-weekly-1.3.dev2324/tests/test_retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_retinanet_predict_utils.py` & `monai-weekly-1.3.dev2324/tests/test_retinanet_predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rotate.py` & `monai-weekly-1.3.dev2324/tests/test_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rotate90.py` & `monai-weekly-1.3.dev2324/tests/test_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rotate90d.py` & `monai-weekly-1.3.dev2324/tests/test_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_rotated.py` & `monai-weekly-1.3.dev2324/tests/test_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_safe_dtype_range.py` & `monai-weekly-1.3.dev2324/tests/test_safe_dtype_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_saliency_inferer.py` & `monai-weekly-1.3.dev2324/tests/test_saliency_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_sample_slices.py` & `monai-weekly-1.3.dev2324/tests/test_sample_slices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_sampler_dist.py` & `monai-weekly-1.3.dev2324/tests/test_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_save_classificationd.py` & `monai-weekly-1.3.dev2324/tests/test_save_classificationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_save_image.py` & `monai-weekly-1.3.dev2324/tests/test_save_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_save_imaged.py` & `monai-weekly-1.3.dev2324/tests/test_save_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_save_state.py` & `monai-weekly-1.3.dev2324/tests/test_save_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_savitzky_golay_filter.py` & `monai-weekly-1.3.dev2324/tests/test_savitzky_golay_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_savitzky_golay_smooth.py` & `monai-weekly-1.3.dev2324/tests/test_savitzky_golay_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_savitzky_golay_smoothd.py` & `monai-weekly-1.3.dev2324/tests/test_savitzky_golay_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_scale_intensity.py` & `monai-weekly-1.3.dev2324/tests/test_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_scale_intensity_range.py` & `monai-weekly-1.3.dev2324/tests/test_scale_intensity_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_scale_intensity_range_percentiles.py` & `monai-weekly-1.3.dev2324/tests/test_scale_intensity_range_percentiles.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_scale_intensity_range_percentilesd.py` & `monai-weekly-1.3.dev2324/tests/test_scale_intensity_range_percentilesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_scale_intensity_ranged.py` & `monai-weekly-1.3.dev2324/tests/test_scale_intensity_ranged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_scale_intensityd.py` & `monai-weekly-1.3.dev2324/tests/test_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_se_block.py` & `monai-weekly-1.3.dev2324/tests/test_se_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_se_blocks.py` & `monai-weekly-1.3.dev2324/tests/test_se_blocks.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_seg_loss_integration.py` & `monai-weekly-1.3.dev2324/tests/test_seg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_segresnet.py` & `monai-weekly-1.3.dev2324/tests/test_segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_segresnet_block.py` & `monai-weekly-1.3.dev2324/tests/test_segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_segresnet_ds.py` & `monai-weekly-1.3.dev2324/tests/test_segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_select_cross_validation_folds.py` & `monai-weekly-1.3.dev2324/tests/test_select_cross_validation_folds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_select_itemsd.py` & `monai-weekly-1.3.dev2324/tests/test_select_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_selfattention.py` & `monai-weekly-1.3.dev2324/tests/test_selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_senet.py` & `monai-weekly-1.3.dev2324/tests/test_senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_separable_filter.py` & `monai-weekly-1.3.dev2324/tests/test_separable_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_set_determinism.py` & `monai-weekly-1.3.dev2324/tests/test_set_determinism.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_set_visible_devices.py` & `monai-weekly-1.3.dev2324/tests/test_set_visible_devices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_shift_intensity.py` & `monai-weekly-1.3.dev2324/tests/test_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_shift_intensityd.py` & `monai-weekly-1.3.dev2324/tests/test_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_shuffle_buffer.py` & `monai-weekly-1.3.dev2324/tests/test_shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_signal_continuouswavelet.py` & `monai-weekly-1.3.dev2324/tests/test_signal_continuouswavelet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_signal_fillempty.py` & `monai-weekly-1.3.dev2324/tests/test_signal_fillempty.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_signal_rand_add_gaussiannoise.py` & `monai-weekly-1.3.dev2324/tests/test_signal_rand_add_gaussiannoise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_signal_rand_add_sine.py` & `monai-weekly-1.3.dev2324/tests/test_signal_rand_add_sine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_signal_rand_add_sine_partial.py` & `monai-weekly-1.3.dev2324/tests/test_signal_rand_add_sine_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_signal_rand_add_squarepulse.py` & `monai-weekly-1.3.dev2324/tests/test_signal_rand_add_squarepulse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_signal_rand_add_squarepulse_partial.py` & `monai-weekly-1.3.dev2324/tests/test_signal_rand_add_squarepulse_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_signal_rand_drop.py` & `monai-weekly-1.3.dev2324/tests/test_signal_rand_drop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_signal_rand_scale.py` & `monai-weekly-1.3.dev2324/tests/test_signal_rand_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_signal_rand_shift.py` & `monai-weekly-1.3.dev2324/tests/test_signal_rand_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_signal_remove_frequency.py` & `monai-weekly-1.3.dev2324/tests/test_signal_remove_frequency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_simple_aspp.py` & `monai-weekly-1.3.dev2324/tests/test_simple_aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_simulatedelay.py` & `monai-weekly-1.3.dev2324/tests/test_simulatedelay.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_simulatedelayd.py` & `monai-weekly-1.3.dev2324/tests/test_simulatedelayd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_skip_connection.py` & `monai-weekly-1.3.dev2324/tests/test_skip_connection.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_slice_inferer.py` & `monai-weekly-1.3.dev2324/tests/test_slice_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_sliding_patch_wsi_dataset.py` & `monai-weekly-1.3.dev2324/tests/test_sliding_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_sliding_window_hovernet_inference.py` & `monai-weekly-1.3.dev2324/tests/test_sliding_window_hovernet_inference.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_sliding_window_inference.py` & `monai-weekly-1.3.dev2324/tests/test_sliding_window_inference.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_sliding_window_splitter.py` & `monai-weekly-1.3.dev2324/tests/test_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_smartcachedataset.py` & `monai-weekly-1.3.dev2324/tests/test_smartcachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_smooth_field.py` & `monai-weekly-1.3.dev2324/tests/test_smooth_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_sobel_gradient.py` & `monai-weekly-1.3.dev2324/tests/test_sobel_gradient.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_sobel_gradientd.py` & `monai-weekly-1.3.dev2324/tests/test_sobel_gradientd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_some_of.py` & `monai-weekly-1.3.dev2324/tests/test_some_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_spacing.py` & `monai-weekly-1.3.dev2324/tests/test_spacing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_spacingd.py` & `monai-weekly-1.3.dev2324/tests/test_spacingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_spatial_combine_transforms.py` & `monai-weekly-1.3.dev2324/tests/test_spatial_combine_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_spatial_crop.py` & `monai-weekly-1.3.dev2324/tests/test_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_spatial_cropd.py` & `monai-weekly-1.3.dev2324/tests/test_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_spatial_pad.py` & `monai-weekly-1.3.dev2324/tests/test_spatial_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_spatial_padd.py` & `monai-weekly-1.3.dev2324/tests/test_spatial_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_spatial_resample.py` & `monai-weekly-1.3.dev2324/tests/test_spatial_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_spatial_resampled.py` & `monai-weekly-1.3.dev2324/tests/test_spatial_resampled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_split_channel.py` & `monai-weekly-1.3.dev2324/tests/test_split_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_split_channeld.py` & `monai-weekly-1.3.dev2324/tests/test_split_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_splitdim.py` & `monai-weekly-1.3.dev2324/tests/test_splitdim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_splitdimd.py` & `monai-weekly-1.3.dev2324/tests/test_splitdimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_squeezedim.py` & `monai-weekly-1.3.dev2324/tests/test_squeezedim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_squeezedimd.py` & `monai-weekly-1.3.dev2324/tests/test_squeezedimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_ssim_loss.py` & `monai-weekly-1.3.dev2324/tests/test_ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_ssim_metric.py` & `monai-weekly-1.3.dev2324/tests/test_ssim_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_state_cacher.py` & `monai-weekly-1.3.dev2324/tests/test_state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_std_shift_intensity.py` & `monai-weekly-1.3.dev2324/tests/test_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_std_shift_intensityd.py` & `monai-weekly-1.3.dev2324/tests/test_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_str2bool.py` & `monai-weekly-1.3.dev2324/tests/test_str2bool.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_str2list.py` & `monai-weekly-1.3.dev2324/tests/test_str2list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_subpixel_upsample.py` & `monai-weekly-1.3.dev2324/tests/test_subpixel_upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_surface_dice.py` & `monai-weekly-1.3.dev2324/tests/test_surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_surface_distance.py` & `monai-weekly-1.3.dev2324/tests/test_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_swin_unetr.py` & `monai-weekly-1.3.dev2324/tests/test_swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_synthetic.py` & `monai-weekly-1.3.dev2324/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_tciadataset.py` & `monai-weekly-1.3.dev2324/tests/test_tciadataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 import os
 import shutil
 import unittest
 
 from monai.apps import TciaDataset
 from monai.apps.tcia import TCIA_LABEL_DICT
 from monai.data import MetaTensor
-from monai.transforms import AddChanneld, Compose, LoadImaged, ScaleIntensityd
+from monai.transforms import Compose, EnsureChannelFirstd, LoadImaged, ScaleIntensityd
 from tests.utils import skip_if_downloading_fails, skip_if_quick
 
 
 class TestTciaDataset(unittest.TestCase):
     @skip_if_quick
     def test_values(self):
         testing_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "testing_data")
         download_len = 1
         val_frac = 1.0
         collection = "QIN-PROSTATE-Repeatability"
 
         transform = Compose(
             [
                 LoadImaged(keys=["image", "seg"], reader="PydicomReader", label_dict=TCIA_LABEL_DICT[collection]),
-                AddChanneld(keys="image"),
+                EnsureChannelFirstd(keys="image", channel_dim="no_channel"),
                 ScaleIntensityd(keys="image"),
             ]
         )
 
         def _test_dataset(dataset):
             self.assertEqual(len(dataset), int(download_len * val_frac))
             self.assertTrue("image" in dataset[0])
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_testtimeaugmentation.py` & `monai-weekly-1.3.dev2324/tests/test_testtimeaugmentation.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from monai.data import CacheDataset, DataLoader, create_test_image_2d
 from monai.data.test_time_augmentation import TestTimeAugmentation
 from monai.data.utils import pad_list_data_collate
 from monai.losses import DiceLoss
 from monai.networks.nets import UNet
 from monai.transforms import (
     Activations,
-    AddChanneld,
     AsDiscrete,
     Compose,
     CropForegroundd,
     DivisiblePadd,
+    EnsureChannelFirstd,
     RandAffined,
     RandScaleIntensityd,
 )
 from monai.transforms.croppad.dictionary import SpatialPadd
 from monai.transforms.spatial.dictionary import RandFlipd
 from monai.utils import optional_import, set_determinism
 from monai.utils.enums import PostFix
@@ -80,15 +80,15 @@
 
         train_data = self.get_data(num_training_ims, input_size)
         test_data = self.get_data(1, input_size)
         device = "cuda" if torch.cuda.is_available() else "cpu"
 
         transforms = Compose(
             [
-                AddChanneld(keys),
+                EnsureChannelFirstd(keys, channel_dim="no_channel"),
                 RandAffined(
                     keys,
                     prob=1.0,
                     spatial_size=(30, 30),
                     rotate_range=(np.pi / 3, np.pi / 3),
                     translate_range=(3, 3),
                     scale_range=((0.8, 1), (0.8, 1)),
@@ -141,29 +141,35 @@
         self.assertTrue(all(np.unique(mode) == (0, 1)))
         self.assertGreaterEqual(mean.min(), 0.0)
         self.assertLessEqual(mean.max(), 1.0)
         self.assertEqual(std.shape, (1,) + input_size)
         self.assertIsInstance(vvc, float)
 
     def test_warn_non_random(self):
-        transforms = Compose([AddChanneld("im"), SpatialPadd("im", 1)])
+        transforms = Compose([EnsureChannelFirstd("im", channel_dim="no_channel"), SpatialPadd("im", 1)])
         with self.assertWarns(UserWarning):
             TestTimeAugmentation(transforms, None, None, None)
 
     def test_warn_random_but_has_no_invertible(self):
         transforms = Compose(
-            [AddChanneld("image"), RandFlipd("image", prob=1.0), RandScaleIntensityd("image", 0.1, prob=1.0)]
+            [
+                EnsureChannelFirstd("image", channel_dim="no_channel"),
+                RandFlipd("image", prob=1.0),
+                RandScaleIntensityd("image", 0.1, prob=1.0),
+            ]
         )
         with self.assertWarns(UserWarning):
             tta = TestTimeAugmentation(transforms, 5, 0, orig_key="image")
             tta(self.get_data(1, (20, 20), data_type=np.float32))
 
     def test_warn_random_but_all_not_invertible(self):
         """test with no invertible stack"""
-        transforms = Compose([AddChanneld("image"), RandScaleIntensityd("image", 0.1, prob=1.0)])
+        transforms = Compose(
+            [EnsureChannelFirstd("image", channel_dim="no_channel"), RandScaleIntensityd("image", 0.1, prob=1.0)]
+        )
         with self.assertWarns(UserWarning):
             tta = TestTimeAugmentation(transforms, 1, 0, orig_key="image")
             tta(self.get_data(1, (20, 20), data_type=np.float32))
 
     def test_single_transform(self):
         for p in TEST_NDARRAYS:
             transforms = RandFlipd(["image", "label"], prob=1.0)
```

### Comparing `monai-weekly-1.2.dev2323/tests/test_text_encoding.py` & `monai-weekly-1.3.dev2324/tests/test_text_encoding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_thread_buffer.py` & `monai-weekly-1.3.dev2324/tests/test_thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_threadcontainer.py` & `monai-weekly-1.3.dev2324/tests/test_threadcontainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_threshold_intensity.py` & `monai-weekly-1.3.dev2324/tests/test_threshold_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_threshold_intensityd.py` & `monai-weekly-1.3.dev2324/tests/test_threshold_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_timedcall_dist.py` & `monai-weekly-1.3.dev2324/tests/test_timedcall_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_to_contiguous.py` & `monai-weekly-1.3.dev2324/tests/test_to_contiguous.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_to_cupy.py` & `monai-weekly-1.3.dev2324/tests/test_to_cupy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_to_cupyd.py` & `monai-weekly-1.3.dev2324/tests/test_to_cupyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_to_device.py` & `monai-weekly-1.3.dev2324/tests/test_to_device.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_to_deviced.py` & `monai-weekly-1.3.dev2324/tests/test_to_deviced.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_to_from_meta_tensord.py` & `monai-weekly-1.3.dev2324/tests/test_to_from_meta_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_to_numpy.py` & `monai-weekly-1.3.dev2324/tests/test_to_numpy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_to_numpyd.py` & `monai-weekly-1.3.dev2324/tests/test_to_numpyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_to_onehot.py` & `monai-weekly-1.3.dev2324/tests/test_to_onehot.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_to_pil.py` & `monai-weekly-1.3.dev2324/tests/test_to_pil.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_to_pild.py` & `monai-weekly-1.3.dev2324/tests/test_to_pild.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_to_tensor.py` & `monai-weekly-1.3.dev2324/tests/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_to_tensord.py` & `monai-weekly-1.3.dev2324/tests/test_to_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_torchscript_utils.py` & `monai-weekly-1.3.dev2324/tests/test_torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_torchvision.py` & `monai-weekly-1.3.dev2324/tests/test_torchvision.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_torchvision_fc_model.py` & `monai-weekly-1.3.dev2324/tests/test_torchvision_fc_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_torchvisiond.py` & `monai-weekly-1.3.dev2324/tests/test_torchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_traceable_transform.py` & `monai-weekly-1.3.dev2324/tests/test_traceable_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_train_mode.py` & `monai-weekly-1.3.dev2324/tests/test_train_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_trainable_bilateral.py` & `monai-weekly-1.3.dev2324/tests/test_trainable_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_trainable_joint_bilateral.py` & `monai-weekly-1.3.dev2324/tests/test_trainable_joint_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_transchex.py` & `monai-weekly-1.3.dev2324/tests/test_transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_transform.py` & `monai-weekly-1.3.dev2324/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_transformerblock.py` & `monai-weekly-1.3.dev2324/tests/test_transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_transpose.py` & `monai-weekly-1.3.dev2324/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_transposed.py` & `monai-weekly-1.3.dev2324/tests/test_transposed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_tversky_loss.py` & `monai-weekly-1.3.dev2324/tests/test_tversky_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_unet.py` & `monai-weekly-1.3.dev2324/tests/test_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_unetr.py` & `monai-weekly-1.3.dev2324/tests/test_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_unetr_block.py` & `monai-weekly-1.3.dev2324/tests/test_unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_unified_focal_loss.py` & `monai-weekly-1.3.dev2324/tests/test_unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_upsample_block.py` & `monai-weekly-1.3.dev2324/tests/test_upsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_utils_pytorch_numpy_unification.py` & `monai-weekly-1.3.dev2324/tests/test_utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_varautoencoder.py` & `monai-weekly-1.3.dev2324/tests/test_varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_varnet.py` & `monai-weekly-1.3.dev2324/tests/test_varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_version_leq.py` & `monai-weekly-1.3.dev2324/tests/test_version_leq.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_video_datasets.py` & `monai-weekly-1.3.dev2324/tests/test_video_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_vis_cam.py` & `monai-weekly-1.3.dev2324/tests/test_vis_cam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_vis_gradbased.py` & `monai-weekly-1.3.dev2324/tests/test_vis_gradbased.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_vis_gradcam.py` & `monai-weekly-1.3.dev2324/tests/test_vis_gradcam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_vit.py` & `monai-weekly-1.3.dev2324/tests/test_vit.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_vitautoenc.py` & `monai-weekly-1.3.dev2324/tests/test_vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_vnet.py` & `monai-weekly-1.3.dev2324/tests/test_vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_vote_ensemble.py` & `monai-weekly-1.3.dev2324/tests/test_vote_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_vote_ensembled.py` & `monai-weekly-1.3.dev2324/tests/test_vote_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_warp.py` & `monai-weekly-1.3.dev2324/tests/test_warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_watershed.py` & `monai-weekly-1.3.dev2324/tests/test_watershed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_watershedd.py` & `monai-weekly-1.3.dev2324/tests/test_watershedd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_weight_init.py` & `monai-weekly-1.3.dev2324/tests/test_weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_weighted_random_sampler_dist.py` & `monai-weekly-1.3.dev2324/tests/test_weighted_random_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_with_allow_missing_keys.py` & `monai-weekly-1.3.dev2324/tests/test_with_allow_missing_keys.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_write_metrics_reports.py` & `monai-weekly-1.3.dev2324/tests/test_write_metrics_reports.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_wsi_sliding_window_splitter.py` & `monai-weekly-1.3.dev2324/tests/test_wsi_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_wsireader.py` & `monai-weekly-1.3.dev2324/tests/test_wsireader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_zipdataset.py` & `monai-weekly-1.3.dev2324/tests/test_zipdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_zoom.py` & `monai-weekly-1.3.dev2324/tests/test_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_zoom_affine.py` & `monai-weekly-1.3.dev2324/tests/test_zoom_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/tests/test_zoomd.py` & `monai-weekly-1.3.dev2324/tests/test_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2323/versioneer.py` & `monai-weekly-1.3.dev2324/versioneer.py`

 * *Files identical despite different names*

