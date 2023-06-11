# Comparing `tmp/apysc-2.8.6.tar.gz` & `tmp/apysc-2.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apysc-2.8.6.tar", last modified: Sun Jun  4 12:27:49 2023, max compression
+gzip compressed data, was "apysc-2.8.7.tar", last modified: Sun Jun 11 10:59:41 2023, max compression
```

## Comparing `apysc-2.8.6.tar` & `apysc-2.8.7.tar`

### file list

```diff
@@ -1,678 +1,682 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.394715 apysc-2.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-04 12:27:26.000000 apysc-2.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 12:27:26.000000 apysc-2.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-04 12:27:49.394715 apysc-2.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-04 12:27:26.000000 apysc-2.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.334715 apysc-2.8.6/apysc/
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.342715 apysc-2.8.6/apysc/_animation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_cx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_cx_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_cy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_cy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_finish_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_height.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_height_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_height_for_ellipse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_line_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_move.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_move_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_parallel_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_pause_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_play_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_radius_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_reset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_reverse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_rotation_around_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_rotation_around_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_scale_x_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_scale_x_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_scale_x_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_scale_x_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_scale_y_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_scale_y_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_scale_y_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_scale_y_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_time_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_width.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_width_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_width_for_ellipse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/animation_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_animation/easing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.342715 apysc-2.8.6/apysc/_auto_reloading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_auto_reloading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_auto_reloading/auto_reloading_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.342715 apysc-2.8.6/apysc/_branch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_branch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_branch/_elif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_branch/_else.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_branch/_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_branch/if_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.342715 apysc-2.8.6/apysc/_callable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_callable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_callable/callable_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.346715 apysc-2.8.6/apysc/_chart/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/add_background_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/add_border_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/axis_label_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/axis_label_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/axis_label_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/axis_label_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/axis_label_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/axis_label_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/axis_line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/axis_line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/axis_line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/background_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/border_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/chart_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/chart_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    20016 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/create_single_column_y_axis_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/initialize_each_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/is_display_axis_label_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/overall_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/set_initial_background_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/set_initial_background_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/set_initial_border_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/set_initial_border_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/set_initial_border_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/set_initial_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/set_initial_horizontal_padding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/set_initial_matrix_data_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/set_initial_overall_container_coordinates_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/set_initial_vertical_padding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/set_initial_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/set_initial_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/set_initial_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/tick_max_num_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/tick_text_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/tick_text_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/tick_text_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/tick_text_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/tick_text_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/tick_text_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/vertical_bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/x_axis_column_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/x_axis_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/x_axis_label_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/x_axis_label_position_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/x_axis_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/y_axis_column_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/y_axis_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/y_axis_label_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/y_axis_label_position_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/y_axis_single_column_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/y_max_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_chart/y_min_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.346715 apysc-2.8.6/apysc/_color/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_color/color_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.346715 apysc-2.8.6/apysc/_console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_console/_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    31274 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_console/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_console/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.346715 apysc-2.8.6/apysc/_converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_converter/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_converter/to_apysc_val_from_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_converter/to_builtin_val_from_apysc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.358715 apysc-2.8.6/apysc/_display/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/_document.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/any_display_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/append_fill_alpha_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/append_fill_color_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/append_line_alpha_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/append_line_cap_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/append_line_color_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/append_line_joints_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/append_line_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/append_line_thickness_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/append_x_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/append_y_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/begin_fill_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/child_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16493 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/css_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/cx_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/cy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/display_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    16425 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/ellipse_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/ellipse_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/flip_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/flip_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/flip_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/get_bounds_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    47941 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/graphics_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/graphics_clear_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/graphics_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_cap_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_caps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_dash_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_dash_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_dash_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_dash_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_joints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_joints_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_round_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_round_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_style_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/parent_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17638 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/points_2d_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/points_var_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/polygon_append_constructor_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/polygon_apply_current_points_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/polygon_x1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/polygon_x2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/polygon_x3_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/polygon_y1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/polygon_y2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/polygon_y3_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16471 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/radius_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18581 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/rotation_around_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/rotation_around_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/rotation_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/scale_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/scale_x_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/scale_x_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/scale_y_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/scale_y_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/set_lower_scale_limit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/set_overflow_visible_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/skew_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/skew_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/sprite.py
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_align_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_delta_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_delta_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_leading_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_set_align_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_set_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_set_delta_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_set_delta_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_set_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_set_font_size_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_set_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_set_leading_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_set_text_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_singleton_for_text_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16394 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/svg_text_text_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/visible_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/width_and_height_mixin_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/x_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/y_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_display/y_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.358715 apysc-2.8.6/apysc/_event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/animation_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/click_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/custom_event_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/custom_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/document_mouse_wheel_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/double_click_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/enter_frame_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/enter_frame_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/handler_circular_calling_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/mouse_down_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/mouse_event_binding_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/mouse_event_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/mouse_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/mouse_event_unbinding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/mouse_move_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/mouse_out_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/mouse_over_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/mouse_up_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/prevent_default_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/set_handler_data_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/stop_propagation_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/timer_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_event/wheel_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.362715 apysc-2.8.6/apysc/_expression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_expression/event_handler_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_expression/expression_data_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_expression/expression_variables_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_expression/get_last_scope_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_expression/indent_num.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_expression/js_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_expression/last_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_expression/var_names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.362715 apysc-2.8.6/apysc/_file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_file/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_file/module_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.362715 apysc-2.8.6/apysc/_geom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_bezier_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_bezier_2d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_bezier_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_bezier_3d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_close.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_control_x1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_control_x2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_control_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_control_y1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_control_y2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_control_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_data_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_data_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_dest_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_dest_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_line_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_move_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_vertical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/path_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/point2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/rectangle_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/rectangle_geom_bottom_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/rectangle_geom_center_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/rectangle_geom_center_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/rectangle_geom_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/rectangle_geom_left_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/rectangle_geom_right_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/rectangle_geom_top_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/rectangle_geom_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_geom/relative_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.366715 apysc-2.8.6/apysc/_html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14536 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_html/debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_html/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_html/html_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_html/html_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.366715 apysc-2.8.6/apysc/_jslib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_jslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    89947 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_jslib/jquery-3.6.3.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_jslib/jquery.mousewheel-3.1.13.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_jslib/jslib_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    78572 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_jslib/svg-3.1.2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19431 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_jslib/underscore-1.12.0.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.366715 apysc-2.8.6/apysc/_jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_jupyter/jupyter_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.366715 apysc-2.8.6/apysc/_lint_and_doc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/conf_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/docs_keyword_link_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/docs_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/docs_toctree_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/docs_translation_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/docstring_to_markdown_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    51969 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/docstring_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/document_text_split_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/document_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.366715 apysc-2.8.6/apysc/_lint_and_doc/fixed_translation_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   214301 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/fixed_translation_mapping/jp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/lint_and_doc_hash_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_lint_and_doc/translation_mapping_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.366715 apysc-2.8.6/apysc/_loop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_loop/_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_loop/_for.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_loop/_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_loop/for_array_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_loop/for_loop_exit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_loop/loop_count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.366715 apysc-2.8.6/apysc/_math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_math/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_math/max_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_math/min_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_math/trunc_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.366715 apysc-2.8.6/apysc/_string/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_string/indent_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_string/string_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.370715 apysc-2.8.6/apysc/_testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_testing/e2e_testing_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_testing/testing_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.370715 apysc-2.8.6/apysc/_time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10869 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/datetime_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/day_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/days_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/fps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/hour_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/left_and_right_datetimes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/millisecond_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/minute_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/month_end_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/month_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/now_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/second_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/timedelta_.py
--rw-r--r--   0 runner    (1001) docker     (123)    22201 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/total_seconds_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/weekday_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_time/year_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.370715 apysc-2.8.6/apysc/_translation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.390715 apysc-2.8.6/apysc/_translation/jp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/about_handler_options_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/add_child_and_remove_child.py
--rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/add_debug_info_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_base_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_base_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_finish.py
--rw-r--r--   0 runner    (1001) docker     (123)   143972 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_interfaces_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_line_color.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_method_chaining.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_move.py
--rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_pause_and_play.py
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_return_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    22568 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_scale_x_and_y_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_scale_x_and_y_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_width_and_height.py
--rw-r--r--   0 runner    (1001) docker     (123)    12950 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_x.py
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/animation_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/append_js_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/array_append_and_push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/array_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/array_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/array_extend_and_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/array_index_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/array_insert_and_insert_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/array_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/array_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/array_pop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/array_remove_and_remove_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/array_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/array_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/array_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    16036 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/assert_defined_and_undefined.py
--rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/assert_equal_and_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/assert_greater_and_greater_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/assert_less_and_less_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/assert_true_and_false.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/assertion_basic_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)    25457 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/bind_and_trigger_custom_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    47227 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/contains.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/continue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/datetime_day.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/datetime_hour.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/datetime_millisecond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/datetime_minute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/datetime_month.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/datetime_now.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/datetime_second.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/datetime_set_month_end.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/datetime_year.py
--rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/dblclick.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/dictionary_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/dictionary_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/dictionary_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/display_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/display_object_get_and_set_css.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/display_object_mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/display_object_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/display_object_visible.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/display_object_x_and_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/display_on_colaboratory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/display_on_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/draw_interfaces_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    84469 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/easing_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/elif.py
--rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/else.py
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/enter_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/for.py
--rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/for_array_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/fps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/fundamental_data_classes_value_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/get_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/get_child_at.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_flip_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_line_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_line_dash_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_line_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_line_round_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    15869 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_scale_from_center.py
--rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_scale_from_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_base_skew.py
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_begin_fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_draw_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_draw_dash_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_draw_dashed_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_draw_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_draw_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_draw_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_draw_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_draw_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_draw_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_draw_round_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_draw_round_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_draw_triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    62521 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_line_style.py
--rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/graphics_move_to_and_line_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/if.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/import_conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19101 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/int_and_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/int_and_number_arithmetic_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/int_and_number_comparison_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/int_and_number_to_fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/math_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/math_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/math_trunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/mouse_event_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/mouse_event_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    27457 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/mousedown_and_mouseup.py
--rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/mousemove.py
--rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/mouseover_and_mouseout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/num_children.py
--rw-r--r--   0 runner    (1001) docker     (123)    60597 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/path_bezier_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/path_bezier_2d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/path_bezier_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/path_bezier_3d_continual.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/path_close.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/path_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/path_line_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/path_move_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/path_vertical.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/point2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    49410 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    51647 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/quick_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/recommended_type_checker_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    51967 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/rectangle_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/remove_children.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/return.py
--rw-r--r--   0 runner    (1001) docker     (123)    17192 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/save_overall_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/sequential_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/set_debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/sprite.py
--rw-r--r--   0 runner    (1001) docker     (123)    30948 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/string_addition_and_multiplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/string_comparison_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/string_lstrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/string_rstrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/string_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/string_strip.py
--rw-r--r--   0 runner    (1001) docker     (123)    47748 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/svg_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    44504 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/svg_text_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/timedelta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/timedelta_days.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/timedelta_total_seconds.py
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/timer_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)    17095 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/timer_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/timer_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/timer_repeat_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/timer_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/timer_start_and_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/to_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    64293 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    14259 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/unset_debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/variable_name_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/what_apysc_can_do.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.394715 apysc-2.8.6/apysc/_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/_return.py
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/any_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    45467 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/attr_linking_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/blank_object_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16294 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/copy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/deleted_object_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    23069 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/dictionary_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/expression_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/initial_substitution_exp_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/number.py
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/number_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/py_builtin_iter_disabling_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/repr_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/revert_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/revert_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    26625 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/string_lstrip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/string_rstrip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/string_split_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/string_strip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/to_fixed_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/to_string_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/type_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/type_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/value_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/variable_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/variable_name_suffix_attr_or_var_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/variable_name_suffix_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_type/variable_name_suffix_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.394715 apysc-2.8.6/apysc/_validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   106002 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/arg_validation_decos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/bool_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/color_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/display_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/event_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/geom_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/matrix_data_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/number_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/parent_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/path_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/string_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/validation_common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-04 12:27:26.000000 apysc-2.8.6/apysc/_validation/variable_name_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:27:49.338715 apysc-2.8.6/apysc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-04 12:27:49.000000 apysc-2.8.6/apysc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25358 2023-06-04 12:27:49.000000 apysc-2.8.6/apysc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:27:49.000000 apysc-2.8.6/apysc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-04 12:27:49.000000 apysc-2.8.6/apysc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 12:27:49.000000 apysc-2.8.6/apysc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 12:27:49.394715 apysc-2.8.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.593850 apysc-2.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-11 10:59:23.000000 apysc-2.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-11 10:59:23.000000 apysc-2.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-11 10:59:41.593850 apysc-2.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-11 10:59:23.000000 apysc-2.8.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.537850 apysc-2.8.7/apysc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.541850 apysc-2.8.7/apysc/_animation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_cx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_cx_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_cy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_cy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_finish_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_height.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_height_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_height_for_ellipse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_move_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_parallel_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_pause_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_play_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_radius_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_reset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_reverse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_rotation_around_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_rotation_around_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_scale_x_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_scale_x_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_scale_x_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_scale_x_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_scale_y_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_scale_y_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_scale_y_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_scale_y_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_time_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_width.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_width_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_width_for_ellipse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/animation_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_animation/easing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.541850 apysc-2.8.7/apysc/_auto_reloading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_auto_reloading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_auto_reloading/auto_reloading_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.541850 apysc-2.8.7/apysc/_branch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_branch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_branch/_elif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_branch/_else.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_branch/_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_branch/if_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.541850 apysc-2.8.7/apysc/_callable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_callable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_callable/callable_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.545850 apysc-2.8.7/apysc/_chart/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/add_background_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/add_border_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/axis_label_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/axis_label_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/axis_label_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/axis_label_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/axis_label_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/axis_label_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/axis_line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/axis_line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/axis_line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/background_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/border_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/chart_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/chart_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20016 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/create_single_column_y_axis_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/initialize_each_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/is_display_axis_label_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/overall_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/set_initial_background_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/set_initial_background_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/set_initial_border_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/set_initial_border_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/set_initial_border_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/set_initial_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/set_initial_horizontal_padding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/set_initial_matrix_data_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/set_initial_overall_container_coordinates_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/set_initial_vertical_padding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/set_initial_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/set_initial_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/set_initial_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/tick_max_num_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/tick_text_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/tick_text_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/tick_text_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/tick_text_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/tick_text_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/tick_text_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/vertical_bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/x_axis_column_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/x_axis_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/x_axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/x_axis_label_position_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/x_axis_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/y_axis_column_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/y_axis_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/y_axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/y_axis_label_position_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/y_axis_single_column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/y_max_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_chart/y_min_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.545850 apysc-2.8.7/apysc/_color/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_color/color_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.545850 apysc-2.8.7/apysc/_console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_console/_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31274 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_console/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_console/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.545850 apysc-2.8.7/apysc/_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_converter/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_converter/to_apysc_val_from_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_converter/to_builtin_val_from_apysc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.557850 apysc-2.8.7/apysc/_display/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/any_display_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/append_fill_alpha_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/append_fill_color_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/append_line_alpha_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/append_line_cap_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/append_line_color_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/append_line_joints_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/append_line_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/append_line_thickness_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/append_x_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/append_y_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/begin_fill_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15386 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/child_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/css_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/cx_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/cy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/display_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/ellipse_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/ellipse_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/flip_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/flip_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/flip_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/get_bounds_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48567 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/graphics_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/graphics_clear_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/graphics_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15548 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_cap_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_caps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_dash_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_dash_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_dash_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_dash_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_joints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_joints_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_round_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_round_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_style_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/parent_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18308 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/points_2d_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/points_var_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/polygon_append_constructor_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/polygon_apply_current_points_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/polygon_x1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/polygon_x2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/polygon_x3_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/polygon_y1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/polygon_y2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/polygon_y3_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17155 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/radius_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19181 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/rotation_around_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/rotation_around_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/rotation_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/scale_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/scale_x_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/scale_x_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/scale_y_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/scale_y_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/set_lower_scale_limit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/set_overflow_visible_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/skew_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/skew_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22626 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_align_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_delta_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_delta_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_leading_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_set_align_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_set_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_set_delta_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_set_delta_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_set_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_set_font_size_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_set_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_set_leading_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_set_text_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_singleton_for_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/svg_text_text_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17486 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/visible_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/width_and_height_mixin_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/x_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/y_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_display/y_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.561850 apysc-2.8.7/apysc/_event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/animation_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/click_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/custom_event_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/custom_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/document_mouse_wheel_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/double_click_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/enter_frame_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/enter_frame_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/handler_circular_calling_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/mouse_down_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/mouse_event_binding_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/mouse_event_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/mouse_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/mouse_event_unbinding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/mouse_move_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/mouse_out_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/mouse_over_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/mouse_up_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/prevent_default_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/set_handler_data_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/stop_propagation_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/timer_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_event/wheel_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.561850 apysc-2.8.7/apysc/_expression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_expression/event_handler_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_expression/expression_data_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_expression/expression_variables_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_expression/get_last_scope_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_expression/indent_num.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_expression/js_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_expression/last_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_expression/var_names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.561850 apysc-2.8.7/apysc/_file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_file/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_file/module_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.565850 apysc-2.8.7/apysc/_geom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_bezier_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_bezier_2d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_bezier_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_bezier_3d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_close.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_control_x1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_control_x2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_control_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_control_y1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_control_y2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_control_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_data_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_dest_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_dest_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_move_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/path_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/rectangle_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/rectangle_geom_bottom_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/rectangle_geom_center_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/rectangle_geom_center_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/rectangle_geom_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/rectangle_geom_left_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/rectangle_geom_right_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/rectangle_geom_top_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/rectangle_geom_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_geom/relative_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.565850 apysc-2.8.7/apysc/_html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14536 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_html/debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_html/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_html/html_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_html/html_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.565850 apysc-2.8.7/apysc/_jslib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_jslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89947 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_jslib/jquery-3.6.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_jslib/jquery.mousewheel-3.1.13.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_jslib/jslib_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78572 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_jslib/svg-3.1.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19431 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_jslib/underscore-1.12.0.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.565850 apysc-2.8.7/apysc/_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_jupyter/jupyter_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.565850 apysc-2.8.7/apysc/_lint_and_doc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/conf_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/docs_keyword_link_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/docs_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/docs_toctree_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/docs_translation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/docstring_to_markdown_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51969 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/docstring_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/document_text_split_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/document_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.565850 apysc-2.8.7/apysc/_lint_and_doc/fixed_translation_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   214930 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/fixed_translation_mapping/jp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/lint_and_doc_hash_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_lint_and_doc/translation_mapping_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.569850 apysc-2.8.7/apysc/_loop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_loop/_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_loop/_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_loop/_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_loop/for_array_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_loop/for_array_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_loop/for_loop_exit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_loop/initialize_for_loop_value_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_loop/loop_count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.569850 apysc-2.8.7/apysc/_math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_math/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_math/max_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_math/min_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_math/trunc_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.569850 apysc-2.8.7/apysc/_string/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_string/indent_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_string/string_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.569850 apysc-2.8.7/apysc/_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_testing/e2e_testing_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_testing/testing_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.569850 apysc-2.8.7/apysc/_time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10869 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/datetime_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/day_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/days_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/fps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/hour_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/left_and_right_datetimes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/millisecond_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/minute_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/month_end_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/month_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/now_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/second_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/timedelta_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22201 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/total_seconds_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/weekday_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_time/year_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.569850 apysc-2.8.7/apysc/_translation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.589850 apysc-2.8.7/apysc/_translation/jp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/about_handler_options_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/add_child_and_remove_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/add_debug_info_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_base_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_base_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143972 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_interfaces_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_method_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_pause_and_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_return_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22568 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_scale_x_and_y_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_scale_x_and_y_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_width_and_height.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12950 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/animation_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/append_js_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/array_append_and_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/array_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/array_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/array_extend_and_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/array_index_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/array_insert_and_insert_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/array_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/array_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/array_pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/array_remove_and_remove_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/array_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/array_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/array_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16036 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/assert_defined_and_undefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/assert_equal_and_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/assert_greater_and_greater_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/assert_less_and_less_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/assert_true_and_false.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/assertion_basic_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25457 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/bind_and_trigger_custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47227 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/contains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/datetime_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/datetime_hour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/datetime_millisecond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/datetime_minute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/datetime_month.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/datetime_now.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/datetime_second.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/datetime_set_month_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/datetime_year.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/dblclick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/dictionary_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/dictionary_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/dictionary_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/display_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/display_object_get_and_set_css.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/display_object_mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/display_object_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/display_object_visible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/display_object_x_and_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/display_on_colaboratory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/display_on_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/draw_interfaces_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84469 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/easing_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/elif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/else.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/enter_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/for.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/for_array_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/for_array_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/fps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/fundamental_data_classes_value_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/get_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/get_child_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_flip_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_line_dash_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_line_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_line_round_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15869 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_scale_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_scale_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_base_skew.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_begin_fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_draw_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_draw_dash_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_draw_dashed_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_draw_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_draw_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_draw_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_draw_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_draw_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_draw_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_draw_round_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_draw_round_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_draw_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62521 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_line_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/graphics_move_to_and_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/import_conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/int_and_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/int_and_number_arithmetic_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/int_and_number_comparison_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/int_and_number_to_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/math_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/math_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/math_trunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/mouse_event_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/mouse_event_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27457 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/mousedown_and_mouseup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/mousemove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/mouseover_and_mouseout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/num_children.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60597 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/path_bezier_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/path_bezier_2d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/path_bezier_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/path_bezier_3d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/path_close.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/path_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/path_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/path_move_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/path_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49410 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51647 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/quick_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/recommended_type_checker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51967 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/rectangle_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/remove_children.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/return.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17192 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/save_overall_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/sequential_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/set_debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30948 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/string_addition_and_multiplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/string_comparison_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/string_lstrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/string_rstrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/string_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/string_strip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47748 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/svg_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44504 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/svg_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/timedelta_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/timedelta_total_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/timer_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17095 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/timer_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/timer_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/timer_repeat_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/timer_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/timer_start_and_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/to_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64293 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14259 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/unset_debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/variable_name_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/what_apysc_can_do.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.593850 apysc-2.8.7/apysc/_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/any_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45902 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/attr_linking_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/blank_object_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/copy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/deleted_object_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23523 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/dictionary_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/expression_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/initial_substitution_exp_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/initialize_locals_and_globals_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34251 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/number_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/py_builtin_iter_disabling_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/repr_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/revert_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/revert_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27064 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/string_lstrip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/string_rstrip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/string_split_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/string_strip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/to_fixed_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/to_string_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/type_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/value_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/variable_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/variable_name_suffix_attr_or_var_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/variable_name_suffix_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_type/variable_name_suffix_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.593850 apysc-2.8.7/apysc/_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107700 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/arg_validation_decos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/bool_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/color_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/display_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/event_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/geom_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/matrix_data_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/number_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/parent_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/path_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/string_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/validation_common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-11 10:59:23.000000 apysc-2.8.7/apysc/_validation/variable_name_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:59:41.537850 apysc-2.8.7/apysc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-11 10:59:41.000000 apysc-2.8.7/apysc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-06-11 10:59:41.000000 apysc-2.8.7/apysc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 10:59:41.000000 apysc-2.8.7/apysc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-11 10:59:41.000000 apysc-2.8.7/apysc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 10:59:41.000000 apysc-2.8.7/apysc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 10:59:41.593850 apysc-2.8.7/setup.cfg
```

### Comparing `apysc-2.8.6/LICENSE` & `apysc-2.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/PKG-INFO` & `apysc-2.8.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apysc
-Version: 2.8.6
+Version: 2.8.7
 Summary: apysc is the Python's frontend library to create html and js file, that has the ActionScript 3 (as3)-like interface.
 Home-page: https://github.com/simon-ritchie/apysc
 Maintainer: simon-ritchie
 Maintainer-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apysc-2.8.6/README.md` & `apysc-2.8.7/README.md`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/__init__.py` & `apysc-2.8.7/apysc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from apysc._type.dictionary import Dictionary
 from apysc._type.any_value import AnyValue
 from apysc._branch._if import If
 from apysc._branch._elif import Elif
 from apysc._branch._else import Else
 from apysc._loop._for import For
 from apysc._loop.for_array_indices import ForArrayIndices
+from apysc._loop.for_array_values import ForArrayValues
 from apysc._loop._continue import Continue
 from apysc._loop._range import range
 from apysc._display.display_object import DisplayObject
 from apysc._display._document import document
 from apysc._display.sprite import Sprite
 from apysc._display.graphics import Graphics
 from apysc._display.stage import Stage
@@ -123,8 +124,8 @@
 from apysc._math.math import Math
 from apysc._auto_reloading.auto_reloading_decorator import set_auto_reloading
 from apysc._chart.x_axis_settings import XAxisSettings
 from apysc._chart.y_axis_single_column_settings import YAxisSingleColumnSettings
 from apysc._chart.x_axis_label_position import XAxisLabelPosition
 from apysc._chart.y_axis_label_position import YAxisLabelPosition
 
-__version__: str = "2.8.6"
+__version__: str = "2.8.7"
```

### Comparing `apysc-2.8.6/apysc/_animation/animation_base.py` & `apysc-2.8.7/apysc/_animation/animation_base.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_cx.py` & `apysc-2.8.7/apysc/_animation/animation_cx.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_cx_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_cx_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_cy.py` & `apysc-2.8.7/apysc/_animation/animation_cy.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_cy_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_cy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_fill_alpha.py` & `apysc-2.8.7/apysc/_animation/animation_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_fill_alpha_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_fill_color.py` & `apysc-2.8.7/apysc/_animation/animation_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_fill_color_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_finish_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_finish_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_height.py` & `apysc-2.8.7/apysc/_animation/animation_height.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_height_for_ellipse.py` & `apysc-2.8.7/apysc/_animation/animation_height_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_height_for_ellipse_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_height_for_ellipse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_height_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_line_alpha.py` & `apysc-2.8.7/apysc/_animation/animation_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_line_alpha_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_line_color.py` & `apysc-2.8.7/apysc/_animation/animation_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_line_color_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_line_thickness.py` & `apysc-2.8.7/apysc/_animation/animation_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_line_thickness_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_mixins.py` & `apysc-2.8.7/apysc/_animation/animation_mixins.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_move.py` & `apysc-2.8.7/apysc/_animation/animation_move.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_move_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_move_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_parallel.py` & `apysc-2.8.7/apysc/_animation/animation_parallel.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_parallel_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_parallel_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_pause_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_pause_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_play_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_play_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_radius.py` & `apysc-2.8.7/apysc/_animation/animation_radius.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_radius_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_radius_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_reset_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_reset_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_reverse_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_reverse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_rotation_around_center.py` & `apysc-2.8.7/apysc/_animation/animation_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_rotation_around_center_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_rotation_around_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_rotation_around_point.py` & `apysc-2.8.7/apysc/_animation/animation_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_rotation_around_point_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_rotation_around_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_scale_x_from_center.py` & `apysc-2.8.7/apysc/_animation/animation_scale_x_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_scale_x_from_center_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_scale_x_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_scale_x_from_point.py` & `apysc-2.8.7/apysc/_animation/animation_scale_x_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_scale_x_from_point_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_scale_x_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_scale_y_from_center.py` & `apysc-2.8.7/apysc/_animation/animation_scale_y_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_scale_y_from_center_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_scale_y_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_scale_y_from_point.py` & `apysc-2.8.7/apysc/_animation/animation_scale_y_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_scale_y_from_point_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_scale_y_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_time_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_time_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_width.py` & `apysc-2.8.7/apysc/_animation/animation_width.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_width_for_ellipse.py` & `apysc-2.8.7/apysc/_animation/animation_width_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_width_for_ellipse_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_width_for_ellipse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_width_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_x.py` & `apysc-2.8.7/apysc/_animation/animation_x.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_x_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_y.py` & `apysc-2.8.7/apysc/_animation/animation_y.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/animation_y_mixin.py` & `apysc-2.8.7/apysc/_animation/animation_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_animation/easing.py` & `apysc-2.8.7/apysc/_animation/easing.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_auto_reloading/auto_reloading_decorator.py` & `apysc-2.8.7/apysc/_auto_reloading/auto_reloading_decorator.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_branch/_elif.py` & `apysc-2.8.7/apysc/_branch/_elif.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_branch/_else.py` & `apysc-2.8.7/apysc/_branch/_else.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_branch/_if.py` & `apysc-2.8.7/apysc/_branch/_if.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_branch/if_base.py` & `apysc-2.8.7/apysc/_branch/if_base.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_callable/callable_util.py` & `apysc-2.8.7/apysc/_callable/callable_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/add_background_mixin.py` & `apysc-2.8.7/apysc/_chart/add_background_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/add_border_mixin.py` & `apysc-2.8.7/apysc/_chart/add_border_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/axis_label_bold_mixin.py` & `apysc-2.8.7/apysc/_chart/axis_label_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/axis_label_fill_alpha_mixin.py` & `apysc-2.8.7/apysc/_chart/axis_label_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/axis_label_fill_color_mixin.py` & `apysc-2.8.7/apysc/_chart/axis_label_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/axis_label_font_family_mixin.py` & `apysc-2.8.7/apysc/_chart/axis_label_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/axis_label_font_size_mixin.py` & `apysc-2.8.7/apysc/_chart/axis_label_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/axis_label_italic_mixin.py` & `apysc-2.8.7/apysc/_chart/axis_label_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/axis_line_alpha_mixin.py` & `apysc-2.8.7/apysc/_chart/axis_line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/axis_line_color_mixin.py` & `apysc-2.8.7/apysc/_chart/axis_line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/axis_line_thickness_mixin.py` & `apysc-2.8.7/apysc/_chart/axis_line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/background_container_mixin.py` & `apysc-2.8.7/apysc/_chart/background_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/border_container_mixin.py` & `apysc-2.8.7/apysc/_chart/border_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/chart_container_mixin.py` & `apysc-2.8.7/apysc/_chart/chart_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/create_single_column_y_axis_mixin.py` & `apysc-2.8.7/apysc/_chart/create_single_column_y_axis_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/initialize_each_container_mixin.py` & `apysc-2.8.7/apysc/_chart/initialize_each_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/is_display_axis_label_mixin.py` & `apysc-2.8.7/apysc/_chart/is_display_axis_label_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/overall_container_mixin.py` & `apysc-2.8.7/apysc/_chart/overall_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/set_initial_background_fill_alpha_mixin.py` & `apysc-2.8.7/apysc/_chart/set_initial_background_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/set_initial_background_fill_color_mixin.py` & `apysc-2.8.7/apysc/_chart/set_initial_background_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/set_initial_border_alpha_mixin.py` & `apysc-2.8.7/apysc/_chart/set_initial_border_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/set_initial_border_color_mixin.py` & `apysc-2.8.7/apysc/_chart/set_initial_border_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/set_initial_border_thickness_mixin.py` & `apysc-2.8.7/apysc/_chart/set_initial_border_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/set_initial_height_mixin.py` & `apysc-2.8.7/apysc/_chart/set_initial_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/set_initial_horizontal_padding_mixin.py` & `apysc-2.8.7/apysc/_chart/set_initial_horizontal_padding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/set_initial_matrix_data_mixin.py` & `apysc-2.8.7/apysc/_chart/set_initial_matrix_data_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/set_initial_overall_container_coordinates_mixin.py` & `apysc-2.8.7/apysc/_chart/set_initial_overall_container_coordinates_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/set_initial_vertical_padding_mixin.py` & `apysc-2.8.7/apysc/_chart/set_initial_vertical_padding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/set_initial_width_mixin.py` & `apysc-2.8.7/apysc/_chart/set_initial_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/set_initial_x_mixin.py` & `apysc-2.8.7/apysc/_chart/set_initial_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/set_initial_y_mixin.py` & `apysc-2.8.7/apysc/_chart/set_initial_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/tick_max_num_mixin.py` & `apysc-2.8.7/apysc/_chart/tick_max_num_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/tick_text_bold_mixin.py` & `apysc-2.8.7/apysc/_chart/tick_text_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/tick_text_fill_alpha_mixin.py` & `apysc-2.8.7/apysc/_chart/tick_text_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/tick_text_fill_color_mixin.py` & `apysc-2.8.7/apysc/_chart/tick_text_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/tick_text_font_family_mixin.py` & `apysc-2.8.7/apysc/_chart/tick_text_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/tick_text_font_size_mixin.py` & `apysc-2.8.7/apysc/_chart/tick_text_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/tick_text_italic_mixin.py` & `apysc-2.8.7/apysc/_chart/tick_text_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/vertical_bar_chart.py` & `apysc-2.8.7/apysc/_chart/vertical_bar_chart.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/x_axis_column_name_mixin.py` & `apysc-2.8.7/apysc/_chart/x_axis_column_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/x_axis_container_mixin.py` & `apysc-2.8.7/apysc/_chart/x_axis_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/x_axis_label_position_mixin.py` & `apysc-2.8.7/apysc/_chart/x_axis_label_position_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/x_axis_settings.py` & `apysc-2.8.7/apysc/_chart/x_axis_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/y_axis_column_name_mixin.py` & `apysc-2.8.7/apysc/_chart/y_axis_column_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/y_axis_container_mixin.py` & `apysc-2.8.7/apysc/_chart/y_axis_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/y_axis_label_position_mixin.py` & `apysc-2.8.7/apysc/_chart/y_axis_label_position_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/y_axis_single_column_settings.py` & `apysc-2.8.7/apysc/_chart/y_axis_single_column_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/y_max_mixin.py` & `apysc-2.8.7/apysc/_chart/y_max_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_chart/y_min_mixin.py` & `apysc-2.8.7/apysc/_chart/y_min_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_color/color_util.py` & `apysc-2.8.7/apysc/_color/color_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_console/_trace.py` & `apysc-2.8.7/apysc/_console/_trace.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_console/assertion.py` & `apysc-2.8.7/apysc/_console/assertion.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_console/loggers.py` & `apysc-2.8.7/apysc/_console/loggers.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_converter/cast.py` & `apysc-2.8.7/apysc/_converter/cast.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_converter/to_apysc_val_from_builtin.py` & `apysc-2.8.7/apysc/_converter/to_apysc_val_from_builtin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_converter/to_builtin_val_from_apysc.py` & `apysc-2.8.7/apysc/_converter/to_builtin_val_from_apysc.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/_document.py` & `apysc-2.8.7/apysc/_display/_document.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/append_fill_alpha_attr_expression_mixin.py` & `apysc-2.8.7/apysc/_display/append_fill_alpha_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/append_fill_color_expression_mixin.py` & `apysc-2.8.7/apysc/_display/append_fill_color_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/append_line_alpha_attr_expression_mixin.py` & `apysc-2.8.7/apysc/_display/append_line_alpha_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/append_line_cap_attr_expression_mixin.py` & `apysc-2.8.7/apysc/_display/append_line_cap_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/append_line_color_attr_expression_mixin.py` & `apysc-2.8.7/apysc/_display/append_line_color_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/append_line_joints_attr_expression_mixin.py` & `apysc-2.8.7/apysc/_display/append_line_joints_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/append_line_point_mixin.py` & `apysc-2.8.7/apysc/_display/append_line_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/append_line_thickness_attr_expression_mixin.py` & `apysc-2.8.7/apysc/_display/append_line_thickness_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/append_x_attr_expression_mixin.py` & `apysc-2.8.7/apysc/_display/append_x_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/append_y_attr_expression_mixin.py` & `apysc-2.8.7/apysc/_display/append_y_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/begin_fill_mixin.py` & `apysc-2.8.7/apysc/_display/begin_fill_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/child_mixin.py` & `apysc-2.8.7/apysc/_display/child_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -296,25 +296,20 @@
         ...     x=150, y=50, width=50, height=50
         ... )
         >>> child_at_index_1: ap.DisplayObject = sprite.graphics.get_child_at(1)
         >>> child_at_index_1 == rectangle_2
         True
         """
         from apysc._display.any_display_object import AnyDisplayObject
-        from apysc._expression import expression_variables_util
-        from apysc._expression import var_names
 
         self._initialize_children_if_not_initialized()
         if self.num_children > index:
             child: DisplayObject = self._children[index]
         else:
-            variable_name: str = expression_variables_util.get_next_variable_name(
-                type_name=var_names.DISPLAY_OBJECT
-            )
-            child = AnyDisplayObject(variable_name=variable_name)
+            child = AnyDisplayObject()
         self._append_get_child_at_expression(child=child, index=index)
         return child
 
     @final
     def _append_get_child_at_expression(
         self, *, child: DisplayObject, index: Union[int, Int]
     ) -> None:
```

### Comparing `apysc-2.8.6/apysc/_display/circle.py` & `apysc-2.8.7/apysc/_display/circle.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,17 @@
 from apysc._display.scale_y_from_point_mixin import ScaleYFromPointMixIn
 from apysc._display.set_overflow_visible_setting_mixin import (
     SetOverflowVisibleSettingMixIn,
 )
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.attr_to_apysc_val_from_builtin_mixin import (
     AttrToApyscValFromBuiltinMixIn,
 )
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
@@ -105,14 +108,15 @@
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
     GetBoundsMixIn,
     VariableNameSuffixMixIn,
     AttrToApyscValFromBuiltinMixIn,
+    InitializeForLoopValueInterface,
 ):
     """
     The circle vector graphics class.
 
     References
     ----------
     - Circle class
@@ -430,7 +434,28 @@
         -------
         repr_str : str
             Type name and variable name will be set
             (e.g., `Circle("<variable_name>")`).
         """
         repr_str: str = f'{Circle.__name__}("{self.variable_name}")'
         return repr_str
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Circle":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        circle : Circle
+            An initialized circle instance.
+        """
+        import apysc as ap
+
+        circle: Circle = Circle(
+            x=-1,
+            y=-1,
+            radius=1,
+        )
+        circle.visible = ap.Boolean(False)
+        return circle
```

### Comparing `apysc-2.8.6/apysc/_display/css_interface.py` & `apysc-2.8.7/apysc/_display/css_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/css_mixin.py` & `apysc-2.8.7/apysc/_display/css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/cx_mixin.py` & `apysc-2.8.7/apysc/_display/cx_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/cy_mixin.py` & `apysc-2.8.7/apysc/_display/cy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/display_object.py` & `apysc-2.8.7/apysc/_display/display_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """Implementations for DisplayObject class.
 """
 
-from typing import TYPE_CHECKING
-
 from apysc._animation.animation_parallel_mixin import AnimationParallelMixIn
 from apysc._display.css_interface import CssInterface
 from apysc._display.parent_mixin import ParentMixIn
 from apysc._display.visible_mixin import VisibleMixIn
 from apysc._event.custom_event_mixin import CustomEventMixIn
 from apysc._event.mouse_event_mixins import MouseEventMixIns
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._validation import arg_validation_decos
 
-if TYPE_CHECKING:
-    pass
-
 
 class DisplayObject(
     ParentMixIn,
     MouseEventMixIns,
     VisibleMixIn,
     CustomEventMixIn,
     CssInterface,
```

### Comparing `apysc-2.8.6/apysc/_display/ellipse.py` & `apysc-2.8.7/apysc/_display/ellipse.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,17 @@
 )
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.width_and_height_mixin_for_ellipse import (
     WidthAndHeightMixInForEllipse,
 )
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.attr_to_apysc_val_from_builtin_mixin import (
     AttrToApyscValFromBuiltinMixIn,
 )
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
@@ -107,14 +110,15 @@
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
     GetBoundsMixIn,
     VariableNameSuffixMixIn,
     AttrToApyscValFromBuiltinMixIn,
+    InitializeForLoopValueInterface,
 ):
     """
     The ellipse vector graphics class.
 
     References
     ----------
     - Ellipse class
@@ -424,7 +428,29 @@
         -------
         repr_str : str
             Type name and variable name will be set
             (e.g., `Ellipse("<variable_name>")`).
         """
         repr_str: str = f'{Ellipse.__name__}("{self.variable_name}")'
         return repr_str
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Ellipse":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        ellipse : Ellipse
+            An initialized ellipse instance.
+        """
+        import apysc as ap
+
+        ellipse: Ellipse = Ellipse(
+            x=-1,
+            y=-1,
+            width=1,
+            height=1,
+        )
+        ellipse.visible = ap.Boolean(False)
+        return ellipse
```

### Comparing `apysc-2.8.6/apysc/_display/ellipse_height_mixin.py` & `apysc-2.8.7/apysc/_display/ellipse_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/ellipse_width_mixin.py` & `apysc-2.8.7/apysc/_display/ellipse_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/fill_alpha_mixin.py` & `apysc-2.8.7/apysc/_display/fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/fill_color_mixin.py` & `apysc-2.8.7/apysc/_display/fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/flip_interface_helper.py` & `apysc-2.8.7/apysc/_display/flip_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/flip_x_mixin.py` & `apysc-2.8.7/apysc/_display/flip_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/flip_y_mixin.py` & `apysc-2.8.7/apysc/_display/flip_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/get_bounds_mixin.py` & `apysc-2.8.7/apysc/_display/get_bounds_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/graphics.py` & `apysc-2.8.7/apysc/_display/graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     SetOverflowVisibleSettingMixIn,
 )
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._geom.path_data_base import PathDataBase
 from apysc._geom.point2d import Point2D
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.array import Array
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._validation import arg_validation_decos
 
 
 class Graphics(
@@ -42,14 +45,15 @@
     SetOverflowVisibleSettingMixIn,
     CssMixIn,
     DisplayObject,
     BeginFillMixIn,
     LineStyleMixIn,
     GraphicsClearMixIn,
     ChildMixIn,
+    InitializeForLoopValueInterface,
 ):
     """
     Create an object that has each vector graphics interface.
 
     References
     ----------
     - Graphics
@@ -1323,7 +1327,25 @@
         -------
         repr_str : str
             Type name and variable name will be set
             (e.g., `Graphics("<variable_name>")`).
         """
         repr_str: str = f'{Graphics.__name__}("{self.variable_name}")'
         return repr_str
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Graphics":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        graphics : Graphics
+            An initialized graphics instance.
+        """
+        import apysc as ap
+
+        sprite_: sprite.Sprite = sprite.Sprite()
+        graphics: Graphics = Graphics(parent=sprite_)
+        graphics.visible = ap.Boolean(False)
+        return graphics
```

### Comparing `apysc-2.8.6/apysc/_display/graphics_base.py` & `apysc-2.8.7/apysc/_display/graphics_base.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/graphics_clear_mixin.py` & `apysc-2.8.7/apysc/_display/graphics_clear_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/graphics_expression.py` & `apysc-2.8.7/apysc/_display/graphics_expression.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/height_mixin.py` & `apysc-2.8.7/apysc/_display/height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line.py` & `apysc-2.8.7/apysc/_display/line.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,17 @@
 )
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._geom import point2d
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
@@ -88,14 +91,15 @@
     AppendLineCapAttrExpressionMixIn,
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
     GetBoundsMixIn,
     VariableNameSuffixMixIn,
+    InitializeForLoopValueInterface,
 ):
     """
     The line vector graphics class.
 
     References
     ----------
     - Line class
@@ -386,7 +390,27 @@
         -------
         repr_str : str
             Type name and variable name will be set
             (e.g., `Line("<variable_name>")`).
         """
         repr_str: str = f'{Line.__name__}("{self.variable_name}")'
         return repr_str
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Line":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        line : Line
+            An initialized line instance.
+        """
+        import apysc as ap
+
+        line: Line = Line(
+            start_point=point2d.Point2D(x=-2, y=-2),
+            end_point=point2d.Point2D(x=-1, y=-1),
+        )
+        line.visible = ap.Boolean(False)
+        return line
```

### Comparing `apysc-2.8.6/apysc/_display/line_alpha_mixin.py` & `apysc-2.8.7/apysc/_display/line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_cap_mixin.py` & `apysc-2.8.7/apysc/_display/line_cap_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_caps.py` & `apysc-2.8.7/apysc/_display/line_caps.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_color_mixin.py` & `apysc-2.8.7/apysc/_display/line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_dash_dot_setting.py` & `apysc-2.8.7/apysc/_display/line_dash_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_dash_dot_setting_mixin.py` & `apysc-2.8.7/apysc/_display/line_dash_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_dash_setting.py` & `apysc-2.8.7/apysc/_display/line_dash_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_dash_setting_mixin.py` & `apysc-2.8.7/apysc/_display/line_dash_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_dot_setting.py` & `apysc-2.8.7/apysc/_display/line_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_dot_setting_mixin.py` & `apysc-2.8.7/apysc/_display/line_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_joints.py` & `apysc-2.8.7/apysc/_display/line_joints.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_joints_mixin.py` & `apysc-2.8.7/apysc/_display/line_joints_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_round_dot_setting.py` & `apysc-2.8.7/apysc/_display/line_round_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_round_dot_setting_mixin.py` & `apysc-2.8.7/apysc/_display/line_round_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_style_mixin.py` & `apysc-2.8.7/apysc/_display/line_style_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/line_thickness_mixin.py` & `apysc-2.8.7/apysc/_display/line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/parent_mixin.py` & `apysc-2.8.7/apysc/_display/parent_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/path.py` & `apysc-2.8.7/apysc/_display/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,17 @@
 )
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._geom.path_data_base import PathDataBase
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
@@ -108,14 +111,15 @@
     AppendLineJointsAttrExpressionMixIn,
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
     GetBoundsMixIn,
     VariableNameSuffixMixIn,
+    InitializeForLoopValueInterface,
 ):
     """
     The path vector graphics class.
 
     References
     ----------
     - Path class
@@ -425,7 +429,29 @@
         -------
         repr_str : str
             Type name and variable name will be set
             (e.g., `Path("<variable_name>")`).
         """
         repr_str: str = f'{Path.__name__}("{self.variable_name}")'
         return repr_str
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Path":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        path : Path
+            An initialized path instance.
+        """
+        import apysc as ap
+
+        path: Path = Path(
+            path_data_list=[
+                ap.PathMoveTo(x=-2, y=-2),
+                ap.PathLineTo(x=-1, y=-1),
+            ],
+        )
+        path.visible = ap.Boolean(False)
+        return path
```

### Comparing `apysc-2.8.6/apysc/_display/points_2d_mixin.py` & `apysc-2.8.7/apysc/_display/points_2d_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/polygon.py` & `apysc-2.8.7/apysc/_display/polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,17 @@
 )
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._geom.point2d import Point2D
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.array import Array
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
@@ -119,14 +122,15 @@
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
     PolygonAppendConstructorExpressionMixIn,
     GetBoundsMixIn,
     VariableNameSuffixMixIn,
+    InitializeForLoopValueInterface,
 ):
     """
     The polygon vector graphics class.
 
     References
     ----------
     - Polygon class
@@ -363,7 +367,30 @@
         -------
         repr_str : str
             Type name and variable name will be set
             (e.g., `Polygon("<variable_name>")`).
         """
         repr_str: str = f'{Polygon.__name__}("{self.variable_name}")'
         return repr_str
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Polygon":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        polygon : Polygon
+            An initialized polygon instance.
+        """
+        import apysc as ap
+
+        polygon: Polygon = Polygon(
+            points=[
+                Point2D(x=-2, y=-2),
+                Point2D(x=-1, y=-2),
+                Point2D(x=-1, y=-1),
+            ]
+        )
+        polygon.visible = ap.Boolean(False)
+        return polygon
```

### Comparing `apysc-2.8.6/apysc/_display/polygon_append_constructor_expression_mixin.py` & `apysc-2.8.7/apysc/_display/polygon_append_constructor_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/polygon_apply_current_points_mixin.py` & `apysc-2.8.7/apysc/_display/polygon_apply_current_points_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/polygon_x1_mixin.py` & `apysc-2.8.7/apysc/_display/polygon_x1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/polygon_x2_mixin.py` & `apysc-2.8.7/apysc/_display/polygon_x2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/polygon_x3_mixin.py` & `apysc-2.8.7/apysc/_display/polygon_x3_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/polygon_y1_mixin.py` & `apysc-2.8.7/apysc/_display/polygon_y1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/polygon_y2_mixin.py` & `apysc-2.8.7/apysc/_display/polygon_y2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/polygon_y3_mixin.py` & `apysc-2.8.7/apysc/_display/polygon_y3_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/polyline.py` & `apysc-2.8.7/apysc/_display/polyline.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,17 @@
 )
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._geom.point2d import Point2D
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.array import Array
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
@@ -116,14 +119,15 @@
     AppendLineJointsAttrExpressionMixIn,
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
     GetBoundsMixIn,
     VariableNameSuffixMixIn,
+    InitializeForLoopValueInterface,
 ):
     """
     The polyline vector graphics class.
 
     References
     ----------
     - Polyline class
@@ -409,7 +413,29 @@
         )
         expression = self._append_y_attr_expression(
             expression=expression, indent_num=INDENT_NUM
         )
         expression += "\n  });"
         ap.append_js_expression(expression=expression)
         self._points_var_name = points_var_name
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Polyline":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        polyline : Polyline
+            An initialized polyline instance
+        """
+        import apysc as ap
+
+        polyline: Polyline = Polyline(
+            points=[
+                Point2D(x=-2, y=-2),
+                Point2D(x=-1, y=-1),
+            ]
+        )
+        polyline.visible = ap.Boolean(False)
+        return polyline
```

### Comparing `apysc-2.8.6/apysc/_display/radius_mixin.py` & `apysc-2.8.7/apysc/_display/radius_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/rectangle.py` & `apysc-2.8.7/apysc/_display/rectangle.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,17 @@
 )
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.width_mixin import WidthMixIn
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
@@ -114,14 +117,15 @@
     AppendLineJointsAttrExpressionMixIn,
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
     GetBoundsMixIn,
     VariableNameSuffixMixIn,
+    InitializeForLoopValueInterface,
 ):
     """
     The rectangle vector graphics class.
 
     References
     ----------
     - Rectangle class
@@ -473,7 +477,24 @@
             expression=expression, indent_num=INDENT_NUM
         )
         expression = self._append_y_attr_expression(
             expression=expression, indent_num=INDENT_NUM
         )
         expression += "\n  });"
         ap.append_js_expression(expression=expression)
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Rectangle":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        rectangle : Rectangle
+            An initialized rectangle instance.
+        """
+        import apysc as ap
+
+        rectangle: Rectangle = Rectangle(x=-2, y=-2, width=1, height=1)
+        rectangle.visible = ap.Boolean(False)
+        return rectangle
```

### Comparing `apysc-2.8.6/apysc/_display/rotation_around_center_mixin.py` & `apysc-2.8.7/apysc/_display/rotation_around_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/rotation_around_point_mixin.py` & `apysc-2.8.7/apysc/_display/rotation_around_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/rotation_interface_helper.py` & `apysc-2.8.7/apysc/_display/rotation_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/scale_interface_helper.py` & `apysc-2.8.7/apysc/_display/scale_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/scale_x_from_center_mixin.py` & `apysc-2.8.7/apysc/_display/scale_x_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/scale_x_from_point_mixin.py` & `apysc-2.8.7/apysc/_display/scale_x_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/scale_y_from_center_mixin.py` & `apysc-2.8.7/apysc/_display/scale_y_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/scale_y_from_point_mixin.py` & `apysc-2.8.7/apysc/_display/scale_y_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/set_lower_scale_limit_mixin.py` & `apysc-2.8.7/apysc/_display/set_lower_scale_limit_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/set_overflow_visible_setting_mixin.py` & `apysc-2.8.7/apysc/_display/set_overflow_visible_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/skew_x_mixin.py` & `apysc-2.8.7/apysc/_display/skew_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/skew_y_mixin.py` & `apysc-2.8.7/apysc/_display/skew_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/sprite.py` & `apysc-2.8.7/apysc/_display/sprite.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 from apysc._display.set_overflow_visible_setting_mixin import (
     SetOverflowVisibleSettingMixIn,
 )
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._event.enter_frame_mixin import EnterFrameMixIn
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.revert_mixin import RevertMixIn
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
 
 _Graphics = graphics.Graphics
 
 
@@ -29,14 +32,15 @@
     SetOverflowVisibleSettingMixIn,
     CssMixIn,
     GetBoundsMixIn,
     DisplayObject,
     ChildMixIn,
     RevertMixIn,
     VariableNameSuffixMixIn,
+    InitializeForLoopValueInterface,
 ):
     """
     This class is for the basic display object that
     can be a parent.
 
     References
     ----------
@@ -194,7 +198,24 @@
         -------
         repr_str : str
             Type name and variable name will be set
             (e.g., `Sprite("<variable_name>")`).
         """
         repr_str: str = f'{Sprite.__name__}("{self.variable_name}")'
         return repr_str
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Sprite":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        sprite : Sprite
+            An initialized sprite instance.
+        """
+        import apysc as ap
+
+        sprite: Sprite = Sprite()
+        sprite.visible = ap.Boolean(False)
+        return sprite
```

### Comparing `apysc-2.8.6/apysc/_display/stage.py` & `apysc-2.8.7/apysc/_display/stage.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text.py` & `apysc-2.8.7/apysc/_display/svg_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,17 @@
 from apysc._display.svg_text_set_leading_mixin import SVGTextSetLeadingMixIn
 from apysc._display.svg_text_set_text_value_mixin import SVGTextSetTextValueMixIn
 from apysc._display.svg_text_span import SVGTextSpan
 from apysc._display.svg_text_text_mixin import SVGTextTextMixIn
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.array import Array
 from apysc._type.boolean import Boolean
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
@@ -114,14 +117,15 @@
     SVGTextSetAlignMixIn,
     SVGTextItalicMixIn,
     SVGTextSetItalicMixIn,
     SVGTextBoldMixIn,
     SVGTextSetBoldMixIn,
     GetBoundsMixIn,
     VariableNameSuffixMixIn,
+    InitializeForLoopValueInterface,
 ):
     """
     The class for an SVG text.
 
     Notes
     -----
     - SVGText's y-coordinate zero-position starts at the bottom of a text.
@@ -566,7 +570,24 @@
         repr_str : str
             This interface returns a type name and variable name
             (e.g., `SVGText("<variable_name>")`).
         """
 
         repr_str: str = f'{SVGText.__name__}("{self.variable_name}")'
         return repr_str
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "SVGText":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        svg_text : SVGText
+            An initialized svg text instance.
+        """
+        import apysc as ap
+
+        svg_text: SVGText = SVGText(text="")
+        svg_text.visible = ap.Boolean(False)
+        return svg_text
```

### Comparing `apysc-2.8.6/apysc/_display/svg_text_align_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_align_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_bold_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_delta_x_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_delta_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_delta_y_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_delta_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_font_family_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_font_size_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_italic_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_leading_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_leading_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_set_align_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_set_align_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_set_bold_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_set_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_set_delta_x_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_set_delta_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_set_delta_y_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_set_delta_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_set_font_family_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_set_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_set_font_size_value_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_set_font_size_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_set_italic_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_set_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_set_leading_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_set_leading_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_set_text_value_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_set_text_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_singleton_for_text_span.py` & `apysc-2.8.7/apysc/_display/svg_text_singleton_for_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/svg_text_span.py` & `apysc-2.8.7/apysc/_display/svg_text_span.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,17 @@
     SVGTextSkipLineColorExpAppendingMixIn,
 )
 from apysc._display.svg_text_skip_line_thickness_exp_appending_mixin import (
     SVGTextSkipLineThicknessExpAppendingMixIn,
 )
 from apysc._display.svg_text_text_mixin import SVGTextTextMixIn
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.array import Array
 from apysc._type.boolean import Boolean
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
@@ -107,14 +110,15 @@
     SVGTextSetBoldMixIn,
     SVGTextDeltaXMixIn,
     SVGTextSetDeltaXMixIn,
     SVGTextDeltaYMixIn,
     SVGTextSetDeltaYMixIn,
     GetBoundsMixIn,
     VariableNameSuffixMixIn,
+    InitializeForLoopValueInterface,
 ):
     """
     The class for an SVG text-span (the child class of `SVGText`).
 
     Notes
     -----
     - If style settings are `None`, its styles inherit parent
@@ -329,14 +333,31 @@
         repr_str : str
             This interface returns a type name and variable name
             (e.g., `SVGTextSpan("<variable_name>")`).
         """
         repr_str: str = f'{SVGTextSpan.__name__}("{self.variable_name}")'
         return repr_str
 
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "SVGTextSpan":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        svg_text_span : SVGTextSpan
+            An initialized text span instance.
+        """
+        import apysc as ap
+
+        svg_text_span: SVGTextSpan = SVGTextSpan(text="")
+        svg_text_span.visible = ap.Boolean(False)
+        return svg_text_span
+
 
 def _get_init_line_color_str(
     *, line_color: Optional[Union[str, String]]
 ) -> Union[str, String]:
     """
     Get an initial line-color string.
```

### Comparing `apysc-2.8.6/apysc/_display/svg_text_text_mixin.py` & `apysc-2.8.7/apysc/_display/svg_text_text_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/triangle.py` & `apysc-2.8.7/apysc/_display/triangle.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,17 @@
 )
 from apysc._display.skew_x_mixin import SkewXMixIn
 from apysc._display.skew_y_mixin import SkewYMixIn
 from apysc._display.x_mixin import XMixIn
 from apysc._display.y_mixin import YMixIn
 from apysc._geom.point2d import Point2D
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.array import Array
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._type.repr_interface import ReprInterface
 from apysc._type.string import String
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
 from apysc._validation import arg_validation_decos
@@ -124,14 +127,15 @@
     LineDotSettingMixIn,
     LineDashSettingMixIn,
     LineRoundDotSettingMixIn,
     LineDashDotSettingMixIn,
     PolygonAppendConstructorExpressionMixIn,
     GetBoundsMixIn,
     VariableNameSuffixMixIn,
+    InitializeForLoopValueInterface,
 ):
     """
     The triangle vector graphics class.
 
     References
     ----------
     - Triangle class
@@ -440,7 +444,31 @@
         -------
         repr_str : str
             Type name and variable name will be set
             (e.g., `Triangle("<variable_name>")`).
         """
         repr_str: str = f'{Triangle.__name__}("{self.variable_name}")'
         return repr_str
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Triangle":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        triangle : Triangle
+            An initialized triangle instance.
+        """
+        import apysc as ap
+
+        triangle: Triangle = Triangle(
+            x1=-2,
+            y1=-2,
+            x2=-1,
+            y2=-2,
+            x3=-1,
+            y3=-1,
+        )
+        triangle.visible = ap.Boolean(False)
+        return triangle
```

### Comparing `apysc-2.8.6/apysc/_display/visible_mixin.py` & `apysc-2.8.7/apysc/_display/visible_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/width_and_height_mixin_for_ellipse.py` & `apysc-2.8.7/apysc/_display/width_and_height_mixin_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/width_mixin.py` & `apysc-2.8.7/apysc/_display/width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/x_interface.py` & `apysc-2.8.7/apysc/_display/x_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/x_mixin.py` & `apysc-2.8.7/apysc/_display/x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/y_interface.py` & `apysc-2.8.7/apysc/_display/y_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_display/y_mixin.py` & `apysc-2.8.7/apysc/_display/y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/animation_event.py` & `apysc-2.8.7/apysc/_event/animation_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/click_mixin.py` & `apysc-2.8.7/apysc/_event/click_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/custom_event_mixin.py` & `apysc-2.8.7/apysc/_event/custom_event_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/document_mouse_wheel_func.py` & `apysc-2.8.7/apysc/_event/document_mouse_wheel_func.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/double_click_mixin.py` & `apysc-2.8.7/apysc/_event/double_click_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/enter_frame_event.py` & `apysc-2.8.7/apysc/_event/enter_frame_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/enter_frame_mixin.py` & `apysc-2.8.7/apysc/_event/enter_frame_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/event.py` & `apysc-2.8.7/apysc/_event/event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/handler.py` & `apysc-2.8.7/apysc/_event/handler.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/handler_circular_calling_util.py` & `apysc-2.8.7/apysc/_event/handler_circular_calling_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/mouse_down_mixin.py` & `apysc-2.8.7/apysc/_event/mouse_down_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/mouse_event.py` & `apysc-2.8.7/apysc/_event/mouse_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/mouse_event_binding_expression_mixin.py` & `apysc-2.8.7/apysc/_event/mouse_event_binding_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/mouse_event_mixins.py` & `apysc-2.8.7/apysc/_event/mouse_event_mixins.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/mouse_event_unbinding_mixin.py` & `apysc-2.8.7/apysc/_event/mouse_event_unbinding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/mouse_move_mixin.py` & `apysc-2.8.7/apysc/_event/mouse_move_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/mouse_out_mixin.py` & `apysc-2.8.7/apysc/_event/mouse_out_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/mouse_over_mixin.py` & `apysc-2.8.7/apysc/_event/mouse_over_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/mouse_up_mixin.py` & `apysc-2.8.7/apysc/_event/mouse_up_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/prevent_default_mixin.py` & `apysc-2.8.7/apysc/_event/prevent_default_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/set_handler_data_mixin.py` & `apysc-2.8.7/apysc/_event/set_handler_data_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/stop_propagation_mixin.py` & `apysc-2.8.7/apysc/_event/stop_propagation_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/timer_event.py` & `apysc-2.8.7/apysc/_event/timer_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_event/wheel_event.py` & `apysc-2.8.7/apysc/_event/wheel_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_expression/event_handler_scope.py` & `apysc-2.8.7/apysc/_expression/event_handler_scope.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_expression/expression_data_util.py` & `apysc-2.8.7/apysc/_expression/expression_data_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_expression/expression_variables_util.py` & `apysc-2.8.7/apysc/_expression/expression_variables_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_expression/indent_num.py` & `apysc-2.8.7/apysc/_expression/indent_num.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_expression/js_functions.py` & `apysc-2.8.7/apysc/_expression/js_functions.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_expression/last_scope.py` & `apysc-2.8.7/apysc/_expression/last_scope.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     NORMAL = 1
     IF = 2
     ELIF = 3
     ELSE = 4
     FOR = 5
     EVENT_HANDLER = 6
     FOR_ARRAY_INDICES = 7
+    FOR_ARRAY_VALUES = 8
 
 
 def reset() -> None:
     """
     Reset last expression's scope information.
     """
     from apysc._expression import expression_data_util
```

### Comparing `apysc-2.8.6/apysc/_expression/var_names.py` & `apysc-2.8.7/apysc/_expression/var_names.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from typing_extensions import Final
 
 DOCUMENT: Final[str] = "document"
 BLANK_OBJECT: Final[str] = "bo"
 DISPLAY_OBJECT: Final[str] = "do"
+ANY_DISPLAY_OBJECT: Final[str] = "ado"
 PARENT: Final[str] = "parent"
 GRAPHICS: Final[str] = "g"
 POINT2D: Final[str] = "p2d"
 RECTANGLE: Final[str] = "rect"
 CIRCLE: Final[str] = "circle"
 ELLIPSE: Final[str] = "ellipse"
 LINE: Final[str] = "line"
```

### Comparing `apysc-2.8.6/apysc/_file/file_util.py` & `apysc-2.8.7/apysc/_file/file_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_file/module_util.py` & `apysc-2.8.7/apysc/_file/module_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_bezier_2d.py` & `apysc-2.8.7/apysc/_geom/path_bezier_2d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_bezier_2d_continual.py` & `apysc-2.8.7/apysc/_geom/path_bezier_2d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_bezier_3d.py` & `apysc-2.8.7/apysc/_geom/path_bezier_3d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_bezier_3d_continual.py` & `apysc-2.8.7/apysc/_geom/path_bezier_3d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_close.py` & `apysc-2.8.7/apysc/_geom/path_close.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_control_x1_mixin.py` & `apysc-2.8.7/apysc/_geom/path_control_x1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_control_x2_mixin.py` & `apysc-2.8.7/apysc/_geom/path_control_x2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_control_x_mixin.py` & `apysc-2.8.7/apysc/_geom/path_control_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_control_y1_mixin.py` & `apysc-2.8.7/apysc/_geom/path_control_y1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_control_y2_mixin.py` & `apysc-2.8.7/apysc/_geom/path_control_y2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_control_y_mixin.py` & `apysc-2.8.7/apysc/_geom/path_control_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_data.py` & `apysc-2.8.7/apysc/_geom/path_data.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_data_base.py` & `apysc-2.8.7/apysc/_geom/path_data_base.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_data_util.py` & `apysc-2.8.7/apysc/_geom/path_data_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_dest_x_mixin.py` & `apysc-2.8.7/apysc/_geom/path_dest_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_dest_y_mixin.py` & `apysc-2.8.7/apysc/_geom/path_dest_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_horizontal.py` & `apysc-2.8.7/apysc/_geom/path_horizontal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_line_to.py` & `apysc-2.8.7/apysc/_geom/path_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_move_to.py` & `apysc-2.8.7/apysc/_geom/path_move_to.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_vertical.py` & `apysc-2.8.7/apysc/_geom/path_vertical.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_x_mixin.py` & `apysc-2.8.7/apysc/_geom/path_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/path_y_mixin.py` & `apysc-2.8.7/apysc/_geom/path_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/point2d.py` & `apysc-2.8.7/apysc/_geom/point2d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/rectangle_geom.py` & `apysc-2.8.7/apysc/_geom/rectangle_geom.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/rectangle_geom_bottom_y_mixin.py` & `apysc-2.8.7/apysc/_geom/rectangle_geom_bottom_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/rectangle_geom_center_x_mixin.py` & `apysc-2.8.7/apysc/_geom/rectangle_geom_center_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/rectangle_geom_center_y_mixin.py` & `apysc-2.8.7/apysc/_geom/rectangle_geom_center_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/rectangle_geom_height_mixin.py` & `apysc-2.8.7/apysc/_geom/rectangle_geom_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/rectangle_geom_left_x_mixin.py` & `apysc-2.8.7/apysc/_geom/rectangle_geom_left_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/rectangle_geom_right_x_mixin.py` & `apysc-2.8.7/apysc/_geom/rectangle_geom_right_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/rectangle_geom_top_y_mixin.py` & `apysc-2.8.7/apysc/_geom/rectangle_geom_top_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/rectangle_geom_width_mixin.py` & `apysc-2.8.7/apysc/_geom/rectangle_geom_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_geom/relative_mixin.py` & `apysc-2.8.7/apysc/_geom/relative_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_html/debug_mode.py` & `apysc-2.8.7/apysc/_html/debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_html/exporter.py` & `apysc-2.8.7/apysc/_html/exporter.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_html/html_util.py` & `apysc-2.8.7/apysc/_html/html_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_jslib/jquery-3.6.3.min.js` & `apysc-2.8.7/apysc/_jslib/jquery-3.6.3.min.js`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_jslib/jquery.mousewheel-3.1.13.min.js` & `apysc-2.8.7/apysc/_jslib/jquery.mousewheel-3.1.13.min.js`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_jslib/jslib_util.py` & `apysc-2.8.7/apysc/_jslib/jslib_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_jslib/svg-3.1.2.min.js` & `apysc-2.8.7/apysc/_jslib/svg-3.1.2.min.js`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_jslib/underscore-1.12.0.min.js` & `apysc-2.8.7/apysc/_jslib/underscore-1.12.0.min.js`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_jupyter/jupyter_util.py` & `apysc-2.8.7/apysc/_jupyter/jupyter_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py` & `apysc-2.8.7/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_lint_and_doc/conf_common.py` & `apysc-2.8.7/apysc/_lint_and_doc/conf_common.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_lint_and_doc/docs_keyword_link_mapping.py` & `apysc-2.8.7/apysc/_lint_and_doc/docs_keyword_link_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,8 +198,10 @@
     "get_bounds": "get_bounds",
     "RectangleGeom": "rectangle_geom",
     "to_string": "to_string",
     "range": "range",
     "lstrip": "string_lstrip",
     "strip": "string_strip",
     "rstrip": "string_rstrip",
+    "ForArrayIndices": "for_array_indices",
+    "ForArrayValues": "for_array_values",
 }
```

### Comparing `apysc-2.8.6/apysc/_lint_and_doc/docs_lang.py` & `apysc-2.8.7/apysc/_lint_and_doc/docs_lang.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_lint_and_doc/docs_toctree_util.py` & `apysc-2.8.7/apysc/_lint_and_doc/docs_toctree_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_lint_and_doc/docs_translation_converter.py` & `apysc-2.8.7/apysc/_lint_and_doc/docs_translation_converter.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_lint_and_doc/docstring_to_markdown_converter.py` & `apysc-2.8.7/apysc/_lint_and_doc/docstring_to_markdown_converter.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_lint_and_doc/docstring_util.py` & `apysc-2.8.7/apysc/_lint_and_doc/docstring_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_lint_and_doc/document_text_split_util.py` & `apysc-2.8.7/apysc/_lint_and_doc/document_text_split_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_lint_and_doc/document_util.py` & `apysc-2.8.7/apysc/_lint_and_doc/document_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py` & `apysc-2.8.7/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_lint_and_doc/fixed_translation_mapping/jp.py` & `apysc-2.8.7/apysc/_lint_and_doc/fixed_translation_mapping/jp.py`

 * *Files 0% similar despite different names*

```diff
@@ -3987,9 +3987,21 @@
             key="Why the apysc library doesn’t use the Python built-in data type",
             val="なぜapyscライブラリではPythonビルトインのデータ型を使っていないのか",
         ),
         Mapping(
             key="Each branch instruction class’s scope variable reverting setting",
             val="各分岐制御のクラスのスコープ内の変数値の復元設定",
         ),
+        Mapping(
+            key="## ForArrayValues API",
+            val="## ForArrayValues API",
+        ),
+        Mapping(
+            key="The loop implementation class for the `ap.Array` values.<hr>",
+            val="`ap.Array`の配列の値のためのループ処理のクラスです。<hr>",
+        ),
+        Mapping(
+            key="  - An array value type. This interface accepts apysc types, such as the `Int`, `String`, `Rectangle`.",
+            val="  - 配列の値の型。このインターフェイスは`Int`、`String`、`Rectangle`などのapyscの型を受け付けます。",
+        ),
     ]
 )
```

### Comparing `apysc-2.8.6/apysc/_lint_and_doc/lint_and_doc_hash_util.py` & `apysc-2.8.7/apysc/_lint_and_doc/lint_and_doc_hash_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_lint_and_doc/translation_mapping_utils.py` & `apysc-2.8.7/apysc/_lint_and_doc/translation_mapping_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_loop/_continue.py` & `apysc-2.8.7/apysc/_loop/_continue.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_loop/_for.py` & `apysc-2.8.7/apysc/_loop/_for.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_loop/_range.py` & `apysc-2.8.7/apysc/_loop/_range.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_loop/for_array_indices.py` & `apysc-2.8.7/apysc/_loop/for_array_indices.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """The loop implementation class for the `ap.Array` indices.
 """
 
 from typing import Any
 from typing import Dict
-from typing import Generic
 from typing import Optional
-from typing import TypeVar
 
 from typing_extensions import final
 
 from apysc._expression.get_last_scope_interface import GetLastScopeInterface
 from apysc._expression.indent_num import Indent
 from apysc._expression.last_scope import LastScope
 from apysc._html.debug_mode import add_debug_info_setting
 from apysc._loop.for_loop_exit_mixin import ForLoopExitMixIn
 from apysc._type.array import Array
+from apysc._type.initialize_locals_and_globals_mixin import (
+    InitializeLocalsAndGlobalsMixIn,
+)
 from apysc._type.int import Int
 from apysc._validation import arg_validation_decos
 
-_ArrValue = TypeVar("_ArrValue")
 
-
-class ForArrayIndices(Generic[_ArrValue], ForLoopExitMixIn, GetLastScopeInterface):
+class ForArrayIndices(
+    ForLoopExitMixIn,
+    GetLastScopeInterface,
+    InitializeLocalsAndGlobalsMixIn,
+):
     """
     The loop implementation class for the `ap.Array` indices.
 
     References
     ----------
     - ForArrayIndices class
         - https://simon-ritchie.github.io/apysc/en/for_array_indices.html
@@ -45,35 +48,35 @@
     >>> with ap.ForArrayIndices(arr=arr) as i:
     ...     indices.append(i)
     ...
 
     >>> _ = ap.assert_arrays_equal(indices, [0, 1, 2])
     """
 
-    _arr: Array[_ArrValue]
+    _arr: Array
     _variable_name_suffix: str
 
     @final
     @arg_validation_decos.is_apysc_array(arg_position_index=1)
     @arg_validation_decos.is_builtin_string(arg_position_index=4, optional=False)
     @add_debug_info_setting(module_name=__name__)
     def __init__(
         self,
-        arr: Array[_ArrValue],
+        arr: Array,
         *,
         locals_: Optional[Dict[str, Any]] = None,
         globals_: Optional[Dict[str, Any]] = None,
         variable_name_suffix: str = "",
     ) -> None:
         """
         The loop implementation class for the `ap.Array` indices.
 
         Parameters
         ----------
-        arr : Array[_ArrValue]
+        arr : Array
             An array to iterate.
         locals_ : Optional[Dict[str, Any]], optional
             Current scope's local variables. Set locals()
             value to this argument. If specified, this interface
             reverts all local scope VariableNameMixIn
             variables (like Int, Sprite) at the end of a with-statement
             scope. This setting is useful when you don't want to
@@ -105,21 +108,16 @@
         >>> indices: ap.Array[ap.Int] = ap.Array([])
         >>> with ap.ForArrayIndices(arr=arr) as i:
         ...     indices.append(i)
         ...
 
         >>> _ = ap.assert_arrays_equal(indices, [0, 1, 2])
         """
-        if locals_ is None:
-            locals_ = {}
-        if globals_ is None:
-            globals_ = {}
+        self._initialize_locals_and_globals(locals_=locals_, globals_=globals_)
         self._arr = arr
-        self._locals = locals_
-        self._globals = globals_
         self._variable_name_suffix = variable_name_suffix
         self._indent = Indent()
 
     @final
     @add_debug_info_setting(module_name=__name__)
     def __enter__(self) -> Int:
         """
```

### Comparing `apysc-2.8.6/apysc/_loop/for_loop_exit_mixin.py` & `apysc-2.8.7/apysc/_loop/for_loop_exit_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_loop/loop_count.py` & `apysc-2.8.7/apysc/_loop/loop_count.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_math/max_mixin.py` & `apysc-2.8.7/apysc/_math/max_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_math/min_mixin.py` & `apysc-2.8.7/apysc/_math/min_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_math/trunc_mixin.py` & `apysc-2.8.7/apysc/_math/trunc_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_string/indent_util.py` & `apysc-2.8.7/apysc/_string/indent_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_string/string_util.py` & `apysc-2.8.7/apysc/_string/string_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_testing/e2e_testing_helper.py` & `apysc-2.8.7/apysc/_testing/e2e_testing_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_testing/testing_helper.py` & `apysc-2.8.7/apysc/_testing/testing_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/datetime_.py` & `apysc-2.8.7/apysc/_time/datetime_.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/day_mixin.py` & `apysc-2.8.7/apysc/_time/day_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/days_mixin.py` & `apysc-2.8.7/apysc/_time/days_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/fps.py` & `apysc-2.8.7/apysc/_time/fps.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/hour_mixin.py` & `apysc-2.8.7/apysc/_time/hour_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/left_and_right_datetimes_mixin.py` & `apysc-2.8.7/apysc/_time/left_and_right_datetimes_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/millisecond_mixin.py` & `apysc-2.8.7/apysc/_time/millisecond_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/minute_mixin.py` & `apysc-2.8.7/apysc/_time/minute_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/month_end_mixin.py` & `apysc-2.8.7/apysc/_time/month_end_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/month_mixin.py` & `apysc-2.8.7/apysc/_time/month_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/now_mixin.py` & `apysc-2.8.7/apysc/_time/now_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/second_mixin.py` & `apysc-2.8.7/apysc/_time/second_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/timedelta_.py` & `apysc-2.8.7/apysc/_time/timedelta_.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/timer.py` & `apysc-2.8.7/apysc/_time/timer.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/total_seconds_mixin.py` & `apysc-2.8.7/apysc/_time/total_seconds_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/weekday_mixin.py` & `apysc-2.8.7/apysc/_time/weekday_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_time/year_mixin.py` & `apysc-2.8.7/apysc/_time/year_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/about_handler_options_type.py` & `apysc-2.8.7/apysc/_translation/jp/about_handler_options_type.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/add_child_and_remove_child.py` & `apysc-2.8.7/apysc/_translation/jp/add_child_and_remove_child.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/add_debug_info_setting.py` & `apysc-2.8.7/apysc/_translation/jp/add_debug_info_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_base_start.py` & `apysc-2.8.7/apysc/_translation/jp/animation_base_start.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_base_target.py` & `apysc-2.8.7/apysc/_translation/jp/animation_base_target.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_complete.py` & `apysc-2.8.7/apysc/_translation/jp/animation_complete.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_delay.py` & `apysc-2.8.7/apysc/_translation/jp/animation_delay.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_duration.py` & `apysc-2.8.7/apysc/_translation/jp/animation_duration.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_event.py` & `apysc-2.8.7/apysc/_translation/jp/animation_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_fill_alpha.py` & `apysc-2.8.7/apysc/_translation/jp/animation_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_fill_color.py` & `apysc-2.8.7/apysc/_translation/jp/animation_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_finish.py` & `apysc-2.8.7/apysc/_translation/jp/animation_finish.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_interfaces_abstract.py` & `apysc-2.8.7/apysc/_translation/jp/animation_interfaces_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_line_alpha.py` & `apysc-2.8.7/apysc/_translation/jp/animation_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_line_color.py` & `apysc-2.8.7/apysc/_translation/jp/animation_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_line_thickness.py` & `apysc-2.8.7/apysc/_translation/jp/animation_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_method_chaining.py` & `apysc-2.8.7/apysc/_translation/jp/animation_method_chaining.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_move.py` & `apysc-2.8.7/apysc/_translation/jp/animation_move.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_parallel.py` & `apysc-2.8.7/apysc/_translation/jp/animation_parallel.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_pause_and_play.py` & `apysc-2.8.7/apysc/_translation/jp/animation_pause_and_play.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_radius.py` & `apysc-2.8.7/apysc/_translation/jp/animation_radius.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_reset.py` & `apysc-2.8.7/apysc/_translation/jp/animation_reset.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_return_value.py` & `apysc-2.8.7/apysc/_translation/jp/animation_return_value.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_reverse.py` & `apysc-2.8.7/apysc/_translation/jp/animation_reverse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_rotation_around_center.py` & `apysc-2.8.7/apysc/_translation/jp/animation_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_rotation_around_point.py` & `apysc-2.8.7/apysc/_translation/jp/animation_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_scale_x_and_y_from_center.py` & `apysc-2.8.7/apysc/_translation/jp/animation_scale_x_and_y_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_scale_x_and_y_from_point.py` & `apysc-2.8.7/apysc/_translation/jp/animation_scale_x_and_y_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_time.py` & `apysc-2.8.7/apysc/_translation/jp/animation_time.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_width_and_height.py` & `apysc-2.8.7/apysc/_translation/jp/animation_width_and_height.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_x.py` & `apysc-2.8.7/apysc/_translation/jp/animation_x.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/animation_y.py` & `apysc-2.8.7/apysc/_translation/jp/animation_y.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/append_js_expression.py` & `apysc-2.8.7/apysc/_translation/jp/append_js_expression.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/array.py` & `apysc-2.8.7/apysc/_translation/jp/array.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/array_append_and_push.py` & `apysc-2.8.7/apysc/_translation/jp/array_append_and_push.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/array_clear.py` & `apysc-2.8.7/apysc/_translation/jp/array_clear.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/array_comparison.py` & `apysc-2.8.7/apysc/_translation/jp/array_comparison.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/array_extend_and_concat.py` & `apysc-2.8.7/apysc/_translation/jp/array_extend_and_concat.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/array_index_of.py` & `apysc-2.8.7/apysc/_translation/jp/array_index_of.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/array_insert_and_insert_at.py` & `apysc-2.8.7/apysc/_translation/jp/array_insert_and_insert_at.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/array_join.py` & `apysc-2.8.7/apysc/_translation/jp/array_join.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/array_length.py` & `apysc-2.8.7/apysc/_translation/jp/array_length.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/array_pop.py` & `apysc-2.8.7/apysc/_translation/jp/array_pop.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/array_remove_and_remove_at.py` & `apysc-2.8.7/apysc/_translation/jp/array_remove_and_remove_at.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/array_reverse.py` & `apysc-2.8.7/apysc/_translation/jp/array_reverse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/array_slice.py` & `apysc-2.8.7/apysc/_translation/jp/array_slice.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/array_sort.py` & `apysc-2.8.7/apysc/_translation/jp/array_sort.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py` & `apysc-2.8.7/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/assert_defined_and_undefined.py` & `apysc-2.8.7/apysc/_translation/jp/assert_defined_and_undefined.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py` & `apysc-2.8.7/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/assert_equal_and_not_equal.py` & `apysc-2.8.7/apysc/_translation/jp/assert_equal_and_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/assert_greater_and_greater_equal.py` & `apysc-2.8.7/apysc/_translation/jp/assert_greater_and_greater_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/assert_less_and_less_equal.py` & `apysc-2.8.7/apysc/_translation/jp/assert_less_and_less_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/assert_true_and_false.py` & `apysc-2.8.7/apysc/_translation/jp/assert_true_and_false.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/assertion_basic_behavior.py` & `apysc-2.8.7/apysc/_translation/jp/assertion_basic_behavior.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/bind_and_trigger_custom_event.py` & `apysc-2.8.7/apysc/_translation/jp/bind_and_trigger_custom_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/boolean.py` & `apysc-2.8.7/apysc/_translation/jp/boolean.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py` & `apysc-2.8.7/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/circle.py` & `apysc-2.8.7/apysc/_translation/jp/circle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/click.py` & `apysc-2.8.7/apysc/_translation/jp/click.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/contains.py` & `apysc-2.8.7/apysc/_translation/jp/contains.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/continue.py` & `apysc-2.8.7/apysc/_translation/jp/continue.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/datetime.py` & `apysc-2.8.7/apysc/_translation/jp/datetime.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/datetime_day.py` & `apysc-2.8.7/apysc/_translation/jp/datetime_day.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/datetime_hour.py` & `apysc-2.8.7/apysc/_translation/jp/datetime_hour.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/datetime_millisecond.py` & `apysc-2.8.7/apysc/_translation/jp/datetime_millisecond.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/datetime_minute.py` & `apysc-2.8.7/apysc/_translation/jp/datetime_minute.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/datetime_month.py` & `apysc-2.8.7/apysc/_translation/jp/datetime_month.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/datetime_now.py` & `apysc-2.8.7/apysc/_translation/jp/datetime_now.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/datetime_second.py` & `apysc-2.8.7/apysc/_translation/jp/datetime_second.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/datetime_set_month_end.py` & `apysc-2.8.7/apysc/_translation/jp/datetime_set_month_end.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py` & `apysc-2.8.7/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/datetime_year.py` & `apysc-2.8.7/apysc/_translation/jp/datetime_year.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/dblclick.py` & `apysc-2.8.7/apysc/_translation/jp/dblclick.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/delete.py` & `apysc-2.8.7/apysc/_translation/jp/delete.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/dictionary.py` & `apysc-2.8.7/apysc/_translation/jp/dictionary.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/dictionary_generic.py` & `apysc-2.8.7/apysc/_translation/jp/dictionary_generic.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/dictionary_get.py` & `apysc-2.8.7/apysc/_translation/jp/dictionary_get.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/dictionary_length.py` & `apysc-2.8.7/apysc/_translation/jp/dictionary_length.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/display_object.py` & `apysc-2.8.7/apysc/_translation/jp/display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py` & `apysc-2.8.7/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/display_object_get_and_set_css.py` & `apysc-2.8.7/apysc/_translation/jp/display_object_get_and_set_css.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/display_object_mouse_event.py` & `apysc-2.8.7/apysc/_translation/jp/display_object_mouse_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/display_object_parent.py` & `apysc-2.8.7/apysc/_translation/jp/display_object_parent.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/display_object_visible.py` & `apysc-2.8.7/apysc/_translation/jp/display_object_visible.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/display_object_x_and_y.py` & `apysc-2.8.7/apysc/_translation/jp/display_object_x_and_y.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/display_on_colaboratory.py` & `apysc-2.8.7/apysc/_translation/jp/display_on_colaboratory.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/display_on_jupyter.py` & `apysc-2.8.7/apysc/_translation/jp/display_on_jupyter.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/draw_interfaces_abstract.py` & `apysc-2.8.7/apysc/_translation/jp/draw_interfaces_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/easing_enum.py` & `apysc-2.8.7/apysc/_translation/jp/easing_enum.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/elif.py` & `apysc-2.8.7/apysc/_translation/jp/elif.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/ellipse.py` & `apysc-2.8.7/apysc/_translation/jp/ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/else.py` & `apysc-2.8.7/apysc/_translation/jp/else.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/enter_frame.py` & `apysc-2.8.7/apysc/_translation/jp/enter_frame.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py` & `apysc-2.8.7/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/for.py` & `apysc-2.8.7/apysc/_translation/jp/for.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/for_array_indices.py` & `apysc-2.8.7/apysc/_translation/jp/for_array_indices.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     ##################################################
     "**[Interface summary]**": "**[インターフェイス概要]**",
     ##################################################
     "The loop implementation class for the `ap.Array` indices.<hr>": "`ap.Array`のインデックス制御のためのループ制御用のクラスです。<hr>",  # noqa
     ##################################################
     "**[Parameters]**": "**[引数]**",
     ##################################################
-    "- `arr`: Array[_ArrValue]": "- `arr`: Array[_ArrValue]",
+    "- `arr`: Array]": "- `arr`: Array]",
     ##################################################
     "  - An array to iterate.": "  - イテレーションのための配列。",
     ##################################################
     "- `locals_`: Optional[Dict[str, Any]], optional": "- `locals_`: Optional[Dict[str, Any]], optional",  # noqa
     ##################################################
     "  - Current scope's local variables. Set locals() value to this argument. If specified, this interface reverts all local scope VariableNameMixIn variables (like Int, Sprite) at the end of a with-statement scope. This setting is useful when you don't want to update each variable.": "  - 現在のスコープの各ローカル変数。この引数にはlocals()関数の返却値を設定してください。もしこの引数が指定された場合、このインターフェイスはローカルスコープのVariableNameMixInの各変数（例 : IntやSpriteなど）の値をwithステートメントの最後で復元します。この設定は各変数を更新したくない場合等に役立ちます。",  # noqa
     ##################################################
```

### Comparing `apysc-2.8.6/apysc/_translation/jp/fps.py` & `apysc-2.8.7/apysc/_translation/jp/fps.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/fundamental_data_classes_value_interface.py` & `apysc-2.8.7/apysc/_translation/jp/fundamental_data_classes_value_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/get_bounds.py` & `apysc-2.8.7/apysc/_translation/jp/get_bounds.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/get_child_at.py` & `apysc-2.8.7/apysc/_translation/jp/get_child_at.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics.py` & `apysc-2.8.7/apysc/_translation/jp/graphics.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_fill_alpha.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_fill_color.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_flip_interfaces.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_flip_interfaces.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_line_alpha.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_line_color.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_line_dash_setting.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_line_dash_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_line_dot_setting.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_line_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_line_round_dot_setting.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_line_round_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_line_thickness.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_rotation_around_center.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_rotation_around_point.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_scale_from_center.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_scale_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_scale_from_point.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_scale_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_base_skew.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_base_skew.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_begin_fill.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_begin_fill.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_clear.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_clear.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_draw_circle.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_draw_circle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_draw_dash_dotted_line.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_draw_dash_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_draw_dashed_line.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_draw_dashed_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_draw_dotted_line.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_draw_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_draw_ellipse.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_draw_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_draw_line.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_draw_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_draw_path.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_draw_path.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_draw_polygon.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_draw_polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_draw_rect.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_draw_rect.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_draw_round_dotted_line.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_draw_round_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_draw_round_rect.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_draw_round_rect.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_draw_triangle.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_draw_triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_line_style.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_line_style.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/graphics_move_to_and_line_to.py` & `apysc-2.8.7/apysc/_translation/jp/graphics_move_to_and_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/if.py` & `apysc-2.8.7/apysc/_translation/jp/if.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/import_conventions.py` & `apysc-2.8.7/apysc/_translation/jp/import_conventions.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/index.py` & `apysc-2.8.7/apysc/_translation/jp/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     ##################################################
     "## Branch instruction": "## 条件分岐の制御",
     ##################################################
     "```{toctree}\n:maxdepth: 1\nif\nelif\nelse\nbranch_instruction_variables_reverting_setting\nreturn\n```": "```{toctree}\n:maxdepth: 1\njp_if\njp_elif\njp_else\njp_branch_instruction_variables_reverting_setting\njp_return\n```",  # noqa
     ##################################################
     "## Loop": "## ループ",
     ##################################################
-    "```{toctree}\n:maxdepth: 1\nfor\nfor_array_indices\ncontinue\nrange\n```": "```{toctree}\n:maxdepth: 1\njp_for\njp_for_array_indices\njp_continue\njp_range\n```",  # noqa
+    "```{toctree}\n:maxdepth: 1\nfor\nfor_array_indices\nfor_array_values\ncontinue\nrange\n```": "```{toctree}\n:maxdepth: 1\njp_for\njp_for_array_indices\njp_for_array_values\njp_continue\njp_range\n```",  # noqa
     ##################################################
     "## Timer and enter-frame": "## タイマーとenter-frame",
     ##################################################
     "```{toctree}\n:maxdepth: 1\ntimer\ntimer_event\ntimer_delay\nfps\ntimer_repeat_count\ntimer_start_and_stop\ntimer_complete\ntimer_reset\nenter_frame\nunbind_enter_frame_and_unbind_enter_frame_all\n```": "```{toctree}\n:maxdepth: 1\njp_timer\njp_timer_event\njp_timer_delay\njp_fps\njp_timer_repeat_count\njp_timer_start_and_stop\njp_timer_complete\njp_timer_reset\njp_enter_frame\njp_unbind_enter_frame_and_unbind_enter_frame_all\n```",  # noqa
     ##################################################
     "## DateTime class": "## DateTime クラス",
     ##################################################
```

### Comparing `apysc-2.8.6/apysc/_translation/jp/int_and_number.py` & `apysc-2.8.7/apysc/_translation/jp/int_and_number.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/int_and_number_arithmetic_operations.py` & `apysc-2.8.7/apysc/_translation/jp/int_and_number_arithmetic_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/int_and_number_comparison_operations.py` & `apysc-2.8.7/apysc/_translation/jp/int_and_number_comparison_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/int_and_number_to_fixed.py` & `apysc-2.8.7/apysc/_translation/jp/int_and_number_to_fixed.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/line.py` & `apysc-2.8.7/apysc/_translation/jp/line.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/math_max.py` & `apysc-2.8.7/apysc/_translation/jp/math_max.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/math_min.py` & `apysc-2.8.7/apysc/_translation/jp/math_min.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/math_trunc.py` & `apysc-2.8.7/apysc/_translation/jp/math_trunc.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/mouse_event_abstract.py` & `apysc-2.8.7/apysc/_translation/jp/mouse_event_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/mouse_event_basic.py` & `apysc-2.8.7/apysc/_translation/jp/mouse_event_basic.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/mousedown_and_mouseup.py` & `apysc-2.8.7/apysc/_translation/jp/mousedown_and_mouseup.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/mousemove.py` & `apysc-2.8.7/apysc/_translation/jp/mousemove.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/mouseover_and_mouseout.py` & `apysc-2.8.7/apysc/_translation/jp/mouseover_and_mouseout.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/num_children.py` & `apysc-2.8.7/apysc/_translation/jp/num_children.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/path.py` & `apysc-2.8.7/apysc/_translation/jp/path.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/path_bezier_2d.py` & `apysc-2.8.7/apysc/_translation/jp/path_bezier_2d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/path_bezier_2d_continual.py` & `apysc-2.8.7/apysc/_translation/jp/path_bezier_2d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/path_bezier_3d.py` & `apysc-2.8.7/apysc/_translation/jp/path_bezier_3d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/path_bezier_3d_continual.py` & `apysc-2.8.7/apysc/_translation/jp/path_bezier_3d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/path_close.py` & `apysc-2.8.7/apysc/_translation/jp/path_close.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/path_horizontal.py` & `apysc-2.8.7/apysc/_translation/jp/path_horizontal.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/path_line_to.py` & `apysc-2.8.7/apysc/_translation/jp/path_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/path_move_to.py` & `apysc-2.8.7/apysc/_translation/jp/path_move_to.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/path_vertical.py` & `apysc-2.8.7/apysc/_translation/jp/path_vertical.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/point2d.py` & `apysc-2.8.7/apysc/_translation/jp/point2d.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/polygon.py` & `apysc-2.8.7/apysc/_translation/jp/polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/polyline.py` & `apysc-2.8.7/apysc/_translation/jp/polyline.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/quick_start.py` & `apysc-2.8.7/apysc/_translation/jp/quick_start.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/range.py` & `apysc-2.8.7/apysc/_translation/jp/range.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/recommended_type_checker_settings.py` & `apysc-2.8.7/apysc/_translation/jp/recommended_type_checker_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/rectangle.py` & `apysc-2.8.7/apysc/_translation/jp/rectangle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/rectangle_geom.py` & `apysc-2.8.7/apysc/_translation/jp/rectangle_geom.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/remove_children.py` & `apysc-2.8.7/apysc/_translation/jp/remove_children.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/return.py` & `apysc-2.8.7/apysc/_translation/jp/return.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/save_overall_html.py` & `apysc-2.8.7/apysc/_translation/jp/save_overall_html.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/sequential_animation.py` & `apysc-2.8.7/apysc/_translation/jp/sequential_animation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/set_debug_mode.py` & `apysc-2.8.7/apysc/_translation/jp/set_debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/sprite.py` & `apysc-2.8.7/apysc/_translation/jp/sprite.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/stage.py` & `apysc-2.8.7/apysc/_translation/jp/stage.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/string.py` & `apysc-2.8.7/apysc/_translation/jp/string.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/string_addition_and_multiplication.py` & `apysc-2.8.7/apysc/_translation/jp/string_addition_and_multiplication.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/string_comparison_operations.py` & `apysc-2.8.7/apysc/_translation/jp/string_comparison_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/string_lstrip.py` & `apysc-2.8.7/apysc/_translation/jp/string_lstrip.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/string_rstrip.py` & `apysc-2.8.7/apysc/_translation/jp/string_rstrip.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/string_split.py` & `apysc-2.8.7/apysc/_translation/jp/string_split.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/string_strip.py` & `apysc-2.8.7/apysc/_translation/jp/string_strip.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/svg_text.py` & `apysc-2.8.7/apysc/_translation/jp/svg_text.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/svg_text_span.py` & `apysc-2.8.7/apysc/_translation/jp/svg_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/timedelta.py` & `apysc-2.8.7/apysc/_translation/jp/timedelta.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/timedelta_days.py` & `apysc-2.8.7/apysc/_translation/jp/timedelta_days.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/timedelta_total_seconds.py` & `apysc-2.8.7/apysc/_translation/jp/timedelta_total_seconds.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/timer.py` & `apysc-2.8.7/apysc/_translation/jp/timer.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/timer_complete.py` & `apysc-2.8.7/apysc/_translation/jp/timer_complete.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/timer_delay.py` & `apysc-2.8.7/apysc/_translation/jp/timer_delay.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/timer_event.py` & `apysc-2.8.7/apysc/_translation/jp/timer_event.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/timer_repeat_count.py` & `apysc-2.8.7/apysc/_translation/jp/timer_repeat_count.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/timer_reset.py` & `apysc-2.8.7/apysc/_translation/jp/timer_reset.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/timer_start_and_stop.py` & `apysc-2.8.7/apysc/_translation/jp/timer_start_and_stop.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/to_string.py` & `apysc-2.8.7/apysc/_translation/jp/to_string.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/trace.py` & `apysc-2.8.7/apysc/_translation/jp/trace.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/triangle.py` & `apysc-2.8.7/apysc/_translation/jp/triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py` & `apysc-2.8.7/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/unset_debug_mode.py` & `apysc-2.8.7/apysc/_translation/jp/unset_debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/variable_name_suffix.py` & `apysc-2.8.7/apysc/_translation/jp/variable_name_suffix.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/what_apysc_can_do.py` & `apysc-2.8.7/apysc/_translation/jp/what_apysc_can_do.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py` & `apysc-2.8.7/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/_delete.py` & `apysc-2.8.7/apysc/_type/_delete.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/_return.py` & `apysc-2.8.7/apysc/_type/_return.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/any_value.py` & `apysc-2.8.7/apysc/_type/any_value.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/array.py` & `apysc-2.8.7/apysc/_type/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from typing import TypeVar
 from typing import Union
 
 from typing_extensions import final
 
 from apysc._event.custom_event_mixin import CustomEventMixIn
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.boolean import Boolean
 from apysc._type.copy_mixin import CopyMixIn
 from apysc._type.initial_substitution_exp_mixin import InitialSubstitutionExpMixIn
 from apysc._type.int import Int
 from apysc._type.py_builtin_iter_disabling_mixin import PyBuiltInIterDisablingMixIn
 from apysc._type.revert_mixin import RevertMixIn
 from apysc._type.string import String
@@ -32,14 +35,15 @@
     ToStringMixIn,
     CopyMixIn,
     RevertMixIn,
     CustomEventMixIn,
     VariableNameSuffixMixIn,
     InitialSubstitutionExpMixIn,
     PyBuiltInIterDisablingMixIn,
+    InitializeForLoopValueInterface,
     Generic[_ArrValue],
 ):
     """
     Array class for the apysc library.
 
     References
     ----------
@@ -1504,7 +1508,20 @@
             Target snapshot name.
         """
         self._value = self._get_snapshot_val_if_exists(
             current_value=self._value,
             snapshot_dict=self._value_snapshots,
             snapshot_name=snapshot_name,
         )
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Array":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        arr_value : Array
+            An initialized array value.
+        """
+        return Array([])
```

### Comparing `apysc-2.8.6/apysc/_type/attr_linking_mixin.py` & `apysc-2.8.7/apysc/_type/attr_linking_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py` & `apysc-2.8.7/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/blank_object_mixin.py` & `apysc-2.8.7/apysc/_type/blank_object_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/boolean.py` & `apysc-2.8.7/apysc/_type/boolean.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from typing import Union
 
 from typing_extensions import Literal
 from typing_extensions import final
 
 from apysc._event.custom_event_mixin import CustomEventMixIn
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.copy_mixin import CopyMixIn
 from apysc._type.initial_substitution_exp_mixin import InitialSubstitutionExpMixIn
 from apysc._type.int import Int
 from apysc._type.revert_mixin import RevertMixIn
 from apysc._type.to_string_mixin import ToStringMixIn
 from apysc._type.variable_name_mixin import VariableNameMixIn
 from apysc._type.variable_name_suffix_mixin import VariableNameSuffixMixIn
@@ -24,15 +27,17 @@
 class Boolean(
     ToStringMixIn,
     CopyMixIn,
     RevertMixIn,
     CustomEventMixIn,
     VariableNameSuffixMixIn,
     InitialSubstitutionExpMixIn,
+    InitializeForLoopValueInterface,
 ):
+
     """
     Boolean class for the apysc library.
 
     Notes
     -----
     The Bool class is the alias of the Boolean, and it behaves
     the same as the Boolean class.
@@ -522,7 +527,20 @@
         result : Boolean
             A result Boolean value.
         """
         import apysc as ap
 
         expression: str = f"{result.variable_name} = " f"!{self.variable_name};"
         ap.append_js_expression(expression=expression)
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Boolean":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        bool_value : Boolean
+            An initialized boolean value.
+        """
+        return Boolean(False)
```

### Comparing `apysc-2.8.6/apysc/_type/copy_mixin.py` & `apysc-2.8.7/apysc/_type/copy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/deleted_object_mixin.py` & `apysc-2.8.7/apysc/_type/deleted_object_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/dictionary.py` & `apysc-2.8.7/apysc/_type/dictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 from typing import TypeVar
 from typing import Union
 
 from typing_extensions import final
 
 from apysc._event.custom_event_mixin import CustomEventMixIn
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.any_value import AnyValue
 from apysc._type.boolean import Boolean
 from apysc._type.copy_mixin import CopyMixIn
 from apysc._type.dictionary_structure import DictionaryStructure
 from apysc._type.expression_string import ExpressionString
 from apysc._type.initial_substitution_exp_mixin import InitialSubstitutionExpMixIn
 from apysc._type.int import Int
@@ -32,21 +35,22 @@
 _BuiltinKeys = Union[str, int, float]
 _Key = TypeVar("_Key")
 _Value = TypeVar("_Value")
 
 
 class Dictionary(
     CustomEventMixIn,
-    Generic[_Key, _Value],
     CopyMixIn,
     RevertMixIn,
     DictionaryStructure,
     VariableNameSuffixMixIn,
     InitialSubstitutionExpMixIn,
     PyBuiltInIterDisablingMixIn,
+    InitializeForLoopValueInterface,
+    Generic[_Key, _Value],
 ):
     """
     Dictionary class for the apysc library.
 
     References
     ----------
     - Dictionary
@@ -746,7 +750,20 @@
             f"if ({key_str} in {self.variable_name}) {{"
             f"\n  {result_value_str} = {self.variable_name}[{key_str}];"
             "\n}else {"
             f"\n  {result_value_str} = {default_value_str};"
             "\n}"
         )
         ap.append_js_expression(expression=expression)
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Dictionary":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        dict_val : Dictionary
+            An initialized dictionary value.
+        """
+        return Dictionary({})
```

### Comparing `apysc-2.8.6/apysc/_type/expression_string.py` & `apysc-2.8.7/apysc/_type/expression_string.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/initial_substitution_exp_mixin.py` & `apysc-2.8.7/apysc/_type/initial_substitution_exp_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/int.py` & `apysc-2.8.7/apysc/_type/int.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,26 @@
 """
 
 from typing import Union
 
 from typing_extensions import final
 
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.number_value_mixin import NumberValueMixIn
 from apysc._type.to_fixed_mixin import ToFixedMixIn
 from apysc._type.to_string_mixin import ToStringMixIn
 from apysc._validation import arg_validation_decos
 
 
 class Int(
     NumberValueMixIn[int, "Int"],
+    InitializeForLoopValueInterface,
     ToStringMixIn,
     ToFixedMixIn,
 ):
     """
     Integer class for the apysc library.
 
     References
@@ -191,7 +195,20 @@
             Representation string of this instance.
         """
         if not hasattr(self, "_value"):
             repr_str: str = "Int(0)"
         else:
             repr_str = f"Int({self._value})"
         return repr_str
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Int":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        int_value : Int
+            An initialized integer value.
+        """
+        return Int(0)
```

### Comparing `apysc-2.8.6/apysc/_type/number.py` & `apysc-2.8.7/apysc/_type/number.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,26 @@
 
 from typing import Any
 from typing import Union
 
 from typing_extensions import final
 
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.number_value_mixin import NumberValueMixIn
 from apysc._type.to_fixed_mixin import ToFixedMixIn
 from apysc._type.to_string_mixin import ToStringMixIn
 from apysc._validation import arg_validation_decos
 
 
 class Number(
     NumberValueMixIn[float, "Number"],
+    InitializeForLoopValueInterface,
     ToStringMixIn,
     ToFixedMixIn,
 ):
     """
     Floating point number class for the apysc library.
 
     Notes
@@ -172,7 +176,20 @@
             Representation string of this instance.
         """
         if not hasattr(self, "_value"):
             repr_str: str = "Number(0)"
         else:
             repr_str = f"Number({self._value})"
         return repr_str
+
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "Number":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        num_value : Number
+            An initialized number value.
+        """
+        return Number(0)
```

### Comparing `apysc-2.8.6/apysc/_type/number_value_mixin.py` & `apysc-2.8.7/apysc/_type/number_value_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Class implementation for number value mix-in.
 """
 
-from abc import ABC
 from abc import abstractmethod
 from typing import Any
 from typing import Dict
 from typing import Generic
 from typing import Optional
 from typing import TypeVar
 from typing import Union
@@ -29,15 +28,14 @@
 class NumberValueMixIn(
     CopyMixIn,
     RevertMixIn,
     CustomEventMixIn,
     VariableNameSuffixMixIn,
     InitialSubstitutionExpMixIn,
     Generic[_ValueType, _InstanceType],
-    ABC,
 ):
 
     _initial_value: _NumType
     _value: _ValueType
 
     @arg_validation_decos.is_num(arg_position_index=1, optional=False)
     @add_debug_info_setting(module_name=__name__)
```

### Comparing `apysc-2.8.6/apysc/_type/py_builtin_iter_disabling_mixin.py` & `apysc-2.8.7/apysc/_type/py_builtin_iter_disabling_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/revert_interface.py` & `apysc-2.8.7/apysc/_type/revert_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/revert_mixin.py` & `apysc-2.8.7/apysc/_type/revert_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/string.py` & `apysc-2.8.7/apysc/_type/string.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from typing import Optional
 from typing import Union
 
 from typing_extensions import final
 
 from apysc._event.custom_event_mixin import CustomEventMixIn
 from apysc._html.debug_mode import add_debug_info_setting
+from apysc._loop.initialize_for_loop_value_interface import (
+    InitializeForLoopValueInterface,
+)
 from apysc._type.copy_mixin import CopyMixIn
 from apysc._type.initial_substitution_exp_mixin import InitialSubstitutionExpMixIn
 from apysc._type.revert_mixin import RevertMixIn
 from apysc._type.string_lstrip_mixin import StringLStripMixIn
 from apysc._type.string_rstrip_mixin import StringRStripMixIn
 from apysc._type.string_split_mixin import StringSplitMixIn
 from apysc._type.string_strip_mixin import StringStripMixIn
@@ -28,14 +31,15 @@
     StringStripMixIn,
     StringRStripMixIn,
     CopyMixIn,
     RevertMixIn,
     CustomEventMixIn,
     VariableNameSuffixMixIn,
     InitialSubstitutionExpMixIn,
+    InitializeForLoopValueInterface,
 ):
     """
     String class for apysc library.
 
     Notes
     -----
     The `Str` class is the alias of `String`.
@@ -835,14 +839,27 @@
         """
         self._value = self._get_snapshot_val_if_exists(
             current_value=self._value,
             snapshot_dict=self._value_snapshots,
             snapshot_name=snapshot_name,
         )
 
+    @classmethod
+    @final
+    def _initialize_for_loop_value(cls) -> "String":
+        """
+        Initialize this instance for a loop value.
+
+        Returns
+        -------
+        str_value : String
+            An initialized string value.
+        """
+        return String("")
+
 
 def _escape_str_value(*, value: Union[str, "String"]) -> Union[str, "String"]:
     """
     Escape a specified string value.
 
     Notes
     -----
```

### Comparing `apysc-2.8.6/apysc/_type/string_lstrip_mixin.py` & `apysc-2.8.7/apysc/_type/string_lstrip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/string_rstrip_mixin.py` & `apysc-2.8.7/apysc/_type/string_rstrip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/string_split_mixin.py` & `apysc-2.8.7/apysc/_type/string_split_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/string_strip_mixin.py` & `apysc-2.8.7/apysc/_type/string_strip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/to_fixed_mixin.py` & `apysc-2.8.7/apysc/_type/to_fixed_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/to_string_mixin.py` & `apysc-2.8.7/apysc/_type/to_string_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/type_util.py` & `apysc-2.8.7/apysc/_type/type_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/value_util.py` & `apysc-2.8.7/apysc/_type/value_util.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/variable_name_mixin.py` & `apysc-2.8.7/apysc/_type/variable_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/variable_name_suffix_attr_or_var_mixin.py` & `apysc-2.8.7/apysc/_type/variable_name_suffix_attr_or_var_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/variable_name_suffix_mixin.py` & `apysc-2.8.7/apysc/_type/variable_name_suffix_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_type/variable_name_suffix_utils.py` & `apysc-2.8.7/apysc/_type/variable_name_suffix_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_validation/arg_validation_decos.py` & `apysc-2.8.7/apysc/_validation/arg_validation_decos.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,17 @@
         is the `XAxisLabelPosition`.
 - is_y_axis_label_position
     - Set a validation to check a specified argument's type
         is the `YAxisLabelPosition`.
 - is_list_or_array_matrix_data
     - Set a validation to check a specified argument's type
         is list of dicts or `ap.Array` of `ap.Dictionary`.
+- is_initialize_for_loop_value_interface_subclass
+    - Set a validation to check a specified class is
+        the `InitializeForLoopValueInterface`'s subclas.
 """
 
 import functools
 import inspect
 from inspect import Signature
 from typing import Any
 from typing import Callable
@@ -3252,7 +3255,55 @@
                 f"`ap.Array` of `ap.Dictionary`: {type(matrix_data).__name__}, "
                 f"\n{callable_and_arg_names_msg}"
             )
 
         return inner_wrapped  # type: ignore
 
     return wrapped  # type: ignore
+
+
+def is_initialize_for_loop_value_interface_subclass(
+    *, arg_position_index: int
+) -> _Callable:
+    """
+    Set a validation to check a specified class is
+    the `InitializeForLoopValueInterface`'s subclas.
+
+    Parameters
+    ----------
+    arg_position_index : int
+        A target argument position index.
+
+    Returns
+    -------
+    wrapped : Callable
+        Wrapped callable object.
+    """
+
+    def wrapped(callable_: _Callable) -> _Callable:
+        @functools.wraps(callable_)
+        def inner_wrapped(*args: Any, **kwargs: Any) -> Any:
+            from apysc._loop.initialize_for_loop_value_interface import (
+                InitializeForLoopValueInterface,
+            )
+
+            class_: Any = _extract_arg_value(
+                args=args,
+                kwargs=kwargs,
+                arg_position_index=arg_position_index,
+                callable_=callable_,
+            )
+            if issubclass(class_, InitializeForLoopValueInterface):
+                return callable_(*args, **kwargs)
+
+            callable_and_arg_names_msg: str = _get_callable_and_arg_names_msg(
+                callable_=callable_, arg_position_index=arg_position_index
+            )
+            raise TypeError(
+                f"A specified class is not an `InitializeForLoopValueInterface`'s "
+                f"subclass: {class_}"
+                f"\n{callable_and_arg_names_msg}"
+            )
+
+        return inner_wrapped  # type: ignore
+
+    return wrapped  # type: ignore
```

### Comparing `apysc-2.8.6/apysc/_validation/bool_validation.py` & `apysc-2.8.7/apysc/_validation/bool_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_validation/color_validation.py` & `apysc-2.8.7/apysc/_validation/color_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_validation/display_validation.py` & `apysc-2.8.7/apysc/_validation/display_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_validation/event_validation.py` & `apysc-2.8.7/apysc/_validation/event_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_validation/geom_validation.py` & `apysc-2.8.7/apysc/_validation/geom_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_validation/handler_validation.py` & `apysc-2.8.7/apysc/_validation/handler_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_validation/matrix_data_validation.py` & `apysc-2.8.7/apysc/_validation/matrix_data_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_validation/number_validation.py` & `apysc-2.8.7/apysc/_validation/number_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_validation/parent_validation.py` & `apysc-2.8.7/apysc/_validation/parent_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_validation/path_validation.py` & `apysc-2.8.7/apysc/_validation/path_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_validation/string_validation.py` & `apysc-2.8.7/apysc/_validation/string_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_validation/validation_common_utils.py` & `apysc-2.8.7/apysc/_validation/validation_common_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc/_validation/variable_name_validation.py` & `apysc-2.8.7/apysc/_validation/variable_name_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-2.8.6/apysc.egg-info/PKG-INFO` & `apysc-2.8.7/apysc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apysc
-Version: 2.8.6
+Version: 2.8.7
 Summary: apysc is the Python's frontend library to create html and js file, that has the ActionScript 3 (as3)-like interface.
 Home-page: https://github.com/simon-ritchie/apysc
 Maintainer: simon-ritchie
 Maintainer-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apysc-2.8.6/apysc.egg-info/SOURCES.txt` & `apysc-2.8.7/apysc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,17 @@
 apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
 apysc/_lint_and_doc/fixed_translation_mapping/jp.py
 apysc/_loop/__init__.py
 apysc/_loop/_continue.py
 apysc/_loop/_for.py
 apysc/_loop/_range.py
 apysc/_loop/for_array_indices.py
+apysc/_loop/for_array_values.py
 apysc/_loop/for_loop_exit_mixin.py
+apysc/_loop/initialize_for_loop_value_interface.py
 apysc/_loop/loop_count.py
 apysc/_math/__init__.py
 apysc/_math/math.py
 apysc/_math/max_mixin.py
 apysc/_math/min_mixin.py
 apysc/_math/trunc_mixin.py
 apysc/_string/__init__.py
@@ -484,14 +486,15 @@
 apysc/_translation/jp/elif.py
 apysc/_translation/jp/ellipse.py
 apysc/_translation/jp/else.py
 apysc/_translation/jp/enter_frame.py
 apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
 apysc/_translation/jp/for.py
 apysc/_translation/jp/for_array_indices.py
+apysc/_translation/jp/for_array_values.py
 apysc/_translation/jp/fps.py
 apysc/_translation/jp/fundamental_data_classes_value_interface.py
 apysc/_translation/jp/get_bounds.py
 apysc/_translation/jp/get_child_at.py
 apysc/_translation/jp/graphics.py
 apysc/_translation/jp/graphics_base_fill_alpha.py
 apysc/_translation/jp/graphics_base_fill_color.py
@@ -604,14 +607,15 @@
 apysc/_type/boolean.py
 apysc/_type/copy_mixin.py
 apysc/_type/deleted_object_mixin.py
 apysc/_type/dictionary.py
 apysc/_type/dictionary_structure.py
 apysc/_type/expression_string.py
 apysc/_type/initial_substitution_exp_mixin.py
+apysc/_type/initialize_locals_and_globals_mixin.py
 apysc/_type/int.py
 apysc/_type/number.py
 apysc/_type/number_value_mixin.py
 apysc/_type/py_builtin_iter_disabling_mixin.py
 apysc/_type/repr_interface.py
 apysc/_type/revert_interface.py
 apysc/_type/revert_mixin.py
```

