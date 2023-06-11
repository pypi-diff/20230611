# Comparing `tmp/GANDLF-0.0.17.dev20230610.tar.gz` & `tmp/GANDLF-0.0.17.dev20230611.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GANDLF-0.0.17.dev20230610.tar", last modified: Sat Jun 10 03:12:36 2023, max compression
+gzip compressed data, was "GANDLF-0.0.17.dev20230611.tar", last modified: Sun Jun 11 03:19:35 2023, max compression
```

## Comparing `GANDLF-0.0.17.dev20230610.tar` & `GANDLF-0.0.17.dev20230611.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.605734 GANDLF-0.0.17.dev20230610/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/Dockerfile-CPU
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/Dockerfile-CUDA11.6
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/Dockerfile-ROCm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.565734 GANDLF-0.0.17.dev20230610/GANDLF/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.565734 GANDLF-0.0.17.dev20230610/GANDLF/anonymize/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/anonymize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/anonymize/convert_to_nifti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.569734 GANDLF-0.0.17.dev20230610/GANDLF/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/cli/generate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/cli/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/cli/patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/cli/post_training_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/cli/preprocess_and_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/cli/recover_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.573734 GANDLF-0.0.17.dev20230610/GANDLF/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/compute/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/compute/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/compute/inference_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/compute/loss_and_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/compute/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/compute/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.573734 GANDLF-0.0.17.dev20230610/GANDLF/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/ImagesFromDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.573734 GANDLF-0.0.17.dev20230610/GANDLF/data/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/augmentation/blur_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/augmentation/noise_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/augmentation/rgb_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/augmentation/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/augmentation/wrap_torchio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/inference_dataloader_histopath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.573734 GANDLF-0.0.17.dev20230610/GANDLF/data/patch_miner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/patch_miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.577734 GANDLF-0.0.17.dev20230610/GANDLF/data/patch_miner/opm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/patch_miner/opm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/patch_miner/opm/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/patch_miner/opm/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/patch_miner/opm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.577734 GANDLF-0.0.17.dev20230610/GANDLF/data/post_process/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/post_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/post_process/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/post_process/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.581734 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/crop_zero_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/non_zero_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/normalize_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/resample_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/rgb_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.581734 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/template_matching/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/template_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/template_matching/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/template_matching/histogram_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/template_matching/stain_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/template_matching/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/threshold_and_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.585734 GANDLF-0.0.17.dev20230610/GANDLF/grad_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/grad_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/grad_clipping/adaptive_gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/grad_clipping/clip_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/grad_clipping/grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/inference_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.585734 GANDLF-0.0.17.dev20230610/GANDLF/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/losses/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/losses/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/losses/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.585734 GANDLF-0.0.17.dev20230610/GANDLF/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/metrics/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.593734 GANDLF-0.0.17.dev20230610/GANDLF/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/MSDNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/brain_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/deep_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/imagenet_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/light_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/light_unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/modelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/sdnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.601734 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/DecodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/DownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/EncodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/FCNUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/IncConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/IncDownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/IncDropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/IncUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/InceptionModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/InitialConv.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/Interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/ResNetModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/UpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/add_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/add_downsample_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/average_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/out_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/transunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/uinc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/models/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.601734 GANDLF-0.0.17.dev20230610/GANDLF/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/optimizers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29587 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/parseConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.601734 GANDLF-0.0.17.dev20230610/GANDLF/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/schedulers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/training_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.605734 GANDLF-0.0.17.dev20230610/GANDLF/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/utils/handle_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/utils/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/utils/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/utils/modelio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/utils/parameter_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/GANDLF/utils/write_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 03:12:29.000000 GANDLF-0.0.17.dev20230610/GANDLF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 03:12:36.565734 GANDLF-0.0.17.dev20230610/GANDLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-10 03:12:36.000000 GANDLF-0.0.17.dev20230610/GANDLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-06-10 03:12:36.000000 GANDLF-0.0.17.dev20230610/GANDLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 03:12:36.000000 GANDLF-0.0.17.dev20230610/GANDLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 03:10:26.000000 GANDLF-0.0.17.dev20230610/GANDLF.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-10 03:12:36.000000 GANDLF-0.0.17.dev20230610/GANDLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-10 03:12:36.000000 GANDLF-0.0.17.dev20230610/GANDLF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-10 03:12:36.605734 GANDLF-0.0.17.dev20230610/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/gandlf_anonymizer
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/gandlf_collectStats
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/gandlf_configGenerator
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/gandlf_constructCSV
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/gandlf_deploy
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/gandlf_generateMetrics
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/gandlf_optimizeModel
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/gandlf_patchMiner
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/gandlf_preprocess
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/gandlf_recoverConfig
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/gandlf_run
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/gandlf_verifyInstall
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 03:12:36.605734 GANDLF-0.0.17.dev20230610/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-10 03:10:11.000000 GANDLF-0.0.17.dev20230610/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.953329 GANDLF-0.0.17.dev20230611/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/Dockerfile-CPU
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/Dockerfile-CUDA11.6
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/Dockerfile-ROCm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.921329 GANDLF-0.0.17.dev20230611/GANDLF/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.921329 GANDLF-0.0.17.dev20230611/GANDLF/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/anonymize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/anonymize/convert_to_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.925329 GANDLF-0.0.17.dev20230611/GANDLF/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/cli/generate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/cli/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/cli/patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/cli/post_training_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/cli/preprocess_and_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/cli/recover_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.925329 GANDLF-0.0.17.dev20230611/GANDLF/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/compute/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/compute/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/compute/inference_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/compute/loss_and_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/compute/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/compute/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.929329 GANDLF-0.0.17.dev20230611/GANDLF/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/ImagesFromDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.929329 GANDLF-0.0.17.dev20230611/GANDLF/data/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/augmentation/blur_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/augmentation/noise_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/augmentation/rgb_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/augmentation/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/augmentation/wrap_torchio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/inference_dataloader_histopath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.929329 GANDLF-0.0.17.dev20230611/GANDLF/data/patch_miner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/patch_miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.929329 GANDLF-0.0.17.dev20230611/GANDLF/data/patch_miner/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/patch_miner/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/patch_miner/opm/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/patch_miner/opm/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/patch_miner/opm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.933329 GANDLF-0.0.17.dev20230611/GANDLF/data/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/post_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/post_process/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/post_process/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.933329 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/crop_zero_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/non_zero_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/normalize_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/resample_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/rgb_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.937329 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/template_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/template_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/template_matching/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/template_matching/histogram_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/template_matching/stain_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/template_matching/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/threshold_and_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.937329 GANDLF-0.0.17.dev20230611/GANDLF/grad_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/grad_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/grad_clipping/adaptive_gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/grad_clipping/clip_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/grad_clipping/grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/inference_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.937329 GANDLF-0.0.17.dev20230611/GANDLF/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/losses/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/losses/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/losses/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.937329 GANDLF-0.0.17.dev20230611/GANDLF/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/metrics/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.945329 GANDLF-0.0.17.dev20230611/GANDLF/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/MSDNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/brain_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/deep_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/imagenet_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/light_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/light_unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/modelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/sdnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.949329 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/DecodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/DownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/EncodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/FCNUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/IncConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/IncDownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/IncDropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/IncUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/InceptionModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/InitialConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/Interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/ResNetModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/UpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/add_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/add_downsample_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/out_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/transunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/uinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/models/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.949329 GANDLF-0.0.17.dev20230611/GANDLF/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/optimizers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29587 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/parseConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.953329 GANDLF-0.0.17.dev20230611/GANDLF/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/schedulers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/training_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.953329 GANDLF-0.0.17.dev20230611/GANDLF/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/utils/handle_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/utils/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/utils/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/utils/modelio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/utils/parameter_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/GANDLF/utils/write_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-11 03:19:29.000000 GANDLF-0.0.17.dev20230611/GANDLF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:19:35.921329 GANDLF-0.0.17.dev20230611/GANDLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-11 03:19:35.000000 GANDLF-0.0.17.dev20230611/GANDLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-06-11 03:19:35.000000 GANDLF-0.0.17.dev20230611/GANDLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:19:35.000000 GANDLF-0.0.17.dev20230611/GANDLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:17:22.000000 GANDLF-0.0.17.dev20230611/GANDLF.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-11 03:19:35.000000 GANDLF-0.0.17.dev20230611/GANDLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 03:19:35.000000 GANDLF-0.0.17.dev20230611/GANDLF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-11 03:19:35.953329 GANDLF-0.0.17.dev20230611/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/gandlf_anonymizer
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/gandlf_collectStats
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/gandlf_configGenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/gandlf_constructCSV
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/gandlf_deploy
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/gandlf_generateMetrics
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/gandlf_optimizeModel
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/gandlf_patchMiner
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/gandlf_preprocess
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/gandlf_recoverConfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/gandlf_run
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/gandlf_verifyInstall
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:19:35.953329 GANDLF-0.0.17.dev20230611/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-11 03:17:03.000000 GANDLF-0.0.17.dev20230611/setup.py
```

### Comparing `GANDLF-0.0.17.dev20230610/CODE_OF_CONDUCT.md` & `GANDLF-0.0.17.dev20230611/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/CONTRIBUTING.md` & `GANDLF-0.0.17.dev20230611/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/Dockerfile-CPU` & `GANDLF-0.0.17.dev20230611/Dockerfile-CPU`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/Dockerfile-CUDA11.6` & `GANDLF-0.0.17.dev20230611/Dockerfile-CUDA11.6`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/Dockerfile-ROCm` & `GANDLF-0.0.17.dev20230611/Dockerfile-ROCm`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/anonymize/__init__.py` & `GANDLF-0.0.17.dev20230611/GANDLF/anonymize/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/anonymize/convert_to_nifti.py` & `GANDLF-0.0.17.dev20230611/GANDLF/anonymize/convert_to_nifti.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/cli/__init__.py` & `GANDLF-0.0.17.dev20230611/GANDLF/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/cli/config_generator.py` & `GANDLF-0.0.17.dev20230611/GANDLF/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/cli/deploy.py` & `GANDLF-0.0.17.dev20230611/GANDLF/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/cli/generate_metrics.py` & `GANDLF-0.0.17.dev20230611/GANDLF/cli/generate_metrics.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/cli/main_run.py` & `GANDLF-0.0.17.dev20230611/GANDLF/cli/main_run.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/cli/patch_extraction.py` & `GANDLF-0.0.17.dev20230611/GANDLF/cli/patch_extraction.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/cli/post_training_model_optimization.py` & `GANDLF-0.0.17.dev20230611/GANDLF/cli/post_training_model_optimization.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,25 +12,31 @@
         model_path (str): Path to the model file.
         config_path (str): Path to the config file.
 
     Returns:
         bool: True if successful, False otherwise.
     """
 
-    parameters = parseConfig(config_path, version_check_flag=False)
+    main_dict = load_model(model_path, "cpu")
+    parameters = main_dict.get("parameters", None)
+    parameters = (
+        parseConfig(config_path, version_check_flag=False)
+        if parameters is None
+        else parameters
+    )
     (
         model,
         _,
         _,
         _,
         _,
         parameters,
     ) = create_pytorch_objects(parameters, device="cpu")
+    parameters["model"]["onnx_export"] = True
 
-    main_dict = load_model(model_path, "cpu")
     version_check(parameters["version"], version_to_check=main_dict["version"])
     model.load_state_dict(main_dict["model_state_dict"])
     optimize_and_save_model(model, parameters, model_path, onnx_export=True)
     optimized_model_path = model_path.replace("pth.tar", "onnx")
     if not os.path.exists(optimized_model_path):
         print("Error while optimizing model.")
         return False
```

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/cli/preprocess_and_save.py` & `GANDLF-0.0.17.dev20230611/GANDLF/cli/preprocess_and_save.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/cli/recover_config.py` & `GANDLF-0.0.17.dev20230611/GANDLF/cli/recover_config.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/compute/forward_pass.py` & `GANDLF-0.0.17.dev20230611/GANDLF/compute/forward_pass.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/compute/generic.py` & `GANDLF-0.0.17.dev20230611/GANDLF/compute/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/compute/inference_loop.py` & `GANDLF-0.0.17.dev20230611/GANDLF/compute/inference_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/compute/loss_and_metric.py` & `GANDLF-0.0.17.dev20230611/GANDLF/compute/loss_and_metric.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/compute/step.py` & `GANDLF-0.0.17.dev20230611/GANDLF/compute/step.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/compute/training_loop.py` & `GANDLF-0.0.17.dev20230611/GANDLF/compute/training_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/ImagesFromDataFrame.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/ImagesFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/__init__.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/augmentation/__init__.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/augmentation/blur_enhanced.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/augmentation/blur_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/augmentation/noise_enhanced.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/augmentation/noise_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/augmentation/rgb_augs.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/augmentation/rgb_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/augmentation/rotations.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/augmentation/rotations.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/augmentation/wrap_torchio.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/augmentation/wrap_torchio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/inference_dataloader_histopath.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/inference_dataloader_histopath.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/patch_miner/opm/patch.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/patch_miner/opm/patch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/patch_miner/opm/patch_manager.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/patch_miner/opm/patch_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/patch_miner/opm/utils.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/patch_miner/opm/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/post_process/morphology.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/post_process/morphology.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/post_process/tensor.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/post_process/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/__init__.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/crop_zero_planes.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/crop_zero_planes.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/non_zero_normalize.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/non_zero_normalize.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/normalize_rgb.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/normalize_rgb.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/resample_minimum.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/resample_minimum.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/rgb_conversion.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/rgb_conversion.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/template_matching/base.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/template_matching/base.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/template_matching/histogram_matching.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/template_matching/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/template_matching/stain_extractors.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/template_matching/stain_extractors.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/template_matching/stain_normalizer.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/template_matching/stain_normalizer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/template_matching/utils.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/template_matching/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/data/preprocessing/threshold_and_clip.py` & `GANDLF-0.0.17.dev20230611/GANDLF/data/preprocessing/threshold_and_clip.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/grad_clipping/adaptive_gradient_clipping.py` & `GANDLF-0.0.17.dev20230611/GANDLF/grad_clipping/adaptive_gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/grad_clipping/clip_gradients.py` & `GANDLF-0.0.17.dev20230611/GANDLF/grad_clipping/clip_gradients.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/grad_clipping/grad_scaler.py` & `GANDLF-0.0.17.dev20230611/GANDLF/grad_clipping/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/inference_manager.py` & `GANDLF-0.0.17.dev20230611/GANDLF/inference_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/logger.py` & `GANDLF-0.0.17.dev20230611/GANDLF/logger.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/losses/__init__.py` & `GANDLF-0.0.17.dev20230611/GANDLF/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/losses/hybrid.py` & `GANDLF-0.0.17.dev20230611/GANDLF/losses/hybrid.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/losses/regression.py` & `GANDLF-0.0.17.dev20230611/GANDLF/losses/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/losses/segmentation.py` & `GANDLF-0.0.17.dev20230611/GANDLF/losses/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/metrics/__init__.py` & `GANDLF-0.0.17.dev20230611/GANDLF/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/metrics/classification.py` & `GANDLF-0.0.17.dev20230611/GANDLF/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/metrics/generic.py` & `GANDLF-0.0.17.dev20230611/GANDLF/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/metrics/regression.py` & `GANDLF-0.0.17.dev20230611/GANDLF/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/metrics/segmentation.py` & `GANDLF-0.0.17.dev20230611/GANDLF/metrics/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/MSDNet.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/MSDNet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/__init__.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/brain_age.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/brain_age.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/deep_unet.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/deep_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/densenet.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/densenet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/efficientnet.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/fcn.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/fcn.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/imagenet_unet.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/imagenet_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/imagenet_vgg.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/imagenet_vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/light_unet.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/light_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/light_unet_multilayer.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/light_unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/modelBase.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/modelBase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/resnet.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/resnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/sdnet.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/sdnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/DecodingModule.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/DecodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/DownsamplingModule.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/DownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/EncodingModule.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/EncodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/FCNUpsamplingModule.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/FCNUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/IncConv.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/IncConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/IncDownsamplingModule.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/IncDownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/IncDropout.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/IncDropout.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/IncUpsamplingModule.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/IncUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/InceptionModule.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/InceptionModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/InitialConv.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/InitialConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/Interpolate.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/Interpolate.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/ResNetModule.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/ResNetModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/UpsamplingModule.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/UpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/add_conv_block.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/add_conv_block.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/average_pool.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/average_pool.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/seg_modules/out_conv.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/seg_modules/out_conv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/transunet.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/transunet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/uinc.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/uinc.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/unet.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/unet_multilayer.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/unetr.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/unetr.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/models/vgg.py` & `GANDLF-0.0.17.dev20230611/GANDLF/models/vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/optimizers/__init__.py` & `GANDLF-0.0.17.dev20230611/GANDLF/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/optimizers/wrap_torch.py` & `GANDLF-0.0.17.dev20230611/GANDLF/optimizers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/parseConfig.py` & `GANDLF-0.0.17.dev20230611/GANDLF/parseConfig.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/schedulers/__init__.py` & `GANDLF-0.0.17.dev20230611/GANDLF/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/schedulers/wrap_torch.py` & `GANDLF-0.0.17.dev20230611/GANDLF/schedulers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/training_manager.py` & `GANDLF-0.0.17.dev20230611/GANDLF/training_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/utils/__init__.py` & `GANDLF-0.0.17.dev20230611/GANDLF/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/utils/generic.py` & `GANDLF-0.0.17.dev20230611/GANDLF/utils/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,16 @@
 
     Args:
         version_string (str): The string to be parsed.
 
     Returns:
         int: The version number.
     """
-    version_string_split = version_string.split(".")
+    version_string_split = version_string.replace("-dev", "")
+    version_string_split = version_string_split.split(".")
     if len(version_string_split) > 3:
         del version_string_split[-1]
     return int("".join(version_string_split))
 
 
 def version_check(version_from_config, version_to_check):
     """
```

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/utils/handle_collisions.py` & `GANDLF-0.0.17.dev20230611/GANDLF/utils/handle_collisions.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/utils/imaging.py` & `GANDLF-0.0.17.dev20230611/GANDLF/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/utils/modelbase.py` & `GANDLF-0.0.17.dev20230611/GANDLF/utils/modelbase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/utils/modelio.py` & `GANDLF-0.0.17.dev20230611/GANDLF/utils/modelio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os, hashlib, pkg_resources, subprocess
 import torch
 
 from .generic import get_unique_timestamp
+from ..version import __version__
 
 # these are the base keys for the model dictionary to save
 model_dict_full = {
     "epoch": 0,
     "model_state_dict": None,
     "optimizer_state_dict": None,
     "loss": None,
@@ -146,15 +147,16 @@
         path (str): The path to save the model dictionary to.
         onnx_export (bool): Whether to export to ONNX and OpenVINO.
     """
     model_dict["timestamp"] = get_unique_timestamp()
     model_dict["timestamp_hash"] = hashlib.sha256(
         str(model_dict["timestamp"]).encode("utf-8")
     ).hexdigest()
-    model_dict["version"] = pkg_resources.require("GANDLF")[0].version
+    model_dict["version"] = __version__
+    model_dict["parameters"] = params
     try:
         model_dict["git_hash"] = (
             subprocess.check_output(["git", "rev-parse", "HEAD"])
             .decode("ascii")
             .strip()
         )
     except subprocess.CalledProcessError:
```

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/utils/parameter_processing.py` & `GANDLF-0.0.17.dev20230611/GANDLF/utils/parameter_processing.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/utils/tensor.py` & `GANDLF-0.0.17.dev20230611/GANDLF/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF/utils/write_parse.py` & `GANDLF-0.0.17.dev20230611/GANDLF/utils/write_parse.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF.egg-info/PKG-INFO` & `GANDLF-0.0.17.dev20230611/GANDLF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230610
+Version: 0.0.17.dev20230611
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230610 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230611 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230610/GANDLF.egg-info/SOURCES.txt` & `GANDLF-0.0.17.dev20230611/GANDLF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/HISTORY.md` & `GANDLF-0.0.17.dev20230611/HISTORY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/LICENSE` & `GANDLF-0.0.17.dev20230611/LICENSE`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/PKG-INFO` & `GANDLF-0.0.17.dev20230611/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230610
+Version: 0.0.17.dev20230611
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230610 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230611 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230610/README.md` & `GANDLF-0.0.17.dev20230611/README.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/SECURITY.md` & `GANDLF-0.0.17.dev20230611/SECURITY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/gandlf_anonymizer` & `GANDLF-0.0.17.dev20230611/gandlf_anonymizer`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/gandlf_collectStats` & `GANDLF-0.0.17.dev20230611/gandlf_collectStats`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/gandlf_configGenerator` & `GANDLF-0.0.17.dev20230611/gandlf_configGenerator`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/gandlf_constructCSV` & `GANDLF-0.0.17.dev20230611/gandlf_constructCSV`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/gandlf_deploy` & `GANDLF-0.0.17.dev20230611/gandlf_deploy`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/gandlf_generateMetrics` & `GANDLF-0.0.17.dev20230611/gandlf_generateMetrics`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/gandlf_optimizeModel` & `GANDLF-0.0.17.dev20230611/gandlf_optimizeModel`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         required=True,
     )
     parser.add_argument(
         "-c",
         "--config",
         metavar="",
         type=str,
-        default="",
+        default=None,
+        required=False,
         help="The configuration file (contains all the information related to the training/inference session).",
     )
 
     args = parser.parse_args()
 
     if post_training_model_optimization(args.model, args.config):
         print("Post-training model optimization successful.")
```

### Comparing `GANDLF-0.0.17.dev20230610/gandlf_patchMiner` & `GANDLF-0.0.17.dev20230611/gandlf_patchMiner`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/gandlf_preprocess` & `GANDLF-0.0.17.dev20230611/gandlf_preprocess`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/gandlf_recoverConfig` & `GANDLF-0.0.17.dev20230611/gandlf_recoverConfig`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/gandlf_run` & `GANDLF-0.0.17.dev20230611/gandlf_run`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/gandlf_verifyInstall` & `GANDLF-0.0.17.dev20230611/gandlf_verifyInstall`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230610/setup.py` & `GANDLF-0.0.17.dev20230611/setup.py`

 * *Files identical despite different names*

