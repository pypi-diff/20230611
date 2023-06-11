# Comparing `tmp/Simba-UW-tf-dev-1.62.8.tar.gz` & `tmp/Simba-UW-tf-dev-1.62.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.62.8.tar", last modified: Wed Jun  7 20:12:49 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.62.9.tar", last modified: Sun Jun 11 20:20:37 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.62.8.tar` & `Simba-UW-tf-dev-1.62.9.tar`

### file list

```diff
@@ -1,520 +1,542 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-30 12:37:26.000000 Simba-UW-tf-dev-1.62.8/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.62.8/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.62.8/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.8/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.62.8/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    35432 2023-06-05 18:05:35.000000 Simba-UW-tf-dev-1.62.8/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.62.8/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.62.8/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.62.8/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.62.8/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.62.8/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.62.8/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-06-05 19:45:58.000000 Simba-UW-tf-dev-1.62.8/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/shap_log_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/shap_log_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/read_files_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.62.8/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    38228 2023-06-07 20:11:55.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     9144 2023-05-28 17:30:45.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    73224 2023-06-06 16:32:51.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18514 2023-05-29 20:20:16.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.62.8/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    21017 2023-06-05 18:05:35.000000 Simba-UW-tf-dev-1.62.8/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-05 17:20:50.000000 Simba-UW-tf-dev-1.62.8/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7396 2023-06-01 13:09:55.000000 Simba-UW-tf-dev-1.62.8/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.62.8/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.62.8/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     8585 2023-06-05 17:07:45.000000 Simba-UW-tf-dev-1.62.8/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.62.8/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.62.8/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    17829 2023-05-25 17:48:38.000000 Simba-UW-tf-dev-1.62.8/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.62.8/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.62.8/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.62.8/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.62.8/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.62.8/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-24 20:39:01.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.62.8/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.62.8/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.62.8/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.62.8/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.62.8/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    65549 2023-05-25 18:24:18.000000 Simba-UW-tf-dev-1.62.8/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.62.8/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.62.8/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.62.8/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.62.8/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.62.8/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.62.8/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-06-07 20:12:48.000000 Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    19299 2023-06-07 20:12:48.000000 Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-06-07 20:12:48.000000 Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-06-07 20:12:48.000000 Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-06-07 20:12:48.000000 Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-06-07 20:12:48.000000 Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.62.8/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.62.8/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.62.8/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.62.8/tests/test_distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    12821 2023-06-07 02:40:14.000000 Simba-UW-tf-dev-1.62.8/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.8/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.62.8/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.62.8/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.62.8/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.62.8/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.62.8/tests/test_featurizers.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.8/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/two_c57/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/two_c57/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/two_c57/models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/two_c57/models/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.62.8/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.62.8/tests/test_validation_clips.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.62.8/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.62.8/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-06-07 20:12:47.000000 Simba-UW-tf-dev-1.62.8/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-30 12:37:26.000000 Simba-UW-tf-dev-1.62.9/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.62.9/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.62.9/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.9/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.62.9/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    35432 2023-06-05 18:05:35.000000 Simba-UW-tf-dev-1.62.9/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.62.9/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.62.9/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20688 2023-06-11 20:18:17.000000 Simba-UW-tf-dev-1.62.9/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.62.9/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.62.9/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.62.9/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.9/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.62.9/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.62.9/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.62.9/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.62.9/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.9/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.9/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-06-07 20:13:46.000000 Simba-UW-tf-dev-1.62.9/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/shap_log_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/shap_log_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30770 2023-06-07 20:29:36.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/read_files_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.62.9/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    38228 2023-06-07 20:11:55.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9144 2023-05-28 17:30:45.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    73254 2023-06-07 20:39:22.000000 Simba-UW-tf-dev-1.62.9/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18001 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18559 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.62.9/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21017 2023-06-05 18:05:35.000000 Simba-UW-tf-dev-1.62.9/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-05 17:20:50.000000 Simba-UW-tf-dev-1.62.9/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7396 2023-06-01 13:09:55.000000 Simba-UW-tf-dev-1.62.9/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.62.9/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.62.9/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     8585 2023-06-05 17:07:45.000000 Simba-UW-tf-dev-1.62.9/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.62.9/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.62.9/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    17829 2023-05-25 17:48:38.000000 Simba-UW-tf-dev-1.62.9/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.62.9/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.62.9/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.62.9/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.62.9/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.62.9/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.9/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-24 20:39:01.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.62.9/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.62.9/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.62.9/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.62.9/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.62.9/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.62.9/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.62.9/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.62.9/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.62.9/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.62.9/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.62.9/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.62.9/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.62.9/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.62.9/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.9/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.62.9/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45563 2023-06-09 13:51:45.000000 Simba-UW-tf-dev-1.62.9/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.62.9/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.62.9/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.62.9/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.62.9/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.62.9/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.62.9/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.62.9/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.62.9/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    65762 2023-06-10 19:40:55.000000 Simba-UW-tf-dev-1.62.9/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.62.9/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.62.9/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.62.9/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.62.9/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.62.9/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.62.9/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.62.9/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.9/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    20040 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-06-11 20:20:36.000000 Simba-UW-tf-dev-1.62.9/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.62.9/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.62.9/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.62.9/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.62.9/tests/test_distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.62.9/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.62.9/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.62.9/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.62.9/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.62.9/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.62.9/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8737 2023-06-09 13:54:50.000000 Simba-UW-tf-dev-1.62.9/tests/test_video_processors.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/two_c57/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/two_c57/video_processing/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/two_c57/video_processing/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/two_c57/video_processing/test_imgs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/two_c57/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/two_c57/models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/two_c57/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/two_c57/expected_animal_bp_dict/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/models/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/models/generated_models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/models/validations/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/models/validations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/project_folder/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/project_folder/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/project_folder/videos/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/project_folder/logs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/project_folder/logs/measures/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.62.9/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.62.9/tests/test_validation_clips.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.62.9/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.62.9/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-06-11 20:20:29.000000 Simba-UW-tf-dev-1.62.9/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-11 20:20:37.000000 Simba-UW-tf-dev-1.62.9/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.62.8/PKG-INFO` & `Simba-UW-tf-dev-1.62.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.62.8
+Version: 1.62.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.62.9/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.62.9/simba/labelling/labelling_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,18 +71,16 @@
             self.data_df = read_df(self.targets_inserted_file_path, self.file_type)
             self.data_df_features = read_df(self.features_extracted_file_path, self.file_type)
             missing_idx = self.data_df_features.index.difference(self.data_df.index)
             if len(missing_idx) > 0:
                 self.data_df_features = self.data_df_features.iloc[self.data_df_features.index.difference(self.data_df.index)]
                 self.data_df = pd.concat([self.data_df, self.data_df_features], axis=0).sort_index()
             self.main_window.title('SIMBA ANNOTATION INTERFACE (CONTINUING ANNOTATIONS) - {}'.format(self.video_name))
-            try:
-                self.frm_no = read_config_entry(self.config, 'Last saved frames', self.video_name, data_type='int')
-            except ValueError:
-                pass
+            self.frm_no = read_config_entry(self.config, 'Last saved frames', self.video_name, data_type='int', default_value=0)
+
         else:
             if setting == 'from_scratch':
                 check_file_exist_and_readable(file_path=self.features_extracted_file_path)
                 self.data_df = read_df(self.features_extracted_file_path, self.file_type)
                 self.main_window.title('SIMBA ANNOTATION INTERFACE (ANNOTATING FROM SCRATCH) - {}'.format(self.video_name))
                 for target in self.target_lst:
                     self.data_df[target] = 0
```

### Comparing `Simba-UW-tf-dev-1.62.8/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.62.9/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.62.9/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.62.9/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.62.9/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.62.9/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.62.9/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.62.9/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.62.9/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.62.9/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -740,16 +740,16 @@
 00002e30: 015a 015c 015d 015f 0168 0169 016b 016c  .Z.\.]._.h.i.k.l
 00002e40: 016e 0177 0178 017a 017b 017d 0186 0187  .n.w.x.z.{.}....
 00002e50: 0189 018a 018c 0195 0196 0199 019a 019c  ................
 00002e60: 019d 01a6 01b3 0000 0000 0000 0201 0000  ................
 00002e70: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
 00002e80: 0000 0000 01b4 0000 000c 0075 006e 0073  ...........u.n.s
 00002e90: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
-00002ea0: 0064 6d6f 4444 626c 6f62 0000 0008 fdf7  .dmoDDblob......
-00002eb0: dec3 530f c541 0000 000c 0075 006e 0073  ..S..A.....u.n.s
+00002ea0: 0064 6d6f 4444 626c 6f62 0000 0008 cbf3  .dmoDDblob......
+00002eb0: 6409 d917 c541 0000 000c 0075 006e 0073  d....A.....u.n.s
 00002ec0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
 00002ed0: 0064 6d6f 6444 626c 6f62 0000 0008 fdf7  .dmodDblob......
 00002ee0: dec3 530f c541 0000 000c 0075 006e 0073  ..S..A.....u.n.s
 00002ef0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
 00002f00: 0064 7068 3153 636f 6d70 0000 0000 0004  .dph1Scomp......
 00002f10: d000 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
 00002f20: 0065 0072 0076 0069 0073 0065 0064 7653  .e.r.v.i.s.e.dvS
@@ -1700,71 +1700,71 @@
 00006a30: 4462 6c6f 6200 0000 0854 1422 3e3d 0fc5  Dblob....T.">=..
 00006a40: 4100 0000 0900 6c00 6100 6200 6500 6c00  A.....l.a.b.e.l.
 00006a50: 6c00 6900 6e00 6770 6831 5363 6f6d 7000  l.i.n.gph1Scomp.
 00006a60: 0000 0000 01e0 0000 0000 0900 6c00 6100  ............l.a.
 00006a70: 6200 6500 6c00 6c00 6900 6e00 6776 5372  b.e.l.l.i.n.gvSr
 00006a80: 6e6c 6f6e 6700 0000 0100 0000 0600 6d00  nlong.........m.
 00006a90: 6900 7800 6900 6e00 7362 7773 7062 6c6f  i.x.i.n.sbwspblo
-00006aa0: 6200 0000 ca62 706c 6973 7430 30d7 0102  b....bplist00...
+00006aa0: 6200 0000 c862 706c 6973 7430 30d7 0102  b....bplist00...
 00006ab0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
 00006ac0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
 00006ad0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
 00006ae0: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
 00006af0: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
 00006b00: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
 00006b10: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
-00006b20: 0908 095f 1019 7b7b 3930 372c 2034 3536  ..._..{{907, 456
-00006b30: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
-00006b40: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
-00006b50: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
-00006b60: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
-00006b70: 0000 0600 6d00 6900 7800 6900 6e00 736c  ....m.i.x.i.n.sl
-00006b80: 6731 5363 6f6d 7000 0000 0000 09ff ab00  g1Scomp.........
-00006b90: 0000 0600 6d00 6900 7800 6900 6e00 736c  ....m.i.x.i.n.sl
-00006ba0: 7376 4362 6c6f 6200 0002 8162 706c 6973  svCblob....bplis
-00006bb0: 7430 30d8 0102 0304 0506 0708 090a 0b16  t00.............
-00006bc0: 4647 480a 5f10 1276 6965 774f 7074 696f  FGH._..viewOptio
-00006bd0: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
-00006be0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-00006bf0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-00006c00: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
-00006c10: 5a73 6f72 7443 6f6c 756d 6e58 6963 6f6e  ZsortColumnXicon
-00006c20: 5369 7a65 5f10 1075 7365 5265 6c61 7469  Size_..useRelati
-00006c30: 7665 4461 7465 7310 0109 ab0c 151a 1f23  veDates........#
-00006c40: 282d 3237 3c41 d40d 0e0f 1011 120a 0a5a  (-27<A.........Z
-00006c50: 6964 656e 7469 6669 6572 5577 6964 7468  identifierUwidth
-00006c60: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
-00006c70: 6c65 546e 616d 6511 01c7 0909 d410 0e0f  leTname.........
-00006c80: 0d16 1716 1908 1023 0858 7562 6971 7569  .......#.Xubiqui
-00006c90: 7479 d40d 0e0f 101b 1c16 0a5c 6461 7465  ty.........\date
-00006ca0: 4d6f 6469 6669 6564 10b5 0809 d40d 0e0f  Modified........
-00006cb0: 1020 1c16 165b 6461 7465 4372 6561 7465  . ...[dateCreate
-00006cc0: 6408 08d4 0d0e 0f10 2425 160a 5473 697a  d.......$%..Tsiz
-00006cd0: 6510 6108 09d4 0d0e 0f10 292a 0a0a 546b  e.a.......)*..Tk
-00006ce0: 696e 6410 7309 09d4 0d0e 0f10 2e2f 0a16  ind.s......../..
-00006cf0: 556c 6162 656c 1064 0908 d40d 0e0f 1033  Ulabel.d.......3
-00006d00: 340a 1657 7665 7273 696f 6e10 4b09 08d4  4..Wversion.K...
-00006d10: 0d0e 0f10 3839 0a16 5863 6f6d 6d65 6e74  ....89..Xcomment
-00006d20: 7311 012c 0908 d40d 0e0f 103d 3e16 165e  s..,.......=>..^
-00006d30: 6461 7465 4c61 7374 4f70 656e 6564 10c8  dateLastOpened..
-00006d40: 0808 d410 0e0f 0d16 1c16 4408 0859 6461  ..........D..Yda
-00006d50: 7465 4164 6465 6408 2340 2800 0000 0000  teAdded.#@(.....
-00006d60: 005c 6461 7465 4d6f 6469 6669 6564 2340  .\dateModified#@
-00006d70: 3000 0000 0000 0009 0008 0019 002e 0040  0..............@
-00006d80: 0048 005c 0065 0070 0079 008c 008e 008f  .H.\.e.p.y......
-00006d90: 009b 00a4 00af 00b5 00bf 00c7 00cc 00cf  ................
-00006da0: 00d0 00d1 00da 00db 00dd 00de 00e7 00f0  ................
-00006db0: 00fd 00ff 0100 0101 010a 0116 0117 0118  ................
-00006dc0: 0121 0126 0128 0129 012a 0133 0138 013a  .!.&.(.).*.3.8.:
-00006dd0: 013b 013c 0145 014b 014d 014e 014f 0158  .;.<.E.K.M.N.O.X
-00006de0: 0160 0162 0163 0164 016d 0176 0179 017a  .`.b.c.d.m.v.y.z
-00006df0: 017b 0184 0193 0195 0196 0197 01a0 01a1  .{..............
-00006e00: 01a2 01ac 01ad 01b6 01c3 01cc 0000 0000  ................
-00006e10: 0000 0201 0000 0000 0000 004a 0000 0000  ...........J....
-00006e20: 0000 0000 0000 0000 0000 01cd 4501 4601  ............E.F.
+00006b20: 0908 095f 1017 7b7b 302c 2031 3035 7d2c  ..._..{{0, 105},
+00006b30: 207b 3131 3939 2c20 3736 397d 7d09 0817   {1199, 769}}...
+00006b40: 2531 3d49 606d 797a 7b7c 7d7e 9800 0000  %1=I`myz{|}~....
+00006b50: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
+00006b60: 0000 0000 0000 0000 0000 0000 9900 0000  ................
+00006b70: 0600 6d00 6900 7800 6900 6e00 736c 6731  ..m.i.x.i.n.slg1
+00006b80: 5363 6f6d 7000 0000 0000 0a25 6f00 0000  Scomp......%o...
+00006b90: 0600 6d00 6900 7800 6900 6e00 736c 7376  ..m.i.x.i.n.slsv
+00006ba0: 4362 6c6f 6200 0002 8162 706c 6973 7430  Cblob....bplist0
+00006bb0: 30d8 0102 0304 0506 0708 090a 0b16 4647  0.............FG
+00006bc0: 480a 5f10 1276 6965 774f 7074 696f 6e73  H._..viewOptions
+00006bd0: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
+00006be0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
+00006bf0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
+00006c00: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
+00006c10: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
+00006c20: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
+00006c30: 4461 7465 7310 0109 ab0c 151a 1f23 282d  Dates........#(-
+00006c40: 3237 3c41 d40d 0e0f 1011 120a 0a5a 6964  27<A.........Zid
+00006c50: 656e 7469 6669 6572 5577 6964 7468 5961  entifierUwidthYa
+00006c60: 7363 656e 6469 6e67 5776 6973 6962 6c65  scendingWvisible
+00006c70: 546e 616d 6511 01c7 0909 d410 0e0f 0d16  Tname...........
+00006c80: 1716 1908 1023 0858 7562 6971 7569 7479  .....#.Xubiquity
+00006c90: d40d 0e0f 101b 1c16 0a5c 6461 7465 4d6f  .........\dateMo
+00006ca0: 6469 6669 6564 10b5 0809 d40d 0e0f 1020  dified......... 
+00006cb0: 1c16 165b 6461 7465 4372 6561 7465 6408  ...[dateCreated.
+00006cc0: 08d4 0d0e 0f10 2425 160a 5473 697a 6510  ......$%..Tsize.
+00006cd0: 6108 09d4 0d0e 0f10 292a 0a0a 546b 696e  a.......)*..Tkin
+00006ce0: 6410 7309 09d4 0d0e 0f10 2e2f 0a16 556c  d.s......../..Ul
+00006cf0: 6162 656c 1064 0908 d40d 0e0f 1033 340a  abel.d.......34.
+00006d00: 1657 7665 7273 696f 6e10 4b09 08d4 0d0e  .Wversion.K.....
+00006d10: 0f10 3839 0a16 5863 6f6d 6d65 6e74 7311  ..89..Xcomments.
+00006d20: 012c 0908 d40d 0e0f 103d 3e16 165e 6461  .,.......=>..^da
+00006d30: 7465 4c61 7374 4f70 656e 6564 10c8 0808  teLastOpened....
+00006d40: d410 0e0f 0d16 1c16 4408 0859 6461 7465  ........D..Ydate
+00006d50: 4164 6465 6408 2340 2800 0000 0000 005c  Added.#@(......\
+00006d60: 6461 7465 4d6f 6469 6669 6564 2340 3000  dateModified#@0.
+00006d70: 0000 0000 0009 0008 0019 002e 0040 0048  .............@.H
+00006d80: 005c 0065 0070 0079 008c 008e 008f 009b  .\.e.p.y........
+00006d90: 00a4 00af 00b5 00bf 00c7 00cc 00cf 00d0  ................
+00006da0: 00d1 00da 00db 00dd 00de 00e7 00f0 00fd  ................
+00006db0: 00ff 0100 0101 010a 0116 0117 0118 0121  ...............!
+00006dc0: 0126 0128 0129 012a 0133 0138 013a 013b  .&.(.).*.3.8.:.;
+00006dd0: 013c 0145 014b 014d 014e 014f 0158 0160  .<.E.K.M.N.O.X.`
+00006de0: 0162 0163 0164 016d 0176 0179 017a 017b  .b.c.d.m.v.y.z.{
+00006df0: 0184 0193 0195 0196 0197 01a0 01a1 01a2  ................
+00006e00: 01ac 01ad 01b6 01c3 01cc 0000 0000 0000  ................
+00006e10: 0201 0000 0000 0000 004a 0000 0000 0000  .........J......
+00006e20: 0000 0000 0000 0000 01cd 3c01 4501 4601  ..........<.E.F.
 00006e30: 4801 4901 4f01 5801 5901 5b01 5c01 6401  H.I.O.X.Y.[.\.d.
 00006e40: 6d01 6e01 7101 7201 7b01 8401 8501 8701  m.n.q.r.{.......
 00006e50: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
 00006e60: bb01 c400 0000 0000 0002 0100 0000 0000  ................
 00006e70: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
 00006e80: 0001 c500 0000 0000 0000 0000 0000 0000  ................
 00006e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1788,20 +1788,20 @@
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
-00007020: 626c 6f62 0000 0008 9aa5 fb6f 3817 c541  blob.......o8..A
+00007020: 626c 6f62 0000 0008 7819 b405 8e18 c541  blob....x......A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00007040: 6d6f 6444 626c 6f62 0000 0008 9aa5 fb6f  modDblob.......o
-00007050: 3817 c541 0000 0006 006d 0069 0078 0069  8..A.....m.i.x.i
+00007040: 6d6f 6444 626c 6f62 0000 0008 7819 b405  modDblob....x...
+00007050: 8e18 c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00007070: 000a e000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
+00007070: 000b 0000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
 000070a0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000070d0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000070e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
@@ -1811,15 +1811,15 @@
 00007120: 6261 7208 0809 0809 5f10 187b 7b33 3037  bar....._..{{307
 00007130: 2c20 3836 7d2c 207b 3130 3736 2c20 3632  , 86}, {1076, 62
 00007140: 317d 7d09 0817 2531 3d49 606d 797a 7b7c  1}}...%1=I`myz{|
 00007150: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
 00007160: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
 00007170: 0000 9a00 0000 0500 6d00 6f00 6400 6500  ........m.o.d.e.
 00007180: 6c6c 6731 5363 6f6d 7000 0000 0000 013b  llg1Scomp......;
-00007190: 6b00 0000 0500 6d00 6f00 6400 6500 6c6c  k.....m.o.d.e.ll
+00007190: 3700 0000 0500 6d00 6f00 6400 6500 6c6c  7.....m.o.d.e.ll
 000071a0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
 000071b0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
 000071c0: 4647 0a49 5869 636f 6e53 697a 655f 100f  FG.IXiconSize_..
 000071d0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 000071e0: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
 000071f0: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
 00007200: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
@@ -1893,15 +1893,15 @@
 00007640: 014e 0150 0159 015a 015b 015d 015f 0168  .N.P.Y.Z.[.]._.h
 00007650: 0169 016a 016c 016e 0177 0178 0179 017b  .i.j.l.n.w.x.y.{
 00007660: 017d 0186 0187 0188 018a 018c 0195 0196  .}..............
 00007670: 0197 019a 019c 019d 01a6 01ab 0000 0000  ................
 00007680: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
 00007690: 0000 0000 0000 0000 0000 01ac 0000 0005  ................
 000076a0: 006d 006f 0064 0065 006c 6d6f 4444 626c  .m.o.d.e.lmoDDbl
-000076b0: 6f62 0000 0008 fe1b 754c 3217 c541 0000  ob......uL2..A..
+000076b0: 6f62 0000 0008 574d 2d38 4017 c541 0000  ob....WM-8@..A..
 000076c0: 0005 006d 006f 0064 0065 006c 6d6f 6444  ...m.o.d.e.lmodD
 000076d0: 626c 6f62 0000 0008 fe1b 754c 3217 c541  blob......uL2..A
 000076e0: 0000 0005 006d 006f 0064 0065 006c 7068  .....m.o.d.e.lph
 000076f0: 3153 636f 6d70 0000 0000 0001 7000 0000  1Scomp......p...
 00007700: 0005 006d 006f 0064 0065 006c 7653 726e  ...m.o.d.e.lvSrn
 00007710: 6c6f 6e67 0000 0001 0000 000d 006f 0075  long.........o.u
 00007720: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
@@ -2830,15 +2830,15 @@
 0000b0d0: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
 0000b0e0: 0000 0000 0101 0000 0000 0000 000f 0000  ................
 0000b0f0: 0000 0000 0000 0000 0000 0000 009b 0000  ................
 0000b100: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
 0000b110: 0076 0069 0073 0065 0064 6473 636c 626f  .v.i.s.e.ddsclbo
 0000b120: 6f6c 0000 0000 0c00 7500 6e00 7300 7500  ol......u.n.s.u.
 0000b130: 7000 6500 7200 7600 6900 7300 6500 646c  p.e.r.v.i.s.e.dl
-0000b140: 6731 5363 6f6d 7000 0000 0000 03e8 6c00  g1Scomp.......l.
+0000b140: 6731 5363 6f6d 7000 0000 0000 03e8 6900  g1Scomp.......i.
 0000b150: 0000 0c00 7500 6e00 7300 7500 7000 6500  ....u.n.s.u.p.e.
 0000b160: 7200 7600 6900 7300 6500 646c 7376 4362  r.v.i.s.e.dlsvCb
 0000b170: 6c6f 6200 0002 8162 706c 6973 7430 30d8  lob....bplist00.
 0000b180: 0102 0304 0506 0708 090a 0b18 4647 0a49  ............FG.I
 0000b190: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
 0000b1a0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
 0000b1b0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
@@ -2916,16 +2916,16 @@
 0000b630: 015a 015c 015d 015f 0168 0169 016b 016c  .Z.\.]._.h.i.k.l
 0000b640: 016e 0177 0178 017a 017b 017d 0186 0187  .n.w.x.z.{.}....
 0000b650: 0189 018a 018c 0195 0196 0199 019a 019c  ................
 0000b660: 019d 01a6 01b3 0000 0000 0000 0201 0000  ................
 0000b670: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
 0000b680: 0000 0000 01b4 0000 000c 0075 006e 0073  ...........u.n.s
 0000b690: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
-0000b6a0: 0064 6d6f 4444 626c 6f62 0000 0008 fdf7  .dmoDDblob......
-0000b6b0: dec3 530f c541 0000 000c 0075 006e 0073  ..S..A.....u.n.s
+0000b6a0: 0064 6d6f 4444 626c 6f62 0000 0008 cbf3  .dmoDDblob......
+0000b6b0: 6409 d917 c541 0000 000c 0075 006e 0073  d....A.....u.n.s
 0000b6c0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
 0000b6d0: 0064 6d6f 6444 626c 6f62 0000 0008 fdf7  .dmodDblob......
 0000b6e0: dec3 530f c541 0000 000c 0075 006e 0073  ..S..A.....u.n.s
 0000b6f0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
 0000b700: 0064 7068 3153 636f 6d70 0000 0000 0004  .dph1Scomp......
 0000b710: d000 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
 0000b720: 0065 0072 0076 0069 0073 0065 0064 7653  .e.r.v.i.s.e.dvS
```

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/shap_log_mp_2.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/shap_log_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/shap_log_mp.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/shap_log_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/read_files_mp_2.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/read_files_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 TAIL_BP_NAMES = ['tail']
 CENTER_BP_NAMES = ['trunk1']
 MOUTH = ['head']
 
 ANGULAR_DISPERSION_S = [10, 5, 2, 1, 0.5, 0.25]
 
 class FishFeatureExtractor(ConfigReader, FeatureExtractionMixin):
+    """
+    A class for calculating primarily angular features for single non-shape shifting animals
+    """
     def __init__(self,
                  config_path: str):
 
         ConfigReader.__init__(self, config_path=config_path)
         FeatureExtractionMixin.__init__(self, config_path=config_path)
         self.timer = SimbaTimer()
         self.timer.start_timer()
```

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.62.9/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/requirements.txt` & `Simba-UW-tf-dev-1.62.9/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.62.9/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.62.9/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.62.9/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi` & `Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc` & `Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc` & `Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.62.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.62.9/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.62.9/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.62.9/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.62.9/simba/mixins/train_model_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1223,19 +1223,19 @@
         :param Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
             part of a grid search.
 
         """
         shap_timer = SimbaTimer(start=True)
         data_df = pd.concat([x_df, y_df], axis=1)
         if save_file_no == None:
-            out_df_shap_path = os.path.join(save_path, f'SHAP_values_{clf_name}.csv')
-            out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{clf_name}.csv')
+            self.out_df_shap_path = os.path.join(save_path, f'SHAP_values_{clf_name}.csv')
+            self.out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{clf_name}.csv')
         else:
-            out_df_shap_path = os.path.join(save_path, f'SHAP_values_{str(save_file_no)}_{clf_name}.csv')
-            out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{str(save_file_no)}_{clf_name}.csv')
+            self.out_df_shap_path = os.path.join(save_path, f'SHAP_values_{str(save_file_no)}_{clf_name}.csv')
+            self.out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{str(save_file_no)}_{clf_name}.csv')
         target_df, nontarget_df = data_df[data_df[y_df.name] == 1], data_df[data_df[y_df.name] == 0]
         if len(target_df) < cnt_present:
             NotEnoughDataWarning(msg=f'Train data contains {str(len(target_df))} behavior-present annotations. This is less the number of frames you specified to calculate shap values for {str(cnt_present)}. SimBA will calculate shap scores for the {str(len(target_df))} behavior-present frames available')
             cnt_present = len(target_df)
         if len(nontarget_df) < cnt_absent:
             NotEnoughDataWarning(msg=f'Train data contains {str(len(nontarget_df))} behavior-absent annotations. This is less the number of frames you specified to calculate shap values for {str(cnt_absent)}. SimBA will calculate shap scores for the {str(len(target_df))} behavior-absent frames available')
             cnt_absent = len(nontarget_df)
@@ -1263,16 +1263,16 @@
                     shap_sum = np.sum(result[0], axis=1).reshape(-1, 1)
                     shap_results.append(np.hstack((result[0], np.full((result[0].shape[0]), expected_value).reshape(-1, 1), shap_sum, proba, result[2])))
                     shap_raw.append(result[1])
             pool.terminate()
             pool.join()
             shap_save_df = pd.DataFrame(data=np.row_stack(shap_results),columns=list(x_names) + ['Expected_value', 'Sum', 'Prediction_probability', clf_name])
             raw_save_df = pd.DataFrame(data=np.row_stack(shap_raw), columns=list(x_names))
-            shap_save_df.to_csv(out_df_shap_path)
-            raw_save_df.to_csv(out_df_raw_path)
+            shap_save_df.to_csv(self.out_df_shap_path)
+            raw_save_df.to_csv(self.out_df_raw_path)
             shap_timer.stop_timer()
             stdout_success(msg='SHAP calculations complete', elapsed_time=shap_timer.elapsed_time_str)
             _ = ShapAggregateStatisticsVisualizer(config_path=ini_file_path,
                                                   classifier_name=clf_name,
                                                   shap_df=shap_save_df,
                                                   shap_baseline_value=int(expected_value * 100),
                                                   save_path=save_path)
```

### Comparing `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = "Simon Nilsson"
+__author__ = "Simon Nilsson / Florian Duclot"
 
 import pandas as pd
 from copy import deepcopy
 import os, glob
 from simba.mixins.config_reader import ConfigReader
 from simba.third_party_label_appenders.tools import is_new_boris_version
 from simba.utils.read_write import get_fn_ext, read_df, write_df
@@ -20,15 +20,16 @@
     Append BORIS human annotations onto featurized pose-estimation data.
 
     :param str config_path: path to SimBA project config file in Configparser format
     :param str data_dir: path to folder holding BORIS data files is CSV format
 
     .. note::
        `Third-party import tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot.md>`__.
-       `Example BORIS input file <https://github.com/sgoldenlab/simba/blob/master/misc/boris_example.csv>`_.
+       `Example I BORIS input file <https://github.com/sgoldenlab/simba/blob/master/misc/boris_example.csv>`_.
+       `Example II BORIS input file <https://github.com/sgoldenlab/simba/blob/master/misc/boris_new_example.csv>`_.
 
     Examples
     ----------
     >>> boris_appender = BorisAppender(config_path='MyProjectConfigPath', data_dir=r'BorisDataFolder')
     >>> boris_appender.create_boris_master_file()
     >>> boris_appender.run()
```

### Comparing `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__author__ = "Simon Nilsson / Florian Duclot"
+
 import pandas as pd
 import numpy as np
 from typing import List, Dict
 from simba.utils.data import detect_bouts
 from simba.utils.read_write import get_fn_ext, read_video_info
 from simba.utils.enums import Methods
 from simba.utils.warnings import ThirdPartyAnnotationsInvalidFileFormatWarning
```

### Comparing `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/third_party_appender.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import pandas as pd
-
+__author__ = "Simon Nilsson / Florian Duclot"
 
+import pandas as pd
 from simba.utils.enums import Methods
 import os, glob
 from copy import deepcopy
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.read_write import read_df, write_df, get_fn_ext
 from simba.utils.checks import check_if_filepath_list_is_empty, check_if_dir_exists
 from simba.utils.printing import stdout_success
```

### Comparing `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.62.9/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.62.9/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.62.9/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/utils/enums.py` & `Simba-UW-tf-dev-1.62.9/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.62.9/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/utils/checks.py` & `Simba-UW-tf-dev-1.62.9/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.62.9/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.62.9/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.62.9/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/utils/errors.py` & `Simba-UW-tf-dev-1.62.9/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/utils/data.py` & `Simba-UW-tf-dev-1.62.9/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/utils/printing.py` & `Simba-UW-tf-dev-1.62.9/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.62.9/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.62.9/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.62.9/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.62.9/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.62.9/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.62.9/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.62.9/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.62.9/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.62.9/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.62.9/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.62.9/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.62.9/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.62.9/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.62.9/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.62.9/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.62.9/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.62.9/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.62.9/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.62.9/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.62.9/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.62.9/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.62.9/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.62.9/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.62.9/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.62.9/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.62.9/simba/video_processors/video_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -656,15 +656,15 @@
                        horizontal: bool) -> None:
 
     """
     Concatenate two videos to a single video
 
     :param str video_one_path: Path to the first video in the concatenated video
     :param str video_two_path: Path to the second video in the concatenated video
-    :param int or str resolution: If str, then the name of the video which resolution you want to retain. E.g., `Video_1`. Else int, representinmg the video width (if vertical concat) or height (if horizontal concat). Aspect raio will be retained.
+    :param int or str resolution: If str, then the name of the video which resolution you want to retain. E.g., `Video_1`. Else int, representing the video width (if vertical concat) or height (if horizontal concat). Aspect raio will be retained.
     :param horizontal: If true, then horizontal concatenation. Else vertical concatenation.
 
     :example:
     >>> video_concatenator(video_one_path='project_folder/videos/Video_1.mp4', video_two_path='project_folder/videos/Video_2.mp4', resolution=800, horizontal=True)
     """
```

### Comparing `Simba-UW-tf-dev-1.62.8/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.62.9/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.62.9/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.62.9/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.62.9/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.62.9/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.62.9/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.62.9/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.62.9/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.62.9/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.62.9/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.62.9/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/SimBA.py` & `Simba-UW-tf-dev-1.62.9/simba/SimBA.py`

 * *Files 0% similar despite different names*

```diff
@@ -675,20 +675,21 @@
 
     def run_feature_extraction(self):
         print(f'Pose-estimation body part setting for feature extraction: {str(self.animal_cnt)} animals {str(self.pose_setting)} body-parts')
         feature_extractor_classes = get_bp_config_code_class_pairs()
         if self.user_defined_var.get():
             _ = run_user_defined_feature_extraction_class(file_path=self.scriptfile.file_path,
                                                           config_path=self.config_path)
+        if self.pose_setting not in feature_extractor_classes.keys():
+            raise InvalidInputError(msg=f'The project pose-configuration key is set to {self.pose_setting} which is invalid. OPTIONS: {list(feature_extractor_classes.keys())}')
+        if self.pose_setting == '8':
+            feature_extractor = feature_extractor_classes[self.pose_setting][self.animal_cnt](config_path=self.config_path)
         else:
-            if self.pose_setting == '8':
-                feature_extractor = feature_extractor_classes[self.pose_setting][self.animal_cnt](config_path=self.config_path)
-            else:
-                feature_extractor = feature_extractor_classes[self.pose_setting](config_path=self.config_path)
-            feature_extractor.run()
+            feature_extractor = feature_extractor_classes[self.pose_setting](config_path=self.config_path)
+        feature_extractor.run()
 
     def set_distance_mm(self):
         check_int(name='DISTANCE IN MILLIMETER', value=self.distance_in_mm_eb.entry_get, min_value=1)
         self.config.set('Frame settings', 'distance_mm', self.distance_in_mm_eb.entry_get)
         with open(self.config_path, 'w') as f:
             self.config.write(f)
```

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.62.9/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.62.9/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.62.9/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.62.9/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.62.9/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.62.9/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.62.9/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.62.9/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.62.9/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.62.9/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.62.9/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.62.9/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.62.9/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.62.9/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.62.9/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.62.9/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.62.9/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.62.9/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.62.8
+Version: 1.62.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.62.9/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -160,14 +160,15 @@
 simba/feature_extractors/.idea/features_scripts.iml
 simba/feature_extractors/.idea/misc.xml
 simba/feature_extractors/.idea/modules.xml
 simba/feature_extractors/.idea/workspace.xml
 simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
 simba/feature_extractors/.idea/libraries/R_User_Library.xml
 simba/feature_extractors/misc/.DS_Store
+simba/feature_extractors/misc/__init__.py
 simba/feature_extractors/misc/add_probability_cnt_features.py
 simba/feature_extractors/misc/convex_hull_3_scratch_3.py
 simba/feature_extractors/misc/convex_hull_scratch_1.py
 simba/feature_extractors/misc/convex_hull_scratch_2.py
 simba/feature_extractors/misc/count_values_in_range.py
 simba/feature_extractors/misc/doctests.py
 simba/feature_extractors/misc/egocentrical_aligner.py
@@ -443,16 +444,27 @@
 tests/test_distance_plotter.py
 tests/test_feature_extraction_mixin.py
 tests/test_featurizers.py
 tests/test_outlier_correctors.py
 tests/test_thirdparty_appenders.py
 tests/test_train_model_mixin.py
 tests/test_validation_clips.py
+tests/test_video_processors.py
 tests/test_visualize_directing_animals.py
 tests/data/__init__.py
 tests/data/test_projects/__init__.py
 tests/data/test_projects/mouse_open_field/__init__.py
 tests/data/test_projects/two_c57/__init__.py
+tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
 tests/data/test_projects/two_c57/models/__init__.py
+tests/data/test_projects/two_c57/video_processing/__init__.py
+tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
 tests/data/test_projects/zebrafish/__init__.py
 tests/data/test_projects/zebrafish/feature_file/__init__.py
-tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+tests/data/test_projects/zebrafish/models/__init__.py
+tests/data/test_projects/zebrafish/models/generated_models/__init__.py
+tests/data/test_projects/zebrafish/models/validations/__init__.py
+tests/data/test_projects/zebrafish/project_folder/__init__.py
+tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
+tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
+tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
```

### Comparing `Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.62.9/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/LICENSE.md` & `Simba-UW-tf-dev-1.62.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.62.9/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/tests/test_distance_plotter.py` & `Simba-UW-tf-dev-1.62.9/tests/test_distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.62.9/tests/test_train_model_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,22 +175,14 @@
 @pytest.mark.parametrize("data_dir", ['/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/project_folder/csv/targets_inserted'])
 def test_read_all_files_in_folder_mp(data_dir):
     file_paths = glob.glob(data_dir + '/*.csv')
     data = TrainModelMixin().read_all_files_in_folder_mp(file_paths=file_paths, file_type='csv', classifier_names=['Attack', 'Sniffing'])
     assert len(data) == 1738
     assert len(data.columns) == 52
 
-@pytest.mark.parametrize("data_dir", ['/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/project_folder/csv/targets_inserted'])
-def test_read_all_files_in_folder_mp(data_dir):
-    file_paths = glob.glob(data_dir + '/*.csv')
-    data = TrainModelMixin().read_all_files_in_folder_mp(file_paths=file_paths, file_type='csv', classifier_names=['Attack', 'Sniffing'])
-    assert len(data) == 1738
-    assert len(data.columns) == 52
-
-
 @pytest.mark.parametrize("config_path, clf_path", [['/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/project_folder/project_config.ini',
                                                    '/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/models/generated_models/Attack.sav']])
 def test_create_shap_log_mp(config_path, clf_path):
     x, y = pd.DataFrame(np.random.randint(1, 10, size=(500, 2))), pd.Series(np.random.randint(0, 2, size=(500)), name='target')
     clf = read_df(file_path=clf_path, file_type='pickle')
     train_model_mixin = TrainModelMixin()
     train_model_mixin.create_shap_log_mp(ini_file_path=config_path,
```

### Comparing `Simba-UW-tf-dev-1.62.8/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.62.9/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.62.9/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.62.9/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.62.9/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.62.9/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.62.9/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.62.9/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.62.9/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/README.md` & `Simba-UW-tf-dev-1.62.9/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.8/setup.py` & `Simba-UW-tf-dev-1.62.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.62.8",
+    version="1.62.9",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

