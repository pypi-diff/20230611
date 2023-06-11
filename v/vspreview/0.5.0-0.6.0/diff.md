# Comparing `tmp/vspreview-0.5.0.tar.gz` & `tmp/vspreview-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vspreview-0.5.0.tar", last modified: Mon Jun  5 20:45:46 2023, max compression
+gzip compressed data, was "vspreview-0.6.0.tar", last modified: Sun Jun 11 01:40:35 2023, max compression
```

## Comparing `vspreview-0.5.0.tar` & `vspreview-0.6.0.tar`

### file list

```diff
@@ -1,104 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 20:45:25.000000 vspreview-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-05 20:45:46.920426 vspreview-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-05 20:45:25.000000 vspreview-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-05 20:45:46.920426 vspreview-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-05 20:45:25.000000 vspreview-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.912425 vspreview-0.5.0/vspreview/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.912425 vspreview-0.5.0/vspreview/api/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/api/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/api/output.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/api/timecodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.912425 vspreview-0.5.0/vspreview/core/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/abstracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/core/custom/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/combobox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/dragnavigator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/edits.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/graphicsview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/notch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/custom/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/types/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/types/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/types/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/types/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    20976 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/types/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/types/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/core/vsenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/main/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/main/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/main/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/main/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    31704 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/main/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/models/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/models/generalmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/models/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/models/scening.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/plugins/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/plugins/frame_props.ppy
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/toolbars/
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/toolbars/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/benchmark/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/benchmark/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.916425 vspreview-0.5.0/vspreview/toolbars/comp/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/comp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/comp/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    30642 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/comp/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/vspreview/toolbars/debug/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/debug/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/debug/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/vspreview/toolbars/main/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/main/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/vspreview/toolbars/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/misc/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/misc/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/vspreview/toolbars/pipette/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/pipette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/pipette/colorview.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/pipette/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/pipette/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/vspreview/toolbars/playback/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/playback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/playback/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    24853 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/playback/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/vspreview/toolbars/scening/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/scening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/scening/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/scening/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    35998 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/toolbars/scening/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.920426 vspreview-0.5.0/vspreview/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-05 20:45:25.000000 vspreview-0.5.0/vspreview/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:45:46.912425 vspreview-0.5.0/vspreview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-05 20:45:46.000000 vspreview-0.5.0/vspreview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-05 20:45:46.000000 vspreview-0.5.0/vspreview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:45:46.000000 vspreview-0.5.0/vspreview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-05 20:45:46.000000 vspreview-0.5.0/vspreview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:45:39.000000 vspreview-0.5.0/vspreview.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-05 20:45:46.000000 vspreview-0.5.0/vspreview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 20:45:46.000000 vspreview-0.5.0/vspreview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.312761 vspreview-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 01:40:07.000000 vspreview-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-11 01:40:35.312761 vspreview-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-11 01:40:07.000000 vspreview-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-11 01:40:35.312761 vspreview-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-11 01:40:07.000000 vspreview-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.296761 vspreview-0.6.0/vspreview/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.300761 vspreview-0.6.0/vspreview/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/api/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/api/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/api/timecodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.300761 vspreview-0.6.0/vspreview/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.304761 vspreview-0.6.0/vspreview/core/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/combobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/dragnavigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/edits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/graphicsview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/notch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.304761 vspreview-0.6.0/vspreview/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/types/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/types/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/types/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/types/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21900 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/types/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/types/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/vsenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.304761 vspreview-0.6.0/vspreview/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/main/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/main/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/main/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30658 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/main/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.304761 vspreview-0.6.0/vspreview/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/models/generalmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/models/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/models/scening.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/plugins/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/plugins/frame_props.ppy
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/plugins/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/plugins/split_view.ppy
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/benchmark/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/benchmark/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/comp/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/comp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/comp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30570 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/comp/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/debug/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/debug/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/main/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/misc/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16070 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/misc/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/pipette/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/pipette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/pipette/colorview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/pipette/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/pipette/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/playback/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/playback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/playback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24791 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/playback/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.312761 vspreview-0.6.0/vspreview/toolbars/scening/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/scening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/scening/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/scening/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35867 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/scening/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.312761 vspreview-0.6.0/vspreview/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.296761 vspreview-0.6.0/vspreview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-11 01:40:35.000000 vspreview-0.6.0/vspreview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-11 01:40:35.000000 vspreview-0.6.0/vspreview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 01:40:35.000000 vspreview-0.6.0/vspreview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-11 01:40:35.000000 vspreview-0.6.0/vspreview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 01:40:25.000000 vspreview-0.6.0/vspreview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-11 01:40:35.000000 vspreview-0.6.0/vspreview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 01:40:35.000000 vspreview-0.6.0/vspreview.egg-info/top_level.txt
```

### Comparing `vspreview-0.5.0/LICENSE` & `vspreview-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/PKG-INFO` & `vspreview-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vspreview
-Version: 0.5.0
+Version: 0.6.0
 Summary: Previewer for VapourSynth scripts
 Author: Endilll
 Author-email: 
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-preview
 Project-URL: Documentation, https://vspreview.encode.moe/en/latest/
```

### Comparing `vspreview-0.5.0/README.md` & `vspreview-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/setup.cfg` & `vspreview-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/setup.py` & `vspreview-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/api/other.py` & `vspreview-0.6.0/vspreview/api/other.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/api/output.py` & `vspreview-0.6.0/vspreview/api/output.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/core/abstracts.py` & `vspreview-0.6.0/vspreview/core/abstracts.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/core/bases.py` & `vspreview-0.6.0/vspreview/core/bases.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/core/custom/combobox.py` & `vspreview-0.6.0/vspreview/core/custom/combobox.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/core/custom/dragnavigator.py` & `vspreview-0.6.0/vspreview/core/custom/dragnavigator.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/core/custom/edits.py` & `vspreview-0.6.0/vspreview/core/custom/edits.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/core/custom/graphicsview.py` & `vspreview-0.6.0/vspreview/core/custom/graphicsview.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,103 @@
 from __future__ import annotations
 
 from enum import IntEnum, auto
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from PyQt6.QtCore import QEvent, QPoint, QPointF, QRect, Qt, pyqtSignal
 from PyQt6.QtGui import (
-    QColor, QMouseEvent, QNativeGestureEvent, QPainter, QPixmap, QResizeEvent, QTransform, QWheelEvent
+    QColor, QMouseEvent, QNativeGestureEvent, QPainter, QPalette, QPixmap, QResizeEvent, QTransform, QWheelEvent
+)
+from PyQt6.QtWidgets import (
+    QApplication, QFrame, QGraphicsPixmapItem, QGraphicsScene, QGraphicsView, QSizePolicy, QWidget
 )
-from PyQt6.QtWidgets import QApplication, QGraphicsPixmapItem, QGraphicsView, QWidget
 
 if TYPE_CHECKING:
     from ...main import MainWindow
     from ..types import CroppingInfo
 
 
 __all__ = [
     'DragEventType',
     'GraphicsView',
-    'GraphicsImageItem'
+    'GraphicsImageItem',
+    'MainVideoOutputGraphicsView'
 ]
 
 
 class DragEventType(IntEnum):
     start = auto()
     stop = auto()
     move = auto()
     repaint = auto()
 
 
+class GraphicsImageItem:
+    __slots__ = ('_graphics_item', '_pixmap')
+
+    def __init__(self, graphics_item: QGraphicsPixmapItem) -> None:
+        self._graphics_item = graphics_item
+        self._pixmap = self._graphics_item.pixmap()
+
+    def contains(self, point: QPointF) -> bool:
+        return self._graphics_item.contains(point)
+
+    def hide(self) -> None:
+        self._graphics_item.hide()
+
+    def pixmap(self) -> QPixmap:
+        return self._graphics_item.pixmap()
+
+    def setPixmap(self, new_pixmap: QPixmap | None, crop_values: CroppingInfo | None = None) -> None:
+        if new_pixmap is None:
+            new_pixmap = self._pixmap
+        else:
+            self._pixmap = new_pixmap
+
+        if crop_values is not None and crop_values.active:
+            padded = QPixmap(new_pixmap.width(), new_pixmap.height())
+            padded.fill(QColor(0, 0, 0, 0))
+            painter = QPainter(padded)
+            painter.drawPixmap(
+                QPoint(crop_values.left, crop_values.top), new_pixmap,
+                QRect(crop_values.left, crop_values.top, crop_values.width, crop_values.height)
+            )
+            painter.end()
+            new_pixmap = padded
+
+        self._graphics_item.setPixmap(new_pixmap)
+
+    def show(self) -> None:
+        self._graphics_item.show()
+
+
+class GraphicsScene(QGraphicsScene):
+    def __init__(self, view: GraphicsView) -> None:
+        self.view = view
+        self.main = self.view.main
+
+        self.graphics_items = list[GraphicsImageItem]()
+
+        super().__init__(self.main)
+
+    def init_scenes(self) -> None:
+        self.clear()
+        self.graphics_items.clear()
+
+        for _ in range(len(self.main.outputs)):
+            raw_frame_item = self.addPixmap(QPixmap())
+            raw_frame_item.hide()
+
+            self.graphics_items.append(GraphicsImageItem(raw_frame_item))
+
+    @property
+    def current_scene(self) -> GraphicsImageItem:
+        return self.graphics_items[self.main.current_output.index]
+
+
 class GraphicsView(QGraphicsView):
     WHEEL_STEP = 15 * 8  # degrees
 
     __slots__ = ('app', 'angleRemainder', 'zoomValue',)
 
     mouseMoved = pyqtSignal(QMouseEvent)
     mousePressed = pyqtSignal(QMouseEvent)
@@ -39,41 +105,111 @@
     wheelScrolled = pyqtSignal(int)
     dragEvent = pyqtSignal(DragEventType)
     drag_mode: QGraphicsView.DragMode
 
     underReload = False
     last_positions = (0, 0)
 
-    autofit = False
+    _autofit = False
     main: MainWindow
 
-    def __init__(self, parent: QWidget | None = None) -> None:
+    def __init__(self, main: MainWindow, parent: QWidget | None = None) -> None:
+        from ...core import CheckBox, HBoxLayout
+        from .combobox import ComboBox
+
         super().__init__(parent)
 
+        self.main = main
+
         self.app = QApplication.instance()
         self.angleRemainder = 0
         self.zoomValue = 0.0
         self.currentZoom = 0.0
         self.setTransformationAnchor(QGraphicsView.ViewportAnchor.AnchorUnderMouse)
         self.drag_mode = self.dragMode()
 
+        self.setBackgroundBrush(self.main.palette().brush(QPalette.ColorRole.Window))
+        self.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
+        self.setDragMode(QGraphicsView.DragMode.ScrollHandDrag)
+
+        if self.main.settings.opengl_rendering_enabled:
+            from PyQt6.QtOpenGLWidgets import QOpenGLWidget
+            self.setViewport(QOpenGLWidget())
+
+        self.wheelScrolled.connect(self.on_wheel_scrolled)
+        self.main.reload_before_signal.connect(self.beforeReload)
+        self.main.reload_after_signal.connect(self.afterReload)
+
+        self.graphics_scene = GraphicsScene(self)
+        self.setScene(self.graphics_scene)
+
+        self.zoom_combobox = ComboBox[float](self, minimumContentsLength=4)
+
+        self.auto_fit_button = CheckBox('Auto-fit', self, clicked=self.auto_fit_button_clicked)
+
+        self.controls = QFrame()
+        HBoxLayout(self.controls, [self.zoom_combobox, self.auto_fit_button])
+
+        self.main.register_graphic_view(self)
+
+        self.dragEvent.connect(self.propagate_move_event)
+
+    def auto_fit_button_clicked(self, checked: bool) -> None:
+        self.autofit = checked
+
+    @property
+    def current_scene(self) -> GraphicsImageItem:
+        return self.graphics_scene.current_scene
+
+    @property
+    def autofit(self) -> bool:
+        return self._autofit
+
+    @autofit.setter
+    def autofit(self, new_state: bool) -> None:
+        self.zoom_combobox.setEnabled(not new_state)
+
+        self._autofit = new_state
+
+        if new_state:
+            self.setZoom(None)
+        else:
+            self.setZoom(self.zoom_combobox.currentData())
+
+    def bind_to(self, other_view: GraphicsView, *, mutual: bool = True) -> None:
+        self.main.bound_graphics_views[other_view].add(self)
+
+        if mutual:
+            self.main.bound_graphics_views[self].add(other_view)
+
+    def on_wheel_scrolled(self, steps: int) -> None:
+        new_index = self.zoom_combobox.currentIndex() + steps
+
+        if new_index < 0:
+            new_index = 0
+        elif new_index >= len(self.main.settings.zoom_levels):
+            new_index = len(self.main.settings.zoom_levels) - 1
+
+        self.zoom_combobox.setCurrentIndex(new_index)
+
     def setZoom(self, value: float | None) -> None:
+        for view in self.main.bound_graphics_views[self]:
+            view._setZoom(value)
+
+    def _setZoom(self, value: float | None) -> None:
         if self.underReload or value == 0:
             return
 
         if value is None:
-            if self.autofit:
-                viewport = self.viewport()
-                value = min(
-                    viewport.width() / self.main.current_output.width,
-                    viewport.height() / self.main.current_output.height
-                )
-            else:
+            if not self.autofit:
                 return
 
+            viewport = self.viewport()
+            value = min(viewport.width() / self.content_width, viewport.height() / self.content_height)
+
         self.currentZoom = value / self.devicePixelRatio()
 
         self.setTransform(QTransform().scale(self.currentZoom, self.currentZoom))
         self.dragEvent.emit(DragEventType.repaint)
 
     def event(self, event: QEvent) -> bool:
         if self.underReload:
@@ -96,14 +232,16 @@
             return event.ignore()
 
         assert self.app
 
         modifier = event.modifiers()
         mouse = event.buttons()
 
+        self.propagate_move_event()
+
         if modifier == Qt.KeyboardModifier.ControlModifier or mouse in {
             Qt.MouseButton.RightButton, Qt.MouseButton.MiddleButton
         }:
             angleDelta = event.angleDelta().y()
 
             # check if wheel wasn't rotated the other way since last rotation
             if self.angleRemainder * angleDelta < 0:
@@ -130,14 +268,15 @@
         if self.underReload or self.autofit:
             return event.ignore()
 
         super().mouseMoveEvent(event)
 
         if self.hasMouseTracking():
             self.mouseMoved.emit(event)
+
         self.dragEvent.emit(DragEventType.move)
 
     def mousePressEvent(self, event: QMouseEvent) -> None:
         if self.underReload or self.autofit:
             return event.ignore()
 
         if event.button() == Qt.MouseButton.LeftButton:
@@ -168,54 +307,46 @@
 
     def afterReload(self) -> None:
         self.underReload = False
         self.verticalScrollBar().setValue(self.last_positions[0])
         self.horizontalScrollBar().setValue(self.last_positions[1])
         self.setTransformationAnchor(QGraphicsView.ViewportAnchor.AnchorUnderMouse)
 
-    def registerReloadEvents(self, main: MainWindow) -> None:
-        self.main = main
-        self.main.reload_before_signal.connect(self.beforeReload)
-        self.main.reload_after_signal.connect(self.afterReload)
-
     def resizeEvent(self, event: QResizeEvent) -> None:
         super().resizeEvent(event)
         self.setZoom(None)
 
+    def propagate_move_event(self, _: Any = None) -> None:
+        scrollbarW, scrollbarH = self.horizontalScrollBar(), self.verticalScrollBar()
 
-class GraphicsImageItem:
-    __slots__ = ('_graphics_item', '_pixmap')
+        if not any({scrollbarW.isVisible(), scrollbarH.isVisible()}):
+            return
 
-    def __init__(self, graphics_item: QGraphicsPixmapItem) -> None:
-        self._graphics_item = graphics_item
-        self._pixmap = self._graphics_item.pixmap()
+        widthMax, heightMax = scrollbarW.maximum(), scrollbarH.maximum()
 
-    def contains(self, point: QPointF) -> bool:
-        return self._graphics_item.contains(point)
+        for view in self.main.bound_graphics_views[self] - {self}:
+            if view.isVisible():
+                wBar, hBar = view.horizontalScrollBar(), view.verticalScrollBar()
 
-    def hide(self) -> None:
-        self._graphics_item.hide()
+                if widthMax:
+                    wBar.setValue(int(scrollbarW.value() * wBar.maximum() / widthMax))
 
-    def pixmap(self) -> QPixmap:
-        return self._graphics_item.pixmap()
+                if heightMax:
+                    hBar.setValue(int(scrollbarH.value() * hBar.maximum() / heightMax))
 
-    def setPixmap(self, new_pixmap: QPixmap | None, crop_values: CroppingInfo | None = None) -> None:
-        if new_pixmap is None:
-            new_pixmap = self._pixmap
-        else:
-            self._pixmap = new_pixmap
+    @property
+    def content_width(self) -> int:
+        raise NotImplementedError
 
-        if crop_values is not None and crop_values.active:
-            padded = QPixmap(new_pixmap.width(), new_pixmap.height())
-            padded.fill(QColor(0, 0, 0, 0))
-            painter = QPainter(padded)
-            painter.drawPixmap(
-                QPoint(crop_values.left, crop_values.top), new_pixmap,
-                QRect(crop_values.left, crop_values.top, crop_values.width, crop_values.height)
-            )
-            painter.end()
-            new_pixmap = padded
+    @property
+    def content_height(self) -> int:
+        raise NotImplementedError
 
-        self._graphics_item.setPixmap(new_pixmap)
 
-    def show(self) -> None:
-        self._graphics_item.show()
+class MainVideoOutputGraphicsView(GraphicsView):
+    @property
+    def content_width(self) -> int:
+        return self.main.current_output.width
+
+    @property
+    def content_height(self) -> int:
+        return self.main.current_output.height
```

### Comparing `vspreview-0.5.0/vspreview/core/custom/misc.py` & `vspreview-0.6.0/vspreview/core/custom/misc.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/core/custom/notch.py` & `vspreview-0.6.0/vspreview/core/custom/notch.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/core/custom/plotting.py` & `vspreview-0.6.0/vspreview/core/custom/plotting.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 from __future__ import annotations
 
+from abc import abstractmethod
+from io import BytesIO
 from math import exp, log
 from pathlib import Path
-from typing import Sequence
+from typing import TYPE_CHECKING, Sequence, cast
 
 import matplotlib.pyplot as plt  # type: ignore
+from matplotlib.backend_bases import MouseEvent as PlotMouseEvent  # type: ignore
 from matplotlib.backends.backend_qtagg import FigureCanvasQTAgg  # type: ignore
 from matplotlib.figure import Figure  # type: ignore
 from matplotlib.layout_engine import ConstrainedLayoutEngine  # type: ignore
+from matplotlib.lines import Line2D  # type: ignore
 from matplotlib.rcsetup import cycler  # type: ignore
 from PyQt6.QtCore import QEvent, QPointF, Qt, pyqtSignal
-from PyQt6.QtGui import QMouseEvent, QNativeGestureEvent, QWheelEvent
+from PyQt6.QtGui import QImage, QMouseEvent, QNativeGestureEvent, QWheelEvent
+from PyQt6.QtWidgets import QFileDialog, QFrame
+
+if TYPE_CHECKING:
+    from ...main import MainWindow
+    from ..types import Frame
 
 STYLE_DIR = Path(__file__).parent / 'plotting.mplstyle'
 
 
 __all__ = [
     'apply_plotting_style',
 
-    'PlottingCanvas'
+    'PlottingCanvas',
+
+    'PlotMouseEvent'
 ]
 
 
 def apply_plotting_style() -> None:
     plt.style.use({
         'axes.edgecolor': '#FFFFFF3D',
         'axes.facecolor': '#FFFFFF07',
@@ -44,36 +55,84 @@
 
 class PlottingCanvas(FigureCanvasQTAgg):
     WHEEL_STEP = 15 * 8  # degrees
 
     mouseMoved = pyqtSignal(QMouseEvent)
     wheelScrolled = pyqtSignal(int)
 
-    def __init__(self, ylog: bool = False, xlog: bool = False) -> None:
+    def __init__(
+        self, main: MainWindow, ylog: bool = False, xlog: bool = False, controls: bool = True,
+        xpad: float | tuple[float, float] | None = None, ypad: float | tuple[float, float] | None = None,
+        figsize: tuple[int, int] = (5, 4)
+    ) -> None:
+        from ..abstracts import HBoxLayout, PushButton
+        from ..types import Stretch
+
+        self.main = main
+
         self.ylog, self.xlog = ylog, xlog
 
-        self.figure = Figure((5, 4), 100)
+        self.figure = Figure(figsize, self.main.settings.base_ppi)
 
         self.axes = self.figure.add_subplot(111)
 
         self.figure.set_layout_engine(ConstrainedLayoutEngine())
 
         super().__init__(self.figure)
 
+        self.mpl_connect('motion_notify_event', self._on_mouse_moved)
+
         self.angleRemainder = 0
         self.zoomValue = 0.0
 
         self.clicked = False
         self.old_pos = QPointF(0.0, 0.0)
 
+        self.controls = QFrame()
+
+        self.copy_frame_button = PushButton('Copy Graph', clicked=self.copy_graph_to_clipboard)
+
+        self.save_frame_as_button = PushButton('Save Graph as', clicked=self.on_save_graph_as_clicked)
+
+        _controls = [self.copy_frame_button, self.save_frame_as_button, Stretch()]
+
+        if controls:
+            self.controls = HBoxLayout(_controls)
+        else:
+            self.controls = QFrame()
+            HBoxLayout(self.controls, _controls)
+            self.controls.hide()
+
+        self.xpad = (xpad, xpad) if (not isinstance(xpad, tuple) and xpad is not None) else xpad
+        self.ypad = (ypad, ypad) if (not isinstance(ypad, tuple) and ypad is not None) else ypad
+
+    def _on_mouse_moved(self, event: PlotMouseEvent) -> None:
+        if not event.inaxes or not self.axes.lines:
+            return
+
+        if event.xdata is None or event.ydata is None:
+            return
+
+        if event.xdata < self.line._xorig[0] or event.xdata > self.line._xorig[-1]:
+            return
+
+        self.on_mouse_moved(event)
+
+    def on_mouse_moved(self, event: PlotMouseEvent) -> None:
+        ...
+
     @classmethod
     def limits_to_range(cls, lim: tuple[int, int]) -> int:
         return lim[1] - lim[0]
 
     @property
+    def line(self) -> Line2D:
+        return cast(Line2D, self.axes.lines[0])
+
+    @property
     def cur_lims(self) -> tuple[tuple[float, float], tuple[float, float]]:
 
         try:
             return (
                 tuple[float, float](log(x) if self.xlog else x for x in self.axes.get_xlim()),
                 tuple[float, float](log(x) if self.ylog else x for x in self.axes.get_ylim())
             )
@@ -206,7 +265,54 @@
 
         if self.xlog:
             self.axes.set_xscale("log")
 
     def draw(self) -> None:
         if 0 not in self.figure.get_size_inches():
             super().draw()
+
+    def copy_graph_to_clipboard(self) -> None:
+        buffer = BytesIO()
+
+        self.figure.savefig(buffer, transparent=False)
+
+        self.main.clipboard.setImage(QImage.fromData(buffer.getvalue()))
+
+        buffer.close()
+
+        self.main.show_message('Graph successfully copied to clipboard')
+
+    def on_save_graph_as_clicked(self, checked: bool | None = None) -> None:
+        save_path_str, _ = QFileDialog.getSaveFileName(
+            self.main, 'Save as', f'graph_{self.main.current_output.last_showed_frame}', 'Graph (*.svg)'
+        )
+
+        self.figure.savefig(save_path_str, transparent=False)
+
+    @abstractmethod
+    def _render(self, frame: Frame) -> None:
+        raise NotImplementedError
+
+    def render(self, frame: Frame, set_lims: bool = True) -> None:
+        if not set_lims:
+            self.zoomValue = 0.0
+
+        lims = self.cur_lims if self.zoomValue else None
+
+        self.clear()
+
+        self._render(frame)
+
+        self.axes.legend()
+        self.figure.canvas.draw_idle()
+
+        if lims:
+            self.cur_lims = lims
+        elif self.xpad or self.ypad:
+            xlim, ylim = self.cur_lims
+
+            line = self.line
+
+            self.cur_lims = (
+                (line._xorig[0] - self.xpad[0], line._xorig[-1] + self.xpad[1]) if self.xpad else xlim,
+                (line._yorig[0] - self.ypad[0], line._yorig[-1] + self.ypad[1]) if self.ypad else ylim
+            )
```

### Comparing `vspreview-0.5.0/vspreview/core/logger.py` & `vspreview-0.6.0/vspreview/core/logger.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/core/types/audio.py` & `vspreview-0.6.0/vspreview/core/types/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,19 @@
     )
 
     def __init__(self, vs_output: vs.AudioNode, index: int, new_storage: bool = False) -> None:
         self.setValue(vs_output, index, new_storage)
 
     def setValue(self, vs_output: vs.AudioNode, index: int, new_storage: bool = False) -> None:
         self.main = main_window()
-        self.index = index
+
+        with self.main.env:
+            vs_outputs = list(vs.get_outputs().values())
+
+        self.index = vs_outputs.index(vs_output)
         self.source_vs_output = vs_output
         self.vs_output = self.source_vs_output
         self.is_mono = self.vs_output.num_channels == 1
 
         (self.arrayType, sampleTypeQ) = (
             'f', QAudioFormat.SampleFormat.Float
         ) if self.vs_output.sample_type == vs.FLOAT else (
@@ -81,17 +85,15 @@
 
         self.audio_buffer = array(self.arrayType, [0] * self.SAMPLES_PER_FRAME * (self.vs_output.bytes_per_sample // 2))
 
         if not hasattr(self, 'name'):
             from ...models.outputs import AudioOutputs
 
             if vs_output in (vs_outputs := list(vs.get_outputs().values())):
-                self.name = self.main.user_output_names[vs.AudioNode].get(
-                    vs_outputs.index(vs_output), 'Track ' + str(self.index)
-                )
+                self.name = self.main.user_output_names[vs.AudioNode].get(self.index, 'Track ' + str(self.index))
                 if isinstance(self.main.toolbars.playback.audio_outputs, AudioOutputs):
                     self.main.toolbars.playback.audio_outputs.setData(
                         self.main.toolbars.playback.audio_outputs.index(index), self.name
                     )
 
     def clear(self) -> None:
         self.source_vs_output = self.vs_output = None  # type: ignore
```

### Comparing `vspreview-0.5.0/vspreview/core/types/scene.py` & `vspreview-0.6.0/vspreview/core/types/scene.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/core/types/units.py` & `vspreview-0.6.0/vspreview/core/types/units.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/core/types/video.py` & `vspreview-0.6.0/vspreview/core/types/video.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from ..abstracts import AbstractYAMLObject, main_window, try_load
 from .misc import CroppingInfo, VideoOutputNode
 from .units import Frame, Time
 
 if TYPE_CHECKING:
     from vstools import VideoFormatT
+    from ..custom.graphicsview import GraphicsImageItem
 
 __all__ = [
     'VideoOutput'
 ]
 
 
 class PackingTypeInfo:
@@ -60,15 +61,15 @@
 class VideoOutput(AbstractYAMLObject):
     storable_attrs = (
         'title', 'last_showed_frame', 'play_fps', 'crop_values'
     )
 
     __slots__ = (
         *storable_attrs, 'index', 'width', 'height', 'fps_num', 'fps_den',
-        'total_frames', 'total_time', 'graphics_scene_item',
+        'total_frames', 'total_time',
         'end_frame', 'fps', 'source', 'prepared',
         'main', 'checkerboard', 'props', '_stateset'
     )
 
     source: VideoOutputNode
     prepared: VideoOutputNode
     title: str | None
@@ -76,23 +77,21 @@
     crop_values: CroppingInfo
     _stateset: bool
 
     def clear(self) -> None:
         self.source = self.prepared = None  # type: ignore
 
     def __init__(
-        self, vs_output: vs.VideoOutputTuple | VideoOutputNode, index: int, new_storage: bool = False
+        self, vs_output: vs.VideoOutputTuple, index: int, new_storage: bool = False
     ) -> None:
         self.setValue(vs_output, index, new_storage)
 
     def setValue(
-        self, vs_output: vs.VideoOutputTuple | VideoOutputNode, index: int, new_storage: bool = False
+        self, vs_output: vs.VideoOutputTuple, index: int, new_storage: bool = False
     ) -> None:
-        from ..custom.graphicsview import GraphicsImageItem
-
         self._stateset = not new_storage
 
         self.main = main_window()
 
         assert self.main.env
 
         self.set_fmt_values()
@@ -100,41 +99,39 @@
         # runtime attributes
         self.source = VideoOutputNode(vs_output.clip, vs_output.alpha)
         self.prepared = VideoOutputNode(vs_output.clip, vs_output.alpha)
 
         if self.source.alpha is not None:
             self.prepared.alpha = self.prepare_vs_output(self.source.alpha, True).std.CopyFrameProps(self.source.alpha)
 
-        self.index = index
+        with self.main.env:
+            vs_outputs = list(vs.get_outputs().values())
+
+        self.vs_index = index
+        self.index = vs_outputs.index(vs_output) if vs_output in vs_outputs else index
 
         self.prepared.clip = self.prepare_vs_output(self.source.clip).std.CopyFrameProps(self.source.clip)
         self.width = self.prepared.clip.width
         self.height = self.prepared.clip.height
         self.fps_num = self.prepared.clip.fps.numerator
         self.fps_den = self.prepared.clip.fps.denominator
         self.fps = self.fps_num / self.fps_den
         self.total_frames = Frame(self.prepared.clip.num_frames)
-        self.title = None
-
-        with self.main.env:
-            if vs_output in (vs_outputs := list(vs.get_outputs().values())):
-                self.title = self.main.user_output_names[vs.VideoNode].get(vs_outputs.index(vs_output))  # type: ignore
-                if self.main.outputs is not None:
-                    self.main.outputs.setData(self.main.outputs.index(index), self.title)
+        self.title = self.main.user_output_names[vs.VideoNode].get(self.vs_index, None)  # type: ignore
+        if self.main.outputs is not None:
+            self.main.outputs.setData(self.main.outputs.index(self.vs_index), self.title)
 
         self.props = cast(vs.FrameProps, {})
 
         if self.source.alpha:
             self.checkerboard = self._generate_checkerboard()
 
         if not hasattr(self, 'last_showed_frame') or not (0 <= self.last_showed_frame < self.total_frames):
             self.last_showed_frame = Frame(0)
 
-        self.graphics_scene_item: GraphicsImageItem
-
         if index in self.main.timecodes:
             timecodes, tden = self.main.timecodes[index]
 
             if self.fps_num == 0:
                 try:
                     play_fps = self.main.toolbars.playback.get_true_fps(0, self.props, True)
                 except Exception:
@@ -397,40 +394,52 @@
 
         pointer = cast(
             sip.voidptr, ccast(frame.get_read_ptr(0), POINTER(point_size * stride)).contents
         )
 
         return QImage(pointer, width, height, stride, qt_format).copy()  # type: ignore
 
+    @property
+    def graphics_scene_item(self) -> GraphicsImageItem | None:
+        if self.main.graphics_view.graphics_scene.graphics_items:
+            try:
+                return self.main.graphics_view.graphics_scene.graphics_items[self.index]
+            except IndexError:
+                ...
+
+        return None
+
     def update_graphic_item(
-        self, pixmap: QPixmap | None = None, crop_values: CroppingInfo | None | bool = None
+        self, pixmap: QPixmap | None = None, crop_values: CroppingInfo | None | bool = None,
+        graphics_scene_item: GraphicsImageItem | None = None
     ) -> QPixmap | None:
         from vstools import complex_hash
 
         old_crop = complex_hash.hash(self.crop_values)
 
         if isinstance(crop_values, bool):
             self.crop_values.active = crop_values
         elif crop_values is not None:
             self.crop_values = crop_values
 
         new_crop = complex_hash.hash(self.crop_values)
 
-        if hasattr(self, 'graphics_scene_item'):
-            self.graphics_scene_item.setPixmap(pixmap, self.crop_values)
+        if graphics_scene_item:
+            graphics_scene_item.setPixmap(pixmap, self.crop_values)
 
         if old_crop != new_crop:
             self.main.cropValuesChanged.emit(self.crop_values)
 
         return pixmap
 
     def render_frame(
         self, frame: Frame | None, vs_frame: vs.VideoFrame | None = None,
-        vs_alpha_frame: vs.VideoFrame | None = None, do_painting: bool = True,
-        output_colorspace: QColorSpace | None = None
+        vs_alpha_frame: vs.VideoFrame | None = None,
+        graphics_scene_item: GraphicsImageItem | None = None,
+        do_painting: bool = True, output_colorspace: QColorSpace | None = None
     ) -> QPixmap:
         if frame is None or not self._stateset:
             return QPixmap()
 
         frame = min(max(frame, Frame(0)), self.total_frames - 1)
 
         vs_frame = vs_frame or self.prepared.clip.get_frame(frame.value)
@@ -443,19 +452,22 @@
             frame_image.setColorSpace(QColorSpace(QColorSpace.NamedColorSpace.SRgb))
             frame_image.convertToColorSpace(output_colorspace)
 
         if not vs_frame.closed:
             vs_frame.close()
             del vs_frame
 
+        if graphics_scene_item is None:
+            graphics_scene_item = self.graphics_scene_item
+
         if self.prepared.alpha is None:
             qpixmap = QPixmap.fromImage(frame_image, Qt.ImageConversionFlag.NoFormatConversion)
 
             if do_painting:
-                self.update_graphic_item(qpixmap)
+                self.update_graphic_item(qpixmap, graphics_scene_item=graphics_scene_item)
 
             return qpixmap
 
         alpha_image = self.frame_to_qimage(
             vs_alpha_frame or self.prepared.alpha.get_frame(frame.value), True
         )
 
@@ -471,15 +483,15 @@
             painter.drawImage(0, 0, self.checkerboard)
 
         painter.end()
 
         qpixmap = QPixmap.fromImage(result_image, Qt.ImageConversionFlag.NoFormatConversion)
 
         if do_painting:
-            self.update_graphic_item(qpixmap)
+            self.update_graphic_item(qpixmap, graphics_scene_item=graphics_scene_item)
 
         return qpixmap
 
     def _generate_checkerboard(self) -> QImage:
         tile_size = self.main.toolbars.playback.settings.CHECKERBOARD_TILE_SIZE
         tile_color_1 = self.main.toolbars.playback.settings.CHECKERBOARD_TILE_COLOR_1
         tile_color_2 = self.main.toolbars.playback.settings.CHECKERBOARD_TILE_COLOR_2
@@ -536,14 +548,26 @@
 
     def to_frame(self, time: Time) -> Frame:
         return Frame(self._calculate_frame(float(time)))
 
     def to_time(self, frame: Frame) -> Time:
         return Time(seconds=self._calculate_seconds(int(frame)))
 
+    def with_node(self, new_node: vs.VideoNode | VideoOutputNode) -> VideoOutput:
+        if isinstance(new_node, vs.VideoNode):
+            new_node = VideoOutputNode(new_node, None)
+
+        new_output = VideoOutput(new_node, self.vs_index, False)
+        new_output.index = self.index
+
+        new_output.last_showed_frame = self.last_showed_frame
+        new_output.name = self.name
+
+        return new_output
+
     def __setstate__(self, state: Mapping[str, Any]) -> None:
         try_load(state, 'title', str, self.__setattr__)
         try_load(state, 'last_showed_frame', Frame, self.__setattr__)
         try_load(state, 'play_fps', Fraction, self.__setattr__)
         try_load(state, 'crop_values', CroppingInfo, self.__setattr__)
 
         self._stateset = True
```

### Comparing `vspreview-0.5.0/vspreview/core/types/yaml.py` & `vspreview-0.6.0/vspreview/core/types/yaml.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/core/vsenv.py` & `vspreview-0.6.0/vspreview/core/vsenv.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/init.py` & `vspreview-0.6.0/vspreview/init.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,24 +11,30 @@
 from PyQt6.QtWidgets import QApplication
 
 # import vsenv as early as possible:
 # This is so other modules cannot accidentally use and lock us into a different policy.
 from .core.vsenv import set_vsengine_loop
 from .core.logger import set_log_level, setup_logger
 from .main import MainWindow
+from .plugins.install import install_plugins, plugins_commands, uninstall_plugins
 
 __all__ = [
     'main'
 ]
 
 
 def main(_args: Sequence[str] | None = None) -> None:
     parser = ArgumentParser(prog='VSPreview')
     parser.add_argument(
-        'script_path', help='Path to Vapoursynth script', type=Path, nargs='?'
+        'script_path_or_command', type=str, nargs='?',
+        help=f'Path to Vapoursynth script or plugins command {",".join(plugins_commands)}'
+    )
+    parser.add_argument(
+        'plugins', type=str, nargs='+',
+        help='Plugins to install/uninstall/update'
     )
     parser.add_argument(
         '--version', '-v', action='version', version='%(prog)s 0.2b'
     )
     parser.add_argument(
         '--preserve-cwd', '-c', action='store_true', help='do not chdir to script parent directory'
     )
@@ -39,14 +45,20 @@
     parser.add_argument(
         '--vscode-setup', type=str, choices=['override', 'append', 'ignore'], nargs='?', const='append',
         help='Installs launch settings in cwd\'s .vscode'
     )
     parser.add_argument(
         "--verbose", help="Set the logging to verbose.", action="store_true"
     )
+    parser.add_argument(
+        "--force", help="Force the install of a plugin even if it exists already.", action="store_true"
+    )
+    parser.add_argument(
+        "--no-deps", help="Ignore downloading dependencies.", action="store_true"
+    )
 
     args = parser.parse_args(_args)
 
     setup_logger()
 
     if args.verbose:
         set_log_level(logging.DEBUG, logging.DEBUG)
@@ -56,19 +68,40 @@
     if args.vscode_setup is not None:
         from .api.other import install_vscode_launch
 
         install_vscode_launch(args.vscode_setup)
 
         sys.exit(0)
 
-    if args.script_path is None:
+    script_path_or_command = args.script_path_or_command
+
+    if not script_path_or_command and not (args.plugins and (script_path_or_command := next(iter(args.plugins)))):
         logging.error('Script path required.')
         sys.exit(1)
 
-    script_path = args.script_path.resolve()
+    if (command := script_path_or_command) in plugins_commands:
+        if not args.plugins:
+            logging.error('You must provide at least one plugin!')
+            sys.exit(1)
+
+        set_log_level(logging.INFO)
+
+        plugins = list(args.plugins)
+
+        if command == 'install':
+            install_plugins(plugins, args.force, args.no_deps)
+        elif command == 'uninstall':
+            uninstall_plugins(plugins)
+        elif command == 'update':
+            uninstall_plugins(plugins, True)
+            install_plugins(plugins, True, args.no_deps)
+
+        sys.exit(0)
+
+    script_path = Path(script_path_or_command).resolve()
     if not script_path.exists():
         logging.error('Script path is invalid.')
         sys.exit(1)
 
     if not args.preserve_cwd:
         os.chdir(script_path.parent)
```

### Comparing `vspreview-0.5.0/vspreview/main/dialog.py` & `vspreview-0.6.0/vspreview/main/dialog.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/main/settings.py` & `vspreview-0.6.0/vspreview/main/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,16 +204,16 @@
             try:
                 old_default_idx = new_levels.index(int(old_default))
             except ValueError:
                 old_default_idx = old_values.index(int(old_default))
                 old_default_idx = min(max(old_default_idx - 1, 0), old_default_idx + 1, len(new_levels) - 1)
             self.zoom_level_default_combobox.setCurrentIndex(old_default_idx)
 
-        if hasattr((main := main_window()), 'toolbars'):
-            main_zoom_comb = main.toolbars.main.zoom_combobox
+        if hasattr((main := main_window()), 'graphics_view'):
+            main_zoom_comb = main.graphics_view.zoom_combobox
             old_index = main_zoom_comb.currentIndex()
             main_zoom_comb.setModel(GeneralModel[float](self.zoom_levels))
             main_zoom_comb.setCurrentIndex(min(max(old_index, 0), len(new_levels) - 1))
 
         self.zoom_levels_lineedit.clear()
 
     @property
@@ -321,15 +321,15 @@
     def __getstate__(self) -> Mapping[str, Any]:
         main = main_window()
 
         return {
             'timeline_mode': main.timeline.mode,
             'window_geometry': bytes(cast(bytearray, main.saveGeometry())),
             'window_state': bytes(cast(bytearray, main.saveState())),
-            'zoom_index': main.toolbars.main.zoom_combobox.currentIndex(),
+            'zoom_index': main.graphics_view.zoom_combobox.currentIndex(),
             'x_pos': main.graphics_view.horizontalScrollBar().value(),
             'y_pos': main.graphics_view.verticalScrollBar().value(),
         }
 
     def __setstate__(self, state: Mapping[str, Any]) -> None:
         try_load(state, 'timeline_mode', str, self.__setattr__)
         try_load(state, 'window_geometry', bytes, self.__setattr__)
@@ -338,14 +338,14 @@
         try_load(state, 'x_pos', int, self.__setattr__)
         try_load(state, 'y_pos', int, self.__setattr__)
 
         main = main_window()
 
         main.timeline.mode = self.timeline_mode
 
-        main.toolbars.main.zoom_combobox.setCurrentIndex(self.zoom_index)
+        main.graphics_view.zoom_combobox.setCurrentIndex(self.zoom_index)
 
         main.graphics_view.horizontalScrollBar().setValue(self.x_pos)
         main.graphics_view.verticalScrollBar().setValue(self.y_pos)
 
         main.restoreState(self.window_state)
         main.restoreGeometry(self.window_geometry)
```

### Comparing `vspreview-0.5.0/vspreview/main/timeline.py` & `vspreview-0.6.0/vspreview/main/timeline.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/main/window.py` & `vspreview-0.6.0/vspreview/main/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from __future__ import annotations
 
 import io
 import logging
 import sys
 from fractions import Fraction
+from functools import partial
 from importlib import reload as reload_module
 from pathlib import Path
 from time import time
 from typing import Any, Iterable, Mapping, cast
 
 import vapoursynth as vs
 from PyQt6 import QtCore
-from PyQt6.QtCore import QEvent, QRectF, pyqtSignal
-from PyQt6.QtGui import QCloseEvent, QColorSpace, QMoveEvent, QPalette, QPixmap, QShowEvent
-from PyQt6.QtOpenGLWidgets import QOpenGLWidget
-from PyQt6.QtWidgets import (
-    QApplication, QGraphicsScene, QGraphicsView, QLabel, QMainWindow, QSizePolicy, QSplitter, QTabWidget
-)
+from PyQt6.QtCore import QEvent, QKeyCombination, QRectF, Qt, pyqtSignal
+from PyQt6.QtGui import QCloseEvent, QColorSpace, QKeySequence, QMoveEvent, QShortcut, QShowEvent
+from PyQt6.QtWidgets import QApplication, QLabel, QMainWindow, QSizePolicy, QSplitter, QTabWidget
 from vsengine import vpy  # type: ignore
 
 from ..core import (
     PRELOADED_MODULES, AbstractQItem, CroppingInfo, DragNavigator, ExtendedWidget, Frame, GraphicsImageItem,
-    GraphicsView, HBoxLayout, QAbstractYAMLObjectSingleton, StatusBar, Time, Timer, VBoxLayout, VideoOutput, ViewMode,
-    _monkey_runpy_dicts, get_current_environment, make_environment
+    GraphicsView, HBoxLayout, QAbstractYAMLObjectSingleton, StatusBar, Time, Timer, VBoxLayout, VideoOutput,
+    _monkey_runpy_dicts, get_current_environment, make_environment, MainVideoOutputGraphicsView
 )
-from ..models import VideoOutputs
+from ..models import GeneralModel, VideoOutputs
 from ..plugins import Plugins
 from ..toolbars import Toolbars
 from ..utils import fire_and_forget, set_status_label
 from .dialog import ScriptErrorDialog, SettingsDialog
 from .settings import MainSettings, WindowSettings
 from .timeline import Timeline
 
@@ -75,38 +73,40 @@
         if self.previous_position == 0 and self.current_position:
             self.main_window.plugins.update()
 
         self.previous_position = self.current_position
 
 
 class MainWindow(AbstractQItem, QMainWindow, QAbstractYAMLObjectSingleton):
-    current_viewmode: ViewMode
-
     VSP_DIR_NAME = '.vspreview'
     VSP_GLOBAL_DIR_NAME = Path(
         expandvars('%APPDATA%') if sys.platform == "win32" else expanduser('~/.config')  # type: ignore
     )
 
+    global_config_dir = VSP_GLOBAL_DIR_NAME / VSP_DIR_NAME
+    global_storage_path = global_config_dir / '.global.yml'
+    global_plugins_dir = global_config_dir / 'plugins'
+
     VSP_VERSION = 3.2
     BREAKING_CHANGES_VERSIONS = list[str](['3.0', '3.1'])
 
     # status bar
     def STATUS_FRAME_PROP(self, prop: Any) -> str:
         return 'Type: %s' % (prop['_PictType'].decode('utf-8') if '_PictType' in prop else '?')
 
     EVENT_POLICY = QSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
 
     storable_attrs = ('settings', 'toolbars')
 
     __slots__ = (
         *storable_attrs, 'app', 'display_scale', 'clipboard',
         'script_path', 'timeline', 'main_layout', 'autosave_timer',
-        'graphics_scene', 'graphics_view', 'script_error_dialog',
+        'graphics_view', 'script_error_dialog',
         'central_widget', 'statusbar', 'storage_not_found',
-        'current_storage_path', 'opengl_widget', 'drag_navigator'
+        'current_storage_path'
     )
 
     # emit when about to reload a script: clear all existing references to existing clips.
     reload_signal = pyqtSignal()
     reload_before_signal = pyqtSignal()
     reload_after_signal = pyqtSignal()
     cropValuesChanged = pyqtSignal(CroppingInfo)
@@ -122,24 +122,23 @@
         from ..toolbars import MainToolbar
 
         super().__init__()
 
         self.settings = MainSettings(MainToolbar)
 
         self.current_config_dir = config_dir / self.VSP_DIR_NAME
-        self.global_config_dir = self.VSP_GLOBAL_DIR_NAME / self.VSP_DIR_NAME
-        self.global_storage_path = self.global_config_dir / '.global.yml'
-        self.global_plugins_dir = self.global_config_dir / 'plugins'
         self.global_plugins_dir.mkdir(parents=True, exist_ok=True)
 
         self.app = cast(QApplication, QApplication.instance())
         assert self.app
 
         self.last_reload_time = time()
 
+        self.bound_graphics_views = dict[GraphicsView, set[GraphicsView]]()
+
         if self.settings.dark_theme_enabled:
             from ..core import apply_plotting_style
 
             try:
                 from qdarkstyle import _load_stylesheet  # type: ignore[import]
             except ImportError:
                 self.settings.dark_theme_enabled = False
@@ -171,27 +170,14 @@
         # global
         self.clipboard = self.app.clipboard()
         self.external_args = list[tuple[str, str]]()
         self.script_path = Path()
         self.script_exec_failed = False
         self.current_storage_path = Path()
 
-        # graphics view
-        self.graphics_scene = QGraphicsScene(self)
-        self.graphics_view.setScene(self.graphics_scene)
-        self.opengl_widget = None
-
-        if self.settings.opengl_rendering_enabled:
-            self.opengl_widget = QOpenGLWidget()
-            self.graphics_view.setViewport(self.opengl_widget)
-
-        self.graphics_view.wheelScrolled.connect(self.on_wheel_scrolled)
-
-        self.graphics_view.registerReloadEvents(self)
-
         # timeline
         self.timeline.clicked.connect(self.on_timeline_clicked)
 
         # display profile
         self.display_profile: QColorSpace | None = None
         self.current_screen = self.app.primaryScreen()
 
@@ -207,32 +193,27 @@
         Plugins(self)
 
         self.app_settings.tab_widget.setUsesScrollButtons(False)
         self.app_settings.setMinimumWidth(
             int(len(self.toolbars) * 1.05 * self.app_settings.tab_widget.geometry().width() / 2)
         )
 
-        self.current_viewmode = ViewMode.NORMAL
-
         self.set_qobject_names()
         self.setObjectName('MainWindow')
 
         self.env: vpy.Script | None = None
 
     def setup_ui(self) -> None:
         self.central_widget = ExtendedWidget(self)
         self.main_layout = VBoxLayout(self.central_widget)
         self.setCentralWidget(self.central_widget)
 
-        self.graphics_view = GraphicsView(self.central_widget)
-        self.graphics_view.setBackgroundBrush(self.palette().brush(QPalette.ColorRole.Window))
-        self.graphics_view.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
-        self.graphics_view.setDragMode(QGraphicsView.DragMode.ScrollHandDrag)
+        self.graphics_view = MainVideoOutputGraphicsView(self, self.central_widget)
 
-        self.drag_navigator = DragNavigator(self, self.graphics_view)
+        DragNavigator(self, self.graphics_view)
 
         self.timeline = Timeline(self.central_widget)
 
         self.plugins_tab = QTabWidget(self.central_widget)
         self.plugins_tab.currentChanged.connect(lambda x: self.plugins.update())
 
         self.main_split = CentralSplitter(self, QtCore.Qt.Orientation.Horizontal)
@@ -261,14 +242,25 @@
 
         # dialogs
         self.script_error_dialog = ScriptErrorDialog(self)
 
         self.autosave_timer = Timer(timeout=self.dump_storage_async)
         self.reload_signal.connect(self.autosave_timer.stop)
 
+        QShortcut(
+            QKeySequence(QKeyCombination(Qt.Modifier.CTRL, Qt.Key.Key_A).toCombined()),
+            self, activated=self.auto_fit_keyswitch
+        )
+
+    def auto_fit_keyswitch(self) -> None:
+        for view in self.graphics_views:
+            if view.underMouse():
+                view.autofit = not view.autofit
+                break
+
     def patch_dark_stylesheet(self, stylesheet: str) -> str:
         return stylesheet + 'QGraphicsView { border: 0px; padding: 0px; }'
 
     def load_script(
         self, script_path: Path, external_args: list[tuple[str, str]] | None = None, reloading: bool = False,
         start_frame: int | None = None
     ) -> None:
@@ -399,16 +391,14 @@
         except Exception as e:
             load_error = e
 
         with self.env:
             vs.register_on_destroy(self.gc_collect)
 
         if load_error is None:
-            self.change_video_viewmode(self.current_viewmode)
-
             self.autosave_timer.start(round(float(self.settings.autosave_interval) * 1000))
 
             if not reloading:
                 self.switch_output(self.settings.output_index)
                 if start_frame is not None:
                     self.switch_frame(Frame(start_frame))
         else:
@@ -585,21 +575,18 @@
 
         return storage_dump.getvalue()
 
     def init_outputs(self) -> None:
         if not self.outputs:
             return
 
-        self.graphics_scene.clear()
+        self.plugins.init_outputs()
 
-        for output in self.outputs:
-            raw_frame_item = self.graphics_scene.addPixmap(QPixmap())
-            raw_frame_item.hide()
-
-            output.graphics_scene_item = GraphicsImageItem(raw_frame_item)
+        for graphics_view in self.graphics_views:
+            graphics_view.graphics_scene.init_scenes()
 
     def reload_script(self) -> None:
         from vstools.utils.vs_proxy import clear_cache
 
         self.reload_before_signal.emit()
 
         self.dump_storage()
@@ -607,15 +594,16 @@
         try:
             with self.env:
                 clear_cache()
         except Exception:
             ...
 
         vs.clear_outputs()
-        self.graphics_scene.clear()
+        for graphics_view in self.graphics_views:
+            graphics_view.graphics_scene.clear()
 
         self.timecodes.clear()
         self.norm_timecodes.clear()
         for v in self.user_output_names.values():
             v.clear()
         if self.outputs:
             self.outputs.clear()
@@ -707,57 +695,69 @@
 
         # current_output relies on outputs_combobox
         self.toolbars.main.on_current_output_changed(index, prev_index)
         self.timeline.set_end_frame(self.current_output)
 
         self.switch_frame(self.current_output.last_showed_frame)
 
-        for output in self.outputs:
-            output.graphics_scene_item.hide()
+        for graphics_view in self.graphics_views:
+            for item in graphics_view.graphics_scene.graphics_items:
+                item.hide()
+
+            graphics_view.current_scene.show()
+            graphics_view.graphics_scene.setSceneRect(
+                QRectF(graphics_view.current_scene.pixmap().rect())
+            )
 
-        self.current_output.graphics_scene_item.show()
-        self.graphics_scene.setSceneRect(QRectF(self.current_output.graphics_scene_item.pixmap().rect()))
         self.timeline.update_notches()
 
         for toolbar in self.toolbars[1:]:
             toolbar.on_current_output_changed(index, prev_index)
 
         self.plugins.on_current_output_changed(index, prev_index)
 
         self.update_statusbar_output_info()
 
     @property
     def current_output(self) -> VideoOutput:
         return cast(VideoOutput, self.toolbars.main.outputs_combobox.currentData())
 
-    @current_output.setter
-    def current_output(self, value: VideoOutput) -> None:
-        if not self.outputs:
-            return
-
-        self.switch_output(self.outputs.index_of(value))
-
     @property
     def outputs(self) -> VideoOutputs | None:
         return self.toolbars.main.outputs
 
+    @property
+    def current_scene(self) -> GraphicsImageItem:
+        return self.graphics_view.current_scene
+
+    @property
+    def graphics_views(self) -> list[GraphicsView]:
+        return list(self.bound_graphics_views.keys())
+
+    def register_graphic_view(self, view: GraphicsView) -> None:
+        self.bound_graphics_views[view] = {view}
+
+        view.zoom_combobox.currentTextChanged.connect(partial(self.on_zoom_changed, bound_view=view))
+
+        view.zoom_combobox.setModel(GeneralModel[float](self.settings.zoom_levels))
+        view.zoom_combobox.setCurrentIndex(self.settings.zoom_default_index)
+
+    def on_zoom_changed(self, text: str | None = None, bound_view: GraphicsView | None = None) -> None:
+        if not bound_view:
+            return
+
+        for view in self.bound_graphics_views[bound_view]:
+            view.setZoom(bound_view.zoom_combobox.currentData())
+
     def handle_script_error(self, message: str, script: bool = False) -> None:
         self.clear_monkey_runpy()
         self.script_error_dialog.label.setText(message)
         self.script_error_dialog.setWindowTitle('Script Loading Error' if script else 'Program Error')
         self.script_error_dialog.open()
 
-    def on_wheel_scrolled(self, steps: int) -> None:
-        new_index = self.toolbars.main.zoom_combobox.currentIndex() + steps
-        if new_index < 0:
-            new_index = 0
-        elif new_index >= len(self.settings.zoom_levels):
-            new_index = len(self.settings.zoom_levels) - 1
-        self.toolbars.main.zoom_combobox.setCurrentIndex(new_index)
-
     def on_timeline_clicked(self, start: int) -> None:
         if self.toolbars.playback.play_timer.isActive():
             self.toolbars.playback.stop()
             self.switch_frame(start)
             self.toolbars.playback.play()
         else:
             self.switch_frame(start)
@@ -826,15 +826,16 @@
             self.timeline.full_repaint()
 
         return super().event(event)
 
     # misc methods
     def showEvent(self, event: QShowEvent) -> None:
         super().showEvent(event)
-        self.graphics_view.setSizePolicy(self.EVENT_POLICY)
+        for graphics_view in self.graphics_views:
+            graphics_view.setSizePolicy(self.EVENT_POLICY)
 
     def closeEvent(self, event: QCloseEvent) -> None:
         if self.settings.autosave_control.value() != Time(seconds=0):
             self.dump_storage_async()
 
         self.reload_signal.emit()
 
@@ -851,44 +852,14 @@
             return
 
         playback_active = self.toolbars.playback.play_timer.isActive()
 
         if playback_active:
             self.toolbars.playback.stop()
 
-        self.outputs.items = [
-            self.outputs.get_new_output(old.source.clip, old)
-            for old in self.outputs.items
-        ]
-
-        self.init_outputs()
-
-        self.switch_output(self.toolbars.main.outputs_combobox.currentIndex())
-
-        if playback_active:
-            self.toolbars.playback.play()
-
-    def change_video_viewmode(self, new_viewmode: ViewMode, force_cache: bool = False) -> None:
-        if not self.outputs:
-            return
-
-        playback_active = self.toolbars.playback.play_timer.isActive()
-
-        if playback_active:
-            self.toolbars.playback.stop()
-
-        if new_viewmode == ViewMode.NORMAL:
-            self.outputs.switchToNormalView()
-        elif new_viewmode == ViewMode.FFTSPECTRUM:
-            self.outputs.switchToFFTSpectrumView(force_cache)
-        else:
-            raise ValueError('Invalid ViewMode passed!')
-
-        self.current_viewmode = new_viewmode
-
         self.init_outputs()
 
         self.switch_output(self.toolbars.main.outputs_combobox.currentIndex())
 
         if playback_active:
             self.toolbars.playback.play()
```

### Comparing `vspreview-0.5.0/vspreview/models/generalmodel.py` & `vspreview-0.6.0/vspreview/models/generalmodel.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/models/scening.py` & `vspreview-0.6.0/vspreview/models/scening.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/plugins/__init__.py` & `vspreview-0.6.0/vspreview/plugins/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 from __future__ import annotations
 
 import logging
+import sys
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterable, Iterator, Mapping, cast, overload
 
 from ..core import AbstractYAMLObjectSingleton, Frame, storage_err_msg
+from . import utils
 from .abstract import AbstractPlugin, PluginConfig
+from .utils import *  # noqa: F401,F403
 
 if TYPE_CHECKING:
     from ..main import MainWindow
 
 
 __all__ = [
-    'AbstractPlugin', 'PluginConfig'
+    'AbstractPlugin', 'PluginConfig',
+    *utils.__all__
 ]
 
 
 class Plugins(AbstractYAMLObjectSingleton):
     __slots__ = ()
 
     _closure = {**globals()}
 
+    # tab idx, clip idx, frame
+    last_frame_change: tuple[int, int, int]
+
+    # tab idx, clip idx
+    last_output_change: tuple[int, int]
+
     @classmethod
     def file_to_plugins(cls, path: Path) -> Iterable[type[AbstractPlugin]]:
         from importlib.util import module_from_spec, spec_from_file_location
         if True:
             # has to be imported after the main
             from importlib._bootstrap_external import SOURCE_SUFFIXES  # type: ignore
             SOURCE_SUFFIXES.append('.ppy')
@@ -59,25 +69,60 @@
 
     def __init__(self, main: MainWindow) -> None:
         main.plugins = self
 
         self.main = main
         self.plugins_tab = main.plugins_tab
         self.main.main_split.setSizes([0, 0])
+        self.main.reload_before_signal.connect(self.reset_last_reload)
 
-        # tab idx, clip idx, frame
-        self.last_frame_change = (-1, -1, -1)
-
-        # tab idx, clip idx
-        self.last_output_change = (-1, -1)
+        self.reset_last_reload()
 
         self.plugins = dict[str, AbstractPlugin]()
 
-        for name in [*Path(__file__).parent.glob('*.ppy'), *self.main.global_plugins_dir.glob('*.ppy')]:
-            for plugin in self.file_to_plugins(name):
+        plugin_files = list[Path]()
+
+        def _find_files(folder: Path, ignore_path: bool = False) -> None:
+            files = list(folder.glob('*.ppy'))
+
+            if files:
+                if not ignore_path:
+                    sys.path.append(str(folder))
+
+                plugin_files.extend(files)
+
+        def _check_folder(folder: str | Path, ignore_path: bool = False) -> None:
+            if not folder:
+                return
+
+            if isinstance(folder, str):
+                folder = folder.strip()
+
+                if folder.startswith(';'):
+                    return
+
+                folder = Path(folder)
+
+            if not folder.is_dir():
+                return
+
+            _find_files(folder, ignore_path)
+
+            for folder in (f for f in folder.glob('*') if f.is_dir()):
+                _find_files(folder, ignore_path)
+
+        _check_folder(Path(__file__).parent, True)
+        _check_folder(self.main.global_plugins_dir)
+
+        for paths_file in self.main.global_plugins_dir.glob('*.pth'):
+            for path in paths_file.read_text('utf8').splitlines():
+                _check_folder(path)
+
+        for plugin_file in plugin_files:
+            for plugin in self.file_to_plugins(plugin_file):
                 if plugin._config.namespace in self.plugins:
                     print(UserWarning(
                         f'Tried to register plugin "{plugin._config.display_name} '
                         f'({plugin._config.namespace})" twice!'
                     ))
 
                 self.plugins[plugin._config.namespace] = plugin(self.main)
@@ -95,14 +140,23 @@
                 continue
 
             plugin.index = i
 
             self.plugins_tab.addTab(plugin, plugin._config.display_name)
             i += 1
 
+    def reset_last_reload(self) -> None:
+        self.last_frame_change = (-1, -1, -1)
+
+        self.last_output_change = (-1, -1)
+
+    def init_outputs(self) -> None:
+        for plugin in self:
+            plugin.init_outputs()
+
     def on_current_frame_changed(self, frame: Frame) -> None:
         tab_idx = self.plugins_tab.currentIndex()
 
         curr_render = (tab_idx, self.main.current_output.index, int(frame))
 
         if self.main.main_split.current_position and self.last_frame_change != curr_render:
             self[tab_idx].on_current_frame_changed(frame)
@@ -129,14 +183,19 @@
             fallback(frame, self.main.current_output.last_showed_frame)
         )
         self.on_current_output_changed(
             fallback(index, self.main.current_output.index),
             fallback(prev_index, self.main.current_output.index),
         )
 
+        sizel, sizer = self.main.main_split.sizes()
+
+        self.main.main_split.setSizes([sizel, sizer - 1])
+        self.main.main_split.setSizes([sizel, sizer])
+
     @overload
     def __getitem__(self, _sub: str | int) -> AbstractPlugin:
         ...
 
     @overload
     def __getitem__(self, _sub: slice) -> list[AbstractPlugin]:
         ...
```

### Comparing `vspreview-0.5.0/vspreview/plugins/abstract.py` & `vspreview-0.6.0/vspreview/plugins/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 
         self.setup_ui()
 
         self.add_shortcuts()
 
         self.set_qobject_names()
 
+    def init_outputs(self) -> None:
+        ...
+
     def add_shortcuts(self) -> None:
         ...
 
     def on_current_frame_changed(self, frame: Frame) -> None:
         ...
 
     def on_current_output_changed(self, index: int, prev_index: int) -> None:
```

### Comparing `vspreview-0.5.0/vspreview/plugins/frame_props.ppy` & `vspreview-0.6.0/vspreview/plugins/frame_props.ppy`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/toolbars/__init__.py` & `vspreview-0.6.0/vspreview/toolbars/__init__.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/toolbars/benchmark/settings.py` & `vspreview-0.6.0/vspreview/toolbars/benchmark/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/toolbars/benchmark/toolbar.py` & `vspreview-0.6.0/vspreview/toolbars/benchmark/toolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,16 @@
     def run(self) -> None:
         if self.settings.clear_cache_enabled:
             from vstools.utils.vs_proxy import clear_cache
             clear_cache()
 
         if self.settings.frame_data_sharing_fix_enabled:
             self.main.current_output.update_graphic_item(
-                self.main.current_output.graphics_scene_item.pixmap().copy()
+                self.main.current_scene.pixmap().copy(),
+                graphics_scene_item=self.main.current_output.graphics_scene_item
             )
 
         self.start_frame = self.start_frame_control.value()
         self.end_frame = self.end_frame_control.value()
         self.total_frames = self.total_frames_control.value()
         self.frames_left = deepcopy(self.total_frames)
         if self.prefetch_checkbox.isChecked():
```

### Comparing `vspreview-0.5.0/vspreview/toolbars/comp/settings.py` & `vspreview-0.6.0/vspreview/toolbars/comp/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/toolbars/comp/toolbar.py` & `vspreview-0.6.0/vspreview/toolbars/comp/toolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -810,17 +810,15 @@
             self.settings.browser_id, self.settings.session_id, tmdb_id, tags
         )
 
     _old_threads_workers = list[Any]()
 
     def upload_to_slowpics(self) -> bool:
         try:
-            self.main.current_output.graphics_scene_item.setPixmap(
-                self.main.current_output.graphics_scene_item.pixmap().copy()
-            )
+            self.main.current_scene.setPixmap(self.main.current_scene.pixmap().copy())
 
             if hasattr(self, 'upload_thread'):
                 self._old_threads_workers.append(self.upload_thread)
 
             if hasattr(self, 'upload_worker'):
                 self._old_threads_workers.append(self.upload_worker)
```

### Comparing `vspreview-0.5.0/vspreview/toolbars/debug/toolbar.py` & `vspreview-0.6.0/vspreview/toolbars/debug/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/toolbars/main/toolbar.py` & `vspreview-0.6.0/vspreview/toolbars/main/toolbar.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from PyQt6.QtCore import QKeyCombination, Qt
 from PyQt6.QtWidgets import QComboBox
 
 from ...core import (
     AbstractToolbar, CheckBox, ComboBox, Frame, FrameEdit, PushButton, Time, TimeEdit, VideoOutput, try_load
 )
-from ...models import GeneralModel, VideoOutputs
+from ...models import VideoOutputs
 from ...utils import qt_silent_call
 
 if TYPE_CHECKING:
     from ...main import MainSettings, MainWindow
 
 
 __all__ = [
@@ -24,32 +24,28 @@
 class MainToolbar(AbstractToolbar):
     _no_visibility_choice = True
     storable_attrs = ('outputs', )
 
     __slots__ = (
         *storable_attrs,
         'outputs_combobox', 'frame_control', 'copy_frame_button',
-        'time_control', 'copy_timestamp_button', 'zoom_combobox',
+        'time_control', 'copy_timestamp_button',
         'switch_timeline_mode_button', 'settings_button'
     )
 
     outputs: VideoOutputs | None
-    zoom_combobox: ComboBox[float]
 
     settings: MainSettings
 
     def __init__(self, main_window: MainWindow) -> None:
         super().__init__(main_window, main_window.settings)
         self.setup_ui()
 
         self.outputs = None
 
-        self.zoom_combobox.setModel(GeneralModel[float](self.settings.zoom_levels))
-        self.zoom_combobox.setCurrentIndex(self.settings.zoom_default_index)
-
         self.add_shortcuts()
 
         self.set_qobject_names()
 
     def setup_ui(self) -> None:
         super().setup_ui()
 
@@ -74,32 +70,27 @@
 
         self.copy_timestamp_button = PushButton('⎘', self, clicked=self.on_copy_timestamp_button_clicked)
 
         self.sync_outputs_checkbox = CheckBox(
             'Sync Outputs', self, checked=self.settings.SYNC_OUTPUTS, clicked=self.on_sync_outputs_clicked
         )
 
-        self.auto_fit_button = CheckBox('Auto-fit', self, clicked=self.auto_fit_button_clicked)
-
-        self.zoom_combobox = ComboBox[float](self, minimumContentsLength=4)
-        self.zoom_combobox.currentTextChanged.connect(self.on_zoom_changed)
-
         self.switch_timeline_mode_button = PushButton(
             'Switch Timeline Mode', self, clicked=self.on_switch_timeline_mode_clicked
         )
 
         self.settings_button = PushButton('Settings', self, clicked=self.main.app_settings.show)
 
         self.hlayout.addWidgets([
             self.outputs_combobox,
             self.frame_control, self.copy_frame_button,
             self.time_control, self.copy_timestamp_button,
             self.sync_outputs_checkbox,
             self.get_separator(),
-            self.auto_fit_button, self.zoom_combobox,
+            self.main.graphics_view.controls,
             self.switch_timeline_mode_button,
             self.settings_button
         ])
 
         self.hlayout.addStretch()
 
     def add_shortcuts(self) -> None:
@@ -133,36 +124,29 @@
                 force_frame = self.main.current_output.last_showed_frame
 
             for output in self.outputs:
                 output.last_showed_frame = output.to_frame(
                     self.main.current_output.to_time(force_frame)
                 )
 
-    def auto_fit_button_clicked(self, checked: bool) -> None:
-        self.zoom_combobox.setEnabled(not checked)
-        self.main.graphics_view.autofit = checked
-        if checked:
-            self.main.graphics_view.setZoom(None)
-        else:
-            self.main.graphics_view.setZoom(self.zoom_combobox.currentData())
-
     def on_current_frame_changed(self, frame: Frame) -> None:
         qt_silent_call(self.frame_control.setValue, frame)
         qt_silent_call(self.time_control.setValue, Time(frame))
 
         if self.outputs and len(self.outputs) > 1 and self.sync_outputs_checkbox.isChecked():
             self.on_sync_outputs_clicked(True, force_frame=frame)
 
     def on_current_output_changed(self, index: int, prev_index: int) -> None:
         qt_silent_call(self.outputs_combobox.setCurrentIndex, index)
         qt_silent_call(self.frame_control.setMaximum, self.main.current_output.total_frames - 1)
         qt_silent_call(self.time_control.setMaximum, self.main.current_output.total_time - Frame(1))
 
-        if self.main.graphics_view.autofit:
-            self.main.graphics_view.setZoom(None)
+        for graphics_view in self.main.graphics_views:
+            if graphics_view.autofit:
+                graphics_view.setZoom(None)
 
     def rescan_outputs(self, outputs: VideoOutputs | None = None) -> None:
         self.outputs = outputs if isinstance(outputs, VideoOutputs) else VideoOutputs(self.main)
         self.main.init_outputs()
         self.outputs_combobox.setModel(self.outputs)
 
     def on_copy_frame_button_clicked(self, checked: bool | None = None) -> None:
@@ -175,17 +159,14 @@
 
     def on_switch_timeline_mode_clicked(self, checked: bool | None = None) -> None:
         if self.main.timeline.mode == self.main.timeline.Mode.TIME:
             self.main.timeline.mode = self.main.timeline.Mode.FRAME
         elif self.main.timeline.mode == self.main.timeline.Mode.FRAME:
             self.main.timeline.mode = self.main.timeline.Mode.TIME
 
-    def on_zoom_changed(self, text: str | None = None) -> None:
-        self.main.graphics_view.setZoom(self.zoom_combobox.currentData())
-
     def __getstate__(self) -> Mapping[str, Any]:
         return super().__getstate__() | {
             'current_output_index': self.outputs_combobox.currentIndex(),
             'sync_outputs': self.sync_outputs_checkbox.isChecked()
         }
 
     def __setstate__(self, state: Mapping[str, Any]) -> None:
```

### Comparing `vspreview-0.5.0/vspreview/toolbars/misc/toolbar.py` & `vspreview-0.6.0/vspreview/toolbars/misc/toolbar.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING, Any, Mapping
 
 from PyQt6.QtCore import QKeyCombination, Qt
 from PyQt6.QtWidgets import QComboBox, QFileDialog, QLabel, QSpacerItem
 
 from ...core import (
     AbstractToolbar, CheckBox, CroppingInfo, HBoxLayout, LineEdit, PushButton, SpinBox, Stretch, Time, VBoxLayout,
-    ViewMode, try_load
+    try_load
 )
 from ...core.custom import ComboBox, Switch
 from ...models import GeneralModel
 from ...utils import qt_silent_call
 from .settings import MiscSettings
 
 if TYPE_CHECKING:
@@ -29,16 +29,15 @@
     __slots__ = (
         'reload_script_button',
         'save_storage_button', 'autosave_checkbox',
         'save_template_lineedit', 'save_frame_as_button',
         'toggle_button', 'save_file_types', 'copy_frame_button',
         'crop_top_spinbox', 'crop_left_spinbox', 'crop_width_spinbox',
         'crop_bottom_spinbox', 'crop_right_spinbox', 'crop_height_spinbox',
-        'crop_active_switch', 'crop_mode_combox', 'crop_copycommand_button',
-        'view_mode_layout', 'view_mode_combox'
+        'crop_active_switch', 'crop_mode_combox', 'crop_copycommand_button'
     )
 
     settings: MiscSettings
 
     def __init__(self, main: MainWindow) -> None:
         super().__init__(main, MiscSettings(self))
 
@@ -91,28 +90,14 @@
                 self.reload_script_button, self.get_separator(),
                 self.save_storage_button, self.get_separator(),
                 self.copy_frame_button, Stretch()
             ]),
             HBoxLayout([self.save_frame_as_button, self.save_template_lineedit, Stretch()])
         ])
 
-        self.view_mode_combox = ComboBox[str](
-            self, model=GeneralModel[str]([str(x.value) for x in ViewMode], False),
-            currentIndex=0, sizeAdjustPolicy=QComboBox.SizeAdjustPolicy.AdjustToContents
-        )
-        self.view_mode_combox.currentTextChanged.connect(
-            lambda mode: self.main.change_video_viewmode(ViewMode(mode))
-        )
-
-        self.view_mode_layout = VBoxLayout(self.hlayout, [
-            HBoxLayout([QLabel('View mode:'), self.view_mode_combox]),
-        ])
-
-        self.view_mode_layout.setAlignment(Qt.AlignmentFlag.AlignTop)
-
         self.hlayout.addStretch()
         self.hlayout.addStretch()
 
         self.crop_active_switch = Switch(10, 22, checked=True, clicked=self.crop_active_onchange)
 
         self.crop_top_spinbox = SpinBox(None, 0, 2 ** 16, valueChanged=self.crop_top_onchange)
         self.crop_left_spinbox = SpinBox(None, 0, 2 ** 16, valueChanged=self.crop_left_onchange)
@@ -161,25 +146,17 @@
         )
         self.main.add_shortcut(
             QKeyCombination(Qt.Modifier.CTRL, Qt.Key.Key_S).toCombined(), self.copy_frame_button.click
         )
         self.main.add_shortcut(
             QKeyCombination(Qt.Modifier.SHIFT, Qt.Key.Key_S).toCombined(), self.save_frame_as_button.click
         )
-        self.main.add_shortcut(
-            QKeyCombination(Qt.Modifier.SHIFT, Qt.Key.Key_F).toCombined(),
-            lambda: self.view_mode_combox.setCurrentText(
-                ViewMode.FFTSPECTRUM if self.main.current_viewmode != ViewMode.FFTSPECTRUM else ViewMode.NORMAL
-            )
-        )
 
     def copy_frame_to_clipboard(self) -> None:
-        self.main.clipboard.setPixmap(
-            self.main.current_output.graphics_scene_item.pixmap()
-        )
+        self.main.clipboard.setPixmap(self.main.current_scene.pixmap())
         self.main.show_message('Current frame successfully copied to clipboard')
 
     def on_autosave_interval_changed(self, new_value: Time | None) -> None:
         if new_value is None:
             return
         if new_value == Time(seconds=0):
             self.main.autosave_timer.stop()
@@ -235,17 +212,15 @@
             self.main.toolbars.debug.toggle_button.setVisible(True)
         elif state == Qt.CheckState.Unchecked:
             if self.main.toolbars.debug.toggle_button.isChecked():
                 self.main.toolbars.debug.toggle_button.click()
             self.main.toolbars.debug.toggle_button.setVisible(False)
 
     def save_as_png(self, path: Path) -> None:
-        self.main.current_output.graphics_scene_item.pixmap().save(
-            str(path), 'PNG', self.main.settings.png_compression_level
-        )
+        self.main.current_scene.pixmap().save(str(path), 'PNG', self.main.settings.png_compression_level)
 
     def on_current_output_changed(self, index: int, prev_index: int) -> None:
         if index != prev_index:
             self.update_crop(prev_index)
 
         curr = self.main.current_output
         crop = curr.crop_values
@@ -275,15 +250,15 @@
 
         output = self.main.current_output if index is None else self.main.outputs[index]
 
         output.update_graphic_item(None, CroppingInfo(
             self.crop_top_spinbox.value(), self.crop_left_spinbox.value(),
             self.crop_width_spinbox.value(), self.crop_height_spinbox.value(),
             self.crop_active_switch.isChecked(), bool(self.crop_mode_combox.currentIndex())
-        ))
+        ), graphics_scene_item=self.main.current_output.graphics_scene_item)
 
     def crop_active_onchange(self, checked: bool) -> None:
         is_absolute = not not self.crop_mode_combox.currentIndex()
 
         self.crop_top_spinbox.setEnabled(checked)
         self.crop_left_spinbox.setEnabled(checked)
```

### Comparing `vspreview-0.5.0/vspreview/toolbars/pipette/colorview.py` & `vspreview-0.6.0/vspreview/toolbars/pipette/colorview.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/toolbars/pipette/toolbar.py` & `vspreview-0.6.0/vspreview/toolbars/pipette/toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,19 +193,19 @@
         return cache[1]
 
     def update_labels(self, local_pos: QPoint) -> None:
         self.last_pos = (self.main.current_output, local_pos)
 
         pos_f = self.main.graphics_view.mapToScene(local_pos)
 
-        if not self.main.current_output.graphics_scene_item.contains(pos_f):
+        if not self.main.current_scene.contains(pos_f):
             return
 
         pos = QPoint(floor(pos_f.x()), floor(pos_f.y()))
-        color = self.main.current_output.graphics_scene_item.pixmap().toImage().pixelColor(pos)
+        color = self.main.current_scene.pixmap().toImage().pixelColor(pos)
         components = color.red(), color.green(), color.blue()
         components_float = tuple[float, ...](x / 255 for x in components)
 
         self.color_view.color = color
         self.position.setText('{:4d},{:4d}'.format(pos.x(), pos.y()))
 
         self.rgb_hex.setText('{:2X},{:2X},{:2X}'.format(*components))
```

### Comparing `vspreview-0.5.0/vspreview/toolbars/playback/settings.py` & `vspreview-0.6.0/vspreview/toolbars/playback/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/toolbars/playback/toolbar.py` & `vspreview-0.6.0/vspreview/toolbars/playback/toolbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,16 +199,15 @@
 
     def rescan_outputs(self, outputs: AudioOutputs | None = None) -> None:
         self.audio_outputs = outputs or AudioOutputs(self.main)
         self.audio_outputs_combobox.setModel(self.audio_outputs)
 
     def get_true_fps(self, n: int | Frame, frameprops: vs.FrameProps, force: bool = False) -> Fraction:
         if (
-            hasattr(self.main.current_output, 'got_timecodes')
-            and self.main.current_output.got_timecodes and not force
+            hasattr(self.main.current_output, 'got_timecodes') and self.main.current_output.got_timecodes and not force
         ):
             return Fraction(self.main.current_output.timecodes[int(n)])
 
         if any({x not in frameprops for x in {'_DurationDen', '_DurationNum'}}):
             raise RuntimeError(
                 'Playback: DurationDen and DurationNum frame props are needed for VFR clips!'
             )
@@ -231,17 +230,16 @@
 
     @property
     def got_debug_fps(self) -> bool:
         return hasattr(self.main.toolbars, 'debug') and self.main.toolbars.debug.settings.DEBUG_PLAY_FPS
 
     def play(self, stop_at_frame: int | Frame | None = None) -> None:
         if (
-            (self.main.current_output.last_showed_frame > self.main.current_output.total_frames)
-            or not video.PACKING_TYPE.can_playback
-        ):
+            self.main.current_output.last_showed_frame > self.main.current_output.total_frames
+        ) or not video.PACKING_TYPE.can_playback:
             return
 
         if self.main.statusbar.label.text() == 'Ready':
             self.main.statusbar.label.setText('Playing')
 
         if self.main.current_output.prepared.alpha is None:
             self.allocate_buffer(False)
@@ -478,19 +476,16 @@
         if checked:
             self.play()
         else:
             self.stop()
 
     def on_timeline_clicked(self, frame: Frame, time: Time) -> None:
         if (
-            not self.play_timer.isActive()
-            or not self.play_timer_audio.isActive()
-            or self.current_audio_output is None
-            or self.current_audio_output.vs_output is None
-        ):
+            not self.play_timer.isActive() or not self.play_timer_audio.isActive() or self.current_audio_output is None
+        ) or self.current_audio_output.vs_output is None:
             return
 
         self.current_audio_output.iodevice.reset()
         self.current_audio_frame = self.current_audio_output.to_frame(time)
 
         for future in self.play_buffer_audio:
             future.add_done_callback(lambda future: future.result())
```

### Comparing `vspreview-0.5.0/vspreview/toolbars/scening/dialog.py` & `vspreview-0.6.0/vspreview/toolbars/scening/dialog.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/toolbars/scening/settings.py` & `vspreview-0.6.0/vspreview/toolbars/scening/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/toolbars/scening/toolbar.py` & `vspreview-0.6.0/vspreview/toolbars/scening/toolbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,18 +237,14 @@
 
         return marks
 
     @property
     def current_list(self) -> SceningList | None:
         return self.items_combobox.currentValue()
 
-    @current_list.setter
-    def current_list(self, item: SceningList) -> None:
-        self.items_combobox.setCurrentValue(item)
-
     @property
     def current_list_index(self) -> int:
         return self.items_combobox.currentIndex()
 
     @current_list_index.setter
     def current_list_index(self, index: int) -> None:
         if (0 <= index < len(self.lists)):
```

### Comparing `vspreview-0.5.0/vspreview/utils/debug.py` & `vspreview-0.6.0/vspreview/utils/debug.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview/utils/utils.py` & `vspreview-0.6.0/vspreview/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.5.0/vspreview.egg-info/PKG-INFO` & `vspreview-0.6.0/vspreview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vspreview
-Version: 0.5.0
+Version: 0.6.0
 Summary: Previewer for VapourSynth scripts
 Author: Endilll
 Author-email: 
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-preview
 Project-URL: Documentation, https://vspreview.encode.moe/en/latest/
```

### Comparing `vspreview-0.5.0/vspreview.egg-info/SOURCES.txt` & `vspreview-0.6.0/vspreview.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 vspreview/models/__init__.py
 vspreview/models/generalmodel.py
 vspreview/models/outputs.py
 vspreview/models/scening.py
 vspreview/plugins/__init__.py
 vspreview/plugins/abstract.py
 vspreview/plugins/frame_props.ppy
+vspreview/plugins/install.py
+vspreview/plugins/split_view.ppy
+vspreview/plugins/utils.py
 vspreview/toolbars/__init__.py
 vspreview/toolbars/benchmark/__init__.py
 vspreview/toolbars/benchmark/settings.py
 vspreview/toolbars/benchmark/toolbar.py
 vspreview/toolbars/comp/__init__.py
 vspreview/toolbars/comp/settings.py
 vspreview/toolbars/comp/toolbar.py
```

