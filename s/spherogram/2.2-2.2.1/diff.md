# Comparing `tmp/spherogram-2.2.tar.gz` & `tmp/spherogram-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spherogram-2.2.tar", last modified: Tue May 23 20:01:39 2023, max compression
+gzip compressed data, was "spherogram-2.2.1.tar", last modified: Sun Jun 11 20:27:27 2023, max compression
```

## Comparing `spherogram-2.2.tar` & `spherogram-2.2.1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.922453 spherogram-2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-23 20:01:24.000000 spherogram-2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-23 20:01:39.918453 spherogram-2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-23 20:01:24.000000 spherogram-2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.906452 spherogram-2.2/dev/
--rw-r--r--   0 runner    (1001) docker     (123)    31967 2023-05-23 20:01:24.000000 spherogram-2.2/dev/DTcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 20:01:24.000000 spherogram-2.2/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-23 20:01:24.000000 spherogram-2.2/dev/conventions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.906452 spherogram-2.2/dev/dev_jennet/
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-23 20:01:24.000000 spherogram-2.2/dev/dev_jennet/AlexanderKauffman.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 20:01:24.000000 spherogram-2.2/dev/dev_jennet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-23 20:01:24.000000 spherogram-2.2/dev/dev_jennet/bridge_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-23 20:01:24.000000 spherogram-2.2/dev/dev_jennet/spanning_trees.py
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-05-23 20:01:24.000000 spherogram-2.2/dev/dev_jennet/test_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-23 20:01:24.000000 spherogram-2.2/dev/dt_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-23 20:01:24.000000 spherogram-2.2/dev/dt_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-23 20:01:24.000000 spherogram-2.2/dev/hard_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-23 20:01:24.000000 spherogram-2.2/dev/issue_35.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-23 20:01:24.000000 spherogram-2.2/dev/other_link_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-23 20:01:24.000000 spherogram-2.2/dev/sage_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-23 20:01:24.000000 spherogram-2.2/dev/sage_link_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-23 20:01:24.000000 spherogram-2.2/dev/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    21769 2023-05-23 20:01:24.000000 spherogram-2.2/dev/tangle_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.906452 spherogram-2.2/planarity_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.914452 spherogram-2.2/planarity_src/c/
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/appconst.h
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graph.h
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphColorVertices.c
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphColorVertices.h
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphColorVertices.private.h
--rw-r--r--   0 runner    (1001) docker     (123)    23963 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphColorVertices_Extensions.c
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphDFSUtils.c
--rw-r--r--   0 runner    (1001) docker     (123)    43741 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphDrawPlanar.c
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphDrawPlanar.h
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphDrawPlanar.private.h
--rw-r--r--   0 runner    (1001) docker     (123)    27468 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphDrawPlanar_Extensions.c
--rw-r--r--   0 runner    (1001) docker     (123)    63389 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphEmbed.c
--rw-r--r--   0 runner    (1001) docker     (123)    23976 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphExtensions.c
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphExtensions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphExtensions.private.h
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphFunctionTable.h
--rw-r--r--   0 runner    (1001) docker     (123)    28630 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphIO.c
--rw-r--r--   0 runner    (1001) docker     (123)    32754 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphIsolator.c
--rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK23Search.c
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK23Search.h
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK23Search.private.h
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK23Search_Extensions.c
--rw-r--r--   0 runner    (1001) docker     (123)    84775 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK33Search.c
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK33Search.h
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK33Search.private.h
--rw-r--r--   0 runner    (1001) docker     (123)    29971 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK33Search_Extensions.c
--rw-r--r--   0 runner    (1001) docker     (123)    60582 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK4Search.c
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK4Search.h
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK4Search.private.h
--rw-r--r--   0 runner    (1001) docker     (123)    19913 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphK4Search_Extensions.c
--rw-r--r--   0 runner    (1001) docker     (123)    31173 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphNonplanar.c
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphOuterplanarObstruction.c
--rw-r--r--   0 runner    (1001) docker     (123)    38887 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphStructures.h
--rw-r--r--   0 runner    (1001) docker     (123)    39125 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphTests.c
--rw-r--r--   0 runner    (1001) docker     (123)    91710 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/graphUtils.c
--rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/listcoll.c
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/listcoll.h
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/planarity.h
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/platformTime.h
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/stack.c
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/c/stack.h
--rw-r--r--   0 runner    (1001) docker     (123)   158817 2023-05-23 20:01:25.000000 spherogram-2.2/planarity_src/planarity.c
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-23 20:01:24.000000 spherogram-2.2/planarity_src/planarity.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.914452 spherogram-2.2/planarmap_src/
--rw-r--r--   0 runner    (1001) docker     (123)   174385 2023-05-23 20:01:25.000000 spherogram-2.2/planarmap_src/planarmap.c
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/planarmap.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.914452 spherogram-2.2/planarmap_src/src/
--rw-r--r--   0 runner    (1001) docker     (123)    15553 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMconjugation.c
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMconjugation.h
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMdef.c
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMdef.h
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMdisplay.h
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMenlight.c
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMenlight.h
--rw-r--r--   0 runner    (1001) docker     (123)    15985 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMextract.c
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMextract.h
--rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMplanmap.c
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/PMplanmap.h
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/interface.h
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/stats.c
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-23 20:01:24.000000 spherogram-2.2/planarmap_src/src/stats.h
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-23 20:01:24.000000 spherogram-2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:01:39.922453 spherogram-2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-05-23 20:01:24.000000 spherogram-2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.914452 spherogram-2.2/spherogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-23 20:01:39.000000 spherogram-2.2/spherogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-23 20:01:39.000000 spherogram-2.2/spherogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:01:39.000000 spherogram-2.2/spherogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:01:39.000000 spherogram-2.2/spherogram.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-23 20:01:39.000000 spherogram-2.2/spherogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 20:01:39.000000 spherogram-2.2/spherogram.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.918453 spherogram-2.2/spherogram_src/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.918453 spherogram-2.2/spherogram_src/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/codecs/Base64LikeDT.py
--rw-r--r--   0 runner    (1001) docker     (123)    35378 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/codecs/DT.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38410 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.918453 spherogram-2.2/spherogram_src/links/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/alexander.py
--rw-r--r--   0 runner    (1001) docker     (123)   100850 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/doc.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/exhaust.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/extra_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    29484 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/jones.py
--rw-r--r--   0 runner    (1001) docker     (123)     9225 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/jones_old.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/links.py
--rw-r--r--   0 runner    (1001) docker     (123)    55123 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/links_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/morse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/ordered_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    26248 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/orthogonal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/planar_isotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/random_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    13120 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/seifert.py
--rw-r--r--   0 runner    (1001) docker     (123)    24336 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)    24252 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/tangles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:01:39.918453 spherogram-2.2/spherogram_src/links/test/
--rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/test/old_testing_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/test/test_montesinos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/torus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/links/twist.py
--rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/presentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/sage_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 20:01:24.000000 spherogram-2.2/spherogram_src/version.py
+drwxr-xr-x   0 nmd        (502) staff       (20)        0 2023-06-11 20:27:27.870024 spherogram-2.2.1/
+-rw-r--r--   0 nmd        (502) staff       (20)      130 2023-05-23 20:07:53.000000 spherogram-2.2.1/MANIFEST.in
+-rw-r--r--   0 nmd        (502) staff       (20)     1136 2023-06-11 20:27:27.869565 spherogram-2.2.1/PKG-INFO
+-rw-r--r--   0 nmd        (502) staff       (20)     1229 2022-03-30 20:14:18.000000 spherogram-2.2.1/README.rst
+drwxr-xr-x   0 nmd        (502) staff       (20)        0 2023-06-11 20:27:27.833828 spherogram-2.2.1/dev/
+-rw-r--r--   0 nmd        (502) staff       (20)    31967 2022-11-20 22:57:34.000000 spherogram-2.2.1/dev/DTcodes.py
+-rw-r--r--   0 nmd        (502) staff       (20)        5 2020-01-04 03:23:39.000000 spherogram-2.2.1/dev/__init__.py
+-rw-r--r--   0 nmd        (502) staff       (20)     1989 2022-11-01 01:12:35.000000 spherogram-2.2.1/dev/conventions.py
+drwxr-xr-x   0 nmd        (502) staff       (20)        0 2023-06-11 20:27:27.835307 spherogram-2.2.1/dev/dev_jennet/
+-rw-r--r--   0 nmd        (502) staff       (20)     2923 2022-11-01 01:12:35.000000 spherogram-2.2.1/dev/dev_jennet/AlexanderKauffman.py
+-rw-r--r--   0 nmd        (502) staff       (20)       33 2022-11-01 01:12:35.000000 spherogram-2.2.1/dev/dev_jennet/__init__.py
+-rw-r--r--   0 nmd        (502) staff       (20)     1458 2022-11-01 01:12:35.000000 spherogram-2.2.1/dev/dev_jennet/bridge_finding.py
+-rw-r--r--   0 nmd        (502) staff       (20)     2093 2022-11-20 22:57:34.000000 spherogram-2.2.1/dev/dev_jennet/spanning_trees.py
+-rw-r--r--   0 nmd        (502) staff       (20)    10695 2022-11-01 01:12:35.000000 spherogram-2.2.1/dev/dev_jennet/test_links.py
+-rw-r--r--   0 nmd        (502) staff       (20)     1864 2022-11-01 01:12:35.000000 spherogram-2.2.1/dev/dt_issue.py
+-rw-r--r--   0 nmd        (502) staff       (20)     1557 2022-06-27 18:19:33.000000 spherogram-2.2.1/dev/dt_tests.py
+-rw-r--r--   0 nmd        (502) staff       (20)    10541 2022-11-20 22:57:34.000000 spherogram-2.2.1/dev/hard_links.py
+-rw-r--r--   0 nmd        (502) staff       (20)     1823 2022-11-20 22:57:34.000000 spherogram-2.2.1/dev/issue_35.py
+-rw-r--r--   0 nmd        (502) staff       (20)     2286 2022-11-20 22:57:34.000000 spherogram-2.2.1/dev/other_link_formats.py
+-rw-r--r--   0 nmd        (502) staff       (20)      480 2022-06-27 18:19:33.000000 spherogram-2.2.1/dev/sage_graph.py
+-rw-r--r--   0 nmd        (502) staff       (20)     1560 2022-11-20 22:57:34.000000 spherogram-2.2.1/dev/sage_link_compare.py
+-rw-r--r--   0 nmd        (502) staff       (20)     4434 2022-11-20 22:57:34.000000 spherogram-2.2.1/dev/signature.py
+-rw-r--r--   0 nmd        (502) staff       (20)    21769 2022-11-20 22:57:34.000000 spherogram-2.2.1/dev/tangle_patch.py
+drwxr-xr-x   0 nmd        (502) staff       (20)        0 2023-06-11 20:27:27.836066 spherogram-2.2.1/planarity_src/
+drwxr-xr-x   0 nmd        (502) staff       (20)        0 2023-06-11 20:27:27.849219 spherogram-2.2.1/planarity_src/c/
+-rw-r--r--   0 nmd        (502) staff       (20)     4491 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/appconst.h
+-rw-r--r--   0 nmd        (502) staff       (20)     6676 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graph.h
+-rw-r--r--   0 nmd        (502) staff       (20)    16505 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphColorVertices.c
+-rw-r--r--   0 nmd        (502) staff       (20)     3053 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphColorVertices.h
+-rw-r--r--   0 nmd        (502) staff       (20)     3414 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphColorVertices.private.h
+-rw-r--r--   0 nmd        (502) staff       (20)    23963 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphColorVertices_Extensions.c
+-rw-r--r--   0 nmd        (502) staff       (20)    18687 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphDFSUtils.c
+-rw-r--r--   0 nmd        (502) staff       (20)    43741 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphDrawPlanar.c
+-rw-r--r--   0 nmd        (502) staff       (20)     2956 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphDrawPlanar.h
+-rw-r--r--   0 nmd        (502) staff       (20)     5452 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphDrawPlanar.private.h
+-rw-r--r--   0 nmd        (502) staff       (20)    27468 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphDrawPlanar_Extensions.c
+-rw-r--r--   0 nmd        (502) staff       (20)    63389 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphEmbed.c
+-rw-r--r--   0 nmd        (502) staff       (20)    23976 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphExtensions.c
+-rw-r--r--   0 nmd        (502) staff       (20)     3319 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphExtensions.h
+-rw-r--r--   0 nmd        (502) staff       (20)     3044 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphExtensions.private.h
+-rw-r--r--   0 nmd        (502) staff       (20)     4229 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphFunctionTable.h
+-rw-r--r--   0 nmd        (502) staff       (20)    28630 2022-03-30 20:14:18.000000 spherogram-2.2.1/planarity_src/c/graphIO.c
+-rw-r--r--   0 nmd        (502) staff       (20)    32754 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphIsolator.c
+-rw-r--r--   0 nmd        (502) staff       (20)    11995 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphK23Search.c
+-rw-r--r--   0 nmd        (502) staff       (20)     2874 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphK23Search.h
+-rw-r--r--   0 nmd        (502) staff       (20)     2872 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphK23Search.private.h
+-rw-r--r--   0 nmd        (502) staff       (20)    11194 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphK23Search_Extensions.c
+-rw-r--r--   0 nmd        (502) staff       (20)    84775 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphK33Search.c
+-rw-r--r--   0 nmd        (502) staff       (20)     2874 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphK33Search.h
+-rw-r--r--   0 nmd        (502) staff       (20)     3805 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphK33Search.private.h
+-rw-r--r--   0 nmd        (502) staff       (20)    29971 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphK33Search_Extensions.c
+-rw-r--r--   0 nmd        (502) staff       (20)    60582 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphK4Search.c
+-rw-r--r--   0 nmd        (502) staff       (20)     2868 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphK4Search.h
+-rw-r--r--   0 nmd        (502) staff       (20)     3971 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphK4Search.private.h
+-rw-r--r--   0 nmd        (502) staff       (20)    19913 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphK4Search_Extensions.c
+-rw-r--r--   0 nmd        (502) staff       (20)    31173 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphNonplanar.c
+-rw-r--r--   0 nmd        (502) staff       (20)     9689 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphOuterplanarObstruction.c
+-rw-r--r--   0 nmd        (502) staff       (20)    38887 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphStructures.h
+-rw-r--r--   0 nmd        (502) staff       (20)    39125 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphTests.c
+-rw-r--r--   0 nmd        (502) staff       (20)    91710 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/graphUtils.c
+-rw-r--r--   0 nmd        (502) staff       (20)    11972 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/listcoll.c
+-rw-r--r--   0 nmd        (502) staff       (20)     6683 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/listcoll.h
+-rw-r--r--   0 nmd        (502) staff       (20)     4383 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/planarity.h
+-rw-r--r--   0 nmd        (502) staff       (20)     3996 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/platformTime.h
+-rw-r--r--   0 nmd        (502) staff       (20)     6293 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/stack.c
+-rw-r--r--   0 nmd        (502) staff       (20)     4685 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarity_src/c/stack.h
+-rw-r--r--   0 nmd        (502) staff       (20)   159020 2023-06-11 20:20:54.000000 spherogram-2.2.1/planarity_src/planarity.c
+-rw-r--r--   0 nmd        (502) staff       (20)     2239 2022-03-30 20:14:18.000000 spherogram-2.2.1/planarity_src/planarity.pyx
+drwxr-xr-x   0 nmd        (502) staff       (20)        0 2023-06-11 20:27:27.849982 spherogram-2.2.1/planarmap_src/
+-rw-r--r--   0 nmd        (502) staff       (20)   174603 2023-06-11 20:27:27.000000 spherogram-2.2.1/planarmap_src/planarmap.c
+-rw-r--r--   0 nmd        (502) staff       (20)     3808 2023-06-11 20:20:31.000000 spherogram-2.2.1/planarmap_src/planarmap.pyx
+drwxr-xr-x   0 nmd        (502) staff       (20)        0 2023-06-11 20:27:27.853860 spherogram-2.2.1/planarmap_src/src/
+-rw-r--r--   0 nmd        (502) staff       (20)    15553 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarmap_src/src/PMconjugation.c
+-rw-r--r--   0 nmd        (502) staff       (20)      601 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarmap_src/src/PMconjugation.h
+-rw-r--r--   0 nmd        (502) staff       (20)     5688 2022-03-30 20:14:18.000000 spherogram-2.2.1/planarmap_src/src/PMdef.c
+-rw-r--r--   0 nmd        (502) staff       (20)     4414 2022-03-30 20:14:18.000000 spherogram-2.2.1/planarmap_src/src/PMdef.h
+-rw-r--r--   0 nmd        (502) staff       (20)       50 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarmap_src/src/PMdisplay.h
+-rw-r--r--   0 nmd        (502) staff       (20)     6519 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarmap_src/src/PMenlight.c
+-rw-r--r--   0 nmd        (502) staff       (20)      445 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarmap_src/src/PMenlight.h
+-rw-r--r--   0 nmd        (502) staff       (20)    15985 2022-03-30 20:14:18.000000 spherogram-2.2.1/planarmap_src/src/PMextract.c
+-rw-r--r--   0 nmd        (502) staff       (20)      977 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarmap_src/src/PMextract.h
+-rw-r--r--   0 nmd        (502) staff       (20)    12608 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarmap_src/src/PMplanmap.c
+-rw-r--r--   0 nmd        (502) staff       (20)      316 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarmap_src/src/PMplanmap.h
+-rw-r--r--   0 nmd        (502) staff       (20)      110 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarmap_src/src/interface.h
+-rw-r--r--   0 nmd        (502) staff       (20)     6579 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarmap_src/src/stats.c
+-rw-r--r--   0 nmd        (502) staff       (20)      185 2020-01-04 03:23:39.000000 spherogram-2.2.1/planarmap_src/src/stats.h
+-rw-r--r--   0 nmd        (502) staff       (20)       99 2023-06-11 19:58:02.000000 spherogram-2.2.1/pyproject.toml
+-rw-r--r--   0 nmd        (502) staff       (20)       38 2023-06-11 20:27:27.870181 spherogram-2.2.1/setup.cfg
+-rw-r--r--   0 nmd        (502) staff       (20)     8389 2023-05-23 20:10:00.000000 spherogram-2.2.1/setup.py
+drwxr-xr-x   0 nmd        (502) staff       (20)        0 2023-06-11 20:27:27.855502 spherogram-2.2.1/spherogram.egg-info/
+-rw-r--r--   0 nmd        (502) staff       (20)     1136 2023-06-11 20:27:27.000000 spherogram-2.2.1/spherogram.egg-info/PKG-INFO
+-rw-r--r--   0 nmd        (502) staff       (20)     3687 2023-06-11 20:27:27.000000 spherogram-2.2.1/spherogram.egg-info/SOURCES.txt
+-rw-r--r--   0 nmd        (502) staff       (20)        1 2023-06-11 20:27:27.000000 spherogram-2.2.1/spherogram.egg-info/dependency_links.txt
+-rw-r--r--   0 nmd        (502) staff       (20)        1 2023-06-11 20:20:54.000000 spherogram-2.2.1/spherogram.egg-info/not-zip-safe
+-rw-r--r--   0 nmd        (502) staff       (20)       68 2023-06-11 20:27:27.000000 spherogram-2.2.1/spherogram.egg-info/requires.txt
+-rw-r--r--   0 nmd        (502) staff       (20)       11 2023-06-11 20:27:27.000000 spherogram-2.2.1/spherogram.egg-info/top_level.txt
+drwxr-xr-x   0 nmd        (502) staff       (20)        0 2023-06-11 20:27:27.857602 spherogram-2.2.1/spherogram_src/
+-rw-r--r--   0 nmd        (502) staff       (20)      911 2022-11-07 14:22:24.000000 spherogram-2.2.1/spherogram_src/__init__.py
+drwxr-xr-x   0 nmd        (502) staff       (20)        0 2023-06-11 20:27:27.858569 spherogram-2.2.1/spherogram_src/codecs/
+-rw-r--r--   0 nmd        (502) staff       (20)     7395 2023-04-01 21:43:20.000000 spherogram-2.2.1/spherogram_src/codecs/Base64LikeDT.py
+-rw-r--r--   0 nmd        (502) staff       (20)    35378 2023-04-01 21:43:20.000000 spherogram-2.2.1/spherogram_src/codecs/DT.py
+-rw-r--r--   0 nmd        (502) staff       (20)       46 2022-03-31 22:17:24.000000 spherogram-2.2.1/spherogram_src/codecs/__init__.py
+-rw-r--r--   0 nmd        (502) staff       (20)    38410 2023-04-01 21:43:20.000000 spherogram-2.2.1/spherogram_src/graphs.py
+drwxr-xr-x   0 nmd        (502) staff       (20)        0 2023-06-11 20:27:27.867259 spherogram-2.2.1/spherogram_src/links/
+-rw-r--r--   0 nmd        (502) staff       (20)     1005 2022-11-07 14:22:24.000000 spherogram-2.2.1/spherogram_src/links/__init__.py
+-rw-r--r--   0 nmd        (502) staff       (20)     8221 2022-05-02 02:20:22.000000 spherogram-2.2.1/spherogram_src/links/alexander.py
+-rw-r--r--   0 nmd        (502) staff       (20)   100850 2022-03-30 20:14:18.000000 spherogram-2.2.1/spherogram_src/links/doc.pdf
+-rw-r--r--   0 nmd        (502) staff       (20)     1744 2022-03-30 20:14:18.000000 spherogram-2.2.1/spherogram_src/links/draw.py
+-rw-r--r--   0 nmd        (502) staff       (20)    15414 2023-05-10 21:18:59.000000 spherogram-2.2.1/spherogram_src/links/exhaust.py
+-rw-r--r--   0 nmd        (502) staff       (20)     3629 2023-04-01 21:43:20.000000 spherogram-2.2.1/spherogram_src/links/extra_tests.py
+-rw-r--r--   0 nmd        (502) staff       (20)    29567 2023-06-11 18:05:25.000000 spherogram-2.2.1/spherogram_src/links/invariants.py
+-rw-r--r--   0 nmd        (502) staff       (20)     6554 2023-05-10 21:56:53.000000 spherogram-2.2.1/spherogram_src/links/jones.py
+-rw-r--r--   0 nmd        (502) staff       (20)     9225 2023-05-10 21:03:23.000000 spherogram-2.2.1/spherogram_src/links/jones_old.py
+-rw-r--r--   0 nmd        (502) staff       (20)      119 2022-03-31 22:17:24.000000 spherogram-2.2.1/spherogram_src/links/links.py
+-rw-r--r--   0 nmd        (502) staff       (20)    55123 2023-04-01 21:43:20.000000 spherogram-2.2.1/spherogram_src/links/links_base.py
+-rw-r--r--   0 nmd        (502) staff       (20)    14648 2023-04-01 21:43:20.000000 spherogram-2.2.1/spherogram_src/links/morse.py
+-rw-r--r--   0 nmd        (502) staff       (20)     1467 2022-10-09 02:22:01.000000 spherogram-2.2.1/spherogram_src/links/ordered_set.py
+-rw-r--r--   0 nmd        (502) staff       (20)    26248 2023-05-10 21:03:23.000000 spherogram-2.2.1/spherogram_src/links/orthogonal.py
+-rw-r--r--   0 nmd        (502) staff       (20)    11143 2022-11-20 22:57:34.000000 spherogram-2.2.1/spherogram_src/links/planar_isotopy.py
+-rw-r--r--   0 nmd        (502) staff       (20)     8294 2022-10-09 02:22:01.000000 spherogram-2.2.1/spherogram_src/links/random_links.py
+-rw-r--r--   0 nmd        (502) staff       (20)    13120 2022-05-02 02:20:22.000000 spherogram-2.2.1/spherogram_src/links/seifert.py
+-rw-r--r--   0 nmd        (502) staff       (20)    24336 2023-05-10 21:03:23.000000 spherogram-2.2.1/spherogram_src/links/simplify.py
+-rw-r--r--   0 nmd        (502) staff       (20)    24252 2023-05-10 21:03:23.000000 spherogram-2.2.1/spherogram_src/links/tangles.py
+drwxr-xr-x   0 nmd        (502) staff       (20)        0 2023-06-11 20:27:27.868884 spherogram-2.2.1/spherogram_src/links/test/
+-rw-r--r--   0 nmd        (502) staff       (20)    12155 2023-05-10 21:03:23.000000 spherogram-2.2.1/spherogram_src/links/test/__init__.py
+-rw-r--r--   0 nmd        (502) staff       (20)     3629 2023-04-01 21:43:20.000000 spherogram-2.2.1/spherogram_src/links/test/old_testing_code.py
+-rw-r--r--   0 nmd        (502) staff       (20)     5784 2022-03-31 22:17:25.000000 spherogram-2.2.1/spherogram_src/links/test/test_montesinos.py
+-rw-r--r--   0 nmd        (502) staff       (20)     2413 2023-05-10 21:03:23.000000 spherogram-2.2.1/spherogram_src/links/torus.py
+-rw-r--r--   0 nmd        (502) staff       (20)     2727 2022-03-31 22:17:25.000000 spherogram-2.2.1/spherogram_src/links/twist.py
+-rw-r--r--   0 nmd        (502) staff       (20)    18436 2023-04-01 21:43:20.000000 spherogram-2.2.1/spherogram_src/presentations.py
+-rw-r--r--   0 nmd        (502) staff       (20)     1157 2023-05-23 13:11:57.000000 spherogram-2.2.1/spherogram_src/sage_helper.py
+-rw-r--r--   0 nmd        (502) staff       (20)     1452 2023-05-09 19:56:04.000000 spherogram-2.2.1/spherogram_src/test.py
+-rw-r--r--   0 nmd        (502) staff       (20)     3084 2022-03-31 22:17:25.000000 spherogram-2.2.1/spherogram_src/test_helper.py
+-rw-r--r--   0 nmd        (502) staff       (20)       18 2023-06-11 18:00:46.000000 spherogram-2.2.1/spherogram_src/version.py
```

### Comparing `spherogram-2.2/PKG-INFO` & `spherogram-2.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spherogram
-Version: 2.2
+Version: 2.2.1
 Summary: Spherical diagrams for 3-manifold topology
 Home-page: https://github.com/3-manifolds/Spherogram
 Author: Marc Culler and Nathan M. Dunfield
 Author-email: culler@marc-culler.info, nathan@dunfield.info
 License: GPLv2+
 Keywords: knot,link,SnapPy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spherogram-2.2/README.rst` & `spherogram-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/dev/DTcodes.py` & `spherogram-2.2.1/dev/DTcodes.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/dev/conventions.py` & `spherogram-2.2.1/dev/conventions.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/dev/dev_jennet/AlexanderKauffman.py` & `spherogram-2.2.1/dev/dev_jennet/AlexanderKauffman.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/dev/dev_jennet/bridge_finding.py` & `spherogram-2.2.1/dev/dev_jennet/bridge_finding.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/dev/dev_jennet/spanning_trees.py` & `spherogram-2.2.1/dev/dev_jennet/spanning_trees.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/dev/dev_jennet/test_links.py` & `spherogram-2.2.1/dev/dev_jennet/test_links.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/dev/dt_issue.py` & `spherogram-2.2.1/dev/dt_issue.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/dev/dt_tests.py` & `spherogram-2.2.1/dev/dt_tests.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/dev/hard_links.py` & `spherogram-2.2.1/dev/hard_links.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/dev/issue_35.py` & `spherogram-2.2.1/dev/issue_35.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/dev/other_link_formats.py` & `spherogram-2.2.1/dev/other_link_formats.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/dev/sage_link_compare.py` & `spherogram-2.2.1/dev/sage_link_compare.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/dev/signature.py` & `spherogram-2.2.1/dev/signature.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/dev/tangle_patch.py` & `spherogram-2.2.1/dev/tangle_patch.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/appconst.h` & `spherogram-2.2.1/planarity_src/c/appconst.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graph.h` & `spherogram-2.2.1/planarity_src/c/graph.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphColorVertices.c` & `spherogram-2.2.1/planarity_src/c/graphColorVertices.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphColorVertices.h` & `spherogram-2.2.1/planarity_src/c/graphColorVertices.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphColorVertices.private.h` & `spherogram-2.2.1/planarity_src/c/graphColorVertices.private.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphColorVertices_Extensions.c` & `spherogram-2.2.1/planarity_src/c/graphColorVertices_Extensions.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphDFSUtils.c` & `spherogram-2.2.1/planarity_src/c/graphDFSUtils.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphDrawPlanar.c` & `spherogram-2.2.1/planarity_src/c/graphDrawPlanar.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphDrawPlanar.h` & `spherogram-2.2.1/planarity_src/c/graphDrawPlanar.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphDrawPlanar.private.h` & `spherogram-2.2.1/planarity_src/c/graphDrawPlanar.private.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphDrawPlanar_Extensions.c` & `spherogram-2.2.1/planarity_src/c/graphDrawPlanar_Extensions.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphEmbed.c` & `spherogram-2.2.1/planarity_src/c/graphEmbed.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphExtensions.c` & `spherogram-2.2.1/planarity_src/c/graphExtensions.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphExtensions.h` & `spherogram-2.2.1/planarity_src/c/graphExtensions.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphExtensions.private.h` & `spherogram-2.2.1/planarity_src/c/graphExtensions.private.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphFunctionTable.h` & `spherogram-2.2.1/planarity_src/c/graphFunctionTable.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphIO.c` & `spherogram-2.2.1/planarity_src/c/graphIO.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphIsolator.c` & `spherogram-2.2.1/planarity_src/c/graphIsolator.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphK23Search.c` & `spherogram-2.2.1/planarity_src/c/graphK23Search.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphK23Search.h` & `spherogram-2.2.1/planarity_src/c/graphK23Search.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphK23Search.private.h` & `spherogram-2.2.1/planarity_src/c/graphK23Search.private.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphK23Search_Extensions.c` & `spherogram-2.2.1/planarity_src/c/graphK23Search_Extensions.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphK33Search.c` & `spherogram-2.2.1/planarity_src/c/graphK33Search.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphK33Search.h` & `spherogram-2.2.1/planarity_src/c/graphK33Search.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphK33Search.private.h` & `spherogram-2.2.1/planarity_src/c/graphK33Search.private.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphK33Search_Extensions.c` & `spherogram-2.2.1/planarity_src/c/graphK33Search_Extensions.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphK4Search.c` & `spherogram-2.2.1/planarity_src/c/graphK4Search.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphK4Search.h` & `spherogram-2.2.1/planarity_src/c/graphK4Search.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphK4Search.private.h` & `spherogram-2.2.1/planarity_src/c/graphK4Search.private.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphK4Search_Extensions.c` & `spherogram-2.2.1/planarity_src/c/graphK4Search_Extensions.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphNonplanar.c` & `spherogram-2.2.1/planarity_src/c/graphNonplanar.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphOuterplanarObstruction.c` & `spherogram-2.2.1/planarity_src/c/graphOuterplanarObstruction.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphStructures.h` & `spherogram-2.2.1/planarity_src/c/graphStructures.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphTests.c` & `spherogram-2.2.1/planarity_src/c/graphTests.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/graphUtils.c` & `spherogram-2.2.1/planarity_src/c/graphUtils.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/listcoll.c` & `spherogram-2.2.1/planarity_src/c/listcoll.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/listcoll.h` & `spherogram-2.2.1/planarity_src/c/listcoll.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/planarity.h` & `spherogram-2.2.1/planarity_src/c/planarity.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/platformTime.h` & `spherogram-2.2.1/planarity_src/c/platformTime.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/stack.c` & `spherogram-2.2.1/planarity_src/c/stack.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/c/stack.h` & `spherogram-2.2.1/planarity_src/c/stack.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarity_src/planarity.c` & `spherogram-2.2.1/planarity_src/planarity.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "planarity_src/c/graph.h"
         ],
@@ -23,16 +23,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -92,16 +92,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -3223,15 +3227,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -3495,15 +3499,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `spherogram-2.2/planarity_src/planarity.pyx` & `spherogram-2.2.1/planarity_src/planarity.pyx`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarmap_src/planarmap.c` & `spherogram-2.2.1/planarmap_src/planarmap.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "planarmap",
         "sources": [
@@ -18,16 +18,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -87,16 +87,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1363,15 +1367,15 @@
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_codeobj__3;
 /* Late includes */
 
-/* "planarmap.pyx":57
+/* "planarmap.pyx":63
  * # We want Planarmap to use the same pseudo-random number generator as Python.
  * 
  * cdef long randrange_callback(long n):             # <<<<<<<<<<<<<<
  *     return random.randrange(n) + 1
  * 
  */
 
@@ -1384,53 +1388,53 @@
   PyObject *__pyx_t_4 = NULL;
   long __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randrange_callback", 0);
 
-  /* "planarmap.pyx":58
+  /* "planarmap.pyx":64
  * 
  * cdef long randrange_callback(long n):
  *     return random.randrange(n) + 1             # <<<<<<<<<<<<<<
  * 
  * set_pmRandom_callback(randrange_callback)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_randrange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_randrange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_5 = __Pyx_PyInt_As_long(__pyx_t_3); if (unlikely((__pyx_t_5 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_long(__pyx_t_3); if (unlikely((__pyx_t_5 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_5;
   goto __pyx_L0;
 
-  /* "planarmap.pyx":57
+  /* "planarmap.pyx":63
  * # We want Planarmap to use the same pseudo-random number generator as Python.
  * 
  * cdef long randrange_callback(long n):             # <<<<<<<<<<<<<<
  *     return random.randrange(n) + 1
  * 
  */
 
@@ -1443,15 +1447,15 @@
   __Pyx_WriteUnraisable("planarmap.randrange_callback", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "planarmap.pyx":65
+/* "planarmap.pyx":71
  * # The main function
  * 
  * def random_map(num_vertices, int edge_connectivity=4,             # <<<<<<<<<<<<<<
  *                int num_link_comps=0, int max_tries=100):
  *     """
  */
 
@@ -1509,15 +1513,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_max_tries);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_map") < 0)) __PYX_ERR(0, 65, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_map") < 0)) __PYX_ERR(0, 71, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -1526,32 +1530,32 @@
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_num_vertices = values[0];
     if (values[1]) {
-      __pyx_v_edge_connectivity = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_edge_connectivity == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
+      __pyx_v_edge_connectivity = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_edge_connectivity == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 71, __pyx_L3_error)
     } else {
       __pyx_v_edge_connectivity = ((int)4);
     }
     if (values[2]) {
-      __pyx_v_num_link_comps = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_num_link_comps == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L3_error)
+      __pyx_v_num_link_comps = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_num_link_comps == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L3_error)
     } else {
       __pyx_v_num_link_comps = ((int)0);
     }
     if (values[3]) {
-      __pyx_v_max_tries = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_max_tries == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L3_error)
+      __pyx_v_max_tries = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_max_tries == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L3_error)
     } else {
       __pyx_v_max_tries = ((int)0x64);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("random_map", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 65, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("random_map", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 71, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("planarmap.random_map", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9planarmap_random_map(__pyx_self, __pyx_v_num_vertices, __pyx_v_edge_connectivity, __pyx_v_num_link_comps, __pyx_v_max_tries);
 
@@ -1588,116 +1592,116 @@
   int __pyx_t_14;
   PyObject *__pyx_t_15 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_map", 0);
 
-  /* "planarmap.pyx":89
+  /* "planarmap.pyx":95
  *     cdef pm_vertex *vert
  * 
  *     if edge_connectivity==2:             # <<<<<<<<<<<<<<
  *         size.m, size.b = 4, 4
  *     elif edge_connectivity==4:
  */
   switch (__pyx_v_edge_connectivity) {
     case 2:
 
-    /* "planarmap.pyx":90
+    /* "planarmap.pyx":96
  * 
  *     if edge_connectivity==2:
  *         size.m, size.b = 4, 4             # <<<<<<<<<<<<<<
  *     elif edge_connectivity==4:
  *         size.m, size.b = 5, 5
  */
     __pyx_t_1 = 4;
     __pyx_t_2 = 4;
     __pyx_v_size.m = __pyx_t_1;
     __pyx_v_size.b = __pyx_t_2;
 
-    /* "planarmap.pyx":89
+    /* "planarmap.pyx":95
  *     cdef pm_vertex *vert
  * 
  *     if edge_connectivity==2:             # <<<<<<<<<<<<<<
  *         size.m, size.b = 4, 4
  *     elif edge_connectivity==4:
  */
     break;
     case 4:
 
-    /* "planarmap.pyx":92
+    /* "planarmap.pyx":98
  *         size.m, size.b = 4, 4
  *     elif edge_connectivity==4:
  *         size.m, size.b = 5, 5             # <<<<<<<<<<<<<<
  *     elif edge_connectivity==6:
  *         size.m, size.b = 6, 5
  */
     __pyx_t_2 = 5;
     __pyx_t_1 = 5;
     __pyx_v_size.m = __pyx_t_2;
     __pyx_v_size.b = __pyx_t_1;
 
-    /* "planarmap.pyx":91
+    /* "planarmap.pyx":97
  *     if edge_connectivity==2:
  *         size.m, size.b = 4, 4
  *     elif edge_connectivity==4:             # <<<<<<<<<<<<<<
  *         size.m, size.b = 5, 5
  *     elif edge_connectivity==6:
  */
     break;
     case 6:
 
-    /* "planarmap.pyx":94
+    /* "planarmap.pyx":100
  *         size.m, size.b = 5, 5
  *     elif edge_connectivity==6:
  *         size.m, size.b = 6, 5             # <<<<<<<<<<<<<<
  *     else:
  *         raise ValueError("Invalid edge_connectivity parameter")
  */
     __pyx_t_1 = 6;
     __pyx_t_2 = 5;
     __pyx_v_size.m = __pyx_t_1;
     __pyx_v_size.b = __pyx_t_2;
 
-    /* "planarmap.pyx":93
+    /* "planarmap.pyx":99
  *     elif edge_connectivity==4:
  *         size.m, size.b = 5, 5
  *     elif edge_connectivity==6:             # <<<<<<<<<<<<<<
  *         size.m, size.b = 6, 5
  *     else:
  */
     break;
     default:
 
-    /* "planarmap.pyx":96
+    /* "planarmap.pyx":102
  *         size.m, size.b = 6, 5
  *     else:
  *         raise ValueError("Invalid edge_connectivity parameter")             # <<<<<<<<<<<<<<
  * 
  *     size.v = num_vertices
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 96, __pyx_L1_error)
+    __PYX_ERR(0, 102, __pyx_L1_error)
     break;
   }
 
-  /* "planarmap.pyx":98
+  /* "planarmap.pyx":104
  *         raise ValueError("Invalid edge_connectivity parameter")
  * 
  *     size.v = num_vertices             # <<<<<<<<<<<<<<
  *     size.e, size.f, size.r, size.g, size.d = 0, 0, 0, 0, 0
  *     size.t = -1
  */
-  __pyx_t_4 = __Pyx_PyInt_As_long(__pyx_v_num_vertices); if (unlikely((__pyx_t_4 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_long(__pyx_v_num_vertices); if (unlikely((__pyx_t_4 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 104, __pyx_L1_error)
   __pyx_v_size.v = __pyx_t_4;
 
-  /* "planarmap.pyx":99
+  /* "planarmap.pyx":105
  * 
  *     size.v = num_vertices
  *     size.e, size.f, size.r, size.g, size.d = 0, 0, 0, 0, 0             # <<<<<<<<<<<<<<
  *     size.t = -1
  *     size.dgArr = NULL
  */
   __pyx_t_4 = 0;
@@ -1707,343 +1711,343 @@
   __pyx_t_8 = 0;
   __pyx_v_size.e = __pyx_t_4;
   __pyx_v_size.f = __pyx_t_5;
   __pyx_v_size.r = __pyx_t_6;
   __pyx_v_size.g = __pyx_t_7;
   __pyx_v_size.d = __pyx_t_8;
 
-  /* "planarmap.pyx":100
+  /* "planarmap.pyx":106
  *     size.v = num_vertices
  *     size.e, size.f, size.r, size.g, size.d = 0, 0, 0, 0, 0
  *     size.t = -1             # <<<<<<<<<<<<<<
  *     size.dgArr = NULL
  * 
  */
   __pyx_v_size.t = -1L;
 
-  /* "planarmap.pyx":101
+  /* "planarmap.pyx":107
  *     size.e, size.f, size.r, size.g, size.d = 0, 0, 0, 0, 0
  *     size.t = -1
  *     size.dgArr = NULL             # <<<<<<<<<<<<<<
  * 
  *     method.core, method.pic = 0, 0
  */
   __pyx_v_size.dgArr = NULL;
 
-  /* "planarmap.pyx":103
+  /* "planarmap.pyx":109
  *     size.dgArr = NULL
  * 
  *     method.core, method.pic = 0, 0             # <<<<<<<<<<<<<<
  *     method.verbose = 0
  *     pmMemoryInit(&size, &method, &memory)
  */
   __pyx_t_2 = 0;
   __pyx_t_1 = 0;
   __pyx_v_method.core = __pyx_t_2;
   __pyx_v_method.pic = __pyx_t_1;
 
-  /* "planarmap.pyx":104
+  /* "planarmap.pyx":110
  * 
  *     method.core, method.pic = 0, 0
  *     method.verbose = 0             # <<<<<<<<<<<<<<
  *     pmMemoryInit(&size, &method, &memory)
  *     pmPlanMap(&size, &method, &memory, &the_map)
  */
   __pyx_v_method.verbose = 0;
 
-  /* "planarmap.pyx":105
+  /* "planarmap.pyx":111
  *     method.core, method.pic = 0, 0
  *     method.verbose = 0
  *     pmMemoryInit(&size, &method, &memory)             # <<<<<<<<<<<<<<
  *     pmPlanMap(&size, &method, &memory, &the_map)
  *     if num_link_comps > 0:
  */
   (void)(pmMemoryInit((&__pyx_v_size), (&__pyx_v_method), (&__pyx_v_memory)));
 
-  /* "planarmap.pyx":106
+  /* "planarmap.pyx":112
  *     method.verbose = 0
  *     pmMemoryInit(&size, &method, &memory)
  *     pmPlanMap(&size, &method, &memory, &the_map)             # <<<<<<<<<<<<<<
  *     if num_link_comps > 0:
  *         tries = 0
  */
   (void)(pmPlanMap((&__pyx_v_size), (&__pyx_v_method), (&__pyx_v_memory), (&__pyx_v_the_map)));
 
-  /* "planarmap.pyx":107
+  /* "planarmap.pyx":113
  *     pmMemoryInit(&size, &method, &memory)
  *     pmPlanMap(&size, &method, &memory, &the_map)
  *     if num_link_comps > 0:             # <<<<<<<<<<<<<<
  *         tries = 0
  *         while pmStatGauss(&the_map) != num_link_comps and tries < max_tries:
  */
   __pyx_t_9 = ((__pyx_v_num_link_comps > 0) != 0);
   if (__pyx_t_9) {
 
-    /* "planarmap.pyx":108
+    /* "planarmap.pyx":114
  *     pmPlanMap(&size, &method, &memory, &the_map)
  *     if num_link_comps > 0:
  *         tries = 0             # <<<<<<<<<<<<<<
  *         while pmStatGauss(&the_map) != num_link_comps and tries < max_tries:
  *             pmFreeMap(&the_map)
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_v_tries = __pyx_int_0;
 
-    /* "planarmap.pyx":109
+    /* "planarmap.pyx":115
  *     if num_link_comps > 0:
  *         tries = 0
  *         while pmStatGauss(&the_map) != num_link_comps and tries < max_tries:             # <<<<<<<<<<<<<<
  *             pmFreeMap(&the_map)
  *             pmPlanMap(&size, &method, &memory, &the_map)
  */
     while (1) {
       __pyx_t_10 = ((pmStatGauss((&__pyx_v_the_map)) != __pyx_v_num_link_comps) != 0);
       if (__pyx_t_10) {
       } else {
         __pyx_t_9 = __pyx_t_10;
         goto __pyx_L6_bool_binop_done;
       }
-      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_max_tries); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_max_tries); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 115, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_11 = PyObject_RichCompare(__pyx_v_tries, __pyx_t_3, Py_LT); __Pyx_XGOTREF(__pyx_t_11); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 109, __pyx_L1_error)
+      __pyx_t_11 = PyObject_RichCompare(__pyx_v_tries, __pyx_t_3, Py_LT); __Pyx_XGOTREF(__pyx_t_11); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 115, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_11); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 109, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_11); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 115, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __pyx_t_9 = __pyx_t_10;
       __pyx_L6_bool_binop_done:;
       if (!__pyx_t_9) break;
 
-      /* "planarmap.pyx":110
+      /* "planarmap.pyx":116
  *         tries = 0
  *         while pmStatGauss(&the_map) != num_link_comps and tries < max_tries:
  *             pmFreeMap(&the_map)             # <<<<<<<<<<<<<<
  *             pmPlanMap(&size, &method, &memory, &the_map)
  *             tries += 1
  */
       (void)(pmFreeMap((&__pyx_v_the_map)));
 
-      /* "planarmap.pyx":111
+      /* "planarmap.pyx":117
  *         while pmStatGauss(&the_map) != num_link_comps and tries < max_tries:
  *             pmFreeMap(&the_map)
  *             pmPlanMap(&size, &method, &memory, &the_map)             # <<<<<<<<<<<<<<
  *             tries += 1
  * 
  */
       (void)(pmPlanMap((&__pyx_v_size), (&__pyx_v_method), (&__pyx_v_memory), (&__pyx_v_the_map)));
 
-      /* "planarmap.pyx":112
+      /* "planarmap.pyx":118
  *             pmFreeMap(&the_map)
  *             pmPlanMap(&size, &method, &memory, &the_map)
  *             tries += 1             # <<<<<<<<<<<<<<
  * 
  *         if tries==max_tries:
  */
-      __pyx_t_11 = __Pyx_PyInt_AddObjC(__pyx_v_tries, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 112, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_AddObjC(__pyx_v_tries, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 118, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF_SET(__pyx_v_tries, __pyx_t_11);
       __pyx_t_11 = 0;
     }
 
-    /* "planarmap.pyx":114
+    /* "planarmap.pyx":120
  *             tries += 1
  * 
  *         if tries==max_tries:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
-    __pyx_t_11 = __Pyx_PyInt_From_int(__pyx_v_max_tries); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_From_int(__pyx_v_max_tries); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_3 = PyObject_RichCompare(__pyx_v_tries, __pyx_t_11, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __pyx_t_3 = PyObject_RichCompare(__pyx_v_tries, __pyx_t_11, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (__pyx_t_9) {
 
-      /* "planarmap.pyx":115
+      /* "planarmap.pyx":121
  * 
  *         if tries==max_tries:
  *             return             # <<<<<<<<<<<<<<
  * 
  *     ans = []
  */
       __Pyx_XDECREF(__pyx_r);
       __pyx_r = Py_None; __Pyx_INCREF(Py_None);
       goto __pyx_L0;
 
-      /* "planarmap.pyx":114
+      /* "planarmap.pyx":120
  *             tries += 1
  * 
  *         if tries==max_tries:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
     }
 
-    /* "planarmap.pyx":107
+    /* "planarmap.pyx":113
  *     pmMemoryInit(&size, &method, &memory)
  *     pmPlanMap(&size, &method, &memory, &the_map)
  *     if num_link_comps > 0:             # <<<<<<<<<<<<<<
  *         tries = 0
  *         while pmStatGauss(&the_map) != num_link_comps and tries < max_tries:
  */
   }
 
-  /* "planarmap.pyx":117
+  /* "planarmap.pyx":123
  *             return
  * 
  *     ans = []             # <<<<<<<<<<<<<<
  *     vert = the_map.root.c_from
  *     while vert != NULL:
  */
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_ans = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "planarmap.pyx":118
+  /* "planarmap.pyx":124
  * 
  *     ans = []
  *     vert = the_map.root.c_from             # <<<<<<<<<<<<<<
  *     while vert != NULL:
  *         edges_at_vert = []
  */
   __pyx_t_12 = __pyx_v_the_map.root->from;
   __pyx_v_vert = __pyx_t_12;
 
-  /* "planarmap.pyx":119
+  /* "planarmap.pyx":125
  *     ans = []
  *     vert = the_map.root.c_from
  *     while vert != NULL:             # <<<<<<<<<<<<<<
  *         edges_at_vert = []
  *         edge = vert.root
  */
   while (1) {
     __pyx_t_9 = ((__pyx_v_vert != NULL) != 0);
     if (!__pyx_t_9) break;
 
-    /* "planarmap.pyx":120
+    /* "planarmap.pyx":126
  *     vert = the_map.root.c_from
  *     while vert != NULL:
  *         edges_at_vert = []             # <<<<<<<<<<<<<<
  *         edge = vert.root
  *         while edge != vert.root.prev:
  */
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_XDECREF_SET(__pyx_v_edges_at_vert, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "planarmap.pyx":121
+    /* "planarmap.pyx":127
  *     while vert != NULL:
  *         edges_at_vert = []
  *         edge = vert.root             # <<<<<<<<<<<<<<
  *         while edge != vert.root.prev:
  *             edges_at_vert.append(edge.label)
  */
     __pyx_t_13 = __pyx_v_vert->root;
     __pyx_v_edge = __pyx_t_13;
 
-    /* "planarmap.pyx":122
+    /* "planarmap.pyx":128
  *         edges_at_vert = []
  *         edge = vert.root
  *         while edge != vert.root.prev:             # <<<<<<<<<<<<<<
  *             edges_at_vert.append(edge.label)
  *             edge = edge.next
  */
     while (1) {
       __pyx_t_9 = ((__pyx_v_edge != __pyx_v_vert->root->prev) != 0);
       if (!__pyx_t_9) break;
 
-      /* "planarmap.pyx":123
+      /* "planarmap.pyx":129
  *         edge = vert.root
  *         while edge != vert.root.prev:
  *             edges_at_vert.append(edge.label)             # <<<<<<<<<<<<<<
  *             edge = edge.next
  *         edges_at_vert.append(edge.label)
  */
-      __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_edge->label); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_edge->label); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_14 = __Pyx_PyList_Append(__pyx_v_edges_at_vert, __pyx_t_3); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 123, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyList_Append(__pyx_v_edges_at_vert, __pyx_t_3); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 129, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "planarmap.pyx":124
+      /* "planarmap.pyx":130
  *         while edge != vert.root.prev:
  *             edges_at_vert.append(edge.label)
  *             edge = edge.next             # <<<<<<<<<<<<<<
  *         edges_at_vert.append(edge.label)
  *         ans.append( (vert.label, tuple(edges_at_vert)) )
  */
       __pyx_t_13 = __pyx_v_edge->next;
       __pyx_v_edge = __pyx_t_13;
     }
 
-    /* "planarmap.pyx":125
+    /* "planarmap.pyx":131
  *             edges_at_vert.append(edge.label)
  *             edge = edge.next
  *         edges_at_vert.append(edge.label)             # <<<<<<<<<<<<<<
  *         ans.append( (vert.label, tuple(edges_at_vert)) )
  *         vert = vert.next
  */
-    __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_edge->label); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_edge->label); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_14 = __Pyx_PyList_Append(__pyx_v_edges_at_vert, __pyx_t_3); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyList_Append(__pyx_v_edges_at_vert, __pyx_t_3); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "planarmap.pyx":126
+    /* "planarmap.pyx":132
  *             edge = edge.next
  *         edges_at_vert.append(edge.label)
  *         ans.append( (vert.label, tuple(edges_at_vert)) )             # <<<<<<<<<<<<<<
  *         vert = vert.next
  *     pmFreeMap(&the_map)
  */
-    __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_vert->label); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_vert->label); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_11 = PyList_AsTuple(__pyx_v_edges_at_vert); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_11 = PyList_AsTuple(__pyx_v_edges_at_vert); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_15 = PyTuple_New(2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_15 = PyTuple_New(2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_11);
     PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_t_11);
     __pyx_t_3 = 0;
     __pyx_t_11 = 0;
-    __pyx_t_14 = __Pyx_PyList_Append(__pyx_v_ans, __pyx_t_15); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyList_Append(__pyx_v_ans, __pyx_t_15); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
 
-    /* "planarmap.pyx":127
+    /* "planarmap.pyx":133
  *         edges_at_vert.append(edge.label)
  *         ans.append( (vert.label, tuple(edges_at_vert)) )
  *         vert = vert.next             # <<<<<<<<<<<<<<
  *     pmFreeMap(&the_map)
  *     return ans
  */
     __pyx_t_12 = __pyx_v_vert->next;
     __pyx_v_vert = __pyx_t_12;
   }
 
-  /* "planarmap.pyx":128
+  /* "planarmap.pyx":134
  *         ans.append( (vert.label, tuple(edges_at_vert)) )
  *         vert = vert.next
  *     pmFreeMap(&the_map)             # <<<<<<<<<<<<<<
  *     return ans
  */
   (void)(pmFreeMap((&__pyx_v_the_map)));
 
-  /* "planarmap.pyx":129
+  /* "planarmap.pyx":135
  *         vert = vert.next
  *     pmFreeMap(&the_map)
  *     return ans             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_ans);
   __pyx_r = __pyx_v_ans;
   goto __pyx_L0;
 
-  /* "planarmap.pyx":65
+  /* "planarmap.pyx":71
  * # The main function
  * 
  * def random_map(num_vertices, int edge_connectivity=4,             # <<<<<<<<<<<<<<
  *                int num_link_comps=0, int max_tries=100):
  *     """
  */
 
@@ -2133,46 +2137,46 @@
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_the_map, __pyx_k_the_map, sizeof(__pyx_k_the_map), 0, 0, 1, 1},
   {&__pyx_n_s_tries, __pyx_k_tries, sizeof(__pyx_k_tries), 0, 0, 1, 1},
   {&__pyx_n_s_vert, __pyx_k_vert, sizeof(__pyx_k_vert), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 102, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "planarmap.pyx":96
+  /* "planarmap.pyx":102
  *         size.m, size.b = 6, 5
  *     else:
  *         raise ValueError("Invalid edge_connectivity parameter")             # <<<<<<<<<<<<<<
  * 
  *     size.v = num_vertices
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Invalid_edge_connectivity_parame); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Invalid_edge_connectivity_parame); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "planarmap.pyx":65
+  /* "planarmap.pyx":71
  * # The main function
  * 
  * def random_map(num_vertices, int edge_connectivity=4,             # <<<<<<<<<<<<<<
  *                int num_link_comps=0, int max_tries=100):
  *     """
  */
-  __pyx_tuple__2 = PyTuple_Pack(13, __pyx_n_s_num_vertices, __pyx_n_s_edge_connectivity, __pyx_n_s_num_link_comps, __pyx_n_s_max_tries, __pyx_n_s_size, __pyx_n_s_method, __pyx_n_s_memory, __pyx_n_s_the_map, __pyx_n_s_edge, __pyx_n_s_vert, __pyx_n_s_tries, __pyx_n_s_ans, __pyx_n_s_edges_at_vert); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(13, __pyx_n_s_num_vertices, __pyx_n_s_edge_connectivity, __pyx_n_s_num_link_comps, __pyx_n_s_max_tries, __pyx_n_s_size, __pyx_n_s_method, __pyx_n_s_memory, __pyx_n_s_the_map, __pyx_n_s_edge, __pyx_n_s_vert, __pyx_n_s_tries, __pyx_n_s_ans, __pyx_n_s_edges_at_vert); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(4, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_planarmap_src_planarmap_pyx, __pyx_n_s_random_map, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(4, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_planarmap_src_planarmap_pyx, __pyx_n_s_random_map, 71, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -2445,51 +2449,51 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "planarmap.pyx":4
+  /* "planarmap.pyx":10
  * 
  * from libc.stdlib cimport malloc, free
  * import random             # <<<<<<<<<<<<<<
  * 
  * cdef extern from 'PMdef.h':
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_random, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_random, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random, __pyx_t_1) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random, __pyx_t_1) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "planarmap.pyx":60
+  /* "planarmap.pyx":66
  *     return random.randrange(n) + 1
  * 
  * set_pmRandom_callback(randrange_callback)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   set_pmRandom_callback(__pyx_f_9planarmap_randrange_callback);
 
-  /* "planarmap.pyx":65
+  /* "planarmap.pyx":71
  * # The main function
  * 
  * def random_map(num_vertices, int edge_connectivity=4,             # <<<<<<<<<<<<<<
  *                int num_link_comps=0, int max_tries=100):
  *     """
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_9planarmap_1random_map, NULL, __pyx_n_s_planarmap); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_9planarmap_1random_map, NULL, __pyx_n_s_planarmap); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_map, __pyx_t_1) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_map, __pyx_t_1) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "planarmap.pyx":1
  * #cython: language_level=3             # <<<<<<<<<<<<<<
- * 
- * from libc.stdlib cimport malloc, free
+ * #cython: legacy_implicit_noexcept=True
+ * #
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /*--- Wrapped vars code ---*/
@@ -3735,15 +3739,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -3969,15 +3973,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `spherogram-2.2/planarmap_src/planarmap.pyx` & `spherogram-2.2.1/planarmap_src/planarmap.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 #cython: language_level=3
+#cython: legacy_implicit_noexcept=True
+#
+# The above line is for Cython 3; to remove, need to declare
+# "randrange_callback" via:
+#
+# cdef long randrange_callback(long n) noexcept:
 
 from libc.stdlib cimport malloc, free
 import random
 
 cdef extern from 'PMdef.h':
     ctypedef struct pmSize:
         char m, b  #  map and basic map type
```

### Comparing `spherogram-2.2/planarmap_src/src/PMconjugation.c` & `spherogram-2.2.1/planarmap_src/src/PMconjugation.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarmap_src/src/PMconjugation.h` & `spherogram-2.2.1/planarmap_src/src/PMconjugation.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarmap_src/src/PMdef.c` & `spherogram-2.2.1/planarmap_src/src/PMdef.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarmap_src/src/PMdef.h` & `spherogram-2.2.1/planarmap_src/src/PMdef.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarmap_src/src/PMenlight.c` & `spherogram-2.2.1/planarmap_src/src/PMenlight.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarmap_src/src/PMextract.c` & `spherogram-2.2.1/planarmap_src/src/PMextract.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarmap_src/src/PMextract.h` & `spherogram-2.2.1/planarmap_src/src/PMextract.h`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarmap_src/src/PMplanmap.c` & `spherogram-2.2.1/planarmap_src/src/PMplanmap.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/planarmap_src/src/stats.c` & `spherogram-2.2.1/planarmap_src/src/stats.c`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/setup.py` & `spherogram-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram.egg-info/PKG-INFO` & `spherogram-2.2.1/spherogram.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spherogram
-Version: 2.2
+Version: 2.2.1
 Summary: Spherical diagrams for 3-manifold topology
 Home-page: https://github.com/3-manifolds/Spherogram
 Author: Marc Culler and Nathan M. Dunfield
 Author-email: culler@marc-culler.info, nathan@dunfield.info
 License: GPLv2+
 Keywords: knot,link,SnapPy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spherogram-2.2/spherogram.egg-info/SOURCES.txt` & `spherogram-2.2.1/spherogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/__init__.py` & `spherogram-2.2.1/spherogram_src/__init__.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/codecs/Base64LikeDT.py` & `spherogram-2.2.1/spherogram_src/codecs/Base64LikeDT.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/codecs/DT.py` & `spherogram-2.2.1/spherogram_src/codecs/DT.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/graphs.py` & `spherogram-2.2.1/spherogram_src/graphs.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/__init__.py` & `spherogram-2.2.1/spherogram_src/links/__init__.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/alexander.py` & `spherogram-2.2.1/spherogram_src/links/alexander.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/doc.pdf` & `spherogram-2.2.1/spherogram_src/links/doc.pdf`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/draw.py` & `spherogram-2.2.1/spherogram_src/links/draw.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/exhaust.py` & `spherogram-2.2.1/spherogram_src/links/exhaust.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/extra_tests.py` & `spherogram-2.2.1/spherogram_src/links/extra_tests.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/invariants.py` & `spherogram-2.2.1/spherogram_src/links/invariants.py`

 * *Files 1% similar despite different names*

```diff
@@ -775,16 +775,19 @@
             Knot represented by 3 crossings
             sage: Link(S)
             <Link: 1 comp; 3 cross>
         """
         if SageKnot is None:
             raise ValueError('Your SageMath does not seem to have a native link type')
         sage_type = SageKnot if len(self.link_components) == 1 else SageLink
-        # Sage's PD_code lists strands *clockwise* not our *anticlockwise*.
-        code = [[x[0], x[3], x[2], x[1]] for x in self.PD_code(min_strand_index=1)]
+        # Sage's PD_code lists strands *clockwise* not our
+        # *anticlockwise* prior to Sage 10.1.
+        code = self.PD_code(min_strand_index=1)
+        if sage_pd_clockwise:
+            code = [[x[0], x[3], x[2], x[1]] for x in code]
         return sage_type(code)
 
     @sage_method
     def _sage_(self):
         """
         A quick test:
```

### Comparing `spherogram-2.2/spherogram_src/links/jones.py` & `spherogram-2.2.1/spherogram_src/links/jones.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/jones_old.py` & `spherogram-2.2.1/spherogram_src/links/jones_old.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/links_base.py` & `spherogram-2.2.1/spherogram_src/links/links_base.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/morse.py` & `spherogram-2.2.1/spherogram_src/links/morse.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/ordered_set.py` & `spherogram-2.2.1/spherogram_src/links/ordered_set.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/orthogonal.py` & `spherogram-2.2.1/spherogram_src/links/orthogonal.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/planar_isotopy.py` & `spherogram-2.2.1/spherogram_src/links/planar_isotopy.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/random_links.py` & `spherogram-2.2.1/spherogram_src/links/random_links.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/seifert.py` & `spherogram-2.2.1/spherogram_src/links/seifert.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/simplify.py` & `spherogram-2.2.1/spherogram_src/links/simplify.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/tangles.py` & `spherogram-2.2.1/spherogram_src/links/tangles.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/test/__init__.py` & `spherogram-2.2.1/spherogram_src/links/test/__init__.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/test/old_testing_code.py` & `spherogram-2.2.1/spherogram_src/links/test/old_testing_code.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/test/test_montesinos.py` & `spherogram-2.2.1/spherogram_src/links/test/test_montesinos.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/torus.py` & `spherogram-2.2.1/spherogram_src/links/torus.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/links/twist.py` & `spherogram-2.2.1/spherogram_src/links/twist.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/presentations.py` & `spherogram-2.2.1/spherogram_src/presentations.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/sage_helper.py` & `spherogram-2.2.1/spherogram_src/sage_helper.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/test.py` & `spherogram-2.2.1/spherogram_src/test.py`

 * *Files identical despite different names*

### Comparing `spherogram-2.2/spherogram_src/test_helper.py` & `spherogram-2.2.1/spherogram_src/test_helper.py`

 * *Files identical despite different names*

