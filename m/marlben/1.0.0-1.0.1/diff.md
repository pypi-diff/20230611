# Comparing `tmp/marlben-1.0.0.tar.gz` & `tmp/marlben-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marlben-1.0.0.tar", last modified: Sun Jun 11 11:53:07 2023, max compression
+gzip compressed data, was "marlben-1.0.1.tar", last modified: Sun Jun 11 18:20:00 2023, max compression
```

## Comparing `marlben-1.0.0.tar` & `marlben-1.0.1.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.215497 marlben-1.0.0/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1068 2023-06-11 10:56:49.000000 marlben-1.0.0/LICENSE
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1675 2023-06-11 11:53:07.215497 marlben-1.0.0/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      548 2023-06-11 10:56:49.000000 marlben-1.0.0/README.md
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.207497 marlben-1.0.0/marlben/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      684 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/__init__.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.207497 marlben-1.0.0/marlben/config/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      110 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/config/__init__.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.207497 marlben-1.0.0/marlben/config/base/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       69 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/config/base/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5665 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/config/base/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1778 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/config/base/presets.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      240 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/config/builders.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1403 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/config/common.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      223 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/config/presets.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.207497 marlben-1.0.0/marlben/config/systems/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      120 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/config/systems/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3346 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/config/systems/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      148 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/config/systems/presets.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.207497 marlben-1.0.0/marlben/core/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      142 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      749 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/agent.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)    17853 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/env.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2128 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/map.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.207497 marlben-1.0.0/marlben/core/map_generation/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/map_generation/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     7051 2023-06-11 11:51:34.000000 marlben-1.0.0/marlben/core/map_generation/base.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2430 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/map_generation/checks.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1397 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/map_generation/pregen_map_generator.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1813 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/map_generation/resources.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3271 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/map_generation/rock_patterns.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3315 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/realm.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.207497 marlben-1.0.0/marlben/core/spawn/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/spawn/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     9237 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/spawn/base_manager.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.207497 marlben-1.0.0/marlben/core/spawn/spawn_system/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      583 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/spawn/spawn_system/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2189 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/spawn/spawn_system/base.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1162 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/spawn/spawn_system/base_samplers.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     4114 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/spawn/spawn_system/position_samplers.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2539 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/spawn/spawn_system/skill_samplers.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3507 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/core/tile.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.207497 marlben-1.0.0/marlben/entity/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       82 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/entity/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5741 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/entity/entity.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3428 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/entity/npc.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2621 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/entity/player.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.207497 marlben-1.0.0/marlben/envs/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3049 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/__init__.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.207497 marlben-1.0.0/marlben/envs/arena/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       76 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/arena/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      753 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/arena/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      775 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/arena/env.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.207497 marlben-1.0.0/marlben/envs/boss_fight/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       63 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/boss_fight/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2810 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/boss_fight/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1099 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/boss_fight/env.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/envs/building/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      111 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/building/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      782 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/building/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      516 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/building/env.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/envs/colors/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       81 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/colors/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      606 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/colors/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      544 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/colors/env.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/envs/corridor/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      110 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/corridor/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3140 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/corridor/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1000 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/corridor/env.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/envs/deathmatch/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       90 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/deathmatch/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1153 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/deathmatch/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      935 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/deathmatch/env.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/envs/exploring/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      103 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/exploring/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      604 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/exploring/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1109 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/exploring/env.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/envs/gathering/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       87 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/gathering/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3535 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/gathering/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      799 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/gathering/env.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/envs/gathering/utils/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3610 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/gathering/utils/map_generator.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/envs/planting/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      111 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/planting/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      809 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/planting/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      807 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/planting/env.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/envs/predator_prey/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       97 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/predator_prey/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2023 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/predator_prey/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      855 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/predator_prey/env.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/envs/pve/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       70 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/pve/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2000 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/pve/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1487 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/pve/env.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/envs/raid/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       57 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/raid/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2054 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/raid/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1021 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/raid/env.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/envs/siege/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       75 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/siege/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2066 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/siege/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      617 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/siege/env.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/envs/spying/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       79 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/spying/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      515 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/spying/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1706 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/spying/env.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/envs/team_deathmatch/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      102 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/team_deathmatch/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1241 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/team_deathmatch/config.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      640 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/envs/team_deathmatch/env.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     8610 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/infrastructure.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.211497 marlben-1.0.0/marlben/io/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/io/__init__.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.215497 marlben-1.0.0/marlben/io/action/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      382 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/io/action/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3170 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/io/action/attack.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1130 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/io/action/base_action.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1052 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/io/action/build.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      860 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/io/action/common.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       24 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/io/action/message.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1646 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/io/action/move.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1384 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/io/action/plant.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2168 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/io/action/share.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6430 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/io/stimulus.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.215497 marlben-1.0.0/marlben/lib/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       52 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/lib/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3858 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/lib/colors.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      515 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/lib/distance.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1169 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/lib/log.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2053 2023-06-11 11:45:18.000000 marlben-1.0.0/marlben/lib/material.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1616 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/lib/overlay.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1564 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/lib/priorityqueue.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2937 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/lib/rating.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2105 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/lib/utils.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5275 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/overlay.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1341 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/scripting.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.215497 marlben-1.0.0/marlben/systems/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       25 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1297 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/achievement.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.215497 marlben-1.0.0/marlben/systems/ai/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       52 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/ai/__init__.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       68 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/ai/attack.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2914 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/ai/behavior.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     4447 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/ai/dynamic_programming.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1726 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/ai/move.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      955 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/ai/policy.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5674 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/ai/utils.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2293 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/combat.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      892 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/droptable.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1227 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/equipment.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      611 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/experience.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      318 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/sharing.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     8517 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/systems/skill.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       22 2023-06-11 11:14:29.000000 marlben-1.0.0/marlben/version.py
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     4511 2023-06-11 10:56:49.000000 marlben-1.0.0/marlben/websocket.py
-drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 11:53:07.207497 marlben-1.0.0/marlben.egg-info/
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1675 2023-06-11 11:53:07.000000 marlben-1.0.0/marlben.egg-info/PKG-INFO
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3848 2023-06-11 11:53:07.000000 marlben-1.0.0/marlben.egg-info/SOURCES.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-06-11 11:53:07.000000 marlben-1.0.0/marlben.egg-info/dependency_links.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      308 2023-06-11 11:53:07.000000 marlben-1.0.0/marlben.egg-info/requires.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        8 2023-06-11 11:53:07.000000 marlben-1.0.0/marlben.egg-info/top_level.txt
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3326 2023-06-11 11:47:33.000000 marlben-1.0.0/pyproject.toml
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-06-11 11:53:07.215497 marlben-1.0.0/setup.cfg
--rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      937 2023-06-11 10:56:49.000000 marlben-1.0.0/setup.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.421457 marlben-1.0.1/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1068 2023-06-11 10:56:49.000000 marlben-1.0.1/LICENSE
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1675 2023-06-11 18:20:00.421457 marlben-1.0.1/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      548 2023-06-11 10:56:49.000000 marlben-1.0.1/README.md
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.409458 marlben-1.0.1/marlben/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      684 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/__init__.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.409458 marlben-1.0.1/marlben/config/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      110 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/config/__init__.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.409458 marlben-1.0.1/marlben/config/base/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       69 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/config/base/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6262 2023-06-11 17:11:45.000000 marlben-1.0.1/marlben/config/base/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2057 2023-06-11 16:01:36.000000 marlben-1.0.1/marlben/config/base/presets.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      240 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/config/builders.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1403 2023-06-11 16:52:57.000000 marlben-1.0.1/marlben/config/common.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      223 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/config/presets.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.409458 marlben-1.0.1/marlben/config/systems/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      120 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/config/systems/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3346 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/config/systems/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      148 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/config/systems/presets.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/core/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      142 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      749 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/agent.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)    17890 2023-06-11 18:01:01.000000 marlben-1.0.1/marlben/core/env.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2128 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/map.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/core/map_generation/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/map_generation/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     7051 2023-06-11 18:12:37.000000 marlben-1.0.1/marlben/core/map_generation/base.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2430 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/map_generation/checks.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1397 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/map_generation/pregen_map_generator.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1813 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/map_generation/resources.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3271 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/map_generation/rock_patterns.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3315 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/realm.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/core/spawn/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/spawn/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     9237 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/spawn/base_manager.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/core/spawn/spawn_system/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      583 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/spawn/spawn_system/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2189 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/spawn/spawn_system/base.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1162 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/spawn/spawn_system/base_samplers.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     4114 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/spawn/spawn_system/position_samplers.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2539 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/spawn/spawn_system/skill_samplers.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3507 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/core/tile.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/entity/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       82 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/entity/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5741 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/entity/entity.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3428 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/entity/npc.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2621 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/entity/player.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/envs/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3049 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/__init__.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/envs/arena/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       76 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/arena/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      753 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/arena/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      775 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/arena/env.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/envs/boss_fight/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       63 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/boss_fight/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2810 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/boss_fight/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1099 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/boss_fight/env.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/envs/building/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      111 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/building/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      782 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/building/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      516 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/building/env.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/envs/colors/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       81 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/colors/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      606 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/colors/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      544 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/colors/env.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/envs/corridor/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      110 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/corridor/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3196 2023-06-11 17:10:58.000000 marlben-1.0.1/marlben/envs/corridor/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1000 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/corridor/env.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/envs/deathmatch/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       90 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/deathmatch/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1153 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/deathmatch/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      935 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/deathmatch/env.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/envs/exploring/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      103 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/exploring/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      604 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/exploring/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1109 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/exploring/env.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/envs/gathering/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       87 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/gathering/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3535 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/gathering/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      799 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/gathering/env.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/envs/gathering/utils/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3610 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/gathering/utils/map_generator.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.413457 marlben-1.0.1/marlben/envs/planting/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      111 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/planting/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      809 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/planting/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      807 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/planting/env.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.417457 marlben-1.0.1/marlben/envs/predator_prey/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       97 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/predator_prey/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2023 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/predator_prey/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      855 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/predator_prey/env.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.417457 marlben-1.0.1/marlben/envs/pve/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       70 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/pve/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2000 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/pve/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1487 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/pve/env.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.417457 marlben-1.0.1/marlben/envs/raid/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       57 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/raid/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2054 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/raid/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1021 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/raid/env.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.417457 marlben-1.0.1/marlben/envs/siege/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       75 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/siege/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2066 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/siege/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      617 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/siege/env.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.417457 marlben-1.0.1/marlben/envs/spying/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       79 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/spying/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      515 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/spying/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1706 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/spying/env.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.417457 marlben-1.0.1/marlben/envs/team_deathmatch/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      102 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/team_deathmatch/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1241 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/team_deathmatch/config.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      640 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/envs/team_deathmatch/env.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     8610 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/infrastructure.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.417457 marlben-1.0.1/marlben/io/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/io/__init__.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.417457 marlben-1.0.1/marlben/io/action/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      382 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/io/action/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3134 2023-06-11 16:23:24.000000 marlben-1.0.1/marlben/io/action/attack.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1130 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/io/action/base_action.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1052 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/io/action/build.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      860 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/io/action/common.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       24 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/io/action/message.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1646 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/io/action/move.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1384 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/io/action/plant.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2132 2023-06-11 16:23:39.000000 marlben-1.0.1/marlben/io/action/share.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     6432 2023-06-11 16:25:23.000000 marlben-1.0.1/marlben/io/stimulus.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.417457 marlben-1.0.1/marlben/lib/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       52 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/lib/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3858 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/lib/colors.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      515 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/lib/distance.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1169 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/lib/log.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2053 2023-06-11 11:45:18.000000 marlben-1.0.1/marlben/lib/material.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1616 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/lib/overlay.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1564 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/lib/priorityqueue.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2937 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/lib/rating.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2105 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/lib/utils.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5275 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/overlay.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1343 2023-06-11 16:23:33.000000 marlben-1.0.1/marlben/scripting.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.417457 marlben-1.0.1/marlben/systems/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       25 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1297 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/achievement.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.421457 marlben-1.0.1/marlben/systems/ai/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       52 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/ai/__init__.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       68 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/ai/attack.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2914 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/ai/behavior.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     4447 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/ai/dynamic_programming.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1726 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/ai/move.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      955 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/ai/policy.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     5674 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/ai/utils.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     2293 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/combat.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      892 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/droptable.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1227 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/equipment.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      611 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/experience.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      318 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/sharing.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     8517 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/systems/skill.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       22 2023-06-11 18:14:30.000000 marlben-1.0.1/marlben/version.py
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     4511 2023-06-11 10:56:49.000000 marlben-1.0.1/marlben/websocket.py
+drwxrwxr-x   0 vladimir  (1000) vladimir  (1000)        0 2023-06-11 18:20:00.409458 marlben-1.0.1/marlben.egg-info/
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     1675 2023-06-11 18:20:00.000000 marlben-1.0.1/marlben.egg-info/PKG-INFO
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3848 2023-06-11 18:20:00.000000 marlben-1.0.1/marlben.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        1 2023-06-11 18:20:00.000000 marlben-1.0.1/marlben.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      308 2023-06-11 18:20:00.000000 marlben-1.0.1/marlben.egg-info/requires.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)        8 2023-06-11 18:20:00.000000 marlben-1.0.1/marlben.egg-info/top_level.txt
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)     3326 2023-06-11 16:03:46.000000 marlben-1.0.1/pyproject.toml
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)       38 2023-06-11 18:20:00.421457 marlben-1.0.1/setup.cfg
+-rw-rw-r--   0 vladimir  (1000) vladimir  (1000)      937 2023-06-11 10:56:49.000000 marlben-1.0.1/setup.py
```

### Comparing `marlben-1.0.0/LICENSE` & `marlben-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/PKG-INFO` & `marlben-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marlben
-Version: 1.0.0
+Version: 1.0.1
 Summary: Marlben is a multi-agent reinforcement learning benchmark based on the NeuralMMO game engine.
 Author-email: JBR AI labs <ego.vladi@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/jbr-ai-labs/marlben
 Project-URL: Repository, https://github.com/jbr-ai-labs/marlben
 Project-URL: Documentation, https://github.com/jbr-ai-labs/marlben/wiki
 Project-URL: Bug Report, https://github.com/jbr-ai-labs/marlben/issues
```

### Comparing `marlben-1.0.0/README.md` & `marlben-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/__init__.py` & `marlben-1.0.1/marlben/__init__.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/config/base/config.py` & `marlben-1.0.1/marlben/config/base/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from dataclasses import field
 
 import marlben
 from marlben.config.common import Template, SequentialLoader
 from marlben.core.spawn.spawn_system import position_samplers, skill_samplers
 from marlben.io.action import Heal
 
 
@@ -40,32 +41,49 @@
    Notes:
       We use Google Fire internally to replace standard manual argparse
       definitions for each Config property. This means you can subclass
       Config to add new static attributes -- CLI definitions will be
       generated automatically.
    '''
 
-    def __init__(self):
+    def __init__(self, dictionary=None):
         super().__init__()
 
-        if __debug__:
-            err = 'config.Config is a base class. Use config.{Small, Medium Large}'''
-            assert type(self) != Config, err
+        if dictionary is not None:
+            self._populate_config(dictionary)
 
+    def _populate_config(self, dictionary):
+        for k, v in dictionary.items():
+            print(k, v)
+            if isinstance(v, dict):
+                self._populate_config(v)
+            else:
+                setattr(self, k, v)
     ############################################################################
     # Meta-Parameters
-    RENDER = False
+    RENDER: bool = False
+
+    def items(self):
+        class_vars = {}
+        for cls in self.__class__.mro()[:-1]:
+            class_vars.update({
+                k: v for k, v in cls.__dict__.items()
+                if k not in object.__dict__ and not k.startswith('_')
+                and not callable(v)
+                and not isinstance(v, property)
+            })
+        return class_vars.items()
 
     def game_system_enabled(self, name) -> bool:
         return hasattr(self, name)
 
     ############################################################################
     # Visibility and Accessibility settings
-    NUM_VISIBILITY_COLORS = 0
-    NUM_ACCESSIBILITY_COLORS = 0
+    NUM_VISIBILITY_COLORS: int = 0
+    NUM_ACCESSIBILITY_COLORS: int = 0
 
     # Population Parameters
     AGENT_LOADER = SequentialLoader
     '''Agent loader class specifying spawn sampling'''
 
     TASKS = []
     '''Tasks for which to compute rewards'''
@@ -83,15 +101,14 @@
 
     NSTIM = 7
     '''Number of tiles an agent can see in any direction'''
 
     N_AGENT_OBS = 100
     '''Number of distinct agent observations'''
 
-    @property
     def WINDOW(self):
         '''Size of the square tile crop visible to an agent'''
         return 2 * self.NSTIM + 1
 
     ############################################################################
     # Agent Parameters
     BASE_HEALTH = 10
```

### Comparing `marlben-1.0.0/marlben/config/base/presets.py` & `marlben-1.0.1/marlben/config/base/presets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,79 @@
+from dataclasses import dataclass, field
+
 from marlben.config.base.config import Config
 from marlben.core.spawn.spawn_system import skill_samplers
 from .config import NPCGroupConfig, PlayerGroupConfig
 from ... import Agent
+from ...core.spawn.spawn_system.skill_samplers import SkillsSampler
 
 
 class SmallNPCGroupConfig(NPCGroupConfig):
     NENT = 32
     SPAWN_SKILLS_SAMPLER = skill_samplers.DefaultNPCSkillSampler(1, 10, 1)
 
 
 class SmallPlayerGroupConfig(PlayerGroupConfig):
     NENT = 1
     AGENTS = [Agent]
 
 
+@dataclass
 class Small(Config):
     '''A small config for debugging and experiments with an expensive outer loop'''
 
-    PATH_MAPS = 'maps/small'
-    MAP_PREVIEW_DOWNSCALE = 4
+    PATH_MAPS: str = 'maps/small'
+    MAP_PREVIEW_DOWNSCALE: int = 4
 
-    TERRAIN_LOG_INTERPOLATE_MIN = 0
+    TERRAIN_LOG_INTERPOLATE_MIN: int = 0
 
-    TERRAIN_CENTER = 8  # 4
-    MAP_HEIGHT = 4
-    MAP_WIDTH = 4
-    PLAYER_GROUPS = [SmallPlayerGroupConfig(), SmallPlayerGroupConfig()]
+    TERRAIN_CENTER: int = 8  # 4
+    MAP_HEIGHT: int = 4
+    MAP_WIDTH: int = 4
+    PLAYER_GROUPS: list = field(default_factory=lambda: [SmallPlayerGroupConfig(), SmallPlayerGroupConfig()])
 
 
+@dataclass
 class MediumNPCGroupConfig(NPCGroupConfig):
-    NENT = 128
-    SPAWN_SKILLS_SAMPLER = skill_samplers.DefaultNPCSkillSampler(1, 30, 5)
+    NENT: int = 128
+    SPAWN_SKILLS_SAMPLER: SkillsSampler = skill_samplers.DefaultNPCSkillSampler(1, 30, 5)
 
 
+@dataclass
 class MediumPlayerGroupConfig(PlayerGroupConfig):
-    NENT = 256
+    NENT: int = 256
 
 
+@dataclass
 class Medium(Config):
     '''A medium config suitable for most academic-scale research'''
 
     PATH_MAPS = 'maps/medium'
     MAP_PREVIEW_DOWNSCALE = 16
 
     TERRAIN_CENTER = 128
     MAP_HEIGHT = 128
     MAP_WIDTH = 128
 
     PLAYER_GROUPS = [MediumPlayerGroupConfig()]
     NPC_GROUPS = [MediumNPCGroupConfig()]
 
 
+@dataclass
 class LargeNPCGroupConfig(NPCGroupConfig):
     NENT = 1024
     SPAWN_SKILLS_SAMPLER = skill_samplers.DefaultNPCSkillSampler(1, 99, 10)
 
 
+@dataclass
 class LargePlayerGroupConfig(PlayerGroupConfig):
     NENT = 2048
 
 
+@dataclass
 class Large(Config):
     '''A large config suitable for large-scale research or fast models'''
 
     PATH_MAPS = 'maps/large'
     MAP_PREVIEW_DOWNSCALE = 64
 
     TERRAIN_CENTER = 1024
```

### Comparing `marlben-1.0.0/marlben/config/common.py` & `marlben-1.0.1/marlben/config/common.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/config/systems/config.py` & `marlben-1.0.1/marlben/config/systems/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/agent.py` & `marlben-1.0.1/marlben/core/agent.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/env.py` & `marlben-1.0.1/marlben/core/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         super().__init__()
 
         if config is None:
             config = marlben.config.Default()
 
         if __debug__:
             err = 'Config {} is not a config instance (did you pass the class?)'
+            print(config)
             assert isinstance(config, marlben.config.Config), err.format(config)
 
         for entity_group in config.PLAYER_GROUPS:
             if not entity_group.AGENTS:
                 from marlben import agent
                 config.AGENTS = [agent.Random]
 
@@ -157,17 +158,17 @@
         if idx is None:
             idx = np.random.randint(self.config.NMAPS) + 1
 
         self.worldIdx = idx
         self.realm.reset(idx)
 
         if step:
-            self.obs, _, _, _ = self.step({})
+            self.obs, _, _, infos = self.step({})
 
-        return self.obs
+        return self.obs, infos
 
     def close(self):
         if self.client is not None:
             self.client.kill()
 
     def step(self, actions):
         '''Simulates one game tick or timestep
```

### Comparing `marlben-1.0.0/marlben/core/map.py` & `marlben-1.0.1/marlben/core/map.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/map_generation/base.py` & `marlben-1.0.1/marlben/core/map_generation/base.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/map_generation/checks.py` & `marlben-1.0.1/marlben/core/map_generation/checks.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/map_generation/pregen_map_generator.py` & `marlben-1.0.1/marlben/core/map_generation/pregen_map_generator.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/map_generation/resources.py` & `marlben-1.0.1/marlben/core/map_generation/resources.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/map_generation/rock_patterns.py` & `marlben-1.0.1/marlben/core/map_generation/rock_patterns.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/realm.py` & `marlben-1.0.1/marlben/core/realm.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/spawn/base_manager.py` & `marlben-1.0.1/marlben/core/spawn/base_manager.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/spawn/spawn_system/__init__.py` & `marlben-1.0.1/marlben/core/spawn/spawn_system/__init__.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/spawn/spawn_system/base.py` & `marlben-1.0.1/marlben/core/spawn/spawn_system/base.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/spawn/spawn_system/base_samplers.py` & `marlben-1.0.1/marlben/core/spawn/spawn_system/base_samplers.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/spawn/spawn_system/position_samplers.py` & `marlben-1.0.1/marlben/core/spawn/spawn_system/position_samplers.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/spawn/spawn_system/skill_samplers.py` & `marlben-1.0.1/marlben/core/spawn/spawn_system/skill_samplers.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/core/tile.py` & `marlben-1.0.1/marlben/core/tile.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/entity/entity.py` & `marlben-1.0.1/marlben/entity/entity.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/entity/npc.py` & `marlben-1.0.1/marlben/entity/npc.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/entity/player.py` & `marlben-1.0.1/marlben/entity/player.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/__init__.py` & `marlben-1.0.1/marlben/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/arena/config.py` & `marlben-1.0.1/marlben/envs/arena/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/arena/env.py` & `marlben-1.0.1/marlben/envs/arena/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/boss_fight/config.py` & `marlben-1.0.1/marlben/envs/boss_fight/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/boss_fight/env.py` & `marlben-1.0.1/marlben/envs/boss_fight/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/building/config.py` & `marlben-1.0.1/marlben/envs/building/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/building/env.py` & `marlben-1.0.1/marlben/envs/building/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/colors/config.py` & `marlben-1.0.1/marlben/envs/colors/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/colors/env.py` & `marlben-1.0.1/marlben/envs/colors/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/corridor/config.py` & `marlben-1.0.1/marlben/envs/corridor/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from dataclasses import dataclass
 from typing import Callable
 from os import path as osp
 
 from marlben.core.agent import Agent
 from marlben.core.spawn.spawn_system.position_samplers import UniformPositionSampler
 from marlben.core.spawn.spawn_system.skill_samplers import CustomSkillSampler
 from marlben.systems.achievement import Task
@@ -92,20 +93,22 @@
 def process_agents(player_groups):
     agents = []
     for group in player_groups:
         agents.extend(group.AGENTS)
     return agents
 
 
+@dataclass
 class ScriptedCorridorConfig(BaseCorridorConfig):
     PLAYER_GROUPS = create_group_config(agents=[CorridorAgent, CorridorAgent])
     AGENTS = process_agents(PLAYER_GROUPS)
 
 
 class OneNeuralCorridorConfig(BaseCorridorConfig):
     PLAYER_GROUPS = create_group_config(agents=[Agent, CorridorAgent])
     AGENTS = process_agents(PLAYER_GROUPS)
 
 
+@dataclass
 class CorridorConfig(BaseCorridorConfig):
     PLAYER_GROUPS = create_group_config(agents=[Agent, Agent])
     AGENTS = process_agents(PLAYER_GROUPS)
```

### Comparing `marlben-1.0.0/marlben/envs/corridor/env.py` & `marlben-1.0.1/marlben/envs/corridor/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/deathmatch/config.py` & `marlben-1.0.1/marlben/envs/deathmatch/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/deathmatch/env.py` & `marlben-1.0.1/marlben/envs/deathmatch/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/exploring/config.py` & `marlben-1.0.1/marlben/envs/exploring/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/exploring/env.py` & `marlben-1.0.1/marlben/envs/exploring/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/gathering/config.py` & `marlben-1.0.1/marlben/envs/gathering/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/gathering/env.py` & `marlben-1.0.1/marlben/envs/gathering/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/gathering/utils/map_generator.py` & `marlben-1.0.1/marlben/envs/gathering/utils/map_generator.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/planting/config.py` & `marlben-1.0.1/marlben/envs/planting/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/planting/env.py` & `marlben-1.0.1/marlben/envs/planting/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/predator_prey/config.py` & `marlben-1.0.1/marlben/envs/predator_prey/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/predator_prey/env.py` & `marlben-1.0.1/marlben/envs/predator_prey/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/pve/config.py` & `marlben-1.0.1/marlben/envs/pve/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/pve/env.py` & `marlben-1.0.1/marlben/envs/pve/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/raid/config.py` & `marlben-1.0.1/marlben/envs/raid/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/raid/env.py` & `marlben-1.0.1/marlben/envs/raid/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/siege/config.py` & `marlben-1.0.1/marlben/envs/siege/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/siege/env.py` & `marlben-1.0.1/marlben/envs/siege/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/spying/config.py` & `marlben-1.0.1/marlben/envs/spying/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/spying/env.py` & `marlben-1.0.1/marlben/envs/spying/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/team_deathmatch/config.py` & `marlben-1.0.1/marlben/envs/team_deathmatch/config.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/envs/team_deathmatch/env.py` & `marlben-1.0.1/marlben/envs/team_deathmatch/env.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/infrastructure.py` & `marlben-1.0.1/marlben/infrastructure.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/io/action/attack.py` & `marlben-1.0.1/marlben/io/action/attack.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,14 @@
 class Target(Node):
     argType = None
 
     # argType = int
 
     @classmethod
     def N(cls, config):
-        # return config.WINDOW ** 2
         return config.N_AGENT_OBS
 
     def args(stim, entity, config):
         # Should pass max range?
         return inRange(entity, stim, config, None)
 
     @staticproperty
```

### Comparing `marlben-1.0.0/marlben/io/action/base_action.py` & `marlben-1.0.1/marlben/io/action/base_action.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/io/action/build.py` & `marlben-1.0.1/marlben/io/action/build.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/io/action/common.py` & `marlben-1.0.1/marlben/io/action/common.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/io/action/move.py` & `marlben-1.0.1/marlben/io/action/move.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/io/action/plant.py` & `marlben-1.0.1/marlben/io/action/plant.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/io/action/share.py` & `marlben-1.0.1/marlben/io/action/share.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
 
 class ResourceAmount(Node):
     argType = int
 
     @classmethod
     def N(cls, config):
-        # return config.WINDOW ** 2
         return config.N_AGENT_OBS
 
     def args(stim, entity, config):
         # Should pass max range?
         return list(range(config.SHARE_MIN, config.SHARE_MAX + 1))
 
     @staticproperty
```

### Comparing `marlben-1.0.0/marlben/io/stimulus.py` & `marlben-1.0.1/marlben/io/stimulus.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
                 self.val = 0
                 self.max = 3
                 self.scale = 0.3
 
     class Tile(metaclass=utils.IterableNameComparable):
         @staticmethod
         def N(config):
-            return config.WINDOW**2
+            return config.WINDOW()**2
 
         class NEnts(Continuous):
             def init(self, config):
                 self.max = config.NENT
                 self.val = 0
                 self.scale = 1.0
```

### Comparing `marlben-1.0.0/marlben/lib/colors.py` & `marlben-1.0.1/marlben/lib/colors.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/lib/distance.py` & `marlben-1.0.1/marlben/lib/distance.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/lib/log.py` & `marlben-1.0.1/marlben/lib/log.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/lib/material.py` & `marlben-1.0.1/marlben/lib/material.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/lib/overlay.py` & `marlben-1.0.1/marlben/lib/overlay.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/lib/priorityqueue.py` & `marlben-1.0.1/marlben/lib/priorityqueue.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/lib/rating.py` & `marlben-1.0.1/marlben/lib/rating.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/lib/utils.py` & `marlben-1.0.1/marlben/lib/utils.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/overlay.py` & `marlben-1.0.1/marlben/overlay.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/scripting.py` & `marlben-1.0.1/marlben/scripting.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         Args:
          rDelta: row offset from current agent
          cDelta: col offset from current agent
 
         Returns:
          Vector corresponding to the specified tile
         """
-        return self.tiles[self.config.WINDOW * (self.delta + rDelta) + self.delta + cDelta]
+        return self.tiles[self.config.WINDOW() * (self.delta + rDelta) + self.delta + cDelta]
 
     @property
     def agent(self):
         """Return the array object corresponding to the current agent"""
         return self.agents[0]
 
     @staticmethod
```

### Comparing `marlben-1.0.0/marlben/systems/achievement.py` & `marlben-1.0.1/marlben/systems/achievement.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/systems/ai/behavior.py` & `marlben-1.0.1/marlben/systems/ai/behavior.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/systems/ai/dynamic_programming.py` & `marlben-1.0.1/marlben/systems/ai/dynamic_programming.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/systems/ai/move.py` & `marlben-1.0.1/marlben/systems/ai/move.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/systems/ai/policy.py` & `marlben-1.0.1/marlben/systems/ai/policy.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/systems/ai/utils.py` & `marlben-1.0.1/marlben/systems/ai/utils.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/systems/combat.py` & `marlben-1.0.1/marlben/systems/combat.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/systems/droptable.py` & `marlben-1.0.1/marlben/systems/droptable.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/systems/equipment.py` & `marlben-1.0.1/marlben/systems/equipment.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/systems/experience.py` & `marlben-1.0.1/marlben/systems/experience.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/systems/skill.py` & `marlben-1.0.1/marlben/systems/skill.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben/websocket.py` & `marlben-1.0.1/marlben/websocket.py`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/marlben.egg-info/PKG-INFO` & `marlben-1.0.1/marlben.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marlben
-Version: 1.0.0
+Version: 1.0.1
 Summary: Marlben is a multi-agent reinforcement learning benchmark based on the NeuralMMO game engine.
 Author-email: JBR AI labs <ego.vladi@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/jbr-ai-labs/marlben
 Project-URL: Repository, https://github.com/jbr-ai-labs/marlben
 Project-URL: Documentation, https://github.com/jbr-ai-labs/marlben/wiki
 Project-URL: Bug Report, https://github.com/jbr-ai-labs/marlben/issues
```

### Comparing `marlben-1.0.0/marlben.egg-info/SOURCES.txt` & `marlben-1.0.1/marlben.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marlben-1.0.0/pyproject.toml` & `marlben-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -29,22 +29,22 @@
     "scipy~=1.8.0",
     "imageio~=2.8.0",
     "Twisted~=19.2.0",
     "autobahn~=19.3.3",
     "vec_noise~=1.1.4",
     "matplotlib >=3.0",
     "openskill~=4.0.0",
-    "gymnasium~=0.28.1"
+    "gymnasium>=0.26.3"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-rllib = ["ray[rllib]~=1.5.2", "torch==1.11.0", "wandb~=0.15.4"]
+rllib = ["ray[rllib]~=2.5.0", "torch==1.13.1", "wandb~=0.15.4"]
 all = [
-    "ray[rllib]~=1.5.2", "torch==1.11.0", "wandb~=0.15.4"
+    "ray[rllib]~=2.5.0", "torch==1.13.1", "wandb~=0.15.4"
 ]
 testing = [
     "pytest ==7.1.1"
 ]
 
 [project.urls]
 Homepage = "https://github.com/jbr-ai-labs/marlben"
```

### Comparing `marlben-1.0.0/setup.py` & `marlben-1.0.1/setup.py`

 * *Files identical despite different names*

