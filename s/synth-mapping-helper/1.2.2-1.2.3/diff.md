# Comparing `tmp/synth_mapping_helper-1.2.2.tar.gz` & `tmp/synth_mapping_helper-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synth_mapping_helper-1.2.2.tar", last modified: Tue May 23 20:11:02 2023, max compression
+gzip compressed data, was "synth_mapping_helper-1.2.3.tar", last modified: Sun Jun 11 15:46:05 2023, max compression
```

## Comparing `synth_mapping_helper-1.2.2.tar` & `synth_mapping_helper-1.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:11:02.772779 synth_mapping_helper-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-23 20:11:02.772779 synth_mapping_helper-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-23 20:11:02.772779 synth_mapping_helper-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:11:02.768779 synth_mapping_helper-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:11:02.768779 synth_mapping_helper-1.2.2/src/synth_mapping_helper/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27126 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28072 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/companion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/finalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/movement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/pattern_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/rails.py
--rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/synth_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:11:02.768779 synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-23 20:11:02.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-23 20:11:02.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:11:02.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-23 20:11:02.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 20:11:02.000000 synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:11:02.772779 synth_mapping_helper-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-23 20:10:50.000000 synth_mapping_helper-1.2.2/tests/test_synth_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:46:05.556155 synth_mapping_helper-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-11 15:46:05.556155 synth_mapping_helper-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-11 15:46:05.556155 synth_mapping_helper-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:46:05.552155 synth_mapping_helper-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:46:05.552155 synth_mapping_helper-1.2.3/src/synth_mapping_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28834 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28072 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/companion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/movement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/pattern_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/rails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/synth_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:46:05.552155 synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-11 15:46:05.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-11 15:46:05.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 15:46:05.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-11 15:46:05.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-11 15:46:05.000000 synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:46:05.556155 synth_mapping_helper-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-11 15:45:55.000000 synth_mapping_helper-1.2.3/tests/test_synth_format.py
```

### Comparing `synth_mapping_helper-1.2.2/LICENSE` & `synth_mapping_helper-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.2/PKG-INFO` & `synth_mapping_helper-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth_mapping_helper
-Version: 1.2.2
+Version: 1.2.3
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
```

### Comparing `synth_mapping_helper-1.2.2/README.md` & `synth_mapping_helper-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.2/setup.py` & `synth_mapping_helper-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.2/src/synth_mapping_helper/cli.py` & `synth_mapping_helper-1.2.3/src/synth_mapping_helper/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,28 +30,54 @@
     if options.wall_rotate is not None:
         data.apply_for_walls(movement.rotate_relative, options.wall_rotate, mirror_left=options.mirror_left, types=filter_types)
     if options.offset is not None:
         _movement_helper(data, options.mirror_left, movement.offset, movement.offset_relative, movement.offset, options.relative, options.pivot, options.offset, types=filter_types)
     if options.outset is not None:
         _movement_helper(data, options.mirror_left, movement.outset, movement.outset_relative, movement.outset_from, options.relative, options.pivot, options.outset, types=filter_types)
 
+def do_random_movement(options, data: synth_format.DataContainer, filter_types: list = synth_format.ALL_TYPES) -> None:
+    if options.rotate_random is not None:
+        if len(options.rotate_random) == 1:
+            area = options.rotate_random[0]
+        else:
+            areas = np.array([
+                max(a[1]-a[1], 0.01)  # area, where 0-width areas are counted as 0.01 for numerical stability
+                for a in options.rotate_random
+            ])
+            area = options.rotate_random[np.random.choice(len(areas), p=areas/sum(areas))]
+        random_angle = np.random.random_sample() * (area[1]-area[0]) + area[0]
+        _movement_helper(data, options.mirror_left, movement.rotate, movement.rotate_relative, movement.rotate_around, options.relative, options.pivot, random_angle, types=filter_types)
+
+    if options.offset_random is not None:
+        if len(options.offset_random) == 1:
+            area = options.offset_random[0]
+        else:
+            areas = np.array([
+                max(a[1,0]-a[0,0], 0.01)*max(a[1,1]-a[0,1], 0.01)  # area, where 0-width axes are counted as 0.01 for numerical stability
+                for a in options.offset_random
+            ])
+            area = options.offset_random[np.random.choice(len(areas), p=areas/sum(areas))]
+        random_offset = pattern_generation.random_xy(1, area[0], area[1])[0]
+        data.apply_for_all(movement.offset, [random_offset[0], random_offset[1], 0], mirror_left=options.mirror_left, types=filter_types)
+    
 def get_parser():
     parser = ArgumentParser(
         formatter_class=RawDescriptionHelpFormatter,
         prog=f"python3 -m {__package__}.{Path(__file__).stem}",
         description='\n'.join([
             f"Note types:\n\t{', '.join(synth_format.NOTE_TYPES)}",
             f"Wall types:\n\t{', '.join(synth_format.WALL_TYPES)}",
             "",
             "Most number values accept decimals, percentages and fractions (ie '0.25', '25%' or '1/4')",
             "\tTime inputs may also be given in seconds (ie '81.5s' or '1:21.5'), which will be converted into beats",
             "If your value starts with a '-', you must add a = between option and value, ie '--rotate=-45' or '--offset=-1,0,0'",
+            "For most options, only the last occurence is considered (exception: '--offset-random' and '--rotate-random')",
             "",
             "Angles are in degrees",
-            "Vectors are specified as 'x,y,time:'",
+            "Vectors are specified as 'x,y,time':",
             "\tX/Y is measured in editor grid squares, where +x is right and +y is up",
             "\tTime is measured in measures/beats from the start of the selection",
             "",
             "Also see the wiki on GitHub, which contains more detailed explainations, as well as some examples and images: https://github.com/adosikas/synth_mapping_helper/wiki",
         ]),
         epilog=f"Version: {__version__}",
     )
@@ -94,15 +120,16 @@
     movement_group.add_argument("-r", "--rotate", type=utils.parse_number, metavar="DEGREES", help="Rotate everything counterclockwise by this many degrees (negative for clockwise)")
     movement_group.add_argument("--wall-rotate", type=utils.parse_number, metavar="DEGREES", help="Rotate walls counterclockwise around themselves by this many degrees (negative for clockwise)")
     movement_group.add_argument("-o", "--offset", type=utils.parse_position, help="Move/Translate by x,y,t")
     movement_group.add_argument("--outset", type=utils.parse_number, metavar="DISTANCE", help="Move outwards (negative for inwards, can move 'across' pivot)")
     rail_stack_group = movement_group.add_mutually_exclusive_group()
     rail_stack_group.add_argument("--offset-along", choices=synth_format.NOTE_TYPES, help="While stacking: Offset objects to follow notes/rails of the specified type")
     rail_stack_group.add_argument("--rotate-with", choices=synth_format.NOTE_TYPES, help="While stacking: Rotate and outset the objects to follow notes/rails of the specified type")
-    movement_group.add_argument("--offset-random", type=utils.parse_xy_range, metavar="[MIN_X:]MAX_X,[MIN_Y:]MAX_Y", help="Offset by a random amount in the X and Y axis. When no MIN is given, uses negative MAX.")
+    movement_group.add_argument("--offset-random", nargs="+", action="extend", type=utils.parse_xy_range, metavar="[MIN_X:]MAX_X,[MIN_Y:]MAX_Y", help="Offset by a random amount in the X and Y axis (ignoring relative & pivot). When no MIN is given, uses negative MAX. Multiple ranges can be specified, separated via space or as separate options (required when starting with '-').")
+    movement_group.add_argument("--rotate-random", nargs="+", action="extend", type=utils.parse_range, metavar="[MIN_ANG:]MAX_ANG", help="Rotate by a random angle (obeying relative & pivot if given). When no MIN is given, uses negative MAX. Multiple ranges can be specified, separated via space or as separate options (required when starting with '-').")
 
     movement_group.add_argument("-c", "--stack-count", type=int, help="Instead of moving, create copies. Must have time offset set.")
     movement_group.add_argument("--stack-duration", type=utils.parse_time, help="Like --stack-count, but you can give it during in beats ('4') or seconds ('2s').")
     movement_group.add_argument("--autostack", nargs="?", choices=("OFFSET", "SPIRAL", "OUTSET", "SCALE"), action="append", metavar="OFFSET/SPIRAL/OUTSET/SCALE", help="Find the first pair of matching objects and continue the pattern. For continuing the positions, the following modes are supported: OFFSET (default, absolute xy), SPIRAL (rotate around implied pivot), OUTSET (distance from pivot) and SCALE (xy ratio).")
 
     postproc_group = parser.add_argument_group("post-processing")
     postproc_group.add_argument("--parallels", type=utils.parse_number, metavar="DISTANCE", help="Create parallel left/right handed patterns with given spacing from input. Negative numbers result in crossovers.")
@@ -321,15 +348,15 @@
             nodes[1::3] -= options.spike_width/2
             nodes[:, :2] += pattern_generation.spikes(options.spikes * direction, count, options.start_angle if direction == 1 else 180 - options.start_angle) * options.radius
             return nodes
         data.apply_for_notes(_add_spikes, types=filter_types, mirror_left=options.mirror_left)
 
     # movement
     if options.stack_count:
-        stacking = data.filtered(types=filter_types)
+        stacking = data.filtered(types=filter_types)  # pre-filter
         if options.offset_along or options.rotate_with:
             if options.offset_along and options.rotate_with:
                 abort("Cannot use offset-along and rotate-with at the same time")
             if options.relative:
                 abort("Cannot use offset-along or rotate-with in relative mode")
             start_pos = rails.get_position_at(getattr(data, options.offset_along or options.rotate_with), 0)
             if start_pos is None:
@@ -356,25 +383,21 @@
                 # outset all objects together by precalculating the offset based on rail position
                 group_outset = [cur_pos[0], cur_pos[1], 0] / np.sqrt(cur_pos.dot(cur_pos)) * distance_diff
                 if options.pivot is not None:
                     tmp.apply_for_all(movement.rotate_around, angle_diff, pivot_3d=options.pivot, mirror_left=options.mirror_left)
                 else:
                     tmp.apply_for_all(movement.rotate, angle_diff, mirror_left=options.mirror_left)
                 tmp.apply_for_all(movement.offset, group_outset)
-            if options.offset_random is not None:
-                random_offset = pattern_generation.random_xy(1, options.offset_random[0], options.offset_random[1])[0]
-                tmp.apply_for_all(movement.offset, [random_offset[0], random_offset[1], 0], mirror_left=options.mirror_left)
+            do_random_movement(options, tmp)
             data.merge(tmp)
     else:
         if options.offset_along or options.rotate_with:
             abort("Cannot use offset-along or rotate-with without stacking")
         do_movement(options, data, filter_types=filter_types)
-        if options.offset_random is not None:
-            random_offset = pattern_generation.random_xy(1, options.offset_random[0], options.offset_random[1])[0]
-            data.apply_for_all(movement.offset, [random_offset[0], random_offset[1], 0], mirror_left=options.mirror_left)
+        do_random_movement(options, data, filter_types=filter_types)
 
     # postprocessing
     if options.parallels:
         left_orig, right_orig = data.left, data.right  # create a backup of the input
         data.left = (
             left_orig
             | {t: nodes - [options.parallels,0,0] for t, nodes in sorted(right_orig.items())}  # shift over right hand by <distance>
```

### Comparing `synth_mapping_helper-1.2.2/src/synth_mapping_helper/companion.py` & `synth_mapping_helper-1.2.3/src/synth_mapping_helper/companion.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.2/src/synth_mapping_helper/finalize.py` & `synth_mapping_helper-1.2.3/src/synth_mapping_helper/finalize.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.2/src/synth_mapping_helper/movement.py` & `synth_mapping_helper-1.2.3/src/synth_mapping_helper/movement.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.2/src/synth_mapping_helper/pattern_generation.py` & `synth_mapping_helper-1.2.3/src/synth_mapping_helper/pattern_generation.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.2/src/synth_mapping_helper/rails.py` & `synth_mapping_helper-1.2.3/src/synth_mapping_helper/rails.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.2/src/synth_mapping_helper/synth_format.py` & `synth_mapping_helper-1.2.3/src/synth_mapping_helper/synth_format.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.2/src/synth_mapping_helper/utils.py` & `synth_mapping_helper-1.2.3/src/synth_mapping_helper/utils.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/PKG-INFO` & `synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth-mapping-helper
-Version: 1.2.2
+Version: 1.2.3
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
```

### Comparing `synth_mapping_helper-1.2.2/src/synth_mapping_helper.egg-info/SOURCES.txt` & `synth_mapping_helper-1.2.3/src/synth_mapping_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

