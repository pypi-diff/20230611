# Comparing `tmp/eqalert-3.5.3.tar.gz` & `tmp/eqalert-3.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eqalert-3.5.3.tar", last modified: Sat Jun 10 14:52:32 2023, max compression
+gzip compressed data, was "eqalert-3.5.4.tar", last modified: Sun Jun 11 19:18:44 2023, max compression
```

## Comparing `eqalert-3.5.3.tar` & `eqalert-3.5.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:32.728043 eqalert-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-10 14:52:32.728043 eqalert-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-10 14:52:18.000000 eqalert-3.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:32.720043 eqalert-3.5.3/eqa/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    62129 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/eqalert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:32.724043 eqalert-3.5.3/eqa/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   123206 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/action.py
--rw-r--r--   0 runner    (1001) docker     (123)   580055 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    82278 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    85313 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/encounter.py
--rw-r--r--   0 runner    (1001) docker     (123)    31830 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/log.py
--rw-r--r--   0 runner    (1001) docker     (123)   488202 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17200 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/lib/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:32.724043 eqalert-3.5.3/eqa/sound/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/sound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/sound/tick.wav
--rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-10 14:52:18.000000 eqalert-3.5.3/eqa/sound/tock.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:52:32.728043 eqalert-3.5.3/eqalert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-10 14:52:32.000000 eqalert-3.5.3/eqalert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-10 14:52:32.000000 eqalert-3.5.3/eqalert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:52:32.000000 eqalert-3.5.3/eqalert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-10 14:52:32.000000 eqalert-3.5.3/eqalert.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-10 14:52:32.000000 eqalert-3.5.3/eqalert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-10 14:52:32.000000 eqalert-3.5.3/eqalert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-10 14:52:32.728043 eqalert-3.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-10 14:52:18.000000 eqalert-3.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:44.736483 eqalert-3.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-11 19:18:44.736483 eqalert-3.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-11 19:18:29.000000 eqalert-3.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:44.732483 eqalert-3.5.4/eqa/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60671 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/eqalert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:44.732483 eqalert-3.5.4/eqa/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125764 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)   580215 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82457 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85313 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/encounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31830 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)   488202 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:44.736483 eqalert-3.5.4/eqa/sound/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/sound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/sound/tick.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/sound/tock.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:44.736483 eqalert-3.5.4/eqalert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-11 19:18:44.000000 eqalert-3.5.4/eqalert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-11 19:18:44.000000 eqalert-3.5.4/eqalert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:18:44.000000 eqalert-3.5.4/eqalert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-11 19:18:44.000000 eqalert-3.5.4/eqalert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-11 19:18:44.000000 eqalert-3.5.4/eqalert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-11 19:18:44.000000 eqalert-3.5.4/eqalert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-11 19:18:44.736483 eqalert-3.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-11 19:18:29.000000 eqalert-3.5.4/setup.py
```

### Comparing `eqalert-3.5.3/PKG-INFO` & `eqalert-3.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eqalert
-Version: 3.5.3
+Version: 3.5.4
 Summary: Configurable and Context Driven Project 1999 Log Parser
 Home-page: https://github.com/mgeitz/eqalert
 Author: M Geitz
 Author-email: git@geitz.xyz
 License: GPL2
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
```

### Comparing `eqalert-3.5.3/README.md` & `eqalert-3.5.4/README.md`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.3/eqa/eqalert.py` & `eqalert-3.5.4/eqa/eqalert.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,38 +335,20 @@
         )
         process_encounter.daemon = True
         process_encounter.start()
 
         # Create Sounds, at most 3 sounds at once (sound blocking enabled)
         ## Consume sound_q
         ## Produce sounds
-
-        ### Thread 1
-        process_sound_1 = threading.Thread(
-            target=eqa_sound.process,
-            args=(configs, sound_q, exit_flag, cfg_reload, state),
-        )
-        process_sound_1.daemon = True
-        process_sound_1.start()
-
-        ### Thread 2
-        process_sound_2 = threading.Thread(
-            target=eqa_sound.process,
-            args=(configs, sound_q, exit_flag, cfg_reload, state),
-        )
-        process_sound_2.daemon = True
-        process_sound_2.start()
-
-        ### Thread 3
-        process_sound_3 = threading.Thread(
+        process_sound = threading.Thread(
             target=eqa_sound.process,
             args=(configs, sound_q, exit_flag, cfg_reload, state),
         )
-        process_sound_3.daemon = True
-        process_sound_3.start()
+        process_sound.daemon = True
+        process_sound.start()
 
         # Draw the TUI
         ## Consume display_q
         ## Produce pretty pictures
         process_display = threading.Thread(
             target=eqa_curses.display,
             args=(screen, display_q, state, configs, exit_flag, cfg_reload, version),
@@ -737,17 +719,15 @@
                             new_state.spell_timer_yours_only
                         )
                         state.set_consider_eval(new_state.consider_eval)
                         #### Stop state dependent processes
                         cfg_reload.set()
                         process_action.join()
                         process_encounter.join()
-                        process_sound_1.join()
-                        process_sound_2.join()
-                        process_sound_3.join()
+                        process_sound.join()
                         process_timer.join()
                         process_watch.join()
                         process_keys.join()
                         process_display.join()
                         cfg_reload.clear()
 
                         # Restart the TUI
@@ -821,38 +801,20 @@
                                 version,
                             ),
                         )
                         process_encounter.daemon = True
                         process_encounter.start()
 
                         #### Restart process_sound
-
-                        ##### Thread 1
-                        process_sound_1 = threading.Thread(
-                            target=eqa_sound.process,
-                            args=(configs, sound_q, exit_flag, cfg_reload, state),
-                        )
-                        process_sound_1.daemon = True
-                        process_sound_1.start()
-
-                        ##### Thread 2
-                        process_sound_2 = threading.Thread(
-                            target=eqa_sound.process,
-                            args=(configs, sound_q, exit_flag, cfg_reload, state),
-                        )
-                        process_sound_2.daemon = True
-                        process_sound_2.start()
-
-                        ##### Thread 3
-                        process_sound_3 = threading.Thread(
+                        process_sound = threading.Thread(
                             target=eqa_sound.process,
                             args=(configs, sound_q, exit_flag, cfg_reload, state),
                         )
-                        process_sound_3.daemon = True
-                        process_sound_3.start()
+                        process_sound.daemon = True
+                        process_sound.start()
 
                         #### Restart process_timer
                         process_timer = threading.Thread(
                             target=eqa_timer.process,
                             args=(
                                 configs,
                                 state,
@@ -915,17 +877,15 @@
     process_watch.join()
     process_log.join()
     process_parse.join()
     process_keys.join()
     process_action.join()
     process_encounter.join()
     process_timer.join()
-    process_sound_1.join()
-    process_sound_2.join()
-    process_sound_3.join()
+    process_sound.join()
     process_display.join()
 
     ## Close curses
     eqa_curses.close_screens(screen)
 
 
 def system_raid(configs, state, display_q, sound_q, new_message):
```

### Comparing `eqalert-3.5.3/eqa/lib/action.py` & `eqalert-3.5.4/eqa/lib/action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1007,15 +1007,15 @@
 
                         # Check if active player could have clicked this spell
                         elif spell_casters["spells"][spell_casting_buffer_you["spell"]][
                             "item"
                         ]:
                             for item in spell_items["spells"][
                                 spell_casting_buffer_you["spell"]
-                            ]:
+                            ].keys():
                                 cast_duration = spell_items["spells"][
                                     spell_casting_buffer_you["spell"]
                                 ][item]["cast"]
                                 if cast_duration > 0:
                                     identified = action_spell_timer_player_click_check(
                                         line_time,
                                         spell_casting_buffer_you["time"],
@@ -1034,107 +1034,85 @@
                                         identified_spell_target = target
 
                 # Check if another player could have cast this
                 if identified_spell_level is None:
                     # For each possible spell
                     for check_spell in possible_spells:
                         # Check each recent cast event
-                        for recent_cast_event in spell_casting_buffer_other:
-                            caster_name = recent_cast_event["caster"]
-                            cast_duration = spell_timers["spells"][check_spell][
-                                "cast_time"
-                            ]
-                            # If we know the class/level of the caster
-                            if caster_name in player_list.keys():
-                                caster_class = player_list[caster_name]["class"]
-                                caster_level = player_list[caster_name]["level"]
-                                if caster_class is not None and caster_level > 0:
-                                    # Check if another player could cast this possible spell
-                                    identified = action_spell_timer_player_cast_check(
-                                        line_time,
-                                        recent_cast_event["time"],
-                                        cast_duration,
-                                        caster_name,
-                                        caster_level,
-                                        caster_class,
-                                        check_spell,
-                                        spell_casters,
-                                    )
-                                    if identified is not None:
-                                        if identified_spell_level is not None:
-                                            if (
-                                                spell_casters["spells"][
-                                                    identified_spell
-                                                ]["classes"][
-                                                    player_list[
-                                                        identified_spell_caster
-                                                    ]["class"]
-                                                ]
-                                                < spell_casters["spells"][
-                                                    identified[2]
-                                                ]["classes"][
-                                                    player_list[identified[0]]["class"]
-                                                ]
-                                            ):
+                        if check_spell in spell_casters["spells"].keys():
+                            for recent_cast_event in spell_casting_buffer_other:
+                                caster_name = recent_cast_event["caster"]
+                                cast_duration = spell_timers["spells"][check_spell][
+                                    "cast_time"
+                                ]
+                                # If we know the class/level of the caster
+                                if caster_name in player_list.keys():
+                                    caster_class = player_list[caster_name]["class"]
+                                    caster_level = player_list[caster_name]["level"]
+                                    if caster_class is not None and caster_level > 0:
+                                        # Check if another player could cast this possible spell
+                                        identified = (
+                                            action_spell_timer_player_cast_check(
+                                                line_time,
+                                                recent_cast_event["time"],
+                                                cast_duration,
+                                                caster_name,
+                                                caster_level,
+                                                caster_class,
+                                                check_spell,
+                                                spell_casters,
+                                            )
+                                        )
+                                        if identified is not None:
+                                            if identified_spell_level is not None:
+                                                if (
+                                                    spell_casters["spells"][
+                                                        identified_spell
+                                                    ]["classes"][
+                                                        player_list[
+                                                            identified_spell_caster
+                                                        ]["class"]
+                                                    ]
+                                                    < spell_casters["spells"][
+                                                        identified[2]
+                                                    ]["classes"][
+                                                        player_list[identified[0]][
+                                                            "class"
+                                                        ]
+                                                    ]
+                                                ):
+                                                    identified_spell_caster = (
+                                                        identified[0]
+                                                    )
+                                                    identified_spell_level = identified[
+                                                        1
+                                                    ]
+                                                    identified_spell = identified[2]
+                                                    identified_spell_target = target
+                                            else:
                                                 identified_spell_caster = identified[0]
                                                 identified_spell_level = identified[1]
                                                 identified_spell = identified[2]
                                                 identified_spell_target = target
-                                        else:
-                                            identified_spell_caster = identified[0]
-                                            identified_spell_level = identified[1]
-                                            identified_spell = identified[2]
-                                            identified_spell_target = target
-                                    # Check if another player used a clicky
-                                    elif check_spell in spell_casters["spells"].keys():
-                                        if spell_casters["spells"][check_spell]["item"]:
-                                            for item in spell_items["spells"][
-                                                check_spell
+                                        # Check if another player used a clicky
+                                        elif (
+                                            check_spell
+                                            in spell_casters["spells"].keys()
+                                        ):
+                                            if spell_casters["spells"][check_spell][
+                                                "item"
                                             ]:
-                                                cast_duration = spell_items["spells"][
-                                                    check_spell
-                                                ][item]["cast"]
-                                                # Non-zero click casts have spell casting messages
-                                                if cast_duration > 0:
-                                                    identified = action_spell_timer_player_click_check(
-                                                        line_time,
-                                                        recent_cast_event["time"],
-                                                        cast_duration,
-                                                        caster_name,
-                                                        caster_level,
-                                                        caster_class,
-                                                        check_spell,
-                                                        spell_items,
-                                                        item,
-                                                    )
-                                                    if identified is not None:
-                                                        identified_spell_caster = (
-                                                            identified[0]
-                                                        )
-                                                        identified_spell_level = (
-                                                            identified[1]
-                                                        )
-                                                        idenfitied_spell = identified[2]
-                                                        identified_spell_target = target
-                                                # Instant click cast event but self only spell
-                                                elif spell_casters["spells"][
+                                                for item in spell_items["spells"][
                                                     check_spell
-                                                ]["self"]:
-                                                    if target in player_list.keys():
-                                                        caster_name = target
-                                                        caster_level = player_list[
-                                                            target
-                                                        ]["level"]
-                                                        caster_class = player_list[
-                                                            target
-                                                        ]["class"]
-                                                    if (
-                                                        caster_class is not None
-                                                        and caster_level > 0
-                                                    ):
+                                                ].keys():
+                                                    cast_duration = spell_items[
+                                                        "spells"
+                                                    ][check_spell][item]["cast"]
+                                                    # Non-zero click casts have spell casting messages
+                                                    if cast_duration > 0:
                                                         identified = action_spell_timer_player_click_check(
                                                             line_time,
                                                             recent_cast_event["time"],
                                                             cast_duration,
                                                             caster_name,
                                                             caster_level,
                                                             caster_class,
@@ -1151,20 +1129,62 @@
                                                             )
                                                             idenfitied_spell = (
                                                                 identified[2]
                                                             )
                                                             identified_spell_target = (
                                                                 target
                                                             )
+                                                    # Instant click cast event but self only spell
+                                                    elif spell_casters["spells"][
+                                                        check_spell
+                                                    ]["self"]:
+                                                        if target in player_list.keys():
+                                                            caster_name = target
+                                                            caster_level = player_list[
+                                                                target
+                                                            ]["level"]
+                                                            caster_class = player_list[
+                                                                target
+                                                            ]["class"]
+                                                        if (
+                                                            caster_class is not None
+                                                            and caster_level > 0
+                                                        ):
+                                                            identified = action_spell_timer_player_click_check(
+                                                                line_time,
+                                                                recent_cast_event[
+                                                                    "time"
+                                                                ],
+                                                                cast_duration,
+                                                                caster_name,
+                                                                caster_level,
+                                                                caster_class,
+                                                                check_spell,
+                                                                spell_items,
+                                                                item,
+                                                            )
+                                                            if identified is not None:
+                                                                identified_spell_caster = identified[
+                                                                    0
+                                                                ]
+                                                                identified_spell_level = identified[
+                                                                    1
+                                                                ]
+                                                                idenfitied_spell = (
+                                                                    identified[2]
+                                                                )
+                                                                identified_spell_target = (
+                                                                    target
+                                                                )
 
                 # Haven't found anything yet, check if it could be an instant click (these have no casting messages)
                 if identified_spell_level is None and target == state.char.lower():
                     for check_spell in possible_spells:
                         if check_spell in spell_items["spells"].keys():
-                            for item in spell_items["spells"][check_spell]:
+                            for item in spell_items["spells"][check_spell].keys():
                                 if (
                                     spell_items["spells"][check_spell][item]["cast"]
                                     == 0
                                 ):
                                     identified = action_spell_timer_player_click_check(
                                         line_time,
                                         line_time,
@@ -1183,86 +1203,97 @@
                                         identified_spell_target = target
 
                 # Time to guess the spell level
                 if identified_spell_level is None and state.spell_timer_guess:
                     # For each possible spell
                     for check_spell in possible_spells:
                         # Check each recent cast event
-                        for recent_cast_event in spell_casting_buffer_other:
-                            # If this is a known npc spell, just set to current player level
-                            if (
-                                spell_casters["spells"][check_spell]["npc"]
-                                and state.char_level is not None
-                                and identified_spell_level is None
-                            ):
-                                identified_spell_caster = recent_cast_event["caster"]
-                                identified_spell_level = state.char_level
-                                identified_spell = check_spell
-                                identified_spell_target = target
-
-                            # If a player could cast this
-                            player_level_could_cast = False
-                            if (
-                                spell_casters["spells"][check_spell]["classes"]
-                                and identified_spell_level is None
-                                or spell_casters["spells"][check_spell]["item"]
-                            ):
-                                # Check if the current player level could cast this (assuming it is a grouped peer or target mob)
-                                for any_class in spell_casters["spells"][check_spell][
-                                    "classes"
-                                ]:
-                                    if state.char_level is not None:
-                                        if (
-                                            state.char_level
-                                            >= spell_casters["spells"][check_spell][
-                                                "classes"
-                                            ][any_class]
-                                        ):
-                                            player_level_could_cast = True
+                        if check_spell in spell_casters["spells"].keys():
+                            for recent_cast_event in spell_casting_buffer_other:
+                                # If this is a known npc spell, just set to current player level
+                                if (
+                                    spell_casters["spells"][check_spell]["npc"]
+                                    and state.char_level is not None
+                                    and identified_spell_level is None
+                                ):
+                                    identified_spell_caster = recent_cast_event[
+                                        "caster"
+                                    ]
+                                    identified_spell_level = state.char_level
+                                    identified_spell = check_spell
+                                    identified_spell_target = target
 
-                                        if (
-                                            identified_spell_level is None
-                                            and spell_casters["spells"][check_spell][
-                                                "item"
-                                            ]
-                                        ):
-                                            for item in spell_items["spells"][
-                                                check_spell
-                                            ]:
-                                                if (
-                                                    spell_items["spells"][check_spell][
-                                                        item
-                                                    ]["cast"]
-                                                    == 0
-                                                ):
-                                                    for clickable_class in spell_items[
-                                                        "spells"
-                                                    ][check_spell][item]["classes"]:
-                                                        if (
-                                                            spell_items["spells"][
-                                                                check_spell
-                                                            ][item]["classes"][
-                                                                clickable_class
-                                                            ]
-                                                            <= state.char_level
-                                                        ):
-                                                            player_level_could_cast = (
-                                                                True
-                                                            )
+                                # If a player could cast this
+                                player_level_could_cast = False
+                                if (
+                                    spell_casters["spells"][check_spell]["classes"]
+                                    and identified_spell_level is None
+                                    or spell_casters["spells"][check_spell]["item"]
+                                ):
+                                    # Check if the current player level could cast this (assuming it is a grouped peer or target mob)
+                                    for any_class in spell_casters["spells"][
+                                        check_spell
+                                    ]["classes"]:
+                                        if state.char_level is not None:
+                                            if (
+                                                state.char_level
+                                                >= spell_casters["spells"][check_spell][
+                                                    "classes"
+                                                ][any_class]
+                                            ):
+                                                player_level_could_cast = True
 
-                                        if player_level_could_cast:
-                                            identified_spell_level = state.char_level
-                                        else:
-                                            identified_spell_level = 60
+                                            if (
+                                                identified_spell_level is None
+                                                and spell_casters["spells"][
+                                                    check_spell
+                                                ]["item"]
+                                            ):
+                                                for item in spell_items["spells"][
+                                                    check_spell
+                                                ].keys():
+                                                    if (
+                                                        spell_items["spells"][
+                                                            check_spell
+                                                        ][item]["cast"]
+                                                        == 0
+                                                    ):
+                                                        for (
+                                                            clickable_class
+                                                        ) in spell_items["spells"][
+                                                            check_spell
+                                                        ][
+                                                            item
+                                                        ][
+                                                            "classes"
+                                                        ]:
+                                                            if (
+                                                                spell_items["spells"][
+                                                                    check_spell
+                                                                ][item]["classes"][
+                                                                    clickable_class
+                                                                ]
+                                                                <= state.char_level
+                                                            ):
+                                                                player_level_could_cast = (
+                                                                    True
+                                                                )
+
+                                            if player_level_could_cast:
+                                                identified_spell_level = (
+                                                    state.char_level
+                                                )
+                                            else:
+                                                identified_spell_level = 60
 
-                                        identified_spell_caster = recent_cast_event[
-                                            "caster"
-                                        ]
-                                        identified_spell = check_spell
-                                        identified_spell_target = target
+                                            identified_spell_caster = recent_cast_event[
+                                                "caster"
+                                            ]
+                                            identified_spell = check_spell
+                                            identified_spell_target = target
 
         # We know the spell which landed
         else:
             # If we have spell_caster info on this spell
             if spell in spell_casters["spells"].keys():
                 # If what just landed is what the active player last cast
                 if (
@@ -1289,15 +1320,15 @@
                             identified_spell_caster = identified[0]
                             identified_spell_level = identified[1]
                             identified_spell = identified[2]
                             identified_spell_target = target
 
                         # Check if active player could have clicked this spell
                         elif spell_casters["spells"][spell]["item"]:
-                            for item in spell_items["spells"][spell]:
+                            for item in spell_items["spells"][spell].keys():
                                 cast_duration = spell_items["spells"][spell][item][
                                     "cast"
                                 ]
                                 if cast_duration > 0:
                                     identified = action_spell_timer_player_click_check(
                                         line_time,
                                         spell_casting_buffer_you["time"],
@@ -1339,15 +1370,15 @@
                                 if identified is not None:
                                     identified_spell_caster = identified[0]
                                     identified_spell_level = identified[1]
                                     identified_spell = identified[2]
                                     identified_spell_target = target
                                 # Check if another player used a clicky
                                 elif spell_casters["spells"][spell]["item"]:
-                                    for item in spell_items["spells"][spell]:
+                                    for item in spell_items["spells"][spell].keys():
                                         cast_duration = spell_items["spells"][spell][
                                             item
                                         ]["cast"]
                                         # Non-zero click casts have spell casting messages
                                         if cast_duration > 0:
                                             identified = (
                                                 action_spell_timer_player_click_check(
@@ -1390,15 +1421,15 @@
                                                 identified_spell_level = identified[1]
                                                 identified_spell = identified[2]
                                                 identified_spell_target = target
 
                 # Haven't found anything yet, check if it could be an instant click (these have no casting messages)
                 if identified_spell_level is None and target == state.char.lower():
                     if spell in spell_items["spells"].keys():
-                        for item in spell_items["spells"][spell]:
+                        for item in spell_items["spells"][spell].keys():
                             if spell_items["spells"][spell][item]["cast"] == 0:
                                 identified = action_spell_timer_player_click_check(
                                     line_time,
                                     line_time,
                                     0,
                                     state.char.lower(),
                                     state.char_level,
@@ -1447,15 +1478,15 @@
                                     ):
                                         player_level_could_cast = True
 
                                     if (
                                         identified_spell_level is None
                                         and spell_casters["spells"][spell]["item"]
                                     ):
-                                        for item in spell_items["spells"][spell]:
+                                        for item in spell_items["spells"][spell].keys():
                                             if (
                                                 spell_items["spells"][spell][item][
                                                     "cast"
                                                 ]
                                                 == 0
                                             ):
                                                 for clickable_class in spell_items[
```

### Comparing `eqalert-3.5.3/eqa/lib/config.py` & `eqalert-3.5.4/eqa/lib/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -6311,16 +6311,16 @@
           "warrior": 0,
           "wizard": 0
         }
       }
     },
     "avatar": {
       "primal_weapon": {
-        "  cast": 0,
-        "  classes": {
+        "cast": 0,
+        "classes": {
           "bard": 0,
           "cleric": 0,
           "druid": 0,
           "enchanter": 0,
           "magician": 0,
           "monk": 0,
           "necromancer": 0,
@@ -6500,15 +6500,15 @@
         "classes": {
           "rogue": 0
         }
       }
     },
     "blessing_of_nature": {
       "razor_fang_of_xygoz": {
-        "  cast": 0,
+        "cast": 0,
         "classes": {
           "ranger": 50,
           "rogue": 50,
           "shadow knight": 50,
           "warrior": 50
         }
       }
@@ -8002,30 +8002,32 @@
         "cast": 0,
         "classes": {
           "monk": 50
         }
       }
     },
     "frostreavers_blessing": {
-      "cast": 0,
-      "classes": {
-        "bard": 0,
-        "cleric": 0,
-        "druid": 0,
-        "enchanter": 0,
-        "magician": 0,
-        "monk": 0,
-        "necromancer": 0,
-        "paladin": 0,
-        "ranger": 0,
-        "rogue": 0,
-        "shadow knight": 0,
-        "shaman": 0,
-        "warrior": 0,
-        "wizard": 0
+      "ring_of_dain_frostraver_iv": {
+        "cast": 0,
+        "classes": {
+          "bard": 0,
+          "cleric": 0,
+          "druid": 0,
+          "enchanter": 0,
+          "magician": 0,
+          "monk": 0,
+          "necromancer": 0,
+          "paladin": 0,
+          "ranger": 0,
+          "rogue": 0,
+          "shadow knight": 0,
+          "shaman": 0,
+          "warrior": 0,
+          "wizard": 0
+        }
       }
     },
     "fungal_regrowth": {
       "fungus_covered_great_staff": {
         "cast": 0,
         "classes": {
           "bard": 0,
@@ -8528,30 +8530,32 @@
           "shaman": 10,
           "warrior": 10,
           "wizard": 10
         }
       }
     },
     "lower_resists_ii": {
-      "cast": 0,
-      "classes": {
-        "bard": 20,
-        "cleric": 20,
-        "druid": 20,
-        "enchanter": 20,
-        "magician": 20,
-        "monk": 20,
-        "necromancer": 20,
-        "paladin": 20,
-        "ranger": 20,
-        "rogue": 20,
-        "shadow knight": 20,
-        "shaman": 20,
-        "warrior": 20,
-        "wizard": 20
+      "dilapidating_ash": {
+        "cast": 0,
+        "classes": {
+          "bard": 20,
+          "cleric": 20,
+          "druid": 20,
+          "enchanter": 20,
+          "magician": 20,
+          "monk": 20,
+          "necromancer": 20,
+          "paladin": 20,
+          "ranger": 20,
+          "rogue": 20,
+          "shadow knight": 20,
+          "shaman": 20,
+          "warrior": 20,
+          "wizard": 20
+        }
       }
     },
     "lower_resists_iii": {
       "cyclic_vertigo": {
         "cast": 0,
         "classes": {
           "bard": 30,
@@ -9577,15 +9581,15 @@
           "  shadow knight": 46,
           "  warrior": 46
         }
       }
     },
     "siphon_strength": {
       "discple_symbol_of_innoruuk": {
-        "  cast": 6,
+        "cast": 6,
         "classes": {
           "cleric": 5,
           "shaman": 5
         }
       }
     },
     "skin_like_diamond": {
@@ -10158,15 +10162,15 @@
       "garduk": {
         "cast": 0,
         "classes": {
           "shaman": 46
         }
       },
       "swarmcaller": {
-        "casat": 0,
+        "cast": 0,
         "classes": {
           "ranger": 46
         }
       }
     },
     "tainted_breath": {
       "poisoned_whip": {
@@ -14093,14 +14097,15 @@
           "by_list": false,
           "filter_list": {
             "spirit_of_wolf": false
           },
           "guild_only": false,
           "yours_only": true
         },
+        "consolidate": true,
         "delay": 24,
         "guess": true,
         "other": true,
         "self": true,
         "zone_drift": true
       }
     }
@@ -14145,15 +14150,15 @@
     "City of Thurgadin": {
       "indoors": true,
       "raid_mode": false,
       "timer": 420
     },
     "Cobalt Scar": {
       "indoors": false,
-      "raid_mode": false,
+      "raid_mode": true,
       "timer": 1200
     },
     "Crushbone": {
       "indoors": false,
       "raid_mode": false,
       "timer": 540
     },
@@ -14170,20 +14175,20 @@
     "Dalnir": {
       "indoors": true,
       "raid_mode": false,
       "timer": 720
     },
     "Dragon Necropolis": {
       "indoors": true,
-      "raid_mode": false,
+      "raid_mode": true,
       "timer": 1620
     },
     "Dreadlands": {
       "indoors": false,
-      "raid_mode": false,
+      "raid_mode": true,
       "timer": 400
     },
     "East Commonlands": {
       "indoors": false,
       "raid_mode": false,
       "timer": 400
     },
@@ -14355,15 +14360,15 @@
     "Misty Thicket": {
       "indoors": false,
       "raid_mode": false,
       "timer": 400
     },
     "Nagafen's Lair": {
       "indoors": true,
-      "raid_mode": false,
+      "raid_mode": true,
       "timer": 1320
     },
     "Najena": {
       "indoors": true,
       "raid_mode": false,
       "timer": 1110
     },
@@ -14395,25 +14400,25 @@
     "Ocean of Tears": {
       "indoors": false,
       "raid_mode": false,
       "timer": 360
     },
     "Old Sebilis": {
       "indoors": true,
-      "raid_mode": false,
+      "raid_mode": true,
       "timer": 1620
     },
     "Paineel": {
       "indoors": false,
       "raid_mode": false,
       "timer": 630
     },
     "Permafrost Caverns": {
       "indoors": true,
-      "raid_mode": false,
+      "raid_mode": true,
       "timer": 1320
     },
     "Plane of Air": {
       "indoors": false,
       "raid_mode": true,
       "timer": 28800
     },
@@ -14460,15 +14465,15 @@
     "Sirens Grotto": {
       "indoors": true,
       "raid_mode": false,
       "timer": 1680
     },
     "Skyfire Mountains": {
       "indoors": false,
-      "raid_mode": false,
+      "raid_mode": true,
       "timer": 780
     },
     "Skyshrine": {
       "indoors": false,
       "raid_mode": true,
       "timer": 1800
     },
@@ -14535,15 +14540,15 @@
     "The City of Mist": {
       "indoors": false,
       "raid_mode": false,
       "timer": 1320
     },
     "The Emerald Jungle": {
       "indoors": false,
-      "raid_mode": false,
+      "raid_mode": true,
       "timer": 0
     },
     "The Feerrott": {
       "indoors": false,
       "raid_mode": false,
       "timer": 400
     },
@@ -14570,15 +14575,15 @@
     "Tower of Frozen Shadow": {
       "indoors": true,
       "raid_mode": false,
       "timer": 1200
     },
     "Timorous Deep": {
       "indoors": false,
-      "raid_mode": false,
+      "raid_mode": true,
       "timer": 720
     },
     "Toxxulia Forest": {
       "indoors": false,
       "raid_mode": false,
       "timer": 400
     },
@@ -14590,15 +14595,15 @@
     "Veeshan's Peak": {
       "indoors": false,
       "raid_mode": true,
       "timer": 0
     },
     "Velketor's Labyrinth": {
       "indoors": true,
-      "raid_mode": false,
+      "raid_mode": true,
       "timer": 1972
     },
     "Warrens": {
       "indoors": false,
       "raid_mode": false,
       "timer": 400
     },
```

### Comparing `eqalert-3.5.3/eqa/lib/curses.py` & `eqalert-3.5.4/eqa/lib/curses.py`

 * *Files 0% similar despite different names*

```diff
@@ -2051,15 +2051,15 @@
                         message = timer.payload
                         timer_scr.addstr(
                             print_timer_y,
                             2 + timestamp_len,
                             message,
                             curses.color_pair(3),
                         )
-                    print_timer_y = print_timer_y + 2
+                    print_timer_y = print_timer_y + 1
             else:
                 draw_mascot_message(timer_scr, "No active timers")
         else:
             draw_mascot_message(timer_scr, "No active timers")
 
     except Exception as e:
         eqa_settings.log(
@@ -2119,77 +2119,81 @@
         helpscr.addstr(13, 15, ":", curses.color_pair(1))
         helpscr.addstr(13, 17, "Quit", curses.color_pair(3))
 
         helpscr.addstr(14, 9, "h", curses.color_pair(2))
         helpscr.addstr(14, 15, ":", curses.color_pair(1))
         helpscr.addstr(14, 17, "Help", curses.color_pair(3))
 
-        # Events commands
-        helpscr.addstr(16, 7, "Events", curses.color_pair(1))
+        helpscr.addstr(15, 9, "t", curses.color_pair(2))
+        helpscr.addstr(15, 15, ":", curses.color_pair(1))
+        helpscr.addstr(15, 17, "Timers", curses.color_pair(3))
 
-        helpscr.addstr(17, 9, "c", curses.color_pair(2))
-        helpscr.addstr(17, 15, ":", curses.color_pair(1))
-        helpscr.addstr(17, 17, "Clear events", curses.color_pair(3))
+        # Events commands
+        helpscr.addstr(17, 7, "Events", curses.color_pair(1))
 
-        helpscr.addstr(18, 9, "d", curses.color_pair(2))
+        helpscr.addstr(18, 9, "c", curses.color_pair(2))
         helpscr.addstr(18, 15, ":", curses.color_pair(1))
-        helpscr.addstr(18, 17, "Toggle debug mode", curses.color_pair(3))
+        helpscr.addstr(18, 17, "Clear events", curses.color_pair(3))
 
-        helpscr.addstr(19, 9, "e", curses.color_pair(2))
+        helpscr.addstr(19, 9, "d", curses.color_pair(2))
         helpscr.addstr(19, 15, ":", curses.color_pair(1))
-        helpscr.addstr(19, 17, "Toggle encounter parsing", curses.color_pair(3))
+        helpscr.addstr(19, 17, "Toggle debug mode", curses.color_pair(3))
 
-        helpscr.addstr(20, 9, "m", curses.color_pair(2))
+        helpscr.addstr(20, 9, "e", curses.color_pair(2))
         helpscr.addstr(20, 15, ":", curses.color_pair(1))
-        helpscr.addstr(20, 17, "Toggle mute", curses.color_pair(3))
+        helpscr.addstr(20, 17, "Toggle encounter parsing", curses.color_pair(3))
 
-        helpscr.addstr(21, 9, "p", curses.color_pair(2))
+        helpscr.addstr(21, 9, "m", curses.color_pair(2))
         helpscr.addstr(21, 15, ":", curses.color_pair(1))
-        helpscr.addstr(21, 17, "Toggle encounter parse save", curses.color_pair(3))
+        helpscr.addstr(21, 17, "Toggle mute", curses.color_pair(3))
 
-        helpscr.addstr(22, 9, "r", curses.color_pair(2))
+        helpscr.addstr(22, 9, "p", curses.color_pair(2))
         helpscr.addstr(22, 15, ":", curses.color_pair(1))
-        helpscr.addstr(22, 17, "Toggle raid mode", curses.color_pair(3))
+        helpscr.addstr(22, 17, "Toggle encounter parse save", curses.color_pair(3))
 
-        helpscr.addstr(23, 9, "t", curses.color_pair(2))
+        helpscr.addstr(23, 9, "r", curses.color_pair(2))
         helpscr.addstr(23, 15, ":", curses.color_pair(1))
+        helpscr.addstr(23, 17, "Toggle raid mode", curses.color_pair(3))
+
+        helpscr.addstr(24, 9, "y", curses.color_pair(2))
+        helpscr.addstr(24, 15, ":", curses.color_pair(1))
         helpscr.addstr(
-            23, 17, "Toggle automatic mob respawn timers", curses.color_pair(3)
+            24, 17, "Toggle automatic mob respawn timers", curses.color_pair(3)
         )
 
         # Settings commands
-        helpscr.addstr(25, 7, "Settings", curses.color_pair(1))
+        helpscr.addstr(26, 7, "Settings", curses.color_pair(1))
 
-        helpscr.addstr(26, 9, "up", curses.color_pair(2))
-        helpscr.addstr(26, 15, ":", curses.color_pair(1))
-        helpscr.addstr(26, 17, "Up in selection", curses.color_pair(3))
-
-        helpscr.addstr(27, 9, "down", curses.color_pair(2))
+        helpscr.addstr(27, 9, "up", curses.color_pair(2))
         helpscr.addstr(27, 15, ":", curses.color_pair(1))
-        helpscr.addstr(27, 17, "Down in selection", curses.color_pair(3))
+        helpscr.addstr(27, 17, "Up in selection", curses.color_pair(3))
 
-        helpscr.addstr(28, 9, "right", curses.color_pair(2))
+        helpscr.addstr(28, 9, "down", curses.color_pair(2))
         helpscr.addstr(28, 15, ":", curses.color_pair(1))
-        helpscr.addstr(28, 17, "Selection options", curses.color_pair(3))
+        helpscr.addstr(28, 17, "Down in selection", curses.color_pair(3))
 
-        helpscr.addstr(29, 9, "left", curses.color_pair(2))
+        helpscr.addstr(29, 9, "right", curses.color_pair(2))
         helpscr.addstr(29, 15, ":", curses.color_pair(1))
         helpscr.addstr(29, 17, "Selection options", curses.color_pair(3))
 
-        helpscr.addstr(30, 9, "space", curses.color_pair(2))
+        helpscr.addstr(30, 9, "left", curses.color_pair(2))
         helpscr.addstr(30, 15, ":", curses.color_pair(1))
-        helpscr.addstr(30, 17, "Select", curses.color_pair(3))
+        helpscr.addstr(30, 17, "Selection options", curses.color_pair(3))
 
-        helpscr.addstr(31, 9, "enter", curses.color_pair(2))
+        helpscr.addstr(31, 9, "space", curses.color_pair(2))
         helpscr.addstr(31, 15, ":", curses.color_pair(1))
         helpscr.addstr(31, 17, "Select", curses.color_pair(3))
 
-        helpscr.addstr(32, 9, "tab", curses.color_pair(2))
+        helpscr.addstr(32, 9, "enter", curses.color_pair(2))
         helpscr.addstr(32, 15, ":", curses.color_pair(1))
-        helpscr.addstr(32, 17, "Cycle category", curses.color_pair(3))
+        helpscr.addstr(32, 17, "Select", curses.color_pair(3))
+
+        helpscr.addstr(33, 9, "tab", curses.color_pair(2))
+        helpscr.addstr(33, 15, ":", curses.color_pair(1))
+        helpscr.addstr(33, 17, "Cycle category", curses.color_pair(3))
 
     except Exception as e:
         eqa_settings.log(
             "draw help: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
```

### Comparing `eqalert-3.5.3/eqa/lib/encounter.py` & `eqalert-3.5.4/eqa/lib/encounter.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.3/eqa/lib/keys.py` & `eqalert-3.5.4/eqa/lib/keys.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.3/eqa/lib/log.py` & `eqalert-3.5.4/eqa/lib/log.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.3/eqa/lib/parser.py` & `eqalert-3.5.4/eqa/lib/parser.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.3/eqa/lib/settings.py` & `eqalert-3.5.4/eqa/lib/settings.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.3/eqa/lib/sound.py` & `eqalert-3.5.4/eqa/lib/sound.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
    with this program; if not, write to the Free Software Foundation, Inc.,
    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 """
 
 import os
 import re
 import time
+import threading
 import sys
 import hashlib
 import gtts
 from playsound import playsound
 
 import eqa.lib.struct as eqa_struct
 import eqa.lib.settings as eqa_settings
@@ -286,15 +287,15 @@
             + str(e)
         )
 
 
 def play_sound(sound):
     """Play the sound given"""
     try:
-        playsound(sound)
+        threading.Thread(target=playsound, args=(sound,), daemon=True).start()
     except Exception as e:
         eqa_settings.log(
             "sound_play_sound: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
```

### Comparing `eqalert-3.5.3/eqa/lib/state.py` & `eqalert-3.5.4/eqa/lib/state.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.3/eqa/lib/struct.py` & `eqalert-3.5.4/eqa/lib/struct.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.3/eqa/lib/timer.py` & `eqalert-3.5.4/eqa/lib/timer.py`

 * *Files 3% similar despite different names*

```diff
@@ -228,14 +228,21 @@
                                         + datetime.timedelta(seconds=int(timer.seconds))
                                     ),
                                     "metronome",
                                     timer.seconds,
                                     timer.payload,
                                 )
                             )
+                    elif timer.type == "spell":
+                        if configs.settings.config["settings"]["timers"]["spell"][
+                            "consolidate"
+                        ]:
+                            timers = consolidate_spell_timers(
+                                timer, timers, sound_q, display_q
+                            )
                     else:
                         sound_q.put(eqa_struct.sound("speak", str(timer.payload)))
                         display_q.put(
                             eqa_struct.display(
                                 eqa_settings.eqa_time(),
                                 "event",
                                 "events",
@@ -339,14 +346,65 @@
             "Remove spell timer: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
+def consolidate_spell_timers(expired_timer, timers, sound_q, display_q):
+    """Consolidate like spell timers"""
+
+    try:
+        new_timers = []
+        for timer_event in timers:
+            if timer_event.type == "spell":
+                if expired_timer.spell == timer_event.spell:
+                    if int((timer_event.time - expired_timer.time).total_seconds()) < 3:
+                        if expired_timer.payload.endswith(" has worn off"):
+                            payload = (
+                                expired_timer.spell.replace("_", " ")
+                                + " on "
+                                + expired_timer.target
+                                + " and others has worn off"
+                            )
+                        else:
+                            payload = (
+                                expired_timer.spell.replace("_", " ")
+                                + " on "
+                                + expired_timer.target
+                                + " and others is wearing off"
+                            )
+                    else:
+                        heapq.heappush(new_timers, timer_event)
+                else:
+                    heapq.heappush(new_timers, timer_event)
+            else:
+                heapq.heappush(new_timers, timer_event)
+
+        sound_q.put(eqa_struct.sound("speak", payload))
+        display_q.put(
+            eqa_struct.display(
+                eqa_settings.eqa_time(),
+                "event",
+                "events",
+                "Timer: " + str(payload),
+            )
+        )
+
+        return new_timers
+
+    except Exception as e:
+        eqa_settings.log(
+            "Consolidate spell timer: Error on line "
+            + str(sys.exc_info()[-1].tb_lineno)
+            + ": "
+            + str(e)
+        )
+
+
 def add_spell_timer(state, timers, new_timer_event):
     """Add a timer"""
 
     try:
         new_timers = []
         for timer_event in timers:
             if timer_event.type == "spell":
```

### Comparing `eqalert-3.5.3/eqa/lib/watch.py` & `eqalert-3.5.4/eqa/lib/watch.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.3/eqa/sound/tick.wav` & `eqalert-3.5.4/eqa/sound/tick.wav`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.3/eqa/sound/tock.wav` & `eqalert-3.5.4/eqa/sound/tock.wav`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.3/eqalert.egg-info/PKG-INFO` & `eqalert-3.5.4/eqalert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eqalert
-Version: 3.5.3
+Version: 3.5.4
 Summary: Configurable and Context Driven Project 1999 Log Parser
 Home-page: https://github.com/mgeitz/eqalert
 Author: M Geitz
 Author-email: git@geitz.xyz
 License: GPL2
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
```

### Comparing `eqalert-3.5.3/eqalert.egg-info/SOURCES.txt` & `eqalert-3.5.4/eqalert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.3/setup.py` & `eqalert-3.5.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="eqalert",
-    version="3.5.3",
+    version="3.5.4",
     author="M Geitz",
     author_email="git@geitz.xyz",
     install_requires=[
         "playsound>=1.3.0",
         "gtts>=2.3.1",
     ],
     python_requires=">=3.9.2",
```

