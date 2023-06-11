# Comparing `tmp/neutronics_material_maker-1.1.3.tar.gz` & `tmp/neutronics_material_maker-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutronics_material_maker-1.1.3.tar", last modified: Fri Apr 21 12:45:01 2023, max compression
+gzip compressed data, was "neutronics_material_maker-1.1.4.tar", last modified: Sun Jun 11 20:03:27 2023, max compression
```

## Comparing `neutronics_material_maker-1.1.3.tar` & `neutronics_material_maker-1.1.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.679106 neutronics_material_maker-1.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.675106 neutronics_material_maker-1.1.3/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.671106 neutronics_material_maker-1.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.675106 neutronics_material_maker-1.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/.github/workflows/python-publish-testpypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-04-21 12:45:01.679106 neutronics_material_maker-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.675106 neutronics_material_maker-1.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/make_docs_from_rst.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.675106 neutronics_material_maker-1.1.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/source/example_material.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/source/example_material_from_library.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/source/example_material_from_mixture.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/docs/source/material.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:45:01.679106 neutronics_material_maker-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.675106 neutronics_material_maker-1.1.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 12:45:01.000000 neutronics_material_maker-1.1.3/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.675106 neutronics_material_maker-1.1.3/src/neutronics_material_maker/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.679106 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/breeder_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/breeder_materials_with_crystal_structure.json
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/coolant_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/insulators.json
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/magnet_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/moderators.json
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/multiplier_and_breeder_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/multiplier_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/plasma_material.json
--rw-r--r--   0 runner    (1001) docker     (123)   144857 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/pnnl_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/scintillators.json
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/structural_materials.json
--rw-r--r--   0 runner    (1001) docker     (123)    37224 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/material.py
--rw-r--r--   0 runner    (1001) docker     (123)    17073 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.675106 neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-04-21 12:45:01.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-21 12:45:01.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:45:01.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-21 12:45:01.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-21 12:45:01.000000 neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:45:01.679106 neutronics_material_maker-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40030 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/tests/test_Material.py
--rw-r--r--   0 runner    (1001) docker     (123)    22717 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/tests/test_Material_from_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-21 12:44:44.000000 neutronics_material_maker-1.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:03:27.729796 neutronics_material_maker-1.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:03:27.725796 neutronics_material_maker-1.1.4/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:03:27.721795 neutronics_material_maker-1.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:03:27.725796 neutronics_material_maker-1.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/.github/workflows/python-publish-testpypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-06-11 20:03:27.729796 neutronics_material_maker-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:03:27.725796 neutronics_material_maker-1.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/docs/make_docs_from_rst.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:03:27.725796 neutronics_material_maker-1.1.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/docs/source/example_material.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/docs/source/example_material_from_library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/docs/source/example_material_from_mixture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/docs/source/material.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 20:03:27.729796 neutronics_material_maker-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:03:27.725796 neutronics_material_maker-1.1.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 20:03:27.000000 neutronics_material_maker-1.1.4/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:03:27.725796 neutronics_material_maker-1.1.4/src/neutronics_material_maker/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:03:27.729796 neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/breeder_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/breeder_materials_with_crystal_structure.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/coolant_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/insulators.json
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/magnet_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/moderators.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/multiplier_and_breeder_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/multiplier_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/plasma_material.json
+-rw-r--r--   0 runner    (1001) docker     (123)   144857 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/pnnl_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/scintillators.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/structural_materials.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37224 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17073 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:03:27.729796 neutronics_material_maker-1.1.4/src/neutronics_material_maker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-06-11 20:03:27.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-11 20:03:27.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 20:03:27.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-11 20:03:27.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-11 20:03:27.000000 neutronics_material_maker-1.1.4/src/neutronics_material_maker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:03:27.729796 neutronics_material_maker-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40030 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/tests/test_Material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22717 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/tests/test_Material_from_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-11 20:03:11.000000 neutronics_material_maker-1.1.4/tox.ini
```

### Comparing `neutronics_material_maker-1.1.3/.circleci/config.yml` & `neutronics_material_maker-1.1.4/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/.github/workflows/black.yml` & `neutronics_material_maker-1.1.4/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/.github/workflows/python-publish-testpypi.yml` & `neutronics_material_maker-1.1.4/.github/workflows/python-publish-testpypi.yml`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/.github/workflows/python-publish.yml` & `neutronics_material_maker-1.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/.gitignore` & `neutronics_material_maker-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/CITATION.cff` & `neutronics_material_maker-1.1.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/Dockerfile` & `neutronics_material_maker-1.1.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/LICENSE.txt` & `neutronics_material_maker-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/PKG-INFO` & `neutronics_material_maker-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutronics_material_maker
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool for making reproducible materials and standardizing use across several neutronics codes
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 License: MIT License
         
         Copyright (c) 2020 UKAEA and neutronics-material-maker contributors
         Copyright (c) 2021 neutronics-material-maker contributors
```

### Comparing `neutronics_material_maker-1.1.3/README.md` & `neutronics_material_maker-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/docs/Makefile` & `neutronics_material_maker-1.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/docs/source/conf.py` & `neutronics_material_maker-1.1.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/docs/source/example_material.rst` & `neutronics_material_maker-1.1.4/docs/source/example_material.rst`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/docs/source/example_material_from_library.rst` & `neutronics_material_maker-1.1.4/docs/source/example_material_from_library.rst`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/docs/source/example_material_from_mixture.rst` & `neutronics_material_maker-1.1.4/docs/source/example_material_from_mixture.rst`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/docs/source/index.rst` & `neutronics_material_maker-1.1.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/docs/source/install.rst` & `neutronics_material_maker-1.1.4/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/pyproject.toml` & `neutronics_material_maker-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/src/neutronics_material_maker/__init__.py` & `neutronics_material_maker-1.1.4/src/neutronics_material_maker/__init__.py`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/breeder_materials.json` & `neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/breeder_materials.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821428571428572%*

 * *Differences: {"'Li'": "{'density': '0.515 - 1.01e-4 * (temperature - 273.15 - 200)'}"}*

```diff
@@ -7,14 +7,14 @@
         "enrichment_target": "Li6",
         "enrichment_type": "ao",
         "percent_type": "ao"
     },
     "Li": {
         "chemical_equation": "Li",
         "comment": "http://aries.ucsd.edu/LIB/PROPS/PANOS/li.html",
-        "density": "0.515 - 1.01e-4 * (temperature + 273.15 - 200)",
+        "density": "0.515 - 1.01e-4 * (temperature - 273.15 - 200)",
         "density_unit": "g/cm3",
         "enrichment_target": "Li6",
         "enrichment_type": "ao",
         "percent_type": "ao"
     }
 }
```

### Comparing `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/breeder_materials_with_crystal_structure.json` & `neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/breeder_materials_with_crystal_structure.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/coolant_materials.json` & `neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/coolant_materials.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/magnet_materials.json` & `neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/magnet_materials.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/multiplier_and_breeder_materials.json` & `neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/multiplier_and_breeder_materials.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785714285714286%*

 * *Differences: {"'FLiBe'": "{'density': '2.214 - 4.2e-4 * (temperature - 273.15)'}",*

 * * "'Pb842Li158'": "{'density': '99.90*(0.1-16.8e-6*(temperature - 273.15))'}",*

 * * "'lithium-lead'": "{'density': '99.90*(0.1-16.8e-6*(temperature - 273.15))'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "FLiBe": {
         "chemical_equation": "F2Li2BeF2",
         "comment": "source http://aries.ucsd.edu/LIB/MEETINGS/0103-TRANSMUT/gohar/Gohar-present.pdf",
-        "density": "2.214 - 4.2e-4 * (temperature + 273.15)",
+        "density": "2.214 - 4.2e-4 * (temperature - 273.15)",
         "density_unit": "g/cm3",
         "enrichment_target": "Li6",
         "enrichment_type": "ao",
         "percent_type": "ao"
     },
     "FLiNaBe": {
         "chemical_equation": "FLiNaBe",
@@ -26,23 +26,23 @@
         "enrichment_type": "ao",
         "percent_type": "ao",
         "volume_of_unit_cell_cm3": 1.4400485967e-22
     },
     "Pb842Li158": {
         "chemical_equation": "Pb842Li158",
         "comment": "density equation valid for in the range 240-350 C. source http://aries.ucsd.edu/LIB/PROPS/PANOS/lipb.html",
-        "density": "99.90*(0.1-16.8e-6*(temperature + 273.15))",
+        "density": "99.90*(0.1-16.8e-6*(temperature - 273.15))",
         "density_unit": "g/cm3",
         "enrichment_target": "Li6",
         "enrichment_type": "ao",
         "percent_type": "ao"
     },
     "lithium-lead": {
         "chemical_equation": "Pb842Li158",
         "comment": "density equation valid for in the range 240-350 C. source http://aries.ucsd.edu/LIB/PROPS/PANOS/lipb.html",
-        "density": "99.90*(0.1-16.8e-6*(temperature + 273.15))",
+        "density": "99.90*(0.1-16.8e-6*(temperature - 273.15))",
         "density_unit": "g/cm3",
         "enrichment_target": "Li6",
         "enrichment_type": "ao",
         "percent_type": "ao"
     }
 }
```

### Comparing `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/multiplier_materials.json` & `neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/multiplier_materials.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/pnnl_materials.json` & `neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/pnnl_materials.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/scintillators.json` & `neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/scintillators.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/src/neutronics_material_maker/data/structural_materials.json` & `neutronics_material_maker-1.1.4/src/neutronics_material_maker/data/structural_materials.json`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/src/neutronics_material_maker/material.py` & `neutronics_material_maker-1.1.4/src/neutronics_material_maker/material.py`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/src/neutronics_material_maker/utils.py` & `neutronics_material_maker-1.1.4/src/neutronics_material_maker/utils.py`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/PKG-INFO` & `neutronics_material_maker-1.1.4/src/neutronics_material_maker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutronics-material-maker
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool for making reproducible materials and standardizing use across several neutronics codes
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 License: MIT License
         
         Copyright (c) 2020 UKAEA and neutronics-material-maker contributors
         Copyright (c) 2021 neutronics-material-maker contributors
```

### Comparing `neutronics_material_maker-1.1.3/src/neutronics_material_maker.egg-info/SOURCES.txt` & `neutronics_material_maker-1.1.4/src/neutronics_material_maker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/tests/test_Material.py` & `neutronics_material_maker-1.1.4/tests/test_Material.py`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/tests/test_Material_from_mixture.py` & `neutronics_material_maker-1.1.4/tests/test_Material_from_mixture.py`

 * *Files identical despite different names*

### Comparing `neutronics_material_maker-1.1.3/tests/test_utils.py` & `neutronics_material_maker-1.1.4/tests/test_utils.py`

 * *Files identical despite different names*

