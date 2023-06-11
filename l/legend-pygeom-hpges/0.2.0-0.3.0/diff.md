# Comparing `tmp/legend_pygeom_hpges-0.2.0.tar.gz` & `tmp/legend_pygeom_hpges-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legend_pygeom_hpges-0.2.0.tar", last modified: Mon May 22 16:12:33 2023, max compression
+gzip compressed data, was "legend_pygeom_hpges-0.3.0.tar", last modified: Sun Jun 11 12:13:35 2023, max compression
```

## Comparing `legend_pygeom_hpges-0.2.0.tar` & `legend_pygeom_hpges-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:33.335785 legend_pygeom_hpges-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-22 16:12:23.000000 legend_pygeom_hpges-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-22 16:12:33.335785 legend_pygeom_hpges-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-22 16:12:23.000000 legend_pygeom_hpges-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-22 16:12:23.000000 legend_pygeom_hpges-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-22 16:12:33.335785 legend_pygeom_hpges-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 16:12:23.000000 legend_pygeom_hpges-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:33.327784 legend_pygeom_hpges-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:33.331785 legend_pygeom_hpges-0.2.0/src/legend_pygeom_hpges.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-22 16:12:33.000000 legend_pygeom_hpges-0.2.0/src/legend_pygeom_hpges.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-22 16:12:33.000000 legend_pygeom_hpges-0.2.0/src/legend_pygeom_hpges.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:12:33.000000 legend_pygeom_hpges-0.2.0/src/legend_pygeom_hpges.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:12:33.000000 legend_pygeom_hpges-0.2.0/src/legend_pygeom_hpges.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-22 16:12:33.000000 legend_pygeom_hpges-0.2.0/src/legend_pygeom_hpges.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 16:12:33.000000 legend_pygeom_hpges-0.2.0/src/legend_pygeom_hpges.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:33.331785 legend_pygeom_hpges-0.2.0/src/legendhpges/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-22 16:12:23.000000 legend_pygeom_hpges-0.2.0/src/legendhpges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 16:12:33.000000 legend_pygeom_hpges-0.2.0/src/legendhpges/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-22 16:12:23.000000 legend_pygeom_hpges-0.2.0/src/legendhpges/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-22 16:12:23.000000 legend_pygeom_hpges-0.2.0/src/legendhpges/bege.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-22 16:12:23.000000 legend_pygeom_hpges-0.2.0/src/legendhpges/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-22 16:12:23.000000 legend_pygeom_hpges-0.2.0/src/legendhpges/invcoax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-22 16:12:23.000000 legend_pygeom_hpges-0.2.0/src/legendhpges/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-22 16:12:23.000000 legend_pygeom_hpges-0.2.0/src/legendhpges/ppc.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-22 16:12:23.000000 legend_pygeom_hpges-0.2.0/src/legendhpges/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-22 16:12:23.000000 legend_pygeom_hpges-0.2.0/src/legendhpges/semicoax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:12:33.331785 legend_pygeom_hpges-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-22 16:12:23.000000 legend_pygeom_hpges-0.2.0/tests/test_det_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:13:35.412088 legend_pygeom_hpges-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-11 12:13:35.412088 legend_pygeom_hpges-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-11 12:13:35.412088 legend_pygeom_hpges-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:13:35.408088 legend_pygeom_hpges-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:13:35.408088 legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-11 12:13:35.000000 legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-11 12:13:35.000000 legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 12:13:35.000000 legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 12:13:35.000000 legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-11 12:13:35.000000 legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 12:13:35.000000 legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:13:35.412088 legend_pygeom_hpges-0.3.0/src/legendhpges/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 12:13:35.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/bege.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/invcoax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/make_hpge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/ppc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/src/legendhpges/semicoax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 12:13:35.412088 legend_pygeom_hpges-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-11 12:13:23.000000 legend_pygeom_hpges-0.3.0/tests/test_det_profile.py
```

### Comparing `legend_pygeom_hpges-0.2.0/LICENSE` & `legend_pygeom_hpges-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.2.0/PKG-INFO` & `legend_pygeom_hpges-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_pygeom_hpges
-Version: 0.2.0
+Version: 0.3.0
 Summary: Geometry management for LEGEND HPGE detectors
 Home-page: https://github.com/legend-exp/legend-pygeom-hpges
 Author: Luigi Pertoldi
 Author-email: gipert@pm.me
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 1 - Planning
@@ -29,14 +29,15 @@
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 # legendhpges
 
+[![PyPI](https://img.shields.io/pypi/v/legend-pygeom-hpges?logo=pypi)](https://pypi.org/project/legend-pygeom-hpges/)
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/legend-exp/legend-pygeom-hpges?logo=git)
 [![GitHub Workflow Status](https://img.shields.io/github/checks-status/legend-exp/legend-pygeom-hpges/main?label=main%20branch&logo=github)](https://github.com/legend-exp/legend-pygeom-hpges/actions)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Codecov](https://img.shields.io/codecov/c/github/legend-exp/legend-pygeom-hpges?logo=codecov)](https://app.codecov.io/gh/legend-exp/legend-pygeom-hpges)
 ![GitHub issues](https://img.shields.io/github/issues/legend-exp/legend-pygeom-hpges?logo=github)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/legend-exp/legend-pygeom-hpges?logo=github)
```

### Comparing `legend_pygeom_hpges-0.2.0/README.md` & `legend_pygeom_hpges-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # legendhpges
 
+[![PyPI](https://img.shields.io/pypi/v/legend-pygeom-hpges?logo=pypi)](https://pypi.org/project/legend-pygeom-hpges/)
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/legend-exp/legend-pygeom-hpges?logo=git)
 [![GitHub Workflow Status](https://img.shields.io/github/checks-status/legend-exp/legend-pygeom-hpges/main?label=main%20branch&logo=github)](https://github.com/legend-exp/legend-pygeom-hpges/actions)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Codecov](https://img.shields.io/codecov/c/github/legend-exp/legend-pygeom-hpges?logo=codecov)](https://app.codecov.io/gh/legend-exp/legend-pygeom-hpges)
 ![GitHub issues](https://img.shields.io/github/issues/legend-exp/legend-pygeom-hpges?logo=github)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/legend-exp/legend-pygeom-hpges?logo=github)
```

### Comparing `legend_pygeom_hpges-0.2.0/setup.cfg` & `legend_pygeom_hpges-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.2.0/src/legend_pygeom_hpges.egg-info/PKG-INFO` & `legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend-pygeom-hpges
-Version: 0.2.0
+Version: 0.3.0
 Summary: Geometry management for LEGEND HPGE detectors
 Home-page: https://github.com/legend-exp/legend-pygeom-hpges
 Author: Luigi Pertoldi
 Author-email: gipert@pm.me
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 1 - Planning
@@ -29,14 +29,15 @@
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 # legendhpges
 
+[![PyPI](https://img.shields.io/pypi/v/legend-pygeom-hpges?logo=pypi)](https://pypi.org/project/legend-pygeom-hpges/)
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/legend-exp/legend-pygeom-hpges?logo=git)
 [![GitHub Workflow Status](https://img.shields.io/github/checks-status/legend-exp/legend-pygeom-hpges/main?label=main%20branch&logo=github)](https://github.com/legend-exp/legend-pygeom-hpges/actions)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Codecov](https://img.shields.io/codecov/c/github/legend-exp/legend-pygeom-hpges?logo=codecov)](https://app.codecov.io/gh/legend-exp/legend-pygeom-hpges)
 ![GitHub issues](https://img.shields.io/github/issues/legend-exp/legend-pygeom-hpges?logo=github)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/legend-exp/legend-pygeom-hpges?logo=github)
```

### Comparing `legend_pygeom_hpges-0.2.0/src/legend_pygeom_hpges.egg-info/SOURCES.txt` & `legend_pygeom_hpges-0.3.0/src/legend_pygeom_hpges.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 src/legend_pygeom_hpges.egg-info/top_level.txt
 src/legendhpges/__init__.py
 src/legendhpges/_version.py
 src/legendhpges/base.py
 src/legendhpges/bege.py
 src/legendhpges/draw.py
 src/legendhpges/invcoax.py
+src/legendhpges/make_hpge.py
 src/legendhpges/materials.py
 src/legendhpges/ppc.py
 src/legendhpges/registry.py
 src/legendhpges/semicoax.py
 tests/test_det_profile.py
```

### Comparing `legend_pygeom_hpges-0.2.0/src/legendhpges/base.py` & `legend_pygeom_hpges-0.3.0/src/legendhpges/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,16 @@
             with open(metadata) as jfile:
                 self.metadata = AttrsDict(json.load(jfile))
         else:
             self.metadata = AttrsDict(metadata)
 
         if name is None:
             self.name = self.metadata.name
+        else:
+            self.name = name
 
         # return ordered r,z lists, default unit [mm]
         r, z = self._decode_polycone_coord()
 
         # build generic polycone, and logical volume, default [mm]
         ic_solid = geant4.solid.GenericPolycone(
             self.name, 0, 2 * math.pi, r, z, registry
```

### Comparing `legend_pygeom_hpges-0.2.0/src/legendhpges/bege.py` & `legend_pygeom_hpges-0.3.0/src/legendhpges/bege.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.2.0/src/legendhpges/draw.py` & `legend_pygeom_hpges-0.3.0/src/legendhpges/draw.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.2.0/src/legendhpges/invcoax.py` & `legend_pygeom_hpges-0.3.0/src/legendhpges/invcoax.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.2.0/src/legendhpges/materials.py` & `legend_pygeom_hpges-0.3.0/src/legendhpges/materials.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,25 +8,30 @@
 
 ge70 = geant4.Isotope("Ge70", 32, 70, 69.9243)
 ge72 = geant4.Isotope("Ge72", 32, 72, 71.9221)
 ge73 = geant4.Isotope("Ge73", 32, 73, 72.9235)
 ge74 = geant4.Isotope("Ge74", 32, 74, 73.9212)
 ge76 = geant4.Isotope("Ge76", 32, 76, 75.9214)
 
-# TODO: enrichment argument, natural germanium, cryogenic density
+# TODO: how to manage densities?
 # TODO: decide on names
 
 
 def _enriched_germanium(ge76_fraction: float = 0.92) -> geant4.MaterialCompound:
     """Enriched Germanium builder."""
-    enrge = geant4.ElementIsotopeMixture(f"Germanium{ge76_fraction:.3f}", "EnrGe", 2)
-    # approximation
-    enrge.add_isotope(ge74, 1 - ge76_fraction)
-    enrge.add_isotope(ge76, ge76_fraction)
-    matenrge = geant4.MaterialCompound(
-        f"EnrichedGermanium{ge76_fraction:.3f}", 5.56, 1, default_g4_registry
-    )
-    matenrge.add_element_massfraction(enrge, 1)
+    enrge_name = f"EnrichedGermanium{ge76_fraction:.3f}"
+
+    if enrge_name not in default_g4_registry.materialDict:
+        enrge = geant4.ElementIsotopeMixture(
+            f"Germanium{ge76_fraction:.3f}", "EnrGe", 2
+        )
+        # approximation
+        enrge.add_isotope(ge74, 1 - ge76_fraction)
+        enrge.add_isotope(ge76, ge76_fraction)
+        matenrge = geant4.MaterialCompound(enrge_name, 5.55, 1, default_g4_registry)
+        matenrge.add_element_massfraction(enrge, 1)
+    else:
+        matenrge = default_g4_registry.materialDict[enrge_name]
     return matenrge
 
 
 enriched_germanium = _enriched_germanium()
```

### Comparing `legend_pygeom_hpges-0.2.0/src/legendhpges/ppc.py` & `legend_pygeom_hpges-0.3.0/src/legendhpges/ppc.py`

 * *Files identical despite different names*

### Comparing `legend_pygeom_hpges-0.2.0/src/legendhpges/semicoax.py` & `legend_pygeom_hpges-0.3.0/src/legendhpges/semicoax.py`

 * *Files identical despite different names*

