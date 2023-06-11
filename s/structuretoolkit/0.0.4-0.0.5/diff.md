# Comparing `tmp/structuretoolkit-0.0.4.tar.gz` & `tmp/structuretoolkit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structuretoolkit-0.0.4.tar", last modified: Sun Jun 11 18:07:10 2023, max compression
+gzip compressed data, was "structuretoolkit-0.0.5.tar", last modified: Sun Jun 11 18:09:37 2023, max compression
```

## Comparing `structuretoolkit-0.0.4.tar` & `structuretoolkit-0.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:07:10.615172 structuretoolkit-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-11 18:07:10.615172 structuretoolkit-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-11 18:07:10.615172 structuretoolkit-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-11 18:07:10.000000 structuretoolkit-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:07:10.615172 structuretoolkit-0.0.4/structuretoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-11 18:07:10.615172 structuretoolkit-0.0.4/structuretoolkit/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:07:10.611172 structuretoolkit-0.0.4/structuretoolkit/analyse/
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/analyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/analyse/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    47432 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/analyse/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/analyse/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/analyse/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)    24392 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/analyse/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/analyse/strain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/analyse/symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:07:10.611172 structuretoolkit-0.0.4/structuretoolkit/build/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/build/aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/build/compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/build/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/build/surface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:07:10.611172 structuretoolkit-0.0.4/structuretoolkit/common/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/common/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/common/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/common/pymatgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/common/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)    30843 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/structuretoolkit/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:07:10.607172 structuretoolkit-0.0.4/structuretoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-11 18:07:10.000000 structuretoolkit-0.0.4/structuretoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-11 18:07:10.000000 structuretoolkit-0.0.4/structuretoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:07:10.000000 structuretoolkit-0.0.4/structuretoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-11 18:07:10.000000 structuretoolkit-0.0.4/structuretoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-11 18:07:10.000000 structuretoolkit-0.0.4/structuretoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:07:10.615172 structuretoolkit-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/tests/test_aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/tests/test_analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/tests/test_compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/tests/test_high_index_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/tests/test_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20089 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/tests/test_pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/tests/test_strain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/tests/test_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/tests/test_visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-11 18:07:07.000000 structuretoolkit-0.0.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:09:37.769641 structuretoolkit-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-11 18:09:37.769641 structuretoolkit-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-11 18:09:37.773642 structuretoolkit-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-11 18:09:37.000000 structuretoolkit-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:09:37.773642 structuretoolkit-0.0.5/structuretoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-11 18:09:37.773642 structuretoolkit-0.0.5/structuretoolkit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:09:37.765642 structuretoolkit-0.0.5/structuretoolkit/analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/analyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/analyse/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47409 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/analyse/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/analyse/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/analyse/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24367 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/analyse/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/analyse/strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/analyse/symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:09:37.765642 structuretoolkit-0.0.5/structuretoolkit/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/build/aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/build/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/build/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/build/surface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:09:37.769641 structuretoolkit-0.0.5/structuretoolkit/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/common/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/common/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/common/pymatgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/common/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30764 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/structuretoolkit/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:09:37.765642 structuretoolkit-0.0.5/structuretoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-11 18:09:37.000000 structuretoolkit-0.0.5/structuretoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-11 18:09:37.000000 structuretoolkit-0.0.5/structuretoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:09:37.000000 structuretoolkit-0.0.5/structuretoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-11 18:09:37.000000 structuretoolkit-0.0.5/structuretoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-11 18:09:37.000000 structuretoolkit-0.0.5/structuretoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:09:37.769641 structuretoolkit-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/tests/test_aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/tests/test_analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/tests/test_compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/tests/test_high_index_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/tests/test_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20089 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/tests/test_pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/tests/test_strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/tests/test_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/tests/test_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-11 18:09:32.000000 structuretoolkit-0.0.5/versioneer.py
```

### Comparing `structuretoolkit-0.0.4/LICENSE` & `structuretoolkit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/PKG-INFO` & `structuretoolkit-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structuretoolkit
-Version: 0.0.4
+Version: 0.0.5
 Summary: structuretoolkit - to analyse, build and visualise atomistic structures.
 Home-page: https://github.com/pyiron/structuretoolkit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `structuretoolkit-0.0.4/README.md` & `structuretoolkit-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/setup.py` & `structuretoolkit-0.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,18 +32,18 @@
     install_requires=[
         'ase>=3.22.1',
         'matplotlib>=3.7.1',  # ase already requires matplotlib
         'numpy>=1.24.3',  # ase already requires numpy
         'scipy>=1.10.1',  # ase already requires scipy
     ],
     extras_require={
-        "grainboundary": ['aimsgb>=0.1.2', 'pymatgen>=2023.5.10'],
+        "grainboundary": ['aimsgb>=0.1.3', 'pymatgen>=2023.5.31'],
         "pyscal": ['pyscal2>=2.10.18'],
-        "nglview": ['nglview>=3.0.4'],
+        "nglview": ['nglview>=3.0.5'],
         "plotly": ['plotly>=5.14.1'],
         "clusters": ['scikit-learn>=1.2.2'],
         "symmetry": ['spglib>=2.0.2'],
-        "surface": ['spglib>=2.0.2', 'pymatgen>=2023.5.10'],
-        "phonopy": ['phonopy>=2.19.0', 'spglib>=2.0.2'],
+        "surface": ['spglib>=2.0.2', 'pymatgen>=2023.5.31'],
+        "phonopy": ['phonopy>=2.19.1', 'spglib>=2.0.2'],
     },
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `structuretoolkit-0.0.4/structuretoolkit/__init__.py` & `structuretoolkit-0.0.5/structuretoolkit/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,75 @@
 # Analyse
 from structuretoolkit.analyse import (
-    get_distances_array,
     find_mic,
-    get_neighbors,
-    get_neighborhood,
-    get_equivalent_atoms,
-    get_steinhardt_parameters,
-    get_centro_symmetry_descriptors,
-    get_diamond_structure_descriptors,
-    get_adaptive_cna_descriptors,
-    get_voronoi_volumes,
     find_solids,
-    get_mean_positions,
+    get_adaptive_cna_descriptors,
     get_average_of_unique_labels,
+    get_centro_symmetry_descriptors,
+    get_cluster_positions,
+    get_delaunay_neighbors,
+    get_diamond_structure_descriptors,
+    get_distances_array,
+    get_equivalent_atoms,
     get_interstitials,
     get_layers,
-    get_voronoi_vertices,
-    get_voronoi_neighbors,
-    get_delaunay_neighbors,
-    get_cluster_positions,
+    get_mean_positions,
+    get_neighborhood,
+    get_neighbors,
+    get_steinhardt_parameters,
     get_strain,
     get_symmetry,
-    # for backwards compatibility
-    get_cluster_positions as cluster_positions,
-    get_equivalent_atoms as analyse_phonopy_equivalent_atoms,
-    get_steinhardt_parameters as get_steinhardt_parameter_structure,
-    get_centro_symmetry_descriptors as analyse_centro_symmetry,
-    get_diamond_structure_descriptors as analyse_diamond_structure,
-    get_adaptive_cna_descriptors as analyse_cna_adaptive,
-    get_voronoi_volumes as analyse_voronoi_volume,
-    find_solids as analyse_find_solids,
+    get_voronoi_neighbors,
+    get_voronoi_vertices,
+    get_voronoi_volumes,
 )
 
 # Build
 from structuretoolkit.build import (
-    grainboundary,
-    get_grainboundary_info,
     B2,
     C14,
     C15,
     C36,
     D03,
-    sqs_structures,
-    high_index_surface,
+    get_grainboundary_info,
     get_high_index_surface_info,
-    # for backwards compatibility
-    grainboundary as grainboundary_build,
-    get_grainboundary_info as grainboundary_info,
-    sqs_structures as get_sqs_structures,
-    get_high_index_surface_info as high_index_surface_info,
+    grainboundary,
+    high_index_surface,
+    sqs_structures,
 )
 
-# Visualize
-from structuretoolkit.visualize import plot3d
-
 # Common
 from structuretoolkit.common import (
+    SymmetryError,
+    apply_strain,
     ase_to_pymatgen,
-    pymatgen_to_ase,
     ase_to_pyscal,
-    get_atomic_numbers,
+    center_coordinates_in_unit_cell,
     get_extended_positions,
     get_vertical_length,
     get_wrapped_coordinates,
+    pymatgen_to_ase,
     select_index,
-    center_coordinates_in_unit_cell,
-    apply_strain,
-    SymmetryError,
+)
+
+# Visualize
+from structuretoolkit.visualize import plot3d
+
+# Analyse - for backwards compatibility
+from structuretoolkit.analyse import (
+    find_solids as analyse_find_solids,
+    get_adaptive_cna_descriptors as analyse_cna_adaptive,
+    get_centro_symmetry_descriptors as analyse_centro_symmetry,
+    get_cluster_positions as cluster_positions,
+    get_diamond_structure_descriptors as analyse_diamond_structure,
+    get_equivalent_atoms as analyse_phonopy_equivalent_atoms,
+    get_steinhardt_parameters as get_steinhardt_parameter_structure,
+    get_voronoi_volumes as analyse_voronoi_volume,
+)
+
+# Build - for backwards compatibility
+from structuretoolkit.build import (
+    get_grainboundary_info as grainboundary_info,
+    get_high_index_surface_info as high_index_surface_info,
+    grainboundary as grainboundary_build,
+    sqs_structures as get_sqs_structures,
 )
```

### Comparing `structuretoolkit-0.0.4/structuretoolkit/analyse/__init__.py` & `structuretoolkit-0.0.5/structuretoolkit/analyse/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-from structuretoolkit.analyse.distance import get_distances_array, find_mic
-from structuretoolkit.analyse.neighbors import get_neighbors, get_neighborhood
+from structuretoolkit.analyse.distance import find_mic, get_distances_array
+from structuretoolkit.analyse.neighbors import get_neighborhood, get_neighbors
 from structuretoolkit.analyse.phonopy import get_equivalent_atoms
 from structuretoolkit.analyse.pyscal import (
-    get_steinhardt_parameters,
+    find_solids,
+    get_adaptive_cna_descriptors,
     get_centro_symmetry_descriptors,
     get_diamond_structure_descriptors,
-    get_adaptive_cna_descriptors,
+    get_steinhardt_parameters,
     get_voronoi_volumes,
-    find_solids,
-    ase_to_pyscal,
 )
 from structuretoolkit.analyse.spatial import (
-    get_mean_positions,
     get_average_of_unique_labels,
+    get_cluster_positions,
+    get_delaunay_neighbors,
     get_interstitials,
     get_layers,
-    get_voronoi_vertices,
+    get_mean_positions,
     get_voronoi_neighbors,
-    get_delaunay_neighbors,
-    get_cluster_positions,
+    get_voronoi_vertices,
 )
 from structuretoolkit.analyse.strain import get_strain
 
 
 def get_symmetry(
     structure, use_magmoms=False, use_elements=True, symprec=1e-5, angle_tolerance=-1.0
 ):
```

### Comparing `structuretoolkit-0.0.4/structuretoolkit/analyse/distance.py` & `structuretoolkit-0.0.5/structuretoolkit/analyse/distance.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/structuretoolkit/analyse/neighbors.py` & `structuretoolkit-0.0.5/structuretoolkit/analyse/neighbors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
+import itertools
+import warnings
+
 import numpy as np
 from scipy.sparse import coo_matrix
-from scipy.special import gamma
-from scipy.spatial.transform import Rotation
-from scipy.special import sph_harm
 from scipy.spatial import cKDTree
-import warnings
-import itertools
+from scipy.spatial.transform import Rotation
+from scipy.special import gamma, sph_harm
+
 from structuretoolkit.common.helper import (
-    get_extended_positions,
     get_average_of_unique_labels,
+    get_extended_positions,
 )
 
 __author__ = "Joerg Neugebauer, Sam Waseda"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
```

### Comparing `structuretoolkit-0.0.4/structuretoolkit/analyse/phonopy.py` & `structuretoolkit-0.0.5/structuretoolkit/analyse/phonopy.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/structuretoolkit/analyse/pyscal.py` & `structuretoolkit-0.0.5/structuretoolkit/analyse/pyscal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
 from ase.atoms import Atoms
+
 from structuretoolkit.common.pyscal import ase_to_pyscal
 
 __author__ = "Sarath Menon, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
```

### Comparing `structuretoolkit-0.0.4/structuretoolkit/analyse/spatial.py` & `structuretoolkit-0.0.5/structuretoolkit/analyse/spatial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
 from scipy.sparse import coo_matrix
-from scipy.spatial import Voronoi, Delaunay
-from scipy.spatial import ConvexHull
+from scipy.spatial import ConvexHull, Delaunay, Voronoi
+
+from structuretoolkit.analyse.neighbors import get_neighborhood
 from structuretoolkit.common.helper import (
+    get_average_of_unique_labels,
     get_extended_positions,
-    get_wrapped_coordinates,
     get_vertical_length,
-    get_average_of_unique_labels,
+    get_wrapped_coordinates,
 )
-from structuretoolkit.analyse.neighbors import get_neighborhood
-
 
 __author__ = "Joerg Neugebauer, Sam Waseda"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
```

### Comparing `structuretoolkit-0.0.4/structuretoolkit/analyse/strain.py` & `structuretoolkit-0.0.5/structuretoolkit/analyse/strain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from scipy.spatial.transform import Rotation
+
 from structuretoolkit.analyse.neighbors import get_neighbors
 from structuretoolkit.analyse.pyscal import get_adaptive_cna_descriptors
 
 
 class Strain:
 
     """
```

### Comparing `structuretoolkit-0.0.4/structuretoolkit/analyse/symmetry.py` & `structuretoolkit-0.0.5/structuretoolkit/analyse/symmetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
+import ast
+
 import numpy as np
-from scipy.spatial import cKDTree
 import spglib
-import ast
+from scipy.spatial import cKDTree
 
 import structuretoolkit.common.helper
 from structuretoolkit.common.error import SymmetryError
 
 __author__ = "Joerg Neugebauer, Sam Waseda"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
```

### Comparing `structuretoolkit-0.0.4/structuretoolkit/build/aimsgb.py` & `structuretoolkit-0.0.5/structuretoolkit/build/aimsgb.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/structuretoolkit/build/compound.py` & `structuretoolkit-0.0.5/structuretoolkit/build/compound.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/structuretoolkit/build/sqs.py` & `structuretoolkit-0.0.5/structuretoolkit/build/sqs.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/structuretoolkit/build/surface.py` & `structuretoolkit-0.0.5/structuretoolkit/build/surface.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/structuretoolkit/common/helper.py` & `structuretoolkit-0.0.5/structuretoolkit/common/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 import numpy as np
-from scipy.sparse import coo_matrix
 from ase.data import atomic_numbers
-
-
-def get_atomic_numbers(structure):
-    return [atomic_numbers[el] for el in structure.get_chemical_symbols()]
+from scipy.sparse import coo_matrix
 
 
 def get_extended_positions(
     structure, width, return_indices=False, norm_order=2, positions=None
 ):
     """
     Get all atoms in the boundary around the supercell which have a distance
```

### Comparing `structuretoolkit-0.0.4/structuretoolkit/visualize.py` & `structuretoolkit-0.0.5/structuretoolkit/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
-import numpy as np
 import warnings
+
+import numpy as np
 from scipy.interpolate import interp1d
-from structuretoolkit.common.helper import get_atomic_numbers
 
 __author__ = "Joerg Neugebauer, Sudarsan Surendralal"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -178,15 +178,15 @@
     try:
         import plotly.express as px
     except ModuleNotFoundError:
         raise ModuleNotFoundError("plotly not installed - use plot3d instead")
     if select_atoms is None:
         select_atoms = np.arange(len(structure))
     elements = structure.get_chemical_symbols()
-    atomic_numbers = get_atomic_numbers(structure=structure)
+    atomic_numbers = structure.get_atomic_numbers()
     if scalar_field is None:
         scalar_field = elements
     fig = px.scatter_3d(
         x=structure.positions[select_atoms, 0],
         y=structure.positions[select_atoms, 1],
         z=structure.positions[select_atoms, 2],
         color=scalar_field,
@@ -296,15 +296,15 @@
     ):
         if len(structure.get_initial_magnetic_moments().shape) == 1:
             scalar_field = structure.get_initial_magnetic_moments()
         else:
             vector_field = structure.get_initial_magnetic_moments()
 
     elements = structure.get_chemical_symbols()
-    atomic_numbers = get_atomic_numbers(structure=structure)
+    atomic_numbers = structure.get_atomic_numbers()
     positions = structure.positions
 
     # If `select_atoms` was given, visualize only a subset of the `parent_basis`
     if select_atoms is not None:
         select_atoms = np.array(select_atoms, dtype=int)
         elements = elements[select_atoms]
         atomic_numbers = atomic_numbers[select_atoms]
```

### Comparing `structuretoolkit-0.0.4/structuretoolkit.egg-info/PKG-INFO` & `structuretoolkit-0.0.5/structuretoolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structuretoolkit
-Version: 0.0.4
+Version: 0.0.5
 Summary: structuretoolkit - to analyse, build and visualise atomistic structures.
 Home-page: https://github.com/pyiron/structuretoolkit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `structuretoolkit-0.0.4/structuretoolkit.egg-info/SOURCES.txt` & `structuretoolkit-0.0.5/structuretoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/tests/test_aimsgb.py` & `structuretoolkit-0.0.5/tests/test_aimsgb.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/tests/test_analyse.py` & `structuretoolkit-0.0.5/tests/test_analyse.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/tests/test_compound.py` & `structuretoolkit-0.0.5/tests/test_compound.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/tests/test_high_index_surface.py` & `structuretoolkit-0.0.5/tests/test_high_index_surface.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/tests/test_neighbors.py` & `structuretoolkit-0.0.5/tests/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/tests/test_pyscal.py` & `structuretoolkit-0.0.5/tests/test_pyscal.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/tests/test_strain.py` & `structuretoolkit-0.0.5/tests/test_strain.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/tests/test_symmetry.py` & `structuretoolkit-0.0.5/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/tests/test_visualize.py` & `structuretoolkit-0.0.5/tests/test_visualize.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.4/versioneer.py` & `structuretoolkit-0.0.5/versioneer.py`

 * *Files identical despite different names*

