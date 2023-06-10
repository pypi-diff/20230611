# Comparing `tmp/mpl_format-0.316.tar.gz` & `tmp/mpl_format-0.317.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_format-0.316.tar", last modified: Fri May 26 22:05:47 2023, max compression
+gzip compressed data, was "mpl_format-0.317.tar", last modified: Sat Jun 10 23:04:56 2023, max compression
```

## Comparing `mpl_format-0.316.tar` & `mpl_format-0.317.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.956600 mpl_format-0.316/
--rw-rw-rw-   0        0        0     1080 2022-01-23 23:53:12.000000 mpl_format-0.316/LICENSE.txt
--rw-rw-rw-   0        0        0      473 2023-05-26 22:05:47.956600 mpl_format-0.316/PKG-INFO
--rw-rw-rw-   0        0        0      156 2022-01-23 23:53:12.000000 mpl_format-0.316/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.461277 mpl_format-0.316/mpl_format/
--rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.500621 mpl_format-0.316/mpl_format/animation/
--rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.514863 mpl_format-0.316/mpl_format/animation/animators/
--rw-rw-rw-   0        0        0       41 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/animators/__init__.py
--rw-rw-rw-   0        0        0     1125 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/animators/axes_animator.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.534863 mpl_format-0.316/mpl_format/animation/kwarg_animations/
--rw-rw-rw-   0        0        0       90 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/kwarg_animations/__init__.py
--rw-rw-rw-   0        0        0     4070 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/kwarg_animations/color_animation.py
--rw-rw-rw-   0        0        0     4970 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/kwarg_animations/float_animation.py
--rw-rw-rw-   0        0        0      864 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/rate.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.609495 mpl_format-0.316/mpl_format/animation/shapes/
--rw-rw-rw-   0        0        0      387 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/shapes/__init__.py
--rw-rw-rw-   0        0        0     3272 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/shapes/arc_animation.py
--rw-rw-rw-   0        0        0     2807 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/shapes/arrow_animation.py
--rw-rw-rw-   0        0        0     1558 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/shapes/base.py
--rw-rw-rw-   0        0        0     2639 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/shapes/circle_animation.py
--rw-rw-rw-   0        0        0     2871 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/shapes/ellipse_animation.py
--rw-rw-rw-   0        0        0     4032 2023-05-26 22:01:30.000000 mpl_format-0.316/mpl_format/animation/shapes/line_animation.py
--rw-rw-rw-   0        0        0     3676 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/shapes/rectangle_animation.py
--rw-rw-rw-   0        0        0     2856 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/shapes/regular_polygon_animation.py
--rw-rw-rw-   0        0        0     4190 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/shapes/text_animation.py
--rw-rw-rw-   0        0        0     3015 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/shapes/wedge_animation.py
--rw-rw-rw-   0        0        0      461 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/animation/type_animations.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.652719 mpl_format-0.316/mpl_format/axes/
--rw-rw-rw-   0        0        0      314 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/axes/__init__.py
--rw-rw-rw-   0        0        0   112188 2023-05-26 22:01:06.000000 mpl_format-0.316/mpl_format/axes/axes_formatter.py
--rw-rw-rw-   0        0        0     1141 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/axes/axes_formatter_array.py
--rw-rw-rw-   0        0        0    15475 2022-10-29 21:01:39.000000 mpl_format-0.316/mpl_format/axes/axis_formatter.py
--rw-rw-rw-   0        0        0     9782 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/axes/axis_formatter_array.py
--rw-rw-rw-   0        0        0      413 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/axes/axis_utils.py
--rw-rw-rw-   0        0        0    14010 2023-05-26 21:58:25.000000 mpl_format-0.316/mpl_format/axes/ticks_formatter.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.668030 mpl_format-0.316/mpl_format/colors/
--rw-rw-rw-   0        0        0      163 2022-10-29 21:01:39.000000 mpl_format-0.316/mpl_format/colors/__init__.py
--rw-rw-rw-   0        0        0     1688 2023-05-26 21:46:47.000000 mpl_format-0.316/mpl_format/colors/color_maps.py
--rw-rw-rw-   0        0        0     5671 2022-10-29 21:01:39.000000 mpl_format-0.316/mpl_format/colors/office.py
--rw-rw-rw-   0        0        0     3196 2023-05-26 22:01:06.000000 mpl_format-0.316/mpl_format/compound_types.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.801619 mpl_format-0.316/mpl_format/enums/
--rw-rw-rw-   0        0        0      698 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/__init__.py
--rw-rw-rw-   0        0        0     1113 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/arrow_style.py
--rw-rw-rw-   0        0        0     1152 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/box_style.py
--rw-rw-rw-   0        0        0      389 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/cap_style.py
--rw-rw-rw-   0        0        0      686 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/connection_style.py
--rw-rw-rw-   0        0        0      751 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/draw_style.py
--rw-rw-rw-   0        0        0      775 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/font_size.py
--rw-rw-rw-   0        0        0     1053 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/font_stretch.py
--rw-rw-rw-   0        0        0      404 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/font_style.py
--rw-rw-rw-   0        0        0      553 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/font_variant.py
--rw-rw-rw-   0        0        0     1145 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/font_weight.py
--rw-rw-rw-   0        0        0      395 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/join_style.py
--rw-rw-rw-   0        0        0      618 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/line_style.py
--rw-rw-rw-   0        0        0      648 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/mappings.py
--rw-rw-rw-   0        0        0     2439 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/enums/marker_style.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.819769 mpl_format-0.316/mpl_format/figures/
--rw-rw-rw-   0        0        0       65 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/figures/__init__.py
--rw-rw-rw-   0        0        0    30493 2023-05-26 21:58:33.000000 mpl_format-0.316/mpl_format/figures/figure_formatter.py
--rw-rw-rw-   0        0        0        6 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/figures/figure_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.830770 mpl_format-0.316/mpl_format/legend/
--rw-rw-rw-   0        0        0       64 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/legend/__init__.py
--rw-rw-rw-   0        0        0    17325 2023-05-26 21:58:25.000000 mpl_format-0.316/mpl_format/legend/legend_formatter.py
--rw-rw-rw-   0        0        0      706 2023-05-26 21:46:47.000000 mpl_format-0.316/mpl_format/literals.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.857499 mpl_format-0.316/mpl_format/patches/
--rw-rw-rw-   0        0        0       72 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/patches/__init__.py
--rw-rw-rw-   0        0        0      981 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/patches/arc_list_formatter.py
--rw-rw-rw-   0        0        0     2781 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/patches/patch_list_formatter.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.872960 mpl_format-0.316/mpl_format/plots/
--rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/plots/__init__.py
--rw-rw-rw-   0        0        0    10229 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/plots/density.py
--rw-rw-rw-   0        0        0       43 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.902639 mpl_format-0.316/mpl_format/text/
--rw-rw-rw-   0        0        0      125 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/text/__init__.py
--rw-rw-rw-   0        0        0     8104 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/text/text_formatter.py
--rw-rw-rw-   0        0        0     5287 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/text/text_list_formatter.py
--rw-rw-rw-   0        0        0     2366 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/text/text_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.931088 mpl_format-0.316/mpl_format/utils/
--rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/utils/__init__.py
--rw-rw-rw-   0        0        0      386 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/utils/arg_checks.py
--rw-rw-rw-   0        0        0     2825 2022-10-29 21:01:39.000000 mpl_format-0.316/mpl_format/utils/arg_transforms.py
--rw-rw-rw-   0        0        0     2157 2023-05-26 21:58:25.000000 mpl_format-0.316/mpl_format/utils/color_utils.py
--rw-rw-rw-   0        0        0     2054 2022-01-23 23:53:12.000000 mpl_format-0.316/mpl_format/utils/io_utils.py
--rw-rw-rw-   0        0        0     1220 2023-05-26 21:58:25.000000 mpl_format-0.316/mpl_format/utils/number_utils.py
--rw-rw-rw-   0        0        0      890 2023-05-26 22:01:06.000000 mpl_format-0.316/mpl_format/utils/type_checks.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.486673 mpl_format-0.316/mpl_format.egg-info/
--rw-rw-rw-   0        0        0      473 2023-05-26 22:05:47.000000 mpl_format-0.316/mpl_format.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2817 2023-05-26 22:05:47.000000 mpl_format-0.316/mpl_format.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 22:05:47.000000 mpl_format-0.316/mpl_format.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 22:05:47.000000 mpl_format-0.316/mpl_format.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-26 22:05:47.000000 mpl_format-0.316/mpl_format.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-26 22:05:47.958057 mpl_format-0.316/setup.cfg
--rw-rw-rw-   0        0        0      757 2023-05-26 22:04:23.000000 mpl_format-0.316/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.948263 mpl_format-0.316/tests/
--rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.316/tests/__init__.py
--rw-rw-rw-   0        0        0     4256 2022-01-23 23:53:12.000000 mpl_format-0.316/tests/test_axis_formatter.py
--rw-rw-rw-   0        0        0      385 2022-01-23 23:53:12.000000 mpl_format-0.316/tests/test_figure_formatter.py
-drwxrwxrwx   0        0        0        0 2023-05-26 22:05:47.955596 mpl_format-0.316/tests/test_text/
--rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.316/tests/test_text/__init__.py
--rw-rw-rw-   0        0        0     1363 2022-01-23 23:53:12.000000 mpl_format-0.316/tests/test_text/test_text_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.393500 mpl_format-0.317/
+-rw-rw-rw-   0        0        0     1080 2022-01-23 23:53:12.000000 mpl_format-0.317/LICENSE.txt
+-rw-rw-rw-   0        0        0      473 2023-06-10 23:04:56.393500 mpl_format-0.317/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2022-01-23 23:53:12.000000 mpl_format-0.317/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:55.853360 mpl_format-0.317/mpl_format/
+-rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:55.900635 mpl_format-0.317/mpl_format/animation/
+-rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:55.918632 mpl_format-0.317/mpl_format/animation/animators/
+-rw-rw-rw-   0        0        0       41 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/animators/__init__.py
+-rw-rw-rw-   0        0        0     1125 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/animators/axes_animator.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:55.947787 mpl_format-0.317/mpl_format/animation/kwarg_animations/
+-rw-rw-rw-   0        0        0       90 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/kwarg_animations/__init__.py
+-rw-rw-rw-   0        0        0     4070 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/kwarg_animations/color_animation.py
+-rw-rw-rw-   0        0        0     4970 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/kwarg_animations/float_animation.py
+-rw-rw-rw-   0        0        0      864 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/rate.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.058596 mpl_format-0.317/mpl_format/animation/shapes/
+-rw-rw-rw-   0        0        0      387 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/__init__.py
+-rw-rw-rw-   0        0        0     3272 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/arc_animation.py
+-rw-rw-rw-   0        0        0     2807 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/arrow_animation.py
+-rw-rw-rw-   0        0        0     1558 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/base.py
+-rw-rw-rw-   0        0        0     2639 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/circle_animation.py
+-rw-rw-rw-   0        0        0     2871 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/ellipse_animation.py
+-rw-rw-rw-   0        0        0     4032 2023-05-26 22:01:30.000000 mpl_format-0.317/mpl_format/animation/shapes/line_animation.py
+-rw-rw-rw-   0        0        0     3676 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/rectangle_animation.py
+-rw-rw-rw-   0        0        0     2856 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/regular_polygon_animation.py
+-rw-rw-rw-   0        0        0     4190 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/text_animation.py
+-rw-rw-rw-   0        0        0     3015 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/shapes/wedge_animation.py
+-rw-rw-rw-   0        0        0      461 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/animation/type_animations.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.090695 mpl_format-0.317/mpl_format/axes/
+-rw-rw-rw-   0        0        0      314 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/axes/__init__.py
+-rw-rw-rw-   0        0        0   112188 2023-05-26 22:01:06.000000 mpl_format-0.317/mpl_format/axes/axes_formatter.py
+-rw-rw-rw-   0        0        0     1141 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/axes/axes_formatter_array.py
+-rw-rw-rw-   0        0        0    15475 2022-10-29 21:01:39.000000 mpl_format-0.317/mpl_format/axes/axis_formatter.py
+-rw-rw-rw-   0        0        0     9782 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/axes/axis_formatter_array.py
+-rw-rw-rw-   0        0        0      413 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/axes/axis_utils.py
+-rw-rw-rw-   0        0        0    14000 2023-06-10 22:56:32.000000 mpl_format-0.317/mpl_format/axes/ticks_formatter.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.106324 mpl_format-0.317/mpl_format/colors/
+-rw-rw-rw-   0        0        0      163 2022-10-29 21:01:39.000000 mpl_format-0.317/mpl_format/colors/__init__.py
+-rw-rw-rw-   0        0        0     1688 2023-05-26 21:46:47.000000 mpl_format-0.317/mpl_format/colors/color_maps.py
+-rw-rw-rw-   0        0        0     5671 2022-10-29 21:01:39.000000 mpl_format-0.317/mpl_format/colors/office.py
+-rw-rw-rw-   0        0        0     3209 2023-06-10 22:55:58.000000 mpl_format-0.317/mpl_format/compound_types.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.233989 mpl_format-0.317/mpl_format/enums/
+-rw-rw-rw-   0        0        0      698 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/__init__.py
+-rw-rw-rw-   0        0        0     1113 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/arrow_style.py
+-rw-rw-rw-   0        0        0     1152 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/box_style.py
+-rw-rw-rw-   0        0        0      389 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/cap_style.py
+-rw-rw-rw-   0        0        0      686 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/connection_style.py
+-rw-rw-rw-   0        0        0      751 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/draw_style.py
+-rw-rw-rw-   0        0        0      775 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/font_size.py
+-rw-rw-rw-   0        0        0     1053 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/font_stretch.py
+-rw-rw-rw-   0        0        0      404 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/font_style.py
+-rw-rw-rw-   0        0        0      553 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/font_variant.py
+-rw-rw-rw-   0        0        0     1145 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/font_weight.py
+-rw-rw-rw-   0        0        0      395 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/join_style.py
+-rw-rw-rw-   0        0        0      618 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/line_style.py
+-rw-rw-rw-   0        0        0      648 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/mappings.py
+-rw-rw-rw-   0        0        0     2439 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/enums/marker_style.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.265605 mpl_format-0.317/mpl_format/figures/
+-rw-rw-rw-   0        0        0       65 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/figures/__init__.py
+-rw-rw-rw-   0        0        0    30493 2023-05-26 21:58:33.000000 mpl_format-0.317/mpl_format/figures/figure_formatter.py
+-rw-rw-rw-   0        0        0        6 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/figures/figure_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.275303 mpl_format-0.317/mpl_format/legend/
+-rw-rw-rw-   0        0        0       64 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/legend/__init__.py
+-rw-rw-rw-   0        0        0    17325 2023-05-26 21:58:25.000000 mpl_format-0.317/mpl_format/legend/legend_formatter.py
+-rw-rw-rw-   0        0        0      706 2023-05-26 21:46:47.000000 mpl_format-0.317/mpl_format/literals.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.297647 mpl_format-0.317/mpl_format/patches/
+-rw-rw-rw-   0        0        0       72 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/patches/__init__.py
+-rw-rw-rw-   0        0        0      981 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/patches/arc_list_formatter.py
+-rw-rw-rw-   0        0        0     2781 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/patches/patch_list_formatter.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.313714 mpl_format-0.317/mpl_format/plots/
+-rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/plots/__init__.py
+-rw-rw-rw-   0        0        0    10229 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/plots/density.py
+-rw-rw-rw-   0        0        0       43 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.345413 mpl_format-0.317/mpl_format/text/
+-rw-rw-rw-   0        0        0      125 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/text/__init__.py
+-rw-rw-rw-   0        0        0     8104 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/text/text_formatter.py
+-rw-rw-rw-   0        0        0     5287 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/text/text_list_formatter.py
+-rw-rw-rw-   0        0        0     2366 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/text/text_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.381492 mpl_format-0.317/mpl_format/utils/
+-rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/utils/__init__.py
+-rw-rw-rw-   0        0        0      386 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/utils/arg_checks.py
+-rw-rw-rw-   0        0        0     2825 2022-10-29 21:01:39.000000 mpl_format-0.317/mpl_format/utils/arg_transforms.py
+-rw-rw-rw-   0        0        0     2157 2023-05-26 21:58:25.000000 mpl_format-0.317/mpl_format/utils/color_utils.py
+-rw-rw-rw-   0        0        0     2054 2022-01-23 23:53:12.000000 mpl_format-0.317/mpl_format/utils/io_utils.py
+-rw-rw-rw-   0        0        0     1210 2023-06-10 22:56:32.000000 mpl_format-0.317/mpl_format/utils/number_utils.py
+-rw-rw-rw-   0        0        0      890 2023-05-26 22:01:06.000000 mpl_format-0.317/mpl_format/utils/type_checks.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:55.878458 mpl_format-0.317/mpl_format.egg-info/
+-rw-rw-rw-   0        0        0      473 2023-06-10 23:04:55.000000 mpl_format-0.317/mpl_format.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2817 2023-06-10 23:04:55.000000 mpl_format-0.317/mpl_format.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 23:04:55.000000 mpl_format-0.317/mpl_format.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 23:04:55.000000 mpl_format-0.317/mpl_format.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-10 23:04:55.000000 mpl_format-0.317/mpl_format.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-10 23:04:56.409447 mpl_format-0.317/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-06-10 23:04:05.000000 mpl_format-0.317/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.393500 mpl_format-0.317/tests/
+-rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.317/tests/__init__.py
+-rw-rw-rw-   0        0        0     4256 2022-01-23 23:53:12.000000 mpl_format-0.317/tests/test_axis_formatter.py
+-rw-rw-rw-   0        0        0      385 2022-01-23 23:53:12.000000 mpl_format-0.317/tests/test_figure_formatter.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:04:56.393500 mpl_format-0.317/tests/test_text/
+-rw-rw-rw-   0        0        0        0 2022-01-23 23:53:12.000000 mpl_format-0.317/tests/test_text/__init__.py
+-rw-rw-rw-   0        0        0     1363 2022-01-23 23:53:12.000000 mpl_format-0.317/tests/test_text/test_text_utils.py
```

### Comparing `mpl_format-0.316/LICENSE.txt` & `mpl_format-0.317/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/animation/animators/axes_animator.py` & `mpl_format-0.317/mpl_format/animation/animators/axes_animator.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/animation/kwarg_animations/color_animation.py` & `mpl_format-0.317/mpl_format/animation/kwarg_animations/color_animation.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/animation/kwarg_animations/float_animation.py` & `mpl_format-0.317/mpl_format/animation/kwarg_animations/float_animation.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/animation/rate.py` & `mpl_format-0.317/mpl_format/animation/rate.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/animation/shapes/arc_animation.py` & `mpl_format-0.317/mpl_format/animation/shapes/arc_animation.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/animation/shapes/arrow_animation.py` & `mpl_format-0.317/mpl_format/animation/shapes/arrow_animation.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/animation/shapes/base.py` & `mpl_format-0.317/mpl_format/animation/shapes/base.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/animation/shapes/circle_animation.py` & `mpl_format-0.317/mpl_format/animation/shapes/circle_animation.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/animation/shapes/ellipse_animation.py` & `mpl_format-0.317/mpl_format/animation/shapes/ellipse_animation.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/animation/shapes/line_animation.py` & `mpl_format-0.317/mpl_format/animation/shapes/line_animation.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/animation/shapes/rectangle_animation.py` & `mpl_format-0.317/mpl_format/animation/shapes/rectangle_animation.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/animation/shapes/regular_polygon_animation.py` & `mpl_format-0.317/mpl_format/animation/shapes/regular_polygon_animation.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/animation/shapes/text_animation.py` & `mpl_format-0.317/mpl_format/animation/shapes/text_animation.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/animation/shapes/wedge_animation.py` & `mpl_format-0.317/mpl_format/animation/shapes/wedge_animation.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/axes/axes_formatter.py` & `mpl_format-0.317/mpl_format/axes/axes_formatter.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/axes/axes_formatter_array.py` & `mpl_format-0.317/mpl_format/axes/axes_formatter_array.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/axes/axis_formatter.py` & `mpl_format-0.317/mpl_format/axes/axis_formatter.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/axes/axis_formatter_array.py` & `mpl_format-0.317/mpl_format/axes/axis_formatter_array.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/axes/ticks_formatter.py` & `mpl_format-0.317/mpl_format/axes/ticks_formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import date
 from itertools import product
 from typing import Union, List, Tuple, Iterator, Iterable, Callable
 
 import matplotlib.pyplot as plt
-from mpl_format.compound_types.built_ins import FloatIterable
+from mpl_format.compound_types import FloatIterable
 from matplotlib.axes import Axes
 from matplotlib.axis import Axis
 
 from mpl_format.compound_types import Color, FontSize, StringMapper
 from mpl_format.enums import FONT_SIZE
 from mpl_format.enums.line_style import LINE_STYLE
 from mpl_format.literals import WHICH_TICKS, WHICH_AXIS
```

### Comparing `mpl_format-0.316/mpl_format/colors/color_maps.py` & `mpl_format-0.317/mpl_format/colors/color_maps.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/colors/office.py` & `mpl_format-0.317/mpl_format/colors/office.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/compound_types.py` & `mpl_format-0.317/mpl_format/compound_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.patches import Patch
 from matplotlib.path import Path
 from numpy import ndarray
 from seaborn import JointGrid, PairGrid
-from typing import TypeVar, Tuple, Union, Dict, Callable, Iterable
+from typing import TypeVar, Tuple, Union, Dict, Callable, Iterable, List, Sized
 
 from mpl_format.enums import FONT_SIZE, FONT_STRETCH, FONT_WEIGHT, FONT_STYLE, \
     FONT_VARIANT, CAP_STYLE, JOIN_STYLE, LINE_STYLE, ARROW_STYLE, \
     CONNECTION_STYLE
 from mpl_format.enums.box_style import BoxStyleType
 
 # built-ins
```

### Comparing `mpl_format-0.316/mpl_format/enums/__init__.py` & `mpl_format-0.317/mpl_format/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/enums/arrow_style.py` & `mpl_format-0.317/mpl_format/enums/arrow_style.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/enums/box_style.py` & `mpl_format-0.317/mpl_format/enums/box_style.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/enums/connection_style.py` & `mpl_format-0.317/mpl_format/enums/connection_style.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/enums/draw_style.py` & `mpl_format-0.317/mpl_format/enums/draw_style.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/enums/font_size.py` & `mpl_format-0.317/mpl_format/enums/font_size.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/enums/font_stretch.py` & `mpl_format-0.317/mpl_format/enums/font_stretch.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/enums/font_variant.py` & `mpl_format-0.317/mpl_format/enums/font_variant.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/enums/font_weight.py` & `mpl_format-0.317/mpl_format/enums/font_weight.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/enums/line_style.py` & `mpl_format-0.317/mpl_format/enums/line_style.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/enums/mappings.py` & `mpl_format-0.317/mpl_format/enums/mappings.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/enums/marker_style.py` & `mpl_format-0.317/mpl_format/enums/marker_style.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/figures/figure_formatter.py` & `mpl_format-0.317/mpl_format/figures/figure_formatter.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/legend/legend_formatter.py` & `mpl_format-0.317/mpl_format/legend/legend_formatter.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/literals.py` & `mpl_format-0.317/mpl_format/literals.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/patches/arc_list_formatter.py` & `mpl_format-0.317/mpl_format/patches/arc_list_formatter.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/patches/patch_list_formatter.py` & `mpl_format-0.317/mpl_format/patches/patch_list_formatter.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/plots/density.py` & `mpl_format-0.317/mpl_format/plots/density.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/text/text_formatter.py` & `mpl_format-0.317/mpl_format/text/text_formatter.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/text/text_list_formatter.py` & `mpl_format-0.317/mpl_format/text/text_list_formatter.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/text/text_utils.py` & `mpl_format-0.317/mpl_format/text/text_utils.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/utils/arg_transforms.py` & `mpl_format-0.317/mpl_format/utils/arg_transforms.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/utils/color_utils.py` & `mpl_format-0.317/mpl_format/utils/color_utils.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/utils/io_utils.py` & `mpl_format-0.317/mpl_format/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format/utils/number_utils.py` & `mpl_format-0.317/mpl_format/utils/number_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from mpl_format.compound_types.built_ins import Scalar
+from mpl_format.compound_types import Scalar
 
 
 def format_as_integer(number: Scalar, kmbt: bool = False) -> str:
     """
     Format a number as an integer, with comma separators and an optional suffix
     of K, M, B or T for large numbers.
```

### Comparing `mpl_format-0.316/mpl_format/utils/type_checks.py` & `mpl_format-0.317/mpl_format/utils/type_checks.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/mpl_format.egg-info/SOURCES.txt` & `mpl_format-0.317/mpl_format.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/setup.py` & `mpl_format-0.317/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='mpl_format',
     packages=find_packages(),
-    version='0.316',
+    version='0.317',
     license='MIT',
     description='Library for easier formatting of matplotlib plots written in '
                 'a functional style.',
     author='Vahndi Minah',
     url='https://github.com/vahndi/mpl-format',
     keywords=['matplotlib'],
     install_requires=[
```

### Comparing `mpl_format-0.316/tests/test_axis_formatter.py` & `mpl_format-0.317/tests/test_axis_formatter.py`

 * *Files identical despite different names*

### Comparing `mpl_format-0.316/tests/test_text/test_text_utils.py` & `mpl_format-0.317/tests/test_text/test_text_utils.py`

 * *Files identical despite different names*

