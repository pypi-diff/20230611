# Comparing `tmp/pedal-2.4.2.tar.gz` & `tmp/pedal-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedal-2.4.2.tar", last modified: Mon May 22 16:55:56 2023, max compression
+gzip compressed data, was "pedal-2.5.1.tar", last modified: Sun Jun 11 14:14:30 2023, max compression
```

## Comparing `pedal-2.4.2.tar` & `pedal-2.5.1.tar`

### file list

```diff
@@ -1,154 +1,156 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.905905 pedal-2.4.2/
--rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.4.2/LICENSE
--rw-rw-rw-   0        0        0     2981 2023-05-22 16:55:56.905905 pedal-2.4.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.777901 pedal-2.4.2/Pedal.egg-info/
--rw-rw-rw-   0        0        0     2981 2023-05-22 16:55:56.000000 pedal-2.4.2/Pedal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3702 2023-05-22 16:55:56.000000 pedal-2.4.2/Pedal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:55:56.000000 pedal-2.4.2/Pedal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-22 16:55:56.000000 pedal-2.4.2/Pedal.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 16:55:56.000000 pedal-2.4.2/Pedal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 16:55:56.000000 pedal-2.4.2/Pedal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1958 2023-05-18 18:40:27.000000 pedal-2.4.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.774889 pedal-2.4.2/pedal/
--rw-rw-rw-   0        0        0      382 2023-05-18 18:14:23.000000 pedal-2.4.2/pedal/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.788890 pedal-2.4.2/pedal/assertions/
--rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/assertions/__init__.py
--rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.4.2/pedal/assertions/classes.py
--rw-rw-rw-   0        0        0    13288 2023-01-17 17:53:58.000000 pedal-2.4.2/pedal/assertions/commands.py
--rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/assertions/constants.py
--rw-rw-rw-   0        0        0    20378 2022-09-17 21:23:34.000000 pedal-2.4.2/pedal/assertions/feedbacks.py
--rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.4.2/pedal/assertions/functions.py
--rw-rw-rw-   0        0        0     5722 2021-01-26 15:12:38.000000 pedal-2.4.2/pedal/assertions/organizers.py
--rw-rw-rw-   0        0        0    33479 2023-01-17 17:50:34.000000 pedal-2.4.2/pedal/assertions/runtime.py
--rw-rw-rw-   0        0        0     3254 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/assertions/setup.py
--rw-rw-rw-   0        0        0    30229 2022-11-17 14:15:37.000000 pedal-2.4.2/pedal/assertions/static.py
--rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/assertions/unittest.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.797891 pedal-2.4.2/pedal/cait/
--rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.4.2/pedal/cait/__init__.py
--rw-rw-rw-   0        0        0     2254 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/cait/ast_helpers.py
--rw-rw-rw-   0        0        0    11371 2021-03-12 21:12:46.000000 pedal-2.4.2/pedal/cait/ast_map.py
--rw-rw-rw-   0        0        0    10523 2021-01-08 04:00:46.000000 pedal-2.4.2/pedal/cait/cait_api.py
--rw-rw-rw-   0        0        0    22471 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/cait/cait_node.py
--rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/cait/constants.py
--rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.4.2/pedal/cait/find_node.py
--rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.4.2/pedal/cait/stretchy_tree_matching.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.803891 pedal-2.4.2/pedal/command_line/
--rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/command_line/__init__.py
--rw-rw-rw-   0        0        0     7897 2022-04-30 18:25:37.000000 pedal-2.4.2/pedal/command_line/command_line.py
--rw-rw-rw-   0        0        0     7493 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/command_line/mocks.py
--rw-rw-rw-   0        0        0    25271 2022-11-11 18:14:58.000000 pedal-2.4.2/pedal/command_line/modes.py
--rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.4.2/pedal/command_line/report.py
--rw-rw-rw-   0        0        0     3540 2020-11-08 16:28:36.000000 pedal-2.4.2/pedal/command_line/verify.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.818888 pedal-2.4.2/pedal/core/
--rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/core/__init__.py
--rw-rw-rw-   0        0        0     9298 2023-05-22 16:32:35.000000 pedal-2.4.2/pedal/core/commands.py
--rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/core/environment.py
--rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/core/errors.py
--rw-rw-rw-   0        0        0    20881 2023-01-17 17:46:13.000000 pedal-2.4.2/pedal/core/feedback.py
--rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/core/feedback_category.py
--rw-rw-rw-   0        0        0     6107 2022-11-17 14:35:13.000000 pedal-2.4.2/pedal/core/final_feedback.py
--rw-rw-rw-   0        0        0     7639 2023-01-17 17:14:11.000000 pedal-2.4.2/pedal/core/formatting.py
--rw-rw-rw-   0        0        0     1915 2022-06-12 19:44:51.000000 pedal-2.4.2/pedal/core/location.py
--rw-rw-rw-   0        0        0    13385 2022-11-28 05:44:51.000000 pedal-2.4.2/pedal/core/report.py
--rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/core/resolver.py
--rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.4.2/pedal/core/scoring.py
--rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.4.2/pedal/core/submission.py
--rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/core/tag.py
--rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.4.2/pedal/core/tool.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.827887 pedal-2.4.2/pedal/environments/
--rw-rw-rw-   0        0        0      657 2020-11-08 17:16:23.000000 pedal-2.4.2/pedal/environments/__init__.py
--rw-rw-rw-   0        0        0     3042 2021-02-26 19:18:08.000000 pedal-2.4.2/pedal/environments/blockpy.py
--rw-rw-rw-   0        0        0     9569 2022-11-23 18:26:45.000000 pedal-2.4.2/pedal/environments/gradescope.py
--rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.4.2/pedal/environments/jupyter.py
--rw-rw-rw-   0        0        0    10351 2021-02-02 16:30:22.000000 pedal-2.4.2/pedal/environments/nbgrader.py
--rw-rw-rw-   0        0        0      368 2020-11-08 17:19:12.000000 pedal-2.4.2/pedal/environments/none.py
--rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/environments/sandbox.py
--rw-rw-rw-   0        0        0     3651 2023-04-19 22:17:37.000000 pedal-2.4.2/pedal/environments/standard.py
--rw-rw-rw-   0        0        0     6259 2020-11-13 04:58:08.000000 pedal-2.4.2/pedal/environments/vpl.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.831887 pedal-2.4.2/pedal/extensions/
--rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/extensions/__init__.py
--rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.4.2/pedal/extensions/microbit.py
--rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.4.2/pedal/extensions/plotting.py
--rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.4.2/pedal/extensions/turtles.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.841892 pedal-2.4.2/pedal/questions/
--rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.4.2/pedal/questions/__init__.py
--rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/questions/constants.py
--rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.4.2/pedal/questions/feedbacks.py
--rw-rw-rw-   0        0        0     6045 2022-11-16 17:32:45.000000 pedal-2.4.2/pedal/questions/graders.py
--rw-rw-rw-   0        0        0     3477 2021-12-05 16:42:01.000000 pedal-2.4.2/pedal/questions/loader.py
--rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.4.2/pedal/questions/pool.py
--rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.4.2/pedal/questions/questions.py
--rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.4.2/pedal/questions/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.849889 pedal-2.4.2/pedal/resolvers/
--rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.4.2/pedal/resolvers/__init__.py
--rw-rw-rw-   0        0        0      654 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/resolvers/core.py
--rw-rw-rw-   0        0        0     2099 2023-05-13 15:07:02.000000 pedal-2.4.2/pedal/resolvers/full.py
--rw-rw-rw-   0        0        0     1886 2022-11-23 18:27:16.000000 pedal-2.4.2/pedal/resolvers/sectional.py
--rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.4.2/pedal/resolvers/silent.py
--rw-rw-rw-   0        0        0     5119 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/resolvers/simple.py
--rw-rw-rw-   0        0        0     1176 2020-11-03 17:24:20.000000 pedal-2.4.2/pedal/resolvers/statistics.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.859906 pedal-2.4.2/pedal/sandbox/
--rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.4.2/pedal/sandbox/__init__.py
--rw-rw-rw-   0        0        0    17919 2023-05-18 18:30:27.000000 pedal-2.4.2/pedal/sandbox/commands.py
--rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/sandbox/constants.py
--rw-rw-rw-   0        0        0     9652 2023-05-13 15:13:44.000000 pedal-2.4.2/pedal/sandbox/data.py
--rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.4.2/pedal/sandbox/exceptions.py
--rw-rw-rw-   0        0        0    10750 2022-10-04 22:22:33.000000 pedal-2.4.2/pedal/sandbox/feedbacks.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.864905 pedal-2.4.2/pedal/sandbox/library/
--rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.4.2/pedal/sandbox/library/__init__.py
--rw-rw-rw-   0        0        0     5028 2022-08-18 18:00:00.000000 pedal-2.4.2/pedal/sandbox/library/designer.py
--rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.4.2/pedal/sandbox/library/matplotlib.py
--rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.4.2/pedal/sandbox/library/microbit.py
--rw-rw-rw-   0        0        0     3400 2022-07-28 21:17:36.000000 pedal-2.4.2/pedal/sandbox/library/turtles.py
--rw-rw-rw-   0        0        0    10124 2023-05-22 15:55:11.000000 pedal-2.4.2/pedal/sandbox/mocked.py
--rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.4.2/pedal/sandbox/result.py
--rw-rw-rw-   0        0        0    38840 2023-05-22 14:40:28.000000 pedal-2.4.2/pedal/sandbox/sandbox.py
--rw-rw-rw-   0        0        0     5048 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/sandbox/timeout.py
--rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.4.2/pedal/sandbox/tracer.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.870905 pedal-2.4.2/pedal/source/
--rw-rw-rw-   0        0        0      912 2022-07-24 20:13:29.000000 pedal-2.4.2/pedal/source/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/source/constants.py
--rw-rw-rw-   0        0        0     5345 2022-10-04 00:04:29.000000 pedal-2.4.2/pedal/source/feedbacks.py
--rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/source/sections.py
--rw-rw-rw-   0        0        0     7441 2022-11-23 18:29:38.000000 pedal-2.4.2/pedal/source/source.py
--rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/source/substitutions.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.880906 pedal-2.4.2/pedal/tifa/
--rw-rw-rw-   0        0        0     3049 2022-11-28 05:46:58.000000 pedal-2.4.2/pedal/tifa/__init__.py
--rw-rw-rw-   0        0        0     2143 2022-10-06 14:36:45.000000 pedal-2.4.2/pedal/tifa/commands.py
--rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/tifa/constants.py
--rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.4.2/pedal/tifa/contexts.py
--rw-rw-rw-   0        0        0    23656 2023-05-22 16:40:08.000000 pedal-2.4.2/pedal/tifa/feedbacks.py
--rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/tifa/identifier.py
--rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.4.2/pedal/tifa/settings.py
--rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.4.2/pedal/tifa/state.py
--rw-rw-rw-   0        0        0    24173 2022-10-07 14:11:04.000000 pedal-2.4.2/pedal/tifa/tifa_core.py
--rw-rw-rw-   0        0        0    42489 2023-05-22 16:39:10.000000 pedal-2.4.2/pedal/tifa/tifa_visitor.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.885906 pedal-2.4.2/pedal/types/
--rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.4.2/pedal/types/__init__.py
--rw-rw-rw-   0        0        0     9115 2022-11-28 06:00:50.000000 pedal-2.4.2/pedal/types/builtin.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.892906 pedal-2.4.2/pedal/types/library/
--rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.4.2/pedal/types/library/__init__.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.4.2/pedal/types/library/cs1_curriculum.py
--rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.4.2/pedal/types/library/designer.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.4.2/pedal/types/library/matplotlib.py
--rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.4.2/pedal/types/library/microbit.py
--rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.4.2/pedal/types/library/turtles.py
--rw-rw-rw-   0        0        0    51752 2022-11-28 05:43:22.000000 pedal-2.4.2/pedal/types/new_types.py
--rw-rw-rw-   0        0        0    14813 2022-11-23 18:45:05.000000 pedal-2.4.2/pedal/types/normalize.py
--rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.4.2/pedal/types/operations.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:55:56.904905 pedal-2.4.2/pedal/utilities/
--rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/utilities/__init__.py
--rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.4.2/pedal/utilities/ast_tools.py
--rw-rw-rw-   0        0        0     6580 2022-07-27 17:31:05.000000 pedal-2.4.2/pedal/utilities/comparisons.py
--rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/utilities/dictionaries.py
--rw-rw-rw-   0        0        0     8300 2022-09-23 12:51:56.000000 pedal-2.4.2/pedal/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.4.2/pedal/utilities/files.py
--rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/utilities/operators.py
--rw-rw-rw-   0        0        0     7037 2022-12-31 17:53:00.000000 pedal-2.4.2/pedal/utilities/progsnap.py
--rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/utilities/sorting.py
--rw-rw-rw-   0        0        0      326 2021-06-28 19:25:31.000000 pedal-2.4.2/pedal/utilities/system.py
--rw-rw-rw-   0        0        0     2313 2022-07-27 16:49:13.000000 pedal-2.4.2/pedal/utilities/text.py
--rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.4.2/pedal/utilities/types.py
--rw-rw-rw-   0        0        0      121 2023-05-22 16:55:56.906905 pedal-2.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1196 2023-05-22 16:26:30.000000 pedal-2.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.832032 pedal-2.5.1/
+-rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.5.1/LICENSE
+-rw-rw-rw-   0        0        0     2564 2023-06-11 14:14:30.832032 pedal-2.5.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.662032 pedal-2.5.1/Pedal.egg-info/
+-rw-rw-rw-   0        0        0     2564 2023-06-11 14:14:30.000000 pedal-2.5.1/Pedal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3759 2023-06-11 14:14:30.000000 pedal-2.5.1/Pedal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 14:14:30.000000 pedal-2.5.1/Pedal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-11 14:14:30.000000 pedal-2.5.1/Pedal.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-11 14:14:30.000000 pedal-2.5.1/Pedal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-11 14:14:30.000000 pedal-2.5.1/Pedal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1958 2023-05-18 18:40:27.000000 pedal-2.5.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.660032 pedal-2.5.1/pedal/
+-rw-rw-rw-   0        0        0      382 2023-05-18 18:14:23.000000 pedal-2.5.1/pedal/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.679032 pedal-2.5.1/pedal/assertions/
+-rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/assertions/__init__.py
+-rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.5.1/pedal/assertions/classes.py
+-rw-rw-rw-   0        0        0    13288 2023-01-17 17:53:58.000000 pedal-2.5.1/pedal/assertions/commands.py
+-rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/assertions/constants.py
+-rw-rw-rw-   0        0        0    20355 2023-05-27 15:44:30.000000 pedal-2.5.1/pedal/assertions/feedbacks.py
+-rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.5.1/pedal/assertions/functions.py
+-rw-rw-rw-   0        0        0     5722 2021-01-26 15:12:38.000000 pedal-2.5.1/pedal/assertions/organizers.py
+-rw-rw-rw-   0        0        0    33752 2023-05-22 19:35:19.000000 pedal-2.5.1/pedal/assertions/runtime.py
+-rw-rw-rw-   0        0        0     3254 2023-05-26 21:11:25.000000 pedal-2.5.1/pedal/assertions/setup.py
+-rw-rw-rw-   0        0        0    30229 2023-05-26 20:52:09.000000 pedal-2.5.1/pedal/assertions/static.py
+-rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/assertions/unittest.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.689033 pedal-2.5.1/pedal/cait/
+-rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.5.1/pedal/cait/__init__.py
+-rw-rw-rw-   0        0        0     2255 2023-05-27 15:47:12.000000 pedal-2.5.1/pedal/cait/ast_helpers.py
+-rw-rw-rw-   0        0        0    11371 2021-03-12 21:12:46.000000 pedal-2.5.1/pedal/cait/ast_map.py
+-rw-rw-rw-   0        0        0    10523 2021-01-08 04:00:46.000000 pedal-2.5.1/pedal/cait/cait_api.py
+-rw-rw-rw-   0        0        0    22471 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/cait/cait_node.py
+-rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/cait/constants.py
+-rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.5.1/pedal/cait/find_node.py
+-rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.5.1/pedal/cait/stretchy_tree_matching.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.697032 pedal-2.5.1/pedal/command_line/
+-rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/command_line/__init__.py
+-rw-rw-rw-   0        0        0     7897 2022-04-30 18:25:37.000000 pedal-2.5.1/pedal/command_line/command_line.py
+-rw-rw-rw-   0        0        0     7301 2023-05-27 15:42:09.000000 pedal-2.5.1/pedal/command_line/mocks.py
+-rw-rw-rw-   0        0        0    24491 2023-05-26 20:56:48.000000 pedal-2.5.1/pedal/command_line/modes.py
+-rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.5.1/pedal/command_line/report.py
+-rw-rw-rw-   0        0        0     3540 2020-11-08 16:28:36.000000 pedal-2.5.1/pedal/command_line/verify.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.717032 pedal-2.5.1/pedal/core/
+-rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/core/__init__.py
+-rw-rw-rw-   0        0        0     9342 2023-05-26 21:10:34.000000 pedal-2.5.1/pedal/core/commands.py
+-rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/core/environment.py
+-rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/core/errors.py
+-rw-rw-rw-   0        0        0    21081 2023-06-09 14:02:52.000000 pedal-2.5.1/pedal/core/feedback.py
+-rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/core/feedback_category.py
+-rw-rw-rw-   0        0        0     7383 2023-05-26 21:59:43.000000 pedal-2.5.1/pedal/core/final_feedback.py
+-rw-rw-rw-   0        0        0     8008 2023-06-10 15:13:23.000000 pedal-2.5.1/pedal/core/formatting.py
+-rw-rw-rw-   0        0        0     1962 2023-05-26 21:48:15.000000 pedal-2.5.1/pedal/core/location.py
+-rw-rw-rw-   0        0        0    13385 2022-11-28 05:44:51.000000 pedal-2.5.1/pedal/core/report.py
+-rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/core/resolver.py
+-rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.5.1/pedal/core/scoring.py
+-rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.5.1/pedal/core/submission.py
+-rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/core/tag.py
+-rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.5.1/pedal/core/tool.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.729031 pedal-2.5.1/pedal/environments/
+-rw-rw-rw-   0        0        0      658 2023-05-27 15:45:02.000000 pedal-2.5.1/pedal/environments/__init__.py
+-rw-rw-rw-   0        0        0     3060 2023-05-26 21:12:20.000000 pedal-2.5.1/pedal/environments/blockpy.py
+-rw-rw-rw-   0        0        0     9587 2023-05-26 21:13:02.000000 pedal-2.5.1/pedal/environments/gradescope.py
+-rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.5.1/pedal/environments/jupyter.py
+-rw-rw-rw-   0        0        0    10369 2023-05-26 21:13:02.000000 pedal-2.5.1/pedal/environments/nbgrader.py
+-rw-rw-rw-   0        0        0      369 2023-06-08 11:46:52.000000 pedal-2.5.1/pedal/environments/none.py
+-rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/environments/sandbox.py
+-rw-rw-rw-   0        0        0     3684 2023-05-26 21:13:56.000000 pedal-2.5.1/pedal/environments/standard.py
+-rw-rw-rw-   0        0        0     2605 2023-06-09 12:58:17.000000 pedal-2.5.1/pedal/environments/terminal.py
+-rw-rw-rw-   0        0        0     6423 2023-06-08 18:48:18.000000 pedal-2.5.1/pedal/environments/vpl.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.735033 pedal-2.5.1/pedal/extensions/
+-rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/extensions/__init__.py
+-rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.5.1/pedal/extensions/microbit.py
+-rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.5.1/pedal/extensions/plotting.py
+-rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.5.1/pedal/extensions/turtles.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.744032 pedal-2.5.1/pedal/questions/
+-rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.5.1/pedal/questions/__init__.py
+-rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/questions/constants.py
+-rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.5.1/pedal/questions/feedbacks.py
+-rw-rw-rw-   0        0        0     6043 2023-05-27 15:45:43.000000 pedal-2.5.1/pedal/questions/graders.py
+-rw-rw-rw-   0        0        0     3477 2023-05-26 21:13:56.000000 pedal-2.5.1/pedal/questions/loader.py
+-rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.5.1/pedal/questions/pool.py
+-rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.5.1/pedal/questions/questions.py
+-rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.5.1/pedal/questions/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.754032 pedal-2.5.1/pedal/resolvers/
+-rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.5.1/pedal/resolvers/__init__.py
+-rw-rw-rw-   0        0        0      650 2023-05-27 15:45:59.000000 pedal-2.5.1/pedal/resolvers/core.py
+-rw-rw-rw-   0        0        0     1504 2023-05-26 21:58:00.000000 pedal-2.5.1/pedal/resolvers/export.py
+-rw-rw-rw-   0        0        0     1753 2023-05-26 21:21:28.000000 pedal-2.5.1/pedal/resolvers/full.py
+-rw-rw-rw-   0        0        0     1545 2023-05-26 21:21:46.000000 pedal-2.5.1/pedal/resolvers/sectional.py
+-rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.5.1/pedal/resolvers/silent.py
+-rw-rw-rw-   0        0        0     4798 2023-05-26 21:21:54.000000 pedal-2.5.1/pedal/resolvers/simple.py
+-rw-rw-rw-   0        0        0     1124 2023-05-26 21:34:10.000000 pedal-2.5.1/pedal/resolvers/statistics.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.767033 pedal-2.5.1/pedal/sandbox/
+-rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.5.1/pedal/sandbox/__init__.py
+-rw-rw-rw-   0        0        0    17919 2023-05-18 18:30:27.000000 pedal-2.5.1/pedal/sandbox/commands.py
+-rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/sandbox/constants.py
+-rw-rw-rw-   0        0        0     9807 2023-05-26 21:45:59.000000 pedal-2.5.1/pedal/sandbox/data.py
+-rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.5.1/pedal/sandbox/exceptions.py
+-rw-rw-rw-   0        0        0    10695 2023-06-10 15:55:30.000000 pedal-2.5.1/pedal/sandbox/feedbacks.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.773032 pedal-2.5.1/pedal/sandbox/library/
+-rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.5.1/pedal/sandbox/library/__init__.py
+-rw-rw-rw-   0        0        0     5032 2023-05-27 15:46:08.000000 pedal-2.5.1/pedal/sandbox/library/designer.py
+-rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.5.1/pedal/sandbox/library/matplotlib.py
+-rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.5.1/pedal/sandbox/library/microbit.py
+-rw-rw-rw-   0        0        0     3404 2023-05-27 15:46:26.000000 pedal-2.5.1/pedal/sandbox/library/turtles.py
+-rw-rw-rw-   0        0        0    10128 2023-05-27 15:46:15.000000 pedal-2.5.1/pedal/sandbox/mocked.py
+-rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.5.1/pedal/sandbox/result.py
+-rw-rw-rw-   0        0        0    38840 2023-05-22 14:40:28.000000 pedal-2.5.1/pedal/sandbox/sandbox.py
+-rw-rw-rw-   0        0        0     5048 2023-05-27 15:46:22.000000 pedal-2.5.1/pedal/sandbox/timeout.py
+-rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.5.1/pedal/sandbox/tracer.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.780031 pedal-2.5.1/pedal/source/
+-rw-rw-rw-   0        0        0      914 2023-05-27 15:44:56.000000 pedal-2.5.1/pedal/source/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/source/constants.py
+-rw-rw-rw-   0        0        0     5913 2023-06-10 16:42:17.000000 pedal-2.5.1/pedal/source/feedbacks.py
+-rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/source/sections.py
+-rw-rw-rw-   0        0        0     7716 2023-06-10 14:14:43.000000 pedal-2.5.1/pedal/source/source.py
+-rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/source/substitutions.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.796032 pedal-2.5.1/pedal/tifa/
+-rw-rw-rw-   0        0        0     3046 2023-05-27 15:47:23.000000 pedal-2.5.1/pedal/tifa/__init__.py
+-rw-rw-rw-   0        0        0     2143 2022-10-06 14:36:45.000000 pedal-2.5.1/pedal/tifa/commands.py
+-rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/tifa/constants.py
+-rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.5.1/pedal/tifa/contexts.py
+-rw-rw-rw-   0        0        0    23656 2023-05-22 16:40:08.000000 pedal-2.5.1/pedal/tifa/feedbacks.py
+-rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/tifa/identifier.py
+-rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.5.1/pedal/tifa/settings.py
+-rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.5.1/pedal/tifa/state.py
+-rw-rw-rw-   0        0        0    24173 2022-10-07 14:11:04.000000 pedal-2.5.1/pedal/tifa/tifa_core.py
+-rw-rw-rw-   0        0        0    42475 2023-06-08 18:43:14.000000 pedal-2.5.1/pedal/tifa/tifa_visitor.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.807034 pedal-2.5.1/pedal/types/
+-rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.5.1/pedal/types/__init__.py
+-rw-rw-rw-   0        0        0     9162 2023-05-27 15:45:10.000000 pedal-2.5.1/pedal/types/builtin.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.816032 pedal-2.5.1/pedal/types/library/
+-rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.5.1/pedal/types/library/__init__.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.5.1/pedal/types/library/cs1_curriculum.py
+-rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.5.1/pedal/types/library/designer.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.5.1/pedal/types/library/matplotlib.py
+-rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.5.1/pedal/types/library/microbit.py
+-rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.5.1/pedal/types/library/turtles.py
+-rw-rw-rw-   0        0        0    51761 2023-05-27 15:40:45.000000 pedal-2.5.1/pedal/types/new_types.py
+-rw-rw-rw-   0        0        0    14912 2023-06-08 18:43:02.000000 pedal-2.5.1/pedal/types/normalize.py
+-rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.5.1/pedal/types/operations.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:14:30.831032 pedal-2.5.1/pedal/utilities/
+-rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.5.1/pedal/utilities/ast_tools.py
+-rw-rw-rw-   0        0        0     6580 2022-07-27 17:31:05.000000 pedal-2.5.1/pedal/utilities/comparisons.py
+-rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/utilities/dictionaries.py
+-rw-rw-rw-   0        0        0     9918 2023-06-10 16:39:35.000000 pedal-2.5.1/pedal/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.5.1/pedal/utilities/files.py
+-rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/utilities/operators.py
+-rw-rw-rw-   0        0        0     7037 2022-12-31 17:53:00.000000 pedal-2.5.1/pedal/utilities/progsnap.py
+-rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/utilities/sorting.py
+-rw-rw-rw-   0        0        0      449 2023-06-08 22:09:02.000000 pedal-2.5.1/pedal/utilities/system.py
+-rw-rw-rw-   0        0        0     2457 2023-06-10 15:07:25.000000 pedal-2.5.1/pedal/utilities/text.py
+-rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.5.1/pedal/utilities/types.py
+-rw-rw-rw-   0        0        0      121 2023-06-11 14:14:30.833032 pedal-2.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-06-09 13:00:00.000000 pedal-2.5.1/setup.py
```

### Comparing `pedal-2.4.2/LICENSE` & `pedal-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/PKG-INFO` & `pedal-2.5.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pedal
-Version: 2.4.2
+Version: 2.5.1
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
-Description: Pedal
-        =====
-        
-        .. image:: https://github.com/pedal-edu/pedal/workflows/Test%20and%20Lint/badge.svg
-            :alt: Unit Tests for 3.6, 3.7, 3.8, 3.9
-        
-        
-        .. image:: https://github.com/pedal-edu/pedal/workflows/Build%20Documentation/badge.svg
-            :alt: Documentation
-        
-        A collection of tools to analyze student's work in a pipeline.
-        Pedal not only provides some of these tools, but it provides a *framework*
-        around those tools.
-        
-        Installation
-        ============
-        
-        Install from PyPi::
-            
-            pip install pedal
-        
-        Or install from the https://github.com/acbart/pedal repository
-        
-        Important Concepts
-        ==================
-        
-        Pedal revolves around providing *Feedback Functions* that can be called in an
-        Instructor Control Script to generate *Feedback* for a *Submission*, which are
-        all attached to a *Report*. A *Resolver* can then transform that Feedback into
-        something that an *Environment* can hand off to a learner (or other interested
-        party). These Feedback Functions are organized into *Tools*.
-        
-        .. image:: https://raw.githubusercontent.com/pedal-edu/pedal/master/docsrc/_static/pedal-overview-v3.png
-        
-        One of our major goals is to attach metadata to feedback to enable easier
-        analysis, versioning, and evaluation. Although Instructor Control Scripts can
-        be written very imperatively to specify very complex (or simple) grading logic,
-        we are trying to reach an elegant, declarative style. This will enable tooling
-        to automatically generate reports on occurrences of feedback, connect to
-        datasets like those in the ProgSnap format, and allow us to "unit test our
-        unit tests".
-        
-        One of our other goals for this project is to categorize Feedbacks' Conditions
-        and Responses, using concepts established by Narciss 2006. For example, we
-        say some Kinds of Responses are "hints" instead of "mistakes". We also say
-        that Conditions can be Categorized as being from "Specifications" or
-        "Runtime".
-        
-        For more information, check out the docs for Pedal_.
-        
-        .. _Pedal: https://pedal-edu.github.io/pedal
-        
 Keywords: feedback education teaching program analysis tifa cait sandbox pedal grading grader grade
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
-Requires-Python: >=3.6
+Requires-Python: >=3.7
+License-File: LICENSE
+
+Pedal
+=====
+
+.. image:: https://github.com/pedal-edu/pedal/workflows/Test%20and%20Lint/badge.svg
+    :alt: Unit Tests for 3.6, 3.7, 3.8, 3.9
+
+
+.. image:: https://github.com/pedal-edu/pedal/workflows/Build%20Documentation/badge.svg
+    :alt: Documentation
+
+A collection of tools to analyze student's work in a pipeline.
+Pedal not only provides some of these tools, but it provides a *framework*
+around those tools.
+
+Installation
+============
+
+Install from PyPi::
+    
+    pip install pedal
+
+Or install from the https://github.com/acbart/pedal repository
+
+Important Concepts
+==================
+
+Pedal revolves around providing *Feedback Functions* that can be called in an
+Instructor Control Script to generate *Feedback* for a *Submission*, which are
+all attached to a *Report*. A *Resolver* can then transform that Feedback into
+something that an *Environment* can hand off to a learner (or other interested
+party). These Feedback Functions are organized into *Tools*.
+
+.. image:: https://raw.githubusercontent.com/pedal-edu/pedal/master/docsrc/_static/pedal-overview-v3.png
+
+One of our major goals is to attach metadata to feedback to enable easier
+analysis, versioning, and evaluation. Although Instructor Control Scripts can
+be written very imperatively to specify very complex (or simple) grading logic,
+we are trying to reach an elegant, declarative style. This will enable tooling
+to automatically generate reports on occurrences of feedback, connect to
+datasets like those in the ProgSnap format, and allow us to "unit test our
+unit tests".
+
+One of our other goals for this project is to categorize Feedbacks' Conditions
+and Responses, using concepts established by Narciss 2006. For example, we
+say some Kinds of Responses are "hints" instead of "mistakes". We also say
+that Conditions can be Categorized as being from "Specifications" or
+"Runtime".
+
+For more information, check out the docs for Pedal_.
+
+.. _Pedal: https://pedal-edu.github.io/pedal
```

### Comparing `pedal-2.4.2/Pedal.egg-info/PKG-INFO` & `pedal-2.5.1/Pedal.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pedal
-Version: 2.4.2
+Version: 2.5.1
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
-Description: Pedal
-        =====
-        
-        .. image:: https://github.com/pedal-edu/pedal/workflows/Test%20and%20Lint/badge.svg
-            :alt: Unit Tests for 3.6, 3.7, 3.8, 3.9
-        
-        
-        .. image:: https://github.com/pedal-edu/pedal/workflows/Build%20Documentation/badge.svg
-            :alt: Documentation
-        
-        A collection of tools to analyze student's work in a pipeline.
-        Pedal not only provides some of these tools, but it provides a *framework*
-        around those tools.
-        
-        Installation
-        ============
-        
-        Install from PyPi::
-            
-            pip install pedal
-        
-        Or install from the https://github.com/acbart/pedal repository
-        
-        Important Concepts
-        ==================
-        
-        Pedal revolves around providing *Feedback Functions* that can be called in an
-        Instructor Control Script to generate *Feedback* for a *Submission*, which are
-        all attached to a *Report*. A *Resolver* can then transform that Feedback into
-        something that an *Environment* can hand off to a learner (or other interested
-        party). These Feedback Functions are organized into *Tools*.
-        
-        .. image:: https://raw.githubusercontent.com/pedal-edu/pedal/master/docsrc/_static/pedal-overview-v3.png
-        
-        One of our major goals is to attach metadata to feedback to enable easier
-        analysis, versioning, and evaluation. Although Instructor Control Scripts can
-        be written very imperatively to specify very complex (or simple) grading logic,
-        we are trying to reach an elegant, declarative style. This will enable tooling
-        to automatically generate reports on occurrences of feedback, connect to
-        datasets like those in the ProgSnap format, and allow us to "unit test our
-        unit tests".
-        
-        One of our other goals for this project is to categorize Feedbacks' Conditions
-        and Responses, using concepts established by Narciss 2006. For example, we
-        say some Kinds of Responses are "hints" instead of "mistakes". We also say
-        that Conditions can be Categorized as being from "Specifications" or
-        "Runtime".
-        
-        For more information, check out the docs for Pedal_.
-        
-        .. _Pedal: https://pedal-edu.github.io/pedal
-        
 Keywords: feedback education teaching program analysis tifa cait sandbox pedal grading grader grade
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
-Requires-Python: >=3.6
+Requires-Python: >=3.7
+License-File: LICENSE
+
+Pedal
+=====
+
+.. image:: https://github.com/pedal-edu/pedal/workflows/Test%20and%20Lint/badge.svg
+    :alt: Unit Tests for 3.6, 3.7, 3.8, 3.9
+
+
+.. image:: https://github.com/pedal-edu/pedal/workflows/Build%20Documentation/badge.svg
+    :alt: Documentation
+
+A collection of tools to analyze student's work in a pipeline.
+Pedal not only provides some of these tools, but it provides a *framework*
+around those tools.
+
+Installation
+============
+
+Install from PyPi::
+    
+    pip install pedal
+
+Or install from the https://github.com/acbart/pedal repository
+
+Important Concepts
+==================
+
+Pedal revolves around providing *Feedback Functions* that can be called in an
+Instructor Control Script to generate *Feedback* for a *Submission*, which are
+all attached to a *Report*. A *Resolver* can then transform that Feedback into
+something that an *Environment* can hand off to a learner (or other interested
+party). These Feedback Functions are organized into *Tools*.
+
+.. image:: https://raw.githubusercontent.com/pedal-edu/pedal/master/docsrc/_static/pedal-overview-v3.png
+
+One of our major goals is to attach metadata to feedback to enable easier
+analysis, versioning, and evaluation. Although Instructor Control Scripts can
+be written very imperatively to specify very complex (or simple) grading logic,
+we are trying to reach an elegant, declarative style. This will enable tooling
+to automatically generate reports on occurrences of feedback, connect to
+datasets like those in the ProgSnap format, and allow us to "unit test our
+unit tests".
+
+One of our other goals for this project is to categorize Feedbacks' Conditions
+and Responses, using concepts established by Narciss 2006. For example, we
+say some Kinds of Responses are "hints" instead of "mistakes". We also say
+that Conditions can be Categorized as being from "Specifications" or
+"Runtime".
+
+For more information, check out the docs for Pedal_.
+
+.. _Pedal: https://pedal-edu.github.io/pedal
```

### Comparing `pedal-2.4.2/Pedal.egg-info/SOURCES.txt` & `pedal-2.5.1/Pedal.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 pedal/environments/blockpy.py
 pedal/environments/gradescope.py
 pedal/environments/jupyter.py
 pedal/environments/nbgrader.py
 pedal/environments/none.py
 pedal/environments/sandbox.py
 pedal/environments/standard.py
+pedal/environments/terminal.py
 pedal/environments/vpl.py
 pedal/extensions/__init__.py
 pedal/extensions/microbit.py
 pedal/extensions/plotting.py
 pedal/extensions/turtles.py
 pedal/questions/__init__.py
 pedal/questions/constants.py
@@ -73,14 +74,15 @@
 pedal/questions/graders.py
 pedal/questions/loader.py
 pedal/questions/pool.py
 pedal/questions/questions.py
 pedal/questions/setup.py
 pedal/resolvers/__init__.py
 pedal/resolvers/core.py
+pedal/resolvers/export.py
 pedal/resolvers/full.py
 pedal/resolvers/sectional.py
 pedal/resolvers/silent.py
 pedal/resolvers/simple.py
 pedal/resolvers/statistics.py
 pedal/sandbox/__init__.py
 pedal/sandbox/commands.py
```

### Comparing `pedal-2.4.2/README.rst` & `pedal-2.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/assertions/__init__.py` & `pedal-2.5.1/pedal/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/assertions/classes.py` & `pedal-2.5.1/pedal/assertions/classes.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/assertions/commands.py` & `pedal-2.5.1/pedal/assertions/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/assertions/feedbacks.py` & `pedal-2.5.1/pedal/assertions/feedbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,16 +431,15 @@
         self.fields['failure_count'] = failure_count = len(self.failures)
         self.fields['error_count'] = error_count = len(self.errors)
         self.fields['success_count'] = success_count = len(self.successes)
         self.fields['total_count'] = total_count = len(self.all_feedback)
         self.fields['name'] = self.name
         self.fields['try_all'] = self.try_all
 
-        stats = []
-        stats.append(f"You passed {success_count}/{total_count} tests.\n")
+        stats = [f"You passed {success_count}/{total_count} tests.\n"]
         if error_count:
             stats.append(f"There were {error_count} errors.\n")
         self.fields['summary_statistics'] = "\n".join(stats)
 
     def format_table(self):
         # Group by their tables
         # TODO: left target, right target, expected_verb
@@ -508,15 +507,15 @@
     assert_equal(call('add', first_arg, 2), first_arg + 3)
     assert_equal(call('add', first_arg, 5), first_arg + 9)
     assert_equal(call('add', first_arg, -2), first_arg + -6)
     assert_greater(call('add', first_arg, 3), 0)
 
 
 if test_add(5) and test_add(-3):
-    set_success()
+    set_correct()
 
 
 def unit_test(function_name, *tests):
     with assert_group(function_name) as group:
         for test in tests:
             args, expected = test
             assert_equal(call(function_name, *args), expected)
```

### Comparing `pedal-2.4.2/pedal/assertions/functions.py` & `pedal-2.5.1/pedal/assertions/functions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/assertions/organizers.py` & `pedal-2.5.1/pedal/assertions/organizers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/assertions/runtime.py` & `pedal-2.5.1/pedal/assertions/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 """
 Runtime assertions.
 
 TODO: assert_has_class
 TODO: assertGraphType, assertGraphValues
 TODO: assert_coverage
 TODO: assert_ran (latest run produced no expections)
+
+
+assert_equal
+assert_not_equal
+assert_less
+assert_less_equal
+assert_greater
+assert_greater_equal
+assert_in
+assert_not_in
+assert_contains_subset
+assert_is
+assert_is_not
+assert_is_none
+assert_is_dataclass
+assert_is_not_dataclass
+assert_true
+assert_false
+assert_length_equal
 """
 import re
 
 try:
     from dataclasses import _FIELDS
 except Exception:
     _FIELDS = '__dataclass_fields__'
```

### Comparing `pedal-2.4.2/pedal/assertions/setup.py` & `pedal-2.5.1/pedal/assertions/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Helper functions and basic setup routines for the entire module.
 """
 
 from pedal.core.report import MAIN_REPORT
-from pedal.core.commands import set_success
+from pedal.core.commands import set_correct
 from pedal.sandbox.exceptions import SandboxStudentCodeException
 from pedal.utilities.sorting import topological_sort
 
 
 def resolve_all(set_successful=False, no_phases_is_success=False, report=MAIN_REPORT):
     """
```

### Comparing `pedal-2.4.2/pedal/assertions/static.py` & `pedal-2.5.1/pedal/assertions/static.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/assertions/unittest.py` & `pedal-2.5.1/pedal/assertions/unittest.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/cait/ast_helpers.py` & `pedal-2.5.1/pedal/cait/ast_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A pretty-printing dump function for the ast module.  The code was copied from
 the ast.dump function and modified slightly to pretty-print.
 
 Alex Leone (acleone ~AT~ gmail.com), 2010-01-30
 
-From http://alexleone.blogspot.co.uk/2010/01/python-ast-pretty-printer.html
+From https://alexleone.blogspot.co.uk/2010/01/python-ast-pretty-printer.html
 """
 
 from ast import AST, iter_fields, parse
 
 
 def dump(node, annotate_fields=True, include_attributes=False, indent='  '):
     """
```

### Comparing `pedal-2.4.2/pedal/cait/ast_map.py` & `pedal-2.5.1/pedal/cait/ast_map.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/cait/cait_api.py` & `pedal-2.5.1/pedal/cait/cait_api.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/cait/cait_node.py` & `pedal-2.5.1/pedal/cait/cait_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/cait/find_node.py` & `pedal-2.5.1/pedal/cait/find_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/cait/stretchy_tree_matching.py` & `pedal-2.5.1/pedal/cait/stretchy_tree_matching.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/command_line/command_line.py` & `pedal-2.5.1/pedal/command_line/command_line.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/command_line/mocks.py` & `pedal-2.5.1/pedal/command_line/mocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,21 +25,15 @@
 """
 
 import sys
 from io import TextIOWrapper
 
 from unittest.mock import Mock, NonCallableMock, DEFAULT
 
-if sys.version_info < (3, 0):
-    try:
-        from cStringIO import StringIO, StringIO as BytesIO
-    except ImportError:
-        from StringIO import StringIO, StringIO as BytesIO
-else:
-    from io import StringIO, BytesIO
+from io import StringIO, BytesIO
 
 
 class FileLikeMock(NonCallableMock):
     """Acts like a file object returned from open()."""
     def __init__(self, name=None, read_data='', *args, **kws):
         kws.update({'spec': TextIOWrapper, })
         super(FileLikeMock, self).__init__(*args, **kws)
```

### Comparing `pedal-2.4.2/pedal/command_line/modes.py` & `pedal-2.5.1/pedal/command_line/modes.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 import warnings
 import argparse
 
 from pedal.command_line.report import StatReport
 from pedal.command_line.verify import generate_report_out, ReportVerifier
 from pedal.core.report import MAIN_REPORT
 from pedal.core.submission import Submission
-from pedal.sandbox.result import is_sandbox_result
 from pedal.utilities.files import normalize_path, find_possible_filenames
 from pedal.utilities.progsnap import SqlProgSnap2
 from pedal.utilities.text import chomp
+from pedal.resolvers.export import PedalJSONEncoder, clean_json
 
 try:
     from tqdm import tqdm
 except ImportError:
     def tqdm(values):
         """ Trivial helper function to replace TQDM's behavior """
         yield from values
@@ -370,39 +370,14 @@
                 print(pedal_json_encoder.encode(final))
             else:
                 with open(self.config.output, 'w') as output_file:
                     print(pedal_json_encoder.encode(final), file=output_file)
         return StatReport(final)
 
 
-class PedalJSONEncoder(json.JSONEncoder):
-    """
-    Custom JSON Encoder to handle weird Pedal values nested in Feedback Functions,
-    including things like SandboxResult.
-    """
-    def _iterencode(self, o, markers=None):
-        if is_sandbox_result(o):
-            return super()._iterencode(o._actual_value, markers)
-        else:
-            return super()._iterencode(o, markers)
-
-    def default(self, obj):
-        return '<not serializable>'
-
-
-def clean_json(obj):
-    if is_sandbox_result(obj):
-        return clean_json(obj._actual_value)
-    if isinstance(obj, dict):
-        return {clean_json(key): clean_json(value) for key, value in obj.items()}
-    elif isinstance(obj, (set, list, tuple)):
-        return [clean_json(value) for value in obj]
-    else:
-        return obj
-
 
 class VerifyPipeline(AbstractPipeline):
     def process_output(self):
         for bundle in self.submissions:
             bundle.run_ics_bundle(resolver=self.config.resolver, skip_tifa=self.config.skip_tifa,
                                   skip_run=self.config.skip_run)
             if bundle.result.error:
```

### Comparing `pedal-2.4.2/pedal/command_line/report.py` & `pedal-2.5.1/pedal/command_line/report.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/command_line/verify.py` & `pedal-2.5.1/pedal/command_line/verify.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/core/commands.py` & `pedal-2.5.1/pedal/core/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Imperative style commands for constructing feedback in a convenient way.
 Uses a global report object (MAIN_REPORT).
 """
 
-__all__ = ['feedback', 'set_success', 'compliment', 'give_partial', 'explain',
+__all__ = ['feedback', 'set_success', 'set_correct', 'compliment', 'give_partial', 'explain',
            'gently', 'hide_correctness', 'suppress', 'log', 'debug',
            'system_error', 'clear_report', 'get_all_feedback', 'guidance',
            'contextualize_report', 'Feedback', 'get_submission', 'set_formatter']
 
 from pedal.core.feedback import (Feedback, FeedbackKind, FeedbackCategory,
                                  FeedbackResponse)
 from pedal.core.report import MAIN_REPORT
@@ -16,15 +16,15 @@
 
 #: Lowercase "function" version that works like other Core Feedback Functions.
 feedback = Feedback
 
 
 # TODO: force_success function, which ignores errors to give the points.
 
-class set_success(FeedbackResponse):
+class set_correct(FeedbackResponse):
     """
     **(Feedback Function)**
 
     Creates Successful feedback for the user, indicating that the entire
     assignment is done.
     """
     title = "Complete"
@@ -32,14 +32,17 @@
     score = 1
     correct = True
     category = FeedbackCategory.COMPLETE
     kind = FeedbackKind.RESULT
     valence = Feedback.POSITIVE_VALENCE
 
 
+set_success = set_correct
+
+
 class compliment(FeedbackResponse):
     """
     Create a positive feedback for the user, potentially on a specific line of
     code.
     """
     category = FeedbackCategory.INSTRUCTOR
     kind = FeedbackKind.COMPLIMENT
@@ -215,14 +218,15 @@
     """
     if not isinstance(submission, Submission):
         submission = Submission(files={filename: submission})
     if clear:
         report.clear()
     report.contextualize(submission)
 
+
 def get_submission(report=MAIN_REPORT) -> Submission:
     """
     Get the current submission from the given report, or the default MAIN_REPORT.
 
     Args:
         report: The report to attach this feedback to (defaults to the
             :py:data:`~pedal.core.report.MAIN_REPORT`).
```

### Comparing `pedal-2.4.2/pedal/core/environment.py` & `pedal-2.5.1/pedal/core/environment.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/core/errors.py` & `pedal-2.5.1/pedal/core/errors.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/core/feedback.py` & `pedal-2.5.1/pedal/core/feedback.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,23 +63,23 @@
             It is ultimately up to the Resolver to decide how to combine all the different scores; a typical
             strategy would be to add all the scores together for any non-muted feedback.
         correct (bool): Indicates that the entire submission should be considered correct (success) and that the
             task is now finished.
         muted (bool): Whether this piece of feedback is something that should be shown to a student. There are
             various use cases for muted feedback: they can serve as flags for later conditionals, suppressed
             default kinds of feedback, or perhaps feedback that is interesting for analysis but not pedagogically
-            helpful to give to the student. They will still contribute to overall score, but not to the correcntess
+            helpful to give to the student. They will still contribute to overall score, but not to the correctness
             of the submission.
         unscored (bool): Whether or not this piece of feedback contributes to
             the score/correctness.
 
         else_message (str): A string to render as a message when a
             NEGATIVE valence feedback is NOT triggered, or a POSITIVE valence
             feedback IS triggered.
-            TODO: Should we also have an else_message_template? Probably.
+        else_message_template (str): Similar to the ``message_template``, but for the ``else_message``.
 
         activate (bool): Used for default feedback objects without a custom
             condition, to indicate whether they should be considered triggered.
             Defaults to True; setting this to False means that the feedback
             object will be deactivated. Note that most inheriting Feedback
             Functions will not respect this parameter.
 
@@ -293,15 +293,15 @@
 
     def condition(self, *args, **kwargs):
         """
         Detect if this feedback is present in the code.
         Defaults to true through the `activate` parameter.
 
         Returns:
-            bool: Whether or not this feedback's condition was detected.
+            bool: Whether this feedback's condition was detected.
         """
         return self.activate
 
     def _get_message(self):
         """
         Determines the appropriate value for the message. It will attempt
         to use this instance's message, but if it's not available then it will
@@ -379,14 +379,23 @@
         for :py:class:`pedal.core.group.FeedbackGroup`, most other feedbacks
         will just not care.
 
         The ``active`` parameter controls whether or not the condition for the
         feedback was met. """
 
     def __xor__(self, other):
+        """
+        Allows you to have two mutually exclusive conditions. Only one condition will be activated.
+
+        Args:
+            other:
+
+        Returns:
+
+        """
         if isinstance(other, Feedback):
             self.muted = bool(self) and not bool(other)
             self.unscored = self.muted
             other.muted = bool(other) and not bool(self)
             other.unscored = other.muted
         if isinstance(other, bool):
             self.muted = bool(self) and not bool(other)
```

### Comparing `pedal-2.4.2/pedal/core/feedback_category.py` & `pedal-2.5.1/pedal/core/feedback_category.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/core/final_feedback.py` & `pedal-2.5.1/pedal/core/final_feedback.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pedal.core.feedback import Feedback
-from pedal.core.commands import set_success
+from pedal.core.commands import set_correct
+from pedal.core.report import Report
 from pedal.core.scoring import Score, combine_scores
 
 
 def parse_feedback(feedback):
     """
 
     Args:
@@ -21,21 +22,38 @@
     """
     Internal class used for organizing the feedback into one place.
     Dumpable into a simple dictionary.
     """
 
     DEFAULT_NO_FEEDBACK_TITLE = "No Errors"
     DEFAULT_NO_FEEDBACK_MESSAGE = "No errors reported."
+    DEFAULT_NO_FEEDBACK_LABEL = "set_correct_no_errors"
 
     # TODO: Change all these so that FinalFeedback also logs considered feedback
 
-    def __init__(self, success=None, score=None, category=None, label=None, title=None,
+    def __init__(self, correct=None, score=None, category=None, label=None, title=None,
                  message=None, data=None, hide_correctness=None,
-                 suppressions=None, suppressed_labels=None):
-        self.success = success
+                 suppressions=None, suppressed_labels=None, success=None):
+        """
+
+        Args:
+            correct:
+            score:
+            category:
+            label:
+            title:
+            message:
+            data:
+            hide_correctness:
+            suppressions:
+            suppressed_labels:
+            success (bool): DEPRECATED. This field is now set by `correct`. The alternative parameter name is
+                kept around for backwards compatibility.
+        """
+        self.success = self.correct = correct if correct is not None else success
         self.score = score
         self._scores = []
         self._scores_feedback = []
         self.category = category
         self.label = label
         self.title = title
         self.message = message
@@ -73,15 +91,15 @@
             for fields in list_of_fields:
                 # Do any of them not match?
                 for field, value in fields.items():
                     if feedback['fields'].get(field, None) != value:
                         break
                 else:
                     return
-        success, partial, message, title, data = parse_feedback(feedback)
+        correct, partial, message, title, data = parse_feedback(feedback)
         if feedback and feedback.category == Feedback.CATEGORIES.SYSTEM:
             self.systems.append(feedback)
         if not feedback.unscored and feedback.score is not None:
             # Triggered Negative leads to opposite behavior for operator
             # Also untriggered positive feedback
             invert_logic = ((feedback.valence != feedback.NEGATIVE_VALENCE) == (not feedback))
             inversion = "!" if invert_logic else ""
@@ -93,40 +111,40 @@
         if not feedback or feedback.muted:
             return
         if feedback.kind == Feedback.KINDS.COMPLIMENT:
             self.positives.append(feedback)
             return feedback
         if feedback.kind == Feedback.KINDS.INSTRUCTIONAL:
             self.instructions.append(feedback)
-        self.success = success and self.success
+        self.success = self.correct = correct and self.correct
         if message is not None and self.message is None:
             self.message = message
             self.title = title
             self.category = feedback.category
             self.label = feedback.label
             self.data = data
             self.used.append(feedback)
         return feedback
 
     def finalize(self):
         if self.message is None:
             self.title = self.DEFAULT_NO_FEEDBACK_TITLE
             self.message = self.DEFAULT_NO_FEEDBACK_MESSAGE
-        self.hide_correctness = self.suppressions.get('success', False)
+        self.hide_correctness = self.suppressions.get('correct', self.suppressions.get('success', False))
         if (not self.hide_correctness and
-                self.label == 'set_success_no_errors' and
+                self.label == self.DEFAULT_NO_FEEDBACK_LABEL and
                 self.category == Feedback.CATEGORIES.COMPLETE):
             # TODO: Promote to be its own atomic feedback function
-            self.title = set_success.title
-            self.message = set_success.message_template
+            self.title = set_correct.title
+            self.message = set_correct.message_template
             self.score = 1
-            self.success = True
+            self.success = self.correct = True
         else:
             self.score = combine_scores(self._scores)
-        self.success = bool(self.success)
+        self.success = self.correct = bool(self.correct)
         return self
 
     def __str__(self) -> str:
         return "FinalFeedback({label!r}, {title!r}, {message!r})".format(label=self.label,
                                                                          title=self.title,
                                                                          message=self.message[:50])
 
@@ -139,17 +157,29 @@
     def to_json(self) -> dict:
         """
 
         Returns:
 
         """
         return {
-            'success': self.success,
+            'correct': self.correct,
+            'success': self.correct,
             'score': self.score,
             "scores": self._scores,
             'category': self.category,
             'label': self.label,
             'title': self.title,
             'message': self.message,
             'data': self.data,
-            'hide_correctness': self.hide_correctness
+            'hide_correctness': self.hide_correctness,
+            'location': self.data.get('location', None) if self.data else None
         }
+
+
+def set_correct_no_errors(report: Report) -> FinalFeedback:
+    return FinalFeedback(correct=True, score=0,
+                         title=None, message=None,
+                         category=Feedback.CATEGORIES.COMPLETE,
+                         label=FinalFeedback.DEFAULT_NO_FEEDBACK_LABEL,
+                         data=[], hide_correctness=False,
+                         suppressions=report.suppressions,
+                         suppressed_labels=report.suppressed_labels)
```

### Comparing `pedal-2.4.2/pedal/core/formatting.py` & `pedal-2.5.1/pedal/core/formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Utilities and classes related to formatting a Feedback Message.
 """
-
+from pedal.core.location import Location
+from pedal.utilities.text import inject_line
 
 def chomp_spec(format_spec, word):
     """ Return a new version of format_spec without the ``word`` and
     (if there are multiple format_spec given) the extra colon. """
     if format_spec.endswith(word):
         format_spec = format_spec[:-len(word)]
         if format_spec and format_spec[-1] == ':':
@@ -81,15 +82,17 @@
     def update_report(self, report):
         """ Change the currently set report for this formatter. """
         self.report = report
 
     def pre(self, text):
         return "\n".join(["    " + line for line in text.split("\n")])
 
-    def python_code(self, code):
+    def python_code(self, code, focus=None):
+        if isinstance(focus, Location):
+            code = inject_line(code, focus.line+1, " "*(focus.col-1) + "^"*(focus.end_col-focus.col))
         return self.pre(code)
 
     def python_expression(self, code):
         return str(code)
 
     def filename(self, filename):
         return filename
@@ -115,16 +118,15 @@
     def frame(self, name):
         return name
 
     def exception(self, exception):
         return self.pre(exception)
 
     def table(self, rows, columns):
-        result = []
-        result.append(" | ".join(columns))
+        result = [" | ".join(columns)]
         for row in rows:
             result.append(" | ".join(row))
         return "\n" + ("\n".join(result))
 
     def check_mark(self):
         # TODO: should be ✓, right?
         return " "
@@ -154,15 +156,17 @@
         return self.html_tag('code', escape_dunders(contents), classes)
 
     def html_span(self, contents, classes=None):
         return self.html_tag('span', contents, classes)
 
     ############################################################################
 
-    def python_code(self, code):
+    def python_code(self, code, focus=None):
+        if isinstance(focus, Location):
+            code = inject_line(code, focus.line+1, " "*(focus.col-1) + "^"*(focus.end_col-focus.col))
         return self.html_tag('pre', self.html_code(code), "pedal-python-code python")
 
     def python_expression(self, code):
         return self.html_code(code)
 
     def filename(self, filename):
         return self.html_code(filename, "pedal-filename")
```

### Comparing `pedal-2.4.2/pedal/core/location.py` & `pedal-2.5.1/pedal/core/location.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Simple data class for storing information about a location within source code.
 """
+from dataclasses import dataclass
 
 __all__ = ['Location']
 
 
+@dataclass
 class Location:
     """
     A class for storing information about a location in source code.
 
     Attributes:
         line (int): A line of source code.
         col (int, optional): A column within a line of source code.
@@ -26,15 +28,15 @@
         self.line = line
         self.col = col
         self.end_line = end_line
         self.end_col = end_col
         self.filename = filename
 
     def __str__(self):
-        return f"<Location({self.line}, {self.col}, {self.filename})>"
+        return f"<Location({self.line}, {self.col}, {self.filename!r})>"
 
     def __repr__(self):
         return str(self)
 
     @classmethod
     def from_ast(cls, node):
         """
```

### Comparing `pedal-2.4.2/pedal/core/report.py` & `pedal-2.5.1/pedal/core/report.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/core/resolver.py` & `pedal-2.5.1/pedal/core/resolver.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/core/scoring.py` & `pedal-2.5.1/pedal/core/scoring.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/core/submission.py` & `pedal-2.5.1/pedal/core/submission.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/core/tool.py` & `pedal-2.5.1/pedal/core/tool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/environments/__init__.py` & `pedal-2.5.1/pedal/environments/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     return tuple(results)
 '''
 
 from pedal.environments.standard import setup_environment
 
 ALL_ENVIRONMENTS = [
     'blockpy', 'gradescope', 'jupyter', 'standard', 'vpl'
-]
+]
```

### Comparing `pedal-2.4.2/pedal/environments/blockpy.py` & `pedal-2.5.1/pedal/environments/blockpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 class BlockPyEnvironment(Environment):
     """
     Configures the BlockPy programming environment.
     """
     def __init__(self, files=None, main_file='answer.py', main_code=None,
                  user=None, assignment=None, course=None, execution=None,
                  instructor_file='on_run.py', skip_tifa=False, skip_run=False,
-                 inputs=None, set_success=True,
+                 inputs=None, set_correct=True, set_success=None,
                  report=MAIN_REPORT, trace=True, threaded=False):
         super().__init__(files=files, main_file=main_file, main_code=main_code,
                          user=user, assignment=assignment, course=course,
                          execution=execution, instructor_file=instructor_file,
                          report=report)
         report.set_formatter(HtmlFormatter(report))
         verify(report=self.report)
```

### Comparing `pedal-2.4.2/pedal/environments/gradescope.py` & `pedal-2.5.1/pedal/environments/gradescope.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     Configures the GradeScope programming environment.
 
     # TODO: Add command line argument to use "simple" resolver instead of full
     """
     def __init__(self, files=None, main_file='answer.py', main_code=None,
                  user=None, assignment=None, course=None, execution=None,
                  instructor_file='on_run.py', skip_tifa=False, skip_run=False,
-                 inputs=None, set_success=True,
+                 inputs=None, set_correct=True, set_success=None,
                  report=MAIN_REPORT, trace=True, threaded=True, **kwargs):
         super().__init__(files=files, main_file=main_file, main_code=main_code,
                          user=user, assignment=assignment, course=course,
                          execution=execution, instructor_file=instructor_file,
                          report=report)
         self.skip_run = skip_run
         self.skip_tifa = skip_tifa
```

### Comparing `pedal-2.4.2/pedal/environments/jupyter.py` & `pedal-2.5.1/pedal/environments/jupyter.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/environments/nbgrader.py` & `pedal-2.5.1/pedal/environments/nbgrader.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     """
     Configures the NBGrader programming environment.
     """
 
     def __init__(self, files=None, main_file='answer.py', main_code=None,
                  user=None, assignment=None, course=None, execution=None,
                  instructor_file='on_run.py', skip_tifa=True, skip_run=True,
-                 inputs=None, set_success=True,
+                 inputs=None, set_correct=True, set_success=None,
                  report=MAIN_REPORT, trace=True):
         super().__init__(files=files, main_file=main_file, main_code=main_code,
                          user=user, assignment=assignment, course=course,
                          execution=execution, instructor_file=instructor_file,
                          report=report)
         # TODO: If WebCAT doesn't want HTML output, then we should switch the default formatter
         self.report.add_hook('pedal.report.add_feedback', self.force_immediate_errors)
```

### Comparing `pedal-2.4.2/pedal/environments/sandbox.py` & `pedal-2.5.1/pedal/environments/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/environments/standard.py` & `pedal-2.5.1/pedal/environments/standard.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,16 +37,16 @@
     result to the command line.
 
     from pedal.environments.standard import setup_pedal
     code, student, resolve = setup_pedal()
     """
     def __init__(self, files=None, main_file='answer.py', main_code=None,
                  user=None, assignment=None, course=None, execution=None,
-                 instructor_file='on_run.py', skip_tifa=False, set_success=True, skip_run=False,
-                 report=MAIN_REPORT, trace=True, threaded=False):
+                 instructor_file='on_run.py', skip_tifa=False, set_correct=True, set_success=None,
+                 skip_run=False, report=MAIN_REPORT, trace=True, threaded=False):
         # Possibly user passed in stuff via the command line.
         if files is None and main_code is None:
             (instructor_file, files, main_file, main_code, user, assignment,
              course, execution) = parse_argv()
         super().__init__(files=files, main_file=main_file, main_code=main_code,
                          user=user, assignment=assignment, course=course,
                          execution=execution, instructor_file=instructor_file,
@@ -64,15 +64,15 @@
                 start_trace()
             student = run(report=report, threaded=threaded)
             student.threaded = threaded
         self.fields = {
             'student': student,
             'resolve': resolve
         }
-        self.set_success = set_success
+        self.set_correct = set_correct or set_success
 
     def print_resolve(self, *args, **kwargs):
         """
         Trivial formatter for resolver, just dumps the
         Title/Label/Score/Message. Any arguments are forwarded to
         :py:func:`pedal.resolvers.simple.resolve`
         """
```

### Comparing `pedal-2.4.2/pedal/environments/vpl.py` & `pedal-2.5.1/pedal/environments/vpl.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,25 +13,28 @@
 from pedal.sandbox import run, get_sandbox, set_input, start_trace
 from pedal.source.sections import FeedbackSourceSection
 from pedal.tifa import tifa_analysis
 from pedal.resolvers.simple import resolve as simple_resolve, by_priority
 from pedal.resolvers.sectional import resolve as original_sectional_resolve
 from pedal.core.formatting import Formatter
 
-import tabulate
+try:
+    import tabulate
+except ImportError:
+    tabulate = None
 
 
 class VPLEnvironment(Environment):
     """
     Configures the BlockPy programming environment.
     """
     def __init__(self, files=None, main_file='answer.py', main_code=None,
                  user=None, assignment=None, course=None, execution=None,
                  instructor_file='on_run.py', skip_tifa=True, skip_run=False,
-                 inputs=None, set_success=True,
+                 inputs=None, set_correct=True, set_success=None,
                  report=MAIN_REPORT, trace=True):
         super().__init__(files=files, main_file=main_file, main_code=main_code,
                          user=user, assignment=assignment, course=course,
                          execution=execution, instructor_file=instructor_file,
                          report=report)
         self.skip_run = skip_run
         self.skip_tifa = skip_tifa
@@ -120,15 +123,18 @@
     def frame(self, name):
         return name
 
     def exception(self, exception):
         return self.pre(exception)
 
     def table(self, rows, columns):
-        return self.pre(tabulate.tabulate(rows, headers=columns))
+        if tabulate:
+            return self.pre(tabulate.tabulate(rows, headers=columns))
+        else:
+            return self.pre(f"Table:\n{columns}\n{rows}")
 
 
 score_maximum = 1
 
 
 def set_maximum_score(number):
     """
```

### Comparing `pedal-2.4.2/pedal/extensions/microbit.py` & `pedal-2.5.1/pedal/extensions/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/extensions/plotting.py` & `pedal-2.5.1/pedal/extensions/plotting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/questions/__init__.py` & `pedal-2.5.1/pedal/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/questions/feedbacks.py` & `pedal-2.5.1/pedal/questions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/questions/graders.py` & `pedal-2.5.1/pedal/questions/graders.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         """
         all_good = True
         if self.UNIT_TEST_TOTAL_POINTS is None:
             TYPE_POINT_ADD = self.UNIT_TEST_TYPE_POINTS
             VALUE_POINT_ADD = self.UNIT_TEST_VALUE_POINTS
         else:
             ratio = self.UNIT_TEST_TYPE_RATIO
-            TYPE_POINT_ADD = (self.UNIT_TEST_TOTAL_POINTS / len(self.tests) * (ratio))
+            TYPE_POINT_ADD = (self.UNIT_TEST_TOTAL_POINTS / len(self.tests) * ratio)
             VALUE_POINT_ADD = (self.UNIT_TEST_TOTAL_POINTS / len(self.tests) * (1 - ratio))
         test_points = 0
         for index, (arguments, expected) in enumerate(self.tests):
             # import sys
             # print(repr(arguments), file=sys.stderr)
             result = self.student.call(self.function_name, *arguments)
             # print(repr(self.student.exception), file=sys.stderr)
```

### Comparing `pedal-2.4.2/pedal/questions/loader.py` & `pedal-2.5.1/pedal/questions/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 syntax:
     prevent:
         ___ + ___
 # Override any of our default feedback messages
 messages:
     FUNCTION_NOT_DEFINED: "Oops you missed a function"
 """
-from pedal.core.commands import set_success, give_partial, gently
+from pedal.core.commands import set_correct, give_partial, gently
 from pedal.core.feedback_category import FeedbackCategory
 from pedal.questions.constants import TOOL_NAME
 
 from pedal.sandbox.commands import get_sandbox, get_student_data
 from pedal.utilities.comparisons import equality_test
 from pedal.assertions.static import ensure_function
 from pedal.assertions.runtime import ensure_function_callable
```

### Comparing `pedal-2.4.2/pedal/questions/pool.py` & `pedal-2.5.1/pedal/questions/pool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/questions/questions.py` & `pedal-2.5.1/pedal/questions/questions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/questions/setup.py` & `pedal-2.5.1/pedal/questions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/resolvers/__init__.py` & `pedal-2.5.1/pedal/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/resolvers/core.py` & `pedal-2.5.1/pedal/resolvers/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from pedal.core.report import MAIN_REPORT
 
 
 def make_resolver(func, report=None):
-    '''
+    """
     Decorates the given function as a Resolver. This means that when the
     function is executed, the `"pedal.resolver.resolve"` event will be
     triggered.
-    
+
     Args:
         func (callable): The function to decorate.
         report (Report): The Report to trigger the event on. If None, then use
             the `MAIN_REPORT`.
-    '''
+    """
     if report is None:
         report = MAIN_REPORT
 
     def resolver_wrapper(*args, **kwargs):
         report.execute_hooks('pedal.resolvers', 'resolve')
         return func(*args, **kwargs)
```

### Comparing `pedal-2.4.2/pedal/resolvers/full.py` & `pedal-2.5.1/pedal/resolvers/full.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pedal.core.final_feedback import FinalFeedback
+from pedal.core.final_feedback import FinalFeedback, set_correct_no_errors
 from pedal.resolvers.core import make_resolver
 from pedal.core.report import MAIN_REPORT
 from pedal.core.feedback import Feedback
 from pedal.resolvers.simple import by_priority
 
 DEFAULT_CATEGORY_PRIORITY = [
     Feedback.CATEGORIES.INSTRUCTIONS,
@@ -42,26 +42,20 @@
         FinalFeedback: The resolved feedback.
     """
 
     # Prepare feedbacks
     feedbacks = report.feedback + report.ignored_feedback
     feedbacks.sort(key=priority_key)
     # Create the initial final feedback
-    final = FinalFeedback(success=True, score=0,
-                          title=None, message=None,
-                          category=Feedback.CATEGORIES.COMPLETE,
-                          label='set_success_no_errors',
-                          data=[], hide_correctness=False,
-                          suppressions=report.suppressions,
-                          suppressed_labels=report.suppressed_labels)
+    final = set_correct_no_errors(report)
     # Process each feedback in turn
     used = []
     for feedback in feedbacks:
         partial = final.merge(feedback)
         if partial is not None:
             used.append(partial)
     # Override empty message
     final.finalize()
     final.used = used
     report.result = final
     report.resolves.append(final)
-    return final
+    return final
```

### Comparing `pedal-2.4.2/pedal/resolvers/sectional.py` & `pedal-2.5.1/pedal/resolvers/sectional.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A version of the resolver that still chooses one piece of feedback, but
 does so per section.
 """
 
 from pedal.core.feedback import Feedback
-from pedal.core.final_feedback import FinalFeedback
+from pedal.core.final_feedback import FinalFeedback, set_correct_no_errors
 from pedal.core.report import MAIN_REPORT
 from pedal.resolvers.core import make_resolver
 from pedal.resolvers.simple import by_priority
 
 
 @make_resolver
 def resolve(report=MAIN_REPORT, priority_key=by_priority):
@@ -31,20 +31,15 @@
         else:
             feedback_by_group[feedback.parent] = [feedback]
     # Process each subgroup
     finals = {}
     for group, feedbacks in feedback_by_group.items():
         feedbacks.sort(key=priority_key)
         # Create the initial final feedback
-        final = FinalFeedback(success=True, score=0,
-                              title=None, message=None,
-                              category=Feedback.CATEGORIES.COMPLETE, label='set_success_no_errors',
-                              data=[], hide_correctness=False,
-                              suppressions=report.suppressions,
-                              suppressed_labels=report.suppressed_labels)
+        final = set_correct_no_errors(report)
         # Process each feedback in turn
         for feedback in feedbacks:
             final.merge(feedback)
         # Override empty message
         final.finalize()
         finals[group] = final
     report.result = finals
```

### Comparing `pedal-2.4.2/pedal/resolvers/simple.py` & `pedal-2.5.1/pedal/resolvers/simple.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 # Give 5% if this does get triggered
 give_partial("+5%")
 ```
 
 """
 from pedal.core.report import MAIN_REPORT
-from pedal.core.final_feedback import FinalFeedback
+from pedal.core.final_feedback import FinalFeedback, set_correct_no_errors
 from pedal.core.feedback import Feedback, DEFAULT_CATEGORY_PRIORITY
 from pedal.resolvers.core import make_resolver
 
 
 def by_priority(feedback):
     """
     Converts a feedback into a numeric representation for sorting.
@@ -133,20 +133,15 @@
     Returns
         str: A string of HTML feedback to be delivered
     """
     # Prepare feedbacks
     feedbacks = report.feedback + report.ignored_feedback
     feedbacks.sort(key=priority_key)
     # Create the initial final feedback
-    final = FinalFeedback(success=True, score=0,
-                          title=None, message=None,
-                          category=Feedback.CATEGORIES.COMPLETE, label='set_success_no_errors',
-                          data=[], hide_correctness=False,
-                          suppressions=report.suppressions,
-                          suppressed_labels=report.suppressed_labels)
+    final = set_correct_no_errors(report)
     # Process each feedback in turn
     for feedback in feedbacks:
         final.merge(feedback)
     # Override empty message
     final.finalize()
     report.result = final
     report.resolves.append(final)
```

### Comparing `pedal-2.4.2/pedal/sandbox/__init__.py` & `pedal-2.5.1/pedal/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/sandbox/commands.py` & `pedal-2.5.1/pedal/sandbox/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/sandbox/data.py` & `pedal-2.5.1/pedal/sandbox/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,17 @@
             str: The description of the action.
         """
         if context.kind == SandboxContextKind.EVAL and context.target in ("", "_"):
             return 'I evaluated the expression'
         else:
             return 'I ran the code'
 
+    def __repr__(self):
+        return f"<SandboxContextKind {self.value}>"
+
 
 class SandboxContext:
     """
     Simple data class holding information about an execution within a sandbox.
     Includes such information as the code that was run, its filename, inputs,
     outputs, exceptions, etc.
 
@@ -113,14 +116,17 @@
         Returns:
             SandboxContext: The new context, copied from the old one except with a new ID.
         """
         return SandboxContext(context_id, self.code, self.filename,
                               self.kind, self.target, list(self.inputs),
                               self.output, self.exception, self.submission)
 
+    def __repr__(self):
+        return f"<SandboxContext {self.context_id}>"
+
 
 class ExecutionTextHolder:
     """
     Helper class for formatting the text of an execution. Keeps track of the last action taken, the current body,
     and the current formatter for this Report.
 
     Args:
```

### Comparing `pedal-2.4.2/pedal/sandbox/exceptions.py` & `pedal-2.5.1/pedal/sandbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/sandbox/feedbacks.py` & `pedal-2.5.1/pedal/sandbox/feedbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,15 @@
         exception_message = exception_message[0].upper() + exception_message[1:] if exception_message else ""
         if type(exception) not in EXCEPTION_FF_MAP:
             title = exception_name
         else:
             title = EXCEPTION_FF_MAP[type(exception)].title
         location = Location(location)
         traceback_stack = traceback.build_traceback()
-        traceback_message = traceback.format_traceback(traceback_stack,
-                                                       report.format)
+        traceback_message = traceback.format_traceback(traceback_stack, report.format)
         if not traceback_message:
             traceback_message = ""
         else:
             traceback_message = f"The traceback was:\n{traceback_message}"
         context_message = format_contexts(context, report.format)
         fields = {'exception': exception,
                   'exception_name': exception_name_proper,
```

### Comparing `pedal-2.4.2/pedal/sandbox/library/designer.py` & `pedal-2.5.1/pedal/sandbox/library/designer.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         if IS_PYTHON_36:
             # Generate patches manually
             return {name: self.getter(name) for name in self.FIELDS}
         else:
             return {'__getattr__': self.getter, '__all__': ['test']}
 
     def getter(self, key):
-        " If anything asks, we prevent the module. Except for __file__. "
+        """ If anything asks, we prevent the module. Except for __file__. """
         # Needed to support coverage - it's okay to ask who I am.
         if key == '__file__':
             return self.module_name
         if key == '__all__':
             return self.FIELDS
 
         def _fake_call_wrapper(*args, **kwargs):
```

### Comparing `pedal-2.4.2/pedal/sandbox/library/matplotlib.py` & `pedal-2.5.1/pedal/sandbox/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/sandbox/library/microbit.py` & `pedal-2.5.1/pedal/sandbox/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/sandbox/library/turtles.py` & `pedal-2.5.1/pedal/sandbox/library/turtles.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         if IS_PYTHON_36:
             # Generate patches manually
             return {name: self.getter(name) for name in self.FIELDS}
         else:
             return {'__getattr__': self.getter}
 
     def getter(self, key):
-        " If anything asks, we prevent the module. Except for __file__. "
+        """ If anything asks, we prevent the module. Except for __file__. """
         # Needed to support coverage - it's okay to ask who I am.
         if key == '__file__':
             return self.module_name
 
         if key == '__all__':
             return self.FIELDS
```

### Comparing `pedal-2.4.2/pedal/sandbox/mocked.py` & `pedal-2.5.1/pedal/sandbox/mocked.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
     def __init__(self, name):
         self.module_name = name
 
     def _generate_patches(self):
         return {'__getattr__': self.getter}
 
     def getter(self, key):
-        " If anything asks, we prevent the module. Except for __file__. "
+        """ If anything asks, we prevent the module. Except for __file__. """
         # Needed to support coverage - it's okay to ask who I am.
         if key == '__file__':
             return self.module_name
         else:
             self.prevent_module()
 
     def prevent_module(self, *args, **kwargs):
```

### Comparing `pedal-2.4.2/pedal/sandbox/result.py` & `pedal-2.5.1/pedal/sandbox/result.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/sandbox/sandbox.py` & `pedal-2.5.1/pedal/sandbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/sandbox/timeout.py` & `pedal-2.5.1/pedal/sandbox/timeout.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,17 +36,17 @@
         try:
             self.result = self.func(*self.args, **self.kwargs)
         except Exception:
             self.exc_info = sys.exc_info()
 
     @staticmethod
     def _async_raise(thread_id, exception):
-        '''
+        """
         Static method to raise an error asychronously using the ctypes module.
-        '''
+        """
         # Cache the function for convenience
         RaiseAsyncException = ctypes.pythonapi.PyThreadState_SetAsyncExc
 
         states_modified = RaiseAsyncException(ctypes.c_long(thread_id),
                                               ctypes.py_object(exception))
         if states_modified == 0:
             raise ValueError("nonexistent thread id")
```

### Comparing `pedal-2.4.2/pedal/sandbox/tracer.py` & `pedal-2.5.1/pedal/sandbox/tracer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/source/__init__.py` & `pedal-2.5.1/pedal/source/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 """
 
 from pedal.source.constants import TOOL_NAME
 from pedal.source.sections import (separate_into_sections, check_section_exists,
                                    stop_sections, next_section)
 from pedal.source.source import (verify, verify_section, set_source, set_source_file, get_program)
-#from pedal.source.rewrite import unparse
+
+# from pedal.source.rewrite import unparse
 
 __all__ = ['TOOL_NAME',
            'set_source', 'verify', 'set_source_file', 'get_program',
            'separate_into_sections',
            'check_section_exists', 'next_section', 'verify_section',
            ]
```

### Comparing `pedal-2.4.2/pedal/source/feedbacks.py` & `pedal-2.5.1/pedal/source/feedbacks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Feedback functions of the Source module
 """
-
+import traceback as tb
 from pedal.core.commands import feedback
 from pedal.core.feedback import FeedbackResponse
 from pedal.core.location import Location
 from pedal.core.report import MAIN_REPORT
 from pedal.utilities.exceptions import ExpandedTraceback
 from pedal.source.constants import TOOL_NAME
+from pedal.utilities.system import IS_AT_LEAST_PYTHON_310
 
 
 class SourceFeedback(FeedbackResponse):
     """ Base class of all Feedback functions for Source Tool """
     category = feedback.CATEGORIES.SYNTAX
     kind = feedback.KINDS.MISTAKE
     tool = TOOL_NAME
@@ -50,78 +51,90 @@
     def __init__(self, name, sections, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
         fields = {'name': name, 'sections': sections}
         group = 0 if sections else kwargs.get('group')
         super().__init__(fields=fields, group=group, **kwargs)
 
 
-
 class syntax_error(SourceFeedback):
     """ Generic feedback for any kind of syntax error. """
     muted = False
     title = "Syntax Error"
-    message_template = ("Bad syntax on line {lineno:line}\n\n"
+    message_template = ("Bad syntax on line {lineno:line}.\n\n"
                         "{traceback_message}\n"
+                        "{suggestion_message}"
                         "Suggestion: Check line {lineno:line}, the line "
-                        "before it, and the line after it. Remember to ignore blank lines.")
-    version = '0.0.2'
+                        "before it, and the line after it. Ignore blank lines.")
+    version = '1.0.0'
     justification = "Syntax error was triggered while calling ast.parse"
 
     def __init__(self, line, filename, code, col_offset,
-                 exception, exc_info, **kwargs):
+                 exception, exc_info, enhance=True, **kwargs):
         report = kwargs.get('report', MAIN_REPORT)
         files = report.submission.get_files_lines()
         if filename not in files:
             files[filename] = code.split("\n")
         if report.submission is not None:
             lines = report.submission.get_lines()
             line_offsets = report.submission.line_offsets
         else:
             lines = code.split("\n")
             line_offsets = {}
-        line_offset = line_offsets.get(filename, 0)
         traceback = ExpandedTraceback(exception, exc_info, False,
                                       [report.submission.instructor_file],
                                       line_offsets, [filename], lines, files)
         traceback_stack = traceback.build_traceback()
-        traceback_message = traceback.format_traceback(traceback_stack,
-                                                       report.format)
-        if not traceback_message:
-            traceback_message = ""
-        else:
+        traceback_message = traceback.format_traceback(traceback_stack, report.format)
+        if traceback_message:
             traceback_message = f"The traceback was:\n{traceback_message}"
+        else:
+            traceback_message = ""
+        #if not enhance:
+        #    self.message_template = "{traceback_message}\n{exception_message}"
         line_offset = line_offsets.get(filename, 0)
-        fields = {'lineno': line+line_offset,
-                  'filename': filename, 'offset': col_offset,
+        suggestion_message = self.make_suggestion_message(exception)
+        fields = {'lineno': line + line_offset,
+                  'filename': filename,
+                  'offset': col_offset,
                   'exception': exception,
                   'exception_message': str(exception),
                   'traceback': traceback,
                   'traceback_stack': traceback_stack,
-                  'traceback_message': traceback_message}
-        location = Location(line=line+line_offset, col=col_offset, filename=filename)
+                  'traceback_message': traceback_message,
+                  'suggestion_message': suggestion_message}
+        location = Location(line=line + line_offset, col=col_offset, filename=filename)
         super().__init__(fields=fields, location=location, **kwargs)
 
+    def make_suggestion_message(self, exception):
+        """ Generate a suggestion message based on the exception. """
+        base_message = exception.msg
+        base_message = base_message.capitalize() + "."
+        if base_message == "Invalid syntax.":
+            return ""
+        return base_message + "\n"
+
 
 class incorrect_number_of_sections(SourceFeedback):
     """ Incorrect number of sections """
     title = "Incorrect Number of Sections"
     message_template = ("Incorrect number of sections in your file. "
                         "Expected {count}, but only found {found}")
     justification = ""
 
     def __init__(self, count, found, **kwargs):
         fields = {'count': count, 'found': found}
         super().__init__(fields=fields, **kwargs)
 
+
 # TODO: TabError
 
 
 class indentation_error(syntax_error):
     """ Generic feedback for indentation errors. """
     title = "Indentation Error"
-    message_template = ("Bad indentation on line {lineno:line} or adjacent line.\n"
-                        "{exception_message:exception}\n\n"
+    message_template = ("Bad indentation on line {lineno:line} or adjacent line.\n\n"
                         "{traceback_message}\n"
+                        "{suggestion_message}"
                         "Suggestion: Check line {lineno:line}, the line "
-                        "before it, and the line after it. Remember to ignore blank lines.")
-    version = '0.0.1'
+                        "before it, and the line after it. Ignore blank lines.")
+    version = '1.0.0'
     justification = "Indentation error was triggered while calling ast.parse"
```

### Comparing `pedal-2.4.2/pedal/source/sections.py` & `pedal-2.5.1/pedal/source/sections.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/source/source.py` & `pedal-2.5.1/pedal/source/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     code. Otherwise, it creates a Substitution and temporarily replaces
     the Submission's current main code.
 
     Args:
         code (str): The contents of the source file.
         filename (str): The filename of the students' code. Defaults to
                         `answer.py`.
-        sections (str or bool): Whether or not the file should be divided into
+        sections (str or bool): Whether the file should be divided into
                                 sections. If a str, then it should be a
                                 Python regular expression for how the sections
                                 are separated. If False, there will be no
                                 sections. If True, then the default pattern
                                 will be used: '^##### Part (\\d+)$'
         independent (bool): Whether the separate sections should be considered
             separate or all existing in an accumulating namespace.
@@ -104,53 +104,54 @@
         old_submission = report[TOOL_NAME]['substitutions'].pop()
         report.submission.replace_main(old_submission.code, old_submission.filename)
         verify(report=report)
 
 
 @CompositeFeedbackFunction(blank_source, syntax_error, indentation_error, source_file_not_found)
 def verify(code=None, filename=DEFAULT_STUDENT_FILENAME, report=MAIN_REPORT,
-           muted=False):
+           muted=False, enhance=True):
     """
     Parses the given source code and checks for syntax errors; if no code is given, defaults to the
     current Main file of the submission.
 
     Args:
-        muted:
+        enhance (bool): Whether to use native Python error messages or the Pedal enhanced ones.
+        muted: Whether this Feedback should be considered for showing to the student.
         code (str): Some code to parse and syntax check.
-        filename: An optional filename to use
+        filename (str): An optional filename to use
         report:
 
     Returns:
 
     """
     if code is None:
         code = report.submission.main_code
         filename = report.submission.main_file
     if report.submission.load_error:
-        source_file_not_found(filename, None)
+        source_file_not_found(filename, None, enhance=enhance, report=report, muted=muted)
         report[TOOL_NAME]['success'] = False
         return False
     if code.strip() == '':
-        blank_source()
+        blank_source(enhance=enhance, report=report, muted=muted)
         report[TOOL_NAME]['success'] = False
     try:
         parsed = ast.parse(code, filename)
         report[TOOL_NAME]['ast'] = parsed
     except IndentationError as e:
         indentation_error(e.lineno, e.filename, code, e.offset, e,
-                     sys.exc_info(), report=report, muted=muted)
+                          sys.exc_info(), report=report, muted=muted, enhance=enhance)
         report[TOOL_NAME]['success'] = False
         report[TOOL_NAME]['ast'] = ast.parse("")
     except SyntaxError as e:
         syntax_error(e.lineno, e.filename, code, e.offset, e,
-                     sys.exc_info(), report=report, muted=muted)
+                     sys.exc_info(), report=report, muted=muted, enhance=enhance)
         report[TOOL_NAME]['success'] = False
         report[TOOL_NAME]['ast'] = ast.parse("")
-        # TODO: Shouldn't this return early?
-    report[TOOL_NAME]['success'] = True
+    else:
+        report[TOOL_NAME]['success'] = True
     return report[TOOL_NAME]['success']
 
 
 # Legacy verify_section; now done by verify since its aware of sections
 verify_section = verify
 
 
@@ -169,15 +170,14 @@
 
     Returns:
 
     """
     return report[TOOL_NAME]['substitutions'][0].code
 
 
-
 @CompositeFeedbackFunction(source_file_not_found)
 def set_source_file(filename: str, sections=False, independent=False, report=MAIN_REPORT):
     """
     Uses the given `filename` on the filesystem as the new main file.
 
     Args:
         filename (str or list[str]): Checks the files, in the given order, to be loaded.
```

### Comparing `pedal-2.4.2/pedal/tifa/__init__.py` & `pedal-2.5.1/pedal/tifa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     Type
         A symbolic representation of the variable's type.
 
     Literal
         Sometimes, we need a specialized representation of a literal value
         to be passed around. This is particularly important for accessing
-        elements in an tuples.
+        elements in tuples.
 
     Name Map
         (Path x Fully Qualified Names) => States
 """
 from pedal.core.report import MAIN_REPORT, Report
 from pedal.tifa.constants import TOOL_NAME
 from pedal.tifa.settings import get_default_tifa_settings
```

### Comparing `pedal-2.4.2/pedal/tifa/commands.py` & `pedal-2.5.1/pedal/tifa/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/tifa/contexts.py` & `pedal-2.5.1/pedal/tifa/contexts.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/tifa/feedbacks.py` & `pedal-2.5.1/pedal/tifa/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/tifa/identifier.py` & `pedal-2.5.1/pedal/tifa/identifier.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/tifa/settings.py` & `pedal-2.5.1/pedal/tifa/settings.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/tifa/state.py` & `pedal-2.5.1/pedal/tifa/state.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/tifa/tifa_core.py` & `pedal-2.5.1/pedal/tifa/tifa_core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/tifa/tifa_visitor.py` & `pedal-2.5.1/pedal/tifa/tifa_visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                                   type_changes, unnecessary_second_branch,
                                   recursive_call, multiple_return_types,
                                   possible_initialization_problem,
                                   incorrect_arity, else_on_loop_body,
                                   module_not_found, nested_function_definition,
                                   unused_returned_value, invalid_indexing,
                                   attribute_type_change)
-from pedal.utilities.system import IS_PYTHON_39, IS_AT_LEAST_PYTHON_38
+from pedal.utilities.system import IS_AT_LEAST_PYTHON_38
 
 
 class Tifa(TifaCore, ast.NodeVisitor):
     """
     TIFA subclass for traversing an AST and finding common issues.
     You can instantiate this class, manipulate settings, and then process
     some code or AST.
```

### Comparing `pedal-2.4.2/pedal/types/builtin.py` & `pedal-2.5.1/pedal/types/builtin.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,26 @@
                                    ListConstructor, StrConstructor, str_function, GeneratorType, SetConstructor,
                                    FrozenSetConstructor, DictConstructor, TupleConstructor)
 
 register_builtin_module('dataclasses', lambda: ModuleType('dataclasses', fields={
     'dataclass': FunctionType('dataclass', definition=make_dataclass)
 }))
 
-register_builtin_module('pprint', lambda: ModuleType('pprint',fields={
+register_builtin_module('pprint', lambda: ModuleType('pprint', fields={
     'pprint': FunctionType(name='pprint', returns=NoneType)
- }))
+}))
 
-register_builtin_module('json', lambda: ModuleType('json',fields={
+register_builtin_module('json', lambda: ModuleType('json', fields={
     'loads': FunctionType(name='loads', returns=AnyType),
     'dumps': FunctionType(name='dumps', returns=StrType)
 }))
 
 register_builtin_module('random', lambda: ModuleType('random', fields={
-     'randint': FunctionType(name='randint', returns=NumType)
- }))
+    'randint': FunctionType(name='randint', returns=NumType)
+}))
 
 register_builtin_module('string', lambda: ModuleType('string', fields={
     'letters': StrType(False),
     'digits': StrType(False),
     'ascii_letters': StrType(False),
     'punctuation': StrType(False),
     'printable': StrType(False),
@@ -43,84 +43,82 @@
     'hexdigits': StrType(False),
     'octdigits': StrType(False),
 }))
 
 
 def reload_math_module():
     math_module = ModuleType('math', fields={
-       f.name: f for f in [
-           int_function('ceil'),
-           int_function('comb'),
-           float_function('copysign'),
-           num_function('fabs'),
-           int_function('factorial'),
-           int_function('floor'),
-           num_function('fmod'),
-           FunctionType('frexp', returns=lambda: TupleType([FloatType(), IntType()])),
-           float_function('fsum'),
-           int_function('gcd'),
-           bool_function('isclose'),
-           bool_function('isfinite'),
-           bool_function('isinf'),
-           bool_function('isnan'),
-           int_function('isqrt'),
-           int_function('lcm'),
-           num_function('ldexp'),
-           FunctionType('modf', returns=lambda: TupleType([FloatType(), FloatType()])),
-           float_function('nextafter'),
-           int_function('perm'),
-           num_function('prod'),
-           float_function('remainder'),
-           int_function('trunc'),
-           float_function('ulp'),
-           float_function('exp'),
-           float_function('expm1'),
-           float_function('log'),
-           float_function('log1p'),
-           float_function('log2'),
-           float_function('log10'),
-           float_function('pow'),
-           float_function('sqrt'),
-           float_function('acos'),
-           float_function('asin'),
-           float_function('atan'),
-           float_function('atan2'),
-           float_function('cos'),
-           float_function('dist'),
-           float_function('hypot'),
-           float_function('sin'),
-           float_function('tan'),
-           num_function('radians'),
-           num_function('degrees'),
-           float_function('acosh'),
-           float_function('asinh'),
-           float_function('atanh'),
-           float_function('cosh'),
-           float_function('sinh'),
-           float_function('tanh'),
-           float_function('erf'),
-           float_function('erfc'),
-           float_function('gamma'),
-           float_function('lgamma')]
-        })
+        f.name: f for f in [
+            int_function('ceil'),
+            int_function('comb'),
+            float_function('copysign'),
+            num_function('fabs'),
+            int_function('factorial'),
+            int_function('floor'),
+            num_function('fmod'),
+            FunctionType('frexp', returns=lambda: TupleType([FloatType(), IntType()])),
+            float_function('fsum'),
+            int_function('gcd'),
+            bool_function('isclose'),
+            bool_function('isfinite'),
+            bool_function('isinf'),
+            bool_function('isnan'),
+            int_function('isqrt'),
+            int_function('lcm'),
+            num_function('ldexp'),
+            FunctionType('modf', returns=lambda: TupleType([FloatType(), FloatType()])),
+            float_function('nextafter'),
+            int_function('perm'),
+            num_function('prod'),
+            float_function('remainder'),
+            int_function('trunc'),
+            float_function('ulp'),
+            float_function('exp'),
+            float_function('expm1'),
+            float_function('log'),
+            float_function('log1p'),
+            float_function('log2'),
+            float_function('log10'),
+            float_function('pow'),
+            float_function('sqrt'),
+            float_function('acos'),
+            float_function('asin'),
+            float_function('atan'),
+            float_function('atan2'),
+            float_function('cos'),
+            float_function('dist'),
+            float_function('hypot'),
+            float_function('sin'),
+            float_function('tan'),
+            num_function('radians'),
+            num_function('degrees'),
+            float_function('acosh'),
+            float_function('asinh'),
+            float_function('atanh'),
+            float_function('cosh'),
+            float_function('sinh'),
+            float_function('tanh'),
+            float_function('erf'),
+            float_function('erfc'),
+            float_function('gamma'),
+            float_function('lgamma')]
+    })
     math_module.fields.update({
         'pi': FloatType(),
         'e': FloatType(),
         'tau': FloatType(),
         'inf': FloatType(),
         'nan': FloatType()
     })
     return math_module
 
 
 register_builtin_module('math', reload_math_module)
 
 
-
-
 def round_definition(tifa, function, callee, arguments, named_arguments, location):
     if len(arguments) == 1:
         return IntType()
     elif len(arguments) == 2:
         return FloatType()
     return ImpossibleType()
```

### Comparing `pedal-2.4.2/pedal/types/library/cs1_curriculum.py` & `pedal-2.5.1/pedal/types/library/cs1_curriculum.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/types/library/designer.py` & `pedal-2.5.1/pedal/types/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/types/library/matplotlib.py` & `pedal-2.5.1/pedal/types/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/types/library/microbit.py` & `pedal-2.5.1/pedal/types/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/types/new_types.py` & `pedal-2.5.1/pedal/types/new_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -570,15 +570,15 @@
 
 
 class TupleType(Type):
     name = "Tuple"
     immutable = True
     # Local
     is_empty: bool
-    element_types: tuple[Type]
+    element_types: tuple #: tuple[Type]
     fields = {}
     parents = []
 
     def __init__(self, element_types=None):
         super().__init__()
         if element_types is None:
             element_types = tuple()
```

### Comparing `pedal-2.4.2/pedal/types/normalize.py` & `pedal-2.5.1/pedal/types/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from pedal.types.new_types import (Type, AnyType, ImpossibleType, NumType, BoolType,
                                    TupleType, ListType, StrType,
                                    DictType, SetType, GeneratorType,
                                    ModuleType, NoneType, FrozenSetType,
                                    FunctionType, TYPE_STRINGS,
                                    LiteralStr, LiteralInt, LiteralFloat, LiteralBool, ClassType, InstanceType,
                                    widest_type, LiteralValue, TypeUnion, PEDAL_TYPE_NAMES, specify_subtype)
-from pedal.utilities.system import IS_PYTHON_39
+from pedal.utilities.system import IS_AT_LEAST_PYTHON_39
 
 import types as dynamic_python_types
 
 try:
     from dataclasses import fields
 except:
     fields = None
@@ -67,20 +67,20 @@
     """
     # Already a Pedal Type
     if isinstance(type_expression, str) and type_expression in PEDAL_TYPE_NAMES:
         return PEDAL_TYPE_NAMES[type_expression]()
     if isinstance(type_expression, Type):
         return type_expression
     # What if it's a builtin type function?
-    if isinstance(type_expression, type):
+    if isinstance(type_expression, (type, dynamic_python_types.GenericAlias)):
         if type_expression.__name__ in TYPE_STRINGS:
             return get_generic_type(type_expression, evaluate_name)
         if evaluate_name:
             type_object = unbox_sandbox_if_needed(evaluate_name(type_expression.__name__))
-            if isinstance(type_object, type):
+            if isinstance(type_object, (type, dynamic_python_types.GenericAlias)):
                 if fields and hasattr(type_object, '__dataclass_fields__'):
                     return ClassType(type_object.__name__, {
                         field.name: normalize_type(field.type, evaluate_name)
                         for field in fields(type_object)
                     })
                 # TODO: Fix this ugly ugly hack!
                 try:
@@ -302,17 +302,17 @@
     elif isinstance(value, ast.Dict):
         if not value.keys:
             return DictType([])
         return DictType([(get_pedal_type_from_ast(k, evaluate_name),
                           get_pedal_type_from_ast(v, evaluate_name))
                          for k, v in zip(value.keys, value.values)])
     # Support new style subscripts (e.g., ``list[int]``)
-    elif ((IS_PYTHON_39 and isinstance(value, ast.Subscript)) or
+    elif ((IS_AT_LEAST_PYTHON_39 and isinstance(value, ast.Subscript)) or
           isinstance(value, ast.Subscript) and isinstance(value.slice, ast.Index)):
-        if IS_PYTHON_39:
+        if IS_AT_LEAST_PYTHON_39:
             slice = value.slice
         else:
             slice = value.slice.value
         slice_type = get_pedal_type_from_ast(slice, evaluate_name)
         value_type = get_pedal_type_from_ast(value.value, evaluate_name)
         result = value_type.index(slice_type)
         if isinstance(slice, ast.Slice):
@@ -337,15 +337,15 @@
     elif isinstance(value, list):
         if value:
             return ListType(False, normalize_type(value[0], evaluate_name))
         else:
             return ListType(True)
     elif isinstance(value, (set, frozenset)):
         return TypeUnion([normalize_type(v, evaluate_name) for v in value])
-    elif isinstance(value, (tuple)):
+    elif isinstance(value, tuple):
         return TupleType([normalize_type(v, evaluate_name) for v in value])
     elif isinstance(value, dict):
         if not value:
             return DictType(True)
         if all(isinstance(value, str) for k in value.keys()):
             return DictType([(LiteralStr(s), normalize_type(vv, evaluate_name))
                             for s, vv in value.items()])
```

### Comparing `pedal-2.4.2/pedal/types/operations.py` & `pedal-2.5.1/pedal/types/operations.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/utilities/__init__.py` & `pedal-2.5.1/pedal/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/utilities/ast_tools.py` & `pedal-2.5.1/pedal/utilities/ast_tools.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/utilities/comparisons.py` & `pedal-2.5.1/pedal/utilities/comparisons.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/utilities/dictionaries.py` & `pedal-2.5.1/pedal/utilities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/utilities/exceptions.py` & `pedal-2.5.1/pedal/utilities/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Utilities for handling exceptions across all of Pedal.
 """
-
+from textwrap import indent
 import traceback
 import os
 import sys
 
+from pedal.utilities.system import IS_AT_LEAST_PYTHON_310
+from pedal.core.location import Location
+
 BuiltinKeyError = KeyError
 
 _backup_stdout = sys.stdout
 
 
 class KeyError(BuiltinKeyError):
     """
@@ -80,19 +83,22 @@
     elif hasattr(e, 'args') and e.args:
         e.args = tuple([e.args[0] + message])
     return e
 
 
 class FakeFrame:
     """ Simplistic hack to make fake StackFrames for SyntaxErrors """
-    def __init__(self, name, filename, lineno, line):
+    def __init__(self, name, filename, lineno, line, colno, end_lineno, end_colno):
         self.name = name
         self.filename = filename
         self.lineno = lineno
         self._line = line
+        self.colno = colno
+        self.end_lineno = end_lineno
+        self.end_colno = end_colno
 
     @property
     def line(self):
         return self._line
 
     def __eq__(self, other):
         try:
@@ -126,14 +132,17 @@
         self.full_traceback = full_traceback
         self.hide_filenames = hide_filenames
         self.show_filenames = show_filenames
         self.line_number = traceback.extract_tb(exc_info[2])[-1][1]
         self.original_code_lines = original_code_lines
         self.student_files = student_files
 
+    def __repr__(self):
+        return f"ExpandedTraceback({self.exception})"
+
     def build_traceback(self):
         """
         Filter out unnecessary frames
         """
         if not self.exception:
             return []
         cl, exc, tb = self.exc_info
@@ -144,16 +153,24 @@
                                             capture_locals=False)
         for frame in tb_e.stack:
             self._fix_frame_line(frame)
         frames = list(tb_e.stack)
         # A SyntaxError has to be handled differently to actually get its output:
         # https://docs.python.org/3/library/traceback.html#traceback.print_exception
         if isinstance(self.exception, SyntaxError):
+            offset = self.exception.offset
+            if IS_AT_LEAST_PYTHON_310:
+                end_lineno = self.exception.end_lineno
+                end_offset = offset if self.exception.end_offset not in {None, 0} else offset
+                end_offset = offset + 1 if offset == end_offset or end_offset == -1 else end_offset
+            else:
+                end_lineno = self.exception.lineno
+                end_offset = offset + 1
             fake_frame = FakeFrame("<module>", self.exception.filename,
-                                   self.exception.lineno, None)
+                                   self.exception.lineno, None, offset-1, end_lineno, end_offset-1)
             self._fix_frame_line(fake_frame)
             # Skulpt compatibility hack, to prevent duplicate tracebacks
             if not frames or fake_frame != frames[-1]:
                 frames.append(fake_frame)
         return frames
 
     def _fix_frame_line(self, frame):
@@ -223,19 +240,31 @@
                 a message.
             formatter (:py:class:`pedal.core.formatters.Formatter`): The
                 formatter to use to make the message.
 
         Returns:
             str: The text of the message.
         """
+
+        # TODO: In 3.10 (or 11?), the colno is available. Indents are not automatically applied. So we need to have
+        # different behavior for those versions to show off the entire line and also highlight "the good bit".
         traceback_message = "\n".join([
             (f"Line {formatter.line(frame.lineno)}"
              f" of file {formatter.filename(frame.filename)}" +
              (f" in {formatter.frame(frame.name)}\n"
               if frame.name != "<module>" and frame.name is not None
               else "\n") +
-             f"{formatter.python_code(frame.line if frame.line is not None else '')}\n")
+             f"{self.format_line(formatter, frame)}\n")
             for frame in traceback_stack
         ])
         if not traceback_message:
             return None
         return formatter.traceback(traceback_message)
+
+    def format_line(self, formatter, frame):
+        if IS_AT_LEAST_PYTHON_310:
+            end_offset = frame.end_colno+1 if frame.lineno == frame.end_lineno else len(frame._line)
+            # Note: Need to use _line because in 3.10 and above, the line gets stripped.
+            # https://github.com/python/cpython/commit/5644c7b3ffd49bed58dc095be6e6148e0bb4431e
+            line = frame._line if frame._line is not None else ''
+            return formatter.python_code(line, focus=Location(0, frame.colno+1, 0, end_offset))
+        return formatter.python_code(frame.line if frame.line is not None else '')
```

### Comparing `pedal-2.4.2/pedal/utilities/files.py` & `pedal-2.5.1/pedal/utilities/files.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/utilities/operators.py` & `pedal-2.5.1/pedal/utilities/operators.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/utilities/progsnap.py` & `pedal-2.5.1/pedal/utilities/progsnap.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/utilities/sorting.py` & `pedal-2.5.1/pedal/utilities/sorting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/pedal/utilities/text.py` & `pedal-2.5.1/pedal/utilities/text.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,7 +75,12 @@
     elif len(items) == 1:
         return items[0]
     elif len(items) == 2:
         return f"{items[0]} and {items[1]}"
     else:
         pre = ", ".join(items[:-1])
         return f"{pre}, and {items[-1]}"
+
+def inject_line(code, line_number, new_line):
+    lines = code.split("\n")
+    lines.insert(line_number, new_line)
+    return "\n".join(lines)
```

### Comparing `pedal-2.4.2/pedal/utilities/types.py` & `pedal-2.5.1/pedal/utilities/types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.4.2/setup.py` & `pedal-2.5.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='pedal',
-    version='2.4.2',
-    python_requires='>=3.6',
+    version='2.5.1',
+    python_requires='>=3.7',
     author='acbart,lukesg08',
     author_email='acbart@udel.edu',
     description='Tools to provide feedback on student code.',
     keywords='feedback education teaching program analysis tifa cait sandbox pedal grading grader grade',
     packages=['pedal', 'pedal.core', 'pedal.utilities', 'pedal.environments',
               'pedal.resolvers', 'pedal.command_line',
               'pedal.source', 'pedal.cait', 'pedal.tifa',
```

