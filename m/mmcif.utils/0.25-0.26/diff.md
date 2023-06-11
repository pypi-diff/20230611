# Comparing `tmp/mmcif.utils-0.25.tar.gz` & `tmp/mmcif.utils-0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcif.utils-0.25.tar", last modified: Thu Apr  7 10:14:43 2022, max compression
+gzip compressed data, was "mmcif.utils-0.26.tar", last modified: Sun Jun 11 18:27:23 2023, max compression
```

## Comparing `mmcif.utils-0.25.tar` & `mmcif.utils-0.26.tar`

### file list

```diff
@@ -1,89 +1,84 @@
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-04-07 10:14:43.873028 mmcif.utils-0.25/
--rw-r--r--   0 peisach    (502) staff       (20)     1248 2019-07-12 07:37:21.000000 mmcif.utils-0.25/.gitignore
--rw-r--r--   0 peisach    (502) staff       (20)     1509 2022-04-07 10:04:08.000000 mmcif.utils-0.25/HISTORY.txt
--rw-r--r--   0 peisach    (502) staff       (20)      552 2018-10-10 20:56:01.000000 mmcif.utils-0.25/LICENSE
--rw-r--r--   0 peisach    (502) staff       (20)       97 2020-08-28 16:16:31.000000 mmcif.utils-0.25/MANIFEST.in
--rw-r--r--   0 peisach    (502) staff       (20)      731 2022-04-07 10:14:43.873402 mmcif.utils-0.25/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)      558 2019-07-12 07:37:21.000000 mmcif.utils-0.25/README.md
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-04-07 10:14:43.841972 mmcif.utils-0.25/mmcif.utils.egg-info/
--rw-r--r--   0 peisach    (502) staff       (20)      731 2022-04-07 10:14:43.000000 mmcif.utils-0.25/mmcif.utils.egg-info/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)     2610 2022-04-07 10:14:43.000000 mmcif.utils-0.25/mmcif.utils.egg-info/SOURCES.txt
--rw-r--r--   0 peisach    (502) staff       (20)        1 2022-04-07 10:14:43.000000 mmcif.utils-0.25/mmcif.utils.egg-info/dependency_links.txt
--rw-r--r--   0 peisach    (502) staff       (20)       62 2022-04-07 10:14:43.000000 mmcif.utils-0.25/mmcif.utils.egg-info/requires.txt
--rw-r--r--   0 peisach    (502) staff       (20)       12 2022-04-07 10:14:43.000000 mmcif.utils-0.25/mmcif.utils.egg-info/top_level.txt
--rw-r--r--   0 peisach    (502) staff       (20)        1 2020-08-28 16:16:33.000000 mmcif.utils-0.25/mmcif.utils.egg-info/zip-safe
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-04-07 10:14:43.842313 mmcif.utils-0.25/mmcif_utils/
--rw-r--r--   0 peisach    (502) staff       (20)      195 2022-04-07 10:04:08.000000 mmcif.utils-0.25/mmcif_utils/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-04-07 10:14:43.845042 mmcif.utils-0.25/mmcif_utils/bird/
--rw-r--r--   0 peisach    (502) staff       (20)     6730 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/bird/PdbxBirdIndex.py
--rw-r--r--   0 peisach    (502) staff       (20)     4634 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/bird/PdbxFamilyIo.py
--rw-r--r--   0 peisach    (502) staff       (20)    18362 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/bird/PdbxPrd.py
--rw-r--r--   0 peisach    (502) staff       (20)     4588 2022-04-07 10:04:08.000000 mmcif.utils-0.25/mmcif_utils/bird/PdbxPrdCcIo.py
--rw-r--r--   0 peisach    (502) staff       (20)     4472 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/bird/PdbxPrdIo.py
--rw-r--r--   0 peisach    (502) staff       (20)    18294 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/bird/PdbxPrdUtils.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/bird/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-04-07 10:14:43.847765 mmcif.utils-0.25/mmcif_utils/bird/cl/
--rwxr-xr-x   0 peisach    (502) staff       (20)     2596 2020-01-12 12:02:04.000000 mmcif.utils-0.25/mmcif_utils/bird/cl/Example-commands.sh
--rw-r--r--   0 peisach    (502) staff       (20)    22027 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/bird/cl/PdbxPrdExec.py
--rw-r--r--   0 peisach    (502) staff       (20)      632 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/bird/cl/REF_ONLY_CC.LIST
--rw-r--r--   0 peisach    (502) staff       (20)        0 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/bird/cl/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-04-07 10:14:43.850485 mmcif.utils-0.25/mmcif_utils/chemcomp/
--rw-r--r--   0 peisach    (502) staff       (20)     8321 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/chemcomp/PdbxChemComp.py
--rw-r--r--   0 peisach    (502) staff       (20)     4233 2022-04-07 10:04:08.000000 mmcif.utils-0.25/mmcif_utils/chemcomp/PdbxChemCompIo.py
--rw-r--r--   0 peisach    (502) staff       (20)     7194 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/chemcomp/PdbxChemCompModel.py
--rw-r--r--   0 peisach    (502) staff       (20)     3157 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/chemcomp/PdbxChemCompModelIo.py
--rw-r--r--   0 peisach    (502) staff       (20)    26448 2019-07-15 17:16:12.000000 mmcif.utils-0.25/mmcif_utils/chemcomp/PdbxChemCompUtils.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/chemcomp/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-04-07 10:14:43.851524 mmcif.utils-0.25/mmcif_utils/inventory/
--rw-r--r--   0 peisach    (502) staff       (20)     3699 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/inventory/InventoryIo.py
--rw-r--r--   0 peisach    (502) staff       (20)    11245 2020-08-28 16:01:33.000000 mmcif.utils-0.25/mmcif_utils/inventory/InventoryIoBatchRunner.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/inventory/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-04-07 10:14:43.852972 mmcif.utils-0.25/mmcif_utils/message/
--rw-r--r--   0 peisach    (502) staff       (20)    12138 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/message/PdbxMessage.py
--rw-r--r--   0 peisach    (502) staff       (20)     4173 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/message/PdbxMessageIo.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/message/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-04-07 10:14:43.856237 mmcif.utils-0.25/mmcif_utils/pdb/
--rw-r--r--   0 peisach    (502) staff       (20)    16392 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/pdb/PdbxAnnFeature.py
--rw-r--r--   0 peisach    (502) staff       (20)     9665 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/pdb/PdbxAtomSite.py
--rw-r--r--   0 peisach    (502) staff       (20)    20174 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/pdb/PdbxConnect.py
--rw-r--r--   0 peisach    (502) staff       (20)     2818 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/pdb/PdbxConnectTests.py
--rw-r--r--   0 peisach    (502) staff       (20)     7737 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/pdb/PdbxVersion.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2018-10-10 20:56:01.000000 mmcif.utils-0.25/mmcif_utils/pdb/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-04-07 10:14:43.857219 mmcif.utils-0.25/mmcif_utils/pdbx/
--rw-r--r--   0 peisach    (502) staff       (20)    34349 2020-11-06 20:52:01.000000 mmcif.utils-0.25/mmcif_utils/pdbx/PdbxIo.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/pdbx/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-04-07 10:14:43.860289 mmcif.utils-0.25/mmcif_utils/persist/
--rw-r--r--   0 peisach    (502) staff       (20)     3587 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/persist/LockFile.py
--rw-r--r--   0 peisach    (502) staff       (20)     9228 2018-11-30 17:32:24.000000 mmcif.utils-0.25/mmcif_utils/persist/PdbxCoreIoAdapter.py
--rw-r--r--   0 peisach    (502) staff       (20)    56025 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/persist/PdbxDictionaryInfo.py
--rw-r--r--   0 peisach    (502) staff       (20)    29289 2019-08-18 17:42:19.000000 mmcif.utils-0.25/mmcif_utils/persist/PdbxPersist.py
--rw-r--r--   0 peisach    (502) staff       (20)     6220 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/persist/PdbxPyIoAdapter.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/persist/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-04-07 10:14:43.869406 mmcif.utils-0.25/mmcif_utils/style/
--rw-r--r--   0 peisach    (502) staff       (20)     8930 2020-08-21 20:39:58.000000 mmcif.utils-0.25/mmcif_utils/style/ChemCompCategoryStyle.py
--rw-r--r--   0 peisach    (502) staff       (20)     9116 2022-04-07 10:04:08.000000 mmcif.utils-0.25/mmcif_utils/style/ChemCompCategoryStyleWithOutStndAtom.py
--rw-r--r--   0 peisach    (502) staff       (20)     5104 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/style/ChemCompModelCategoryStyle.py
--rw-r--r--   0 peisach    (502) staff       (20)     7115 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/style/PdbxCategoryStyleBase.py
--rw-r--r--   0 peisach    (502) staff       (20)    43128 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/style/PdbxEmExtensionCategoryStyle.py
--rw-r--r--   0 peisach    (502) staff       (20)    13170 2020-11-06 20:52:01.000000 mmcif.utils-0.25/mmcif_utils/style/PdbxEntryInfoCategoryStyle.py
--rw-r--r--   0 peisach    (502) staff       (20)    11861 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/style/PdbxGeometryReportCategoryStyle.py
--rw-r--r--   0 peisach    (502) staff       (20)     3225 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/style/PdbxItemMappingCategoryStyle.py
--rw-r--r--   0 peisach    (502) staff       (20)     2061 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/style/PdbxLocalMapIndexCategoryStyle.py
--rw-r--r--   0 peisach    (502) staff       (20)     6326 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/style/PdbxMessageCategoryStyle.py
--rw-r--r--   0 peisach    (502) staff       (20)    72178 2021-12-03 18:55:23.000000 mmcif.utils-0.25/mmcif_utils/style/PdbxReportCategoryStyle.py
--rw-r--r--   0 peisach    (502) staff       (20)     2256 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/style/PdbxStatusHistoryCategoryStyle.py
--rw-r--r--   0 peisach    (502) staff       (20)    28868 2022-04-07 10:04:08.000000 mmcif.utils-0.25/mmcif_utils/style/PdbxStyleIoUtil.py
--rw-r--r--   0 peisach    (502) staff       (20)     9642 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/style/PdbxStyleUtilBase.py-save
--rw-r--r--   0 peisach    (502) staff       (20)     8779 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/style/PdbxXrayExpReportCategoryStyle.py
--rw-r--r--   0 peisach    (502) staff       (20)    15738 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/style/PrdCategoryStyle.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/style/__init__.py
--rw-r--r--   0 peisach    (502) staff       (20)     2233 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/style/make-style-from-item-list.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2022-04-07 10:14:43.872547 mmcif.utils-0.25/mmcif_utils/trans/
--rw-r--r--   0 peisach    (502) staff       (20)     9412 2020-08-22 13:16:25.000000 mmcif.utils-0.25/mmcif_utils/trans/DictionaryMapper.py
--rw-r--r--   0 peisach    (502) staff       (20)     1845 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/trans/DictionaryMapperIo.py
--rw-r--r--   0 peisach    (502) staff       (20)     7332 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/trans/FilterCif.py
--rw-r--r--   0 peisach    (502) staff       (20)    21504 2020-08-22 13:21:20.000000 mmcif.utils-0.25/mmcif_utils/trans/InstanceMapper.py
--rw-r--r--   0 peisach    (502) staff       (20)        0 2018-10-10 20:56:02.000000 mmcif.utils-0.25/mmcif_utils/trans/__init__.py
--rwxr-xr-x   0 peisach    (502) staff       (20)      108 2022-04-07 10:14:43.874618 mmcif.utils-0.25/setup.cfg
--rwxr-xr-x   0 peisach    (502) staff       (20)     2062 2022-04-07 10:13:49.000000 mmcif.utils-0.25/setup.py
--rw-r--r--   0 peisach    (502) staff       (20)      411 2020-08-28 16:08:42.000000 mmcif.utils-0.25/tox.ini
+drwxr-xr-x   0 peisach    (502) wheel        (0)        0 2023-06-11 18:27:23.211784 mmcif.utils-0.26/
+-rw-r--r--   0 peisach    (502) wheel        (0)     1578 2023-06-11 18:26:33.000000 mmcif.utils-0.26/HISTORY.txt
+-rw-r--r--   0 peisach    (502) wheel        (0)      552 2023-06-11 18:26:33.000000 mmcif.utils-0.26/LICENSE
+-rw-r--r--   0 peisach    (502) wheel        (0)       97 2023-06-11 18:26:33.000000 mmcif.utils-0.26/MANIFEST.in
+-rw-r--r--   0 peisach    (502) wheel        (0)      712 2023-06-11 18:27:23.211969 mmcif.utils-0.26/PKG-INFO
+-rw-r--r--   0 peisach    (502) wheel        (0)      558 2023-06-11 18:26:33.000000 mmcif.utils-0.26/README.md
+drwxr-xr-x   0 peisach    (502) wheel        (0)        0 2023-06-11 18:27:23.187251 mmcif.utils-0.26/mmcif.utils.egg-info/
+-rw-r--r--   0 peisach    (502) wheel        (0)      712 2023-06-11 18:27:23.000000 mmcif.utils-0.26/mmcif.utils.egg-info/PKG-INFO
+-rw-r--r--   0 peisach    (502) wheel        (0)     2470 2023-06-11 18:27:23.000000 mmcif.utils-0.26/mmcif.utils.egg-info/SOURCES.txt
+-rw-r--r--   0 peisach    (502) wheel        (0)        1 2023-06-11 18:27:23.000000 mmcif.utils-0.26/mmcif.utils.egg-info/dependency_links.txt
+-rw-r--r--   0 peisach    (502) wheel        (0)       62 2023-06-11 18:27:23.000000 mmcif.utils-0.26/mmcif.utils.egg-info/requires.txt
+-rw-r--r--   0 peisach    (502) wheel        (0)       12 2023-06-11 18:27:23.000000 mmcif.utils-0.26/mmcif.utils.egg-info/top_level.txt
+-rw-r--r--   0 peisach    (502) wheel        (0)        1 2023-06-11 18:26:47.000000 mmcif.utils-0.26/mmcif.utils.egg-info/zip-safe
+drwxr-xr-x   0 peisach    (502) wheel        (0)        0 2023-06-11 18:27:23.187740 mmcif.utils-0.26/mmcif_utils/
+-rw-r--r--   0 peisach    (502) wheel        (0)      195 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/__init__.py
+drwxr-xr-x   0 peisach    (502) wheel        (0)        0 2023-06-11 18:27:23.191290 mmcif.utils-0.26/mmcif_utils/bird/
+-rw-r--r--   0 peisach    (502) wheel        (0)     6730 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/bird/PdbxBirdIndex.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     4634 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/bird/PdbxFamilyIo.py
+-rw-r--r--   0 peisach    (502) wheel        (0)    18362 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/bird/PdbxPrd.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     4588 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/bird/PdbxPrdCcIo.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     4472 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/bird/PdbxPrdIo.py
+-rw-r--r--   0 peisach    (502) wheel        (0)    18294 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/bird/PdbxPrdUtils.py
+-rw-r--r--   0 peisach    (502) wheel        (0)        0 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/bird/__init__.py
+drwxr-xr-x   0 peisach    (502) wheel        (0)        0 2023-06-11 18:27:23.192166 mmcif.utils-0.26/mmcif_utils/bird/cl/
+-rw-r--r--   0 peisach    (502) wheel        (0)    22027 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/bird/cl/PdbxPrdExec.py
+-rw-r--r--   0 peisach    (502) wheel        (0)        0 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/bird/cl/__init__.py
+drwxr-xr-x   0 peisach    (502) wheel        (0)        0 2023-06-11 18:27:23.194716 mmcif.utils-0.26/mmcif_utils/chemcomp/
+-rw-r--r--   0 peisach    (502) wheel        (0)     8321 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/chemcomp/PdbxChemComp.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     4579 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/chemcomp/PdbxChemCompIo.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     7194 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/chemcomp/PdbxChemCompModel.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     3157 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/chemcomp/PdbxChemCompModelIo.py
+-rw-r--r--   0 peisach    (502) wheel        (0)    26793 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/chemcomp/PdbxChemCompUtils.py
+-rw-r--r--   0 peisach    (502) wheel        (0)        0 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/chemcomp/__init__.py
+drwxr-xr-x   0 peisach    (502) wheel        (0)        0 2023-06-11 18:27:23.195917 mmcif.utils-0.26/mmcif_utils/inventory/
+-rw-r--r--   0 peisach    (502) wheel        (0)     3699 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/inventory/InventoryIo.py
+-rw-r--r--   0 peisach    (502) wheel        (0)    11245 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/inventory/InventoryIoBatchRunner.py
+-rw-r--r--   0 peisach    (502) wheel        (0)        0 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/inventory/__init__.py
+drwxr-xr-x   0 peisach    (502) wheel        (0)        0 2023-06-11 18:27:23.196923 mmcif.utils-0.26/mmcif_utils/message/
+-rw-r--r--   0 peisach    (502) wheel        (0)    12138 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/message/PdbxMessage.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     4173 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/message/PdbxMessageIo.py
+-rw-r--r--   0 peisach    (502) wheel        (0)        0 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/message/__init__.py
+drwxr-xr-x   0 peisach    (502) wheel        (0)        0 2023-06-11 18:27:23.199612 mmcif.utils-0.26/mmcif_utils/pdb/
+-rw-r--r--   0 peisach    (502) wheel        (0)    16392 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/pdb/PdbxAnnFeature.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     9665 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/pdb/PdbxAtomSite.py
+-rw-r--r--   0 peisach    (502) wheel        (0)    20174 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/pdb/PdbxConnect.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     2818 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/pdb/PdbxConnectTests.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     7737 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/pdb/PdbxVersion.py
+-rw-r--r--   0 peisach    (502) wheel        (0)        0 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/pdb/__init__.py
+drwxr-xr-x   0 peisach    (502) wheel        (0)        0 2023-06-11 18:27:23.200850 mmcif.utils-0.26/mmcif_utils/pdbx/
+-rw-r--r--   0 peisach    (502) wheel        (0)    34349 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/pdbx/PdbxIo.py
+-rw-r--r--   0 peisach    (502) wheel        (0)        0 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/pdbx/__init__.py
+drwxr-xr-x   0 peisach    (502) wheel        (0)        0 2023-06-11 18:27:23.203624 mmcif.utils-0.26/mmcif_utils/persist/
+-rw-r--r--   0 peisach    (502) wheel        (0)     3587 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/persist/LockFile.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     9228 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/persist/PdbxCoreIoAdapter.py
+-rw-r--r--   0 peisach    (502) wheel        (0)    56025 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/persist/PdbxDictionaryInfo.py
+-rw-r--r--   0 peisach    (502) wheel        (0)    29289 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/persist/PdbxPersist.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     6220 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/persist/PdbxPyIoAdapter.py
+-rw-r--r--   0 peisach    (502) wheel        (0)        0 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/persist/__init__.py
+drwxr-xr-x   0 peisach    (502) wheel        (0)        0 2023-06-11 18:27:23.209637 mmcif.utils-0.26/mmcif_utils/style/
+-rw-r--r--   0 peisach    (502) wheel        (0)     8930 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/ChemCompCategoryStyle.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     9116 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/ChemCompCategoryStyleWithOutStndAtom.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     5104 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/ChemCompModelCategoryStyle.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     7115 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/PdbxCategoryStyleBase.py
+-rw-r--r--   0 peisach    (502) wheel        (0)    43128 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/PdbxEmExtensionCategoryStyle.py
+-rw-r--r--   0 peisach    (502) wheel        (0)    13170 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/PdbxEntryInfoCategoryStyle.py
+-rw-r--r--   0 peisach    (502) wheel        (0)    11861 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/PdbxGeometryReportCategoryStyle.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     3225 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/PdbxItemMappingCategoryStyle.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     2061 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/PdbxLocalMapIndexCategoryStyle.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     6326 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/PdbxMessageCategoryStyle.py
+-rw-r--r--   0 peisach    (502) wheel        (0)    72178 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/PdbxReportCategoryStyle.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     2256 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/PdbxStatusHistoryCategoryStyle.py
+-rw-r--r--   0 peisach    (502) wheel        (0)    28868 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/PdbxStyleIoUtil.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     8779 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/PdbxXrayExpReportCategoryStyle.py
+-rw-r--r--   0 peisach    (502) wheel        (0)    15738 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/PrdCategoryStyle.py
+-rw-r--r--   0 peisach    (502) wheel        (0)        0 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/__init__.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     2233 2023-06-11 18:26:33.000000 mmcif.utils-0.26/mmcif_utils/style/make-style-from-item-list.py
+drwxr-xr-x   0 peisach    (502) wheel        (0)        0 2023-06-11 18:27:23.211552 mmcif.utils-0.26/mmcif_utils/trans/
+-rw-r--r--   0 peisach    (502) wheel        (0)     9412 2023-06-11 18:26:34.000000 mmcif.utils-0.26/mmcif_utils/trans/DictionaryMapper.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     1845 2023-06-11 18:26:34.000000 mmcif.utils-0.26/mmcif_utils/trans/DictionaryMapperIo.py
+-rw-r--r--   0 peisach    (502) wheel        (0)     7332 2023-06-11 18:26:34.000000 mmcif.utils-0.26/mmcif_utils/trans/FilterCif.py
+-rw-r--r--   0 peisach    (502) wheel        (0)    21504 2023-06-11 18:26:34.000000 mmcif.utils-0.26/mmcif_utils/trans/InstanceMapper.py
+-rw-r--r--   0 peisach    (502) wheel        (0)        0 2023-06-11 18:26:34.000000 mmcif.utils-0.26/mmcif_utils/trans/__init__.py
+-rwxr-xr-x   0 peisach    (502) wheel        (0)      108 2023-06-11 18:27:23.212566 mmcif.utils-0.26/setup.cfg
+-rwxr-xr-x   0 peisach    (502) wheel        (0)     2062 2023-06-11 18:26:34.000000 mmcif.utils-0.26/setup.py
```

### Comparing `mmcif.utils-0.25/HISTORY.txt` & `mmcif.utils-0.26/HISTORY.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 25-Nov-2019  - v0.19 Fixes for python 3.8
 11-Jan-2020  - v0.20 In ChemCompCategoryStyle add ordinal to pdbx_chem_comp_synonyms. Test dependency order fix.
 28-Aug-2020  - v0.21 Correct em->emd translator when copying key from_parent. Python 3.8 support
 05-Nov-2020  - v0.22 Support parsing of em_depui category.
 03-May-2020  - v0.23 In PdbxStyleIoUtil() drop passing logtag to IoAdapter which no longer supports
 03-Dec-2021  - v0.24 In PdbxReportCategoryStyle() correct _struct_ref_seq_dif.pdbx_pdb_strand_id
 06-Apr-2022  - v0.25 Add ChemCompCategoryStyleWithOutStndAtom.py. Add "styleObject" parameter to PdbxPrdCcIo.py & PdbxChemCompIo.py
-
+11-Jun-2023  - v0.26 Adjust hash paths for CCD layout when length > 3
```

### Comparing `mmcif.utils-0.25/LICENSE` & `mmcif.utils-0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/PKG-INFO` & `mmcif.utils-0.26/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: mmcif.utils
-Version: 0.25
+Version: 0.26
 Summary: mmCIF Utility Classes
 Home-page: http://mmcif.wwpdb.org
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 See:  README.md
-
```

### Comparing `mmcif.utils-0.25/README.md` & `mmcif.utils-0.26/README.md`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif.utils.egg-info/PKG-INFO` & `mmcif.utils-0.26/mmcif.utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: mmcif.utils
-Version: 0.25
+Version: 0.26
 Summary: mmCIF Utility Classes
 Home-page: http://mmcif.wwpdb.org
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 See:  README.md
-
```

### Comparing `mmcif.utils-0.25/mmcif.utils.egg-info/SOURCES.txt` & `mmcif.utils-0.26/mmcif.utils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-.gitignore
 HISTORY.txt
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
-tox.ini
 mmcif.utils.egg-info/PKG-INFO
 mmcif.utils.egg-info/SOURCES.txt
 mmcif.utils.egg-info/dependency_links.txt
 mmcif.utils.egg-info/requires.txt
 mmcif.utils.egg-info/top_level.txt
 mmcif.utils.egg-info/zip-safe
 mmcif_utils/__init__.py
 mmcif_utils/bird/PdbxBirdIndex.py
 mmcif_utils/bird/PdbxFamilyIo.py
 mmcif_utils/bird/PdbxPrd.py
 mmcif_utils/bird/PdbxPrdCcIo.py
 mmcif_utils/bird/PdbxPrdIo.py
 mmcif_utils/bird/PdbxPrdUtils.py
 mmcif_utils/bird/__init__.py
-mmcif_utils/bird/cl/Example-commands.sh
 mmcif_utils/bird/cl/PdbxPrdExec.py
-mmcif_utils/bird/cl/REF_ONLY_CC.LIST
 mmcif_utils/bird/cl/__init__.py
 mmcif_utils/chemcomp/PdbxChemComp.py
 mmcif_utils/chemcomp/PdbxChemCompIo.py
 mmcif_utils/chemcomp/PdbxChemCompModel.py
 mmcif_utils/chemcomp/PdbxChemCompModelIo.py
 mmcif_utils/chemcomp/PdbxChemCompUtils.py
 mmcif_utils/chemcomp/__init__.py
@@ -59,15 +55,14 @@
 mmcif_utils/style/PdbxGeometryReportCategoryStyle.py
 mmcif_utils/style/PdbxItemMappingCategoryStyle.py
 mmcif_utils/style/PdbxLocalMapIndexCategoryStyle.py
 mmcif_utils/style/PdbxMessageCategoryStyle.py
 mmcif_utils/style/PdbxReportCategoryStyle.py
 mmcif_utils/style/PdbxStatusHistoryCategoryStyle.py
 mmcif_utils/style/PdbxStyleIoUtil.py
-mmcif_utils/style/PdbxStyleUtilBase.py-save
 mmcif_utils/style/PdbxXrayExpReportCategoryStyle.py
 mmcif_utils/style/PrdCategoryStyle.py
 mmcif_utils/style/__init__.py
 mmcif_utils/style/make-style-from-item-list.py
 mmcif_utils/trans/DictionaryMapper.py
 mmcif_utils/trans/DictionaryMapperIo.py
 mmcif_utils/trans/FilterCif.py
```

### Comparing `mmcif.utils-0.25/mmcif_utils/bird/PdbxBirdIndex.py` & `mmcif.utils-0.26/mmcif_utils/bird/PdbxBirdIndex.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/bird/PdbxFamilyIo.py` & `mmcif.utils-0.26/mmcif_utils/bird/PdbxFamilyIo.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/bird/PdbxPrd.py` & `mmcif.utils-0.26/mmcif_utils/bird/PdbxPrd.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/bird/PdbxPrdCcIo.py` & `mmcif.utils-0.26/mmcif_utils/bird/PdbxPrdCcIo.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/bird/PdbxPrdIo.py` & `mmcif.utils-0.26/mmcif_utils/bird/PdbxPrdIo.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/bird/PdbxPrdUtils.py` & `mmcif.utils-0.26/mmcif_utils/bird/PdbxPrdUtils.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/bird/cl/PdbxPrdExec.py` & `mmcif.utils-0.26/mmcif_utils/bird/cl/PdbxPrdExec.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/chemcomp/PdbxChemComp.py` & `mmcif.utils-0.26/mmcif_utils/chemcomp/PdbxChemComp.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/chemcomp/PdbxChemCompIo.py` & `mmcif.utils-0.26/mmcif_utils/chemcomp/PdbxChemCompIo.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,16 @@
         """ Set the identifier for the target chemical component.   The internal target file path
             is set to the chemmical component definition file stored in the organization of
             CVS repository for chemical components if this exists.
 
             returns True for success or False otherwise.
         """
         self.__ccU = compId.upper()
-        self.__filePath = os.path.join(self.__topCachePath, self.__ccU[0:1], self.__ccU, self.__ccU + '.cif')
+        hashd = self.__getCcdHash(self.__ccU)
+        self.__filePath = os.path.join(self.__topCachePath, hashd, self.__ccU, self.__ccU + '.cif')
         if self.readFile(self.__filePath):
             return self.setContainer(containerName=self.__ccU)
         else:
             return False
 
     def getCategory(self, catName='chem_comp'):
         return self.getItemDictList(catName)
@@ -123,7 +124,19 @@
         return self.newContainer(containerName=blockId)
 
     def update(self, catName, attributeName, value, iRow=0):
         return self.updateAttribute(catName, attributeName, value, iRow=iRow)
 
     def write(self, filePath):
         return self.writeFile(filePath)
+
+    def __getCcdHash(self, idCode):
+        """Returns the hash code for a CCD id.  Currently first letter"""
+        if not idCode:
+            return None
+
+        if len(idCode) > 3:
+            hash_key = idCode.upper()[-2:]
+        else:
+            hash_key = idCode.upper()[0]
+
+        return hash_key
```

### Comparing `mmcif.utils-0.25/mmcif_utils/chemcomp/PdbxChemCompModel.py` & `mmcif.utils-0.26/mmcif_utils/chemcomp/PdbxChemCompModel.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/chemcomp/PdbxChemCompModelIo.py` & `mmcif.utils-0.26/mmcif_utils/chemcomp/PdbxChemCompModelIo.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/chemcomp/PdbxChemCompUtils.py` & `mmcif.utils-0.26/mmcif_utils/chemcomp/PdbxChemCompUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,16 @@
 
     def setCompId(self, compId):
         """ Set the identifier for the target chemical component.   The internal target file path
             is set to the chemmical component definition file stored in the organization of
             CVS repository for chemical components if this exists.
         """
         self.__ccU = compId.upper()
-        self.__filePath = os.path.join(self.__topCachePath, self.__ccU[0:1], self.__ccU, self.__ccU + '.cif')
+        hashd = self.__getCcdHash(self.__ccU)
+        self.__filePath = os.path.join(self.__topCachePath, hashd, self.__ccU, self.__ccU + '.cif')
         if (not os.access(self.__filePath, os.R_OK)):
             if (self.__verbose):
                 logger.debug("+ERROR- PdbxChemCompReader.setCompId() Missing file %s\n" % self.__filePath)
             return False
         return True
 
     def setFilePath(self, filePath, compId=None):
@@ -441,14 +442,25 @@
     def __attributePart(self, name):
         i = name.find(".")
         if i == -1:
             return None
         else:
             return name[i + 1:]
 
+    def __getCcdHash(self, idCode):
+        """Returns the hash code for a CCD id.  Currently first letter"""
+        if not idCode:
+            return None
+
+        if len(idCode) > 3:
+            hash_key = idCode.upper()[-2:]
+        else:
+            hash_key = idCode.upper()[0]
+
+        return hash_key
 
 class PdbxChemCompUpdater(object):
     ''' Utility methods for updating chemical component definition data files.
 
     '''
 
     def __init__(self, verbose=True, log=sys.stderr):
```

### Comparing `mmcif.utils-0.25/mmcif_utils/inventory/InventoryIo.py` & `mmcif.utils-0.26/mmcif_utils/inventory/InventoryIo.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/inventory/InventoryIoBatchRunner.py` & `mmcif.utils-0.26/mmcif_utils/inventory/InventoryIoBatchRunner.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/message/PdbxMessage.py` & `mmcif.utils-0.26/mmcif_utils/message/PdbxMessage.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/message/PdbxMessageIo.py` & `mmcif.utils-0.26/mmcif_utils/message/PdbxMessageIo.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/pdb/PdbxAnnFeature.py` & `mmcif.utils-0.26/mmcif_utils/pdb/PdbxAnnFeature.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/pdb/PdbxAtomSite.py` & `mmcif.utils-0.26/mmcif_utils/pdb/PdbxAtomSite.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/pdb/PdbxConnect.py` & `mmcif.utils-0.26/mmcif_utils/pdb/PdbxConnect.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/pdb/PdbxConnectTests.py` & `mmcif.utils-0.26/mmcif_utils/pdb/PdbxConnectTests.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/pdb/PdbxVersion.py` & `mmcif.utils-0.26/mmcif_utils/pdb/PdbxVersion.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/pdbx/PdbxIo.py` & `mmcif.utils-0.26/mmcif_utils/pdbx/PdbxIo.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/persist/LockFile.py` & `mmcif.utils-0.26/mmcif_utils/persist/LockFile.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/persist/PdbxCoreIoAdapter.py` & `mmcif.utils-0.26/mmcif_utils/persist/PdbxCoreIoAdapter.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/persist/PdbxDictionaryInfo.py` & `mmcif.utils-0.26/mmcif_utils/persist/PdbxDictionaryInfo.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/persist/PdbxPersist.py` & `mmcif.utils-0.26/mmcif_utils/persist/PdbxPersist.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/persist/PdbxPyIoAdapter.py` & `mmcif.utils-0.26/mmcif_utils/persist/PdbxPyIoAdapter.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/ChemCompCategoryStyle.py` & `mmcif.utils-0.26/mmcif_utils/style/ChemCompCategoryStyle.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/ChemCompCategoryStyleWithOutStndAtom.py` & `mmcif.utils-0.26/mmcif_utils/style/ChemCompCategoryStyleWithOutStndAtom.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/ChemCompModelCategoryStyle.py` & `mmcif.utils-0.26/mmcif_utils/style/ChemCompModelCategoryStyle.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/PdbxCategoryStyleBase.py` & `mmcif.utils-0.26/mmcif_utils/style/PdbxCategoryStyleBase.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/PdbxEmExtensionCategoryStyle.py` & `mmcif.utils-0.26/mmcif_utils/style/PdbxEmExtensionCategoryStyle.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/PdbxEntryInfoCategoryStyle.py` & `mmcif.utils-0.26/mmcif_utils/style/PdbxEntryInfoCategoryStyle.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/PdbxGeometryReportCategoryStyle.py` & `mmcif.utils-0.26/mmcif_utils/style/PdbxGeometryReportCategoryStyle.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/PdbxItemMappingCategoryStyle.py` & `mmcif.utils-0.26/mmcif_utils/style/PdbxItemMappingCategoryStyle.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/PdbxLocalMapIndexCategoryStyle.py` & `mmcif.utils-0.26/mmcif_utils/style/PdbxLocalMapIndexCategoryStyle.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/PdbxMessageCategoryStyle.py` & `mmcif.utils-0.26/mmcif_utils/style/PdbxMessageCategoryStyle.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/PdbxReportCategoryStyle.py` & `mmcif.utils-0.26/mmcif_utils/style/PdbxReportCategoryStyle.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/PdbxStatusHistoryCategoryStyle.py` & `mmcif.utils-0.26/mmcif_utils/style/PdbxStatusHistoryCategoryStyle.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/PdbxStyleIoUtil.py` & `mmcif.utils-0.26/mmcif_utils/style/PdbxStyleIoUtil.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/PdbxXrayExpReportCategoryStyle.py` & `mmcif.utils-0.26/mmcif_utils/style/PdbxXrayExpReportCategoryStyle.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/PrdCategoryStyle.py` & `mmcif.utils-0.26/mmcif_utils/style/PrdCategoryStyle.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/style/make-style-from-item-list.py` & `mmcif.utils-0.26/mmcif_utils/style/make-style-from-item-list.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/trans/DictionaryMapper.py` & `mmcif.utils-0.26/mmcif_utils/trans/DictionaryMapper.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/trans/DictionaryMapperIo.py` & `mmcif.utils-0.26/mmcif_utils/trans/DictionaryMapperIo.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/trans/FilterCif.py` & `mmcif.utils-0.26/mmcif_utils/trans/FilterCif.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/mmcif_utils/trans/InstanceMapper.py` & `mmcif.utils-0.26/mmcif_utils/trans/InstanceMapper.py`

 * *Files identical despite different names*

### Comparing `mmcif.utils-0.25/setup.py` & `mmcif.utils-0.26/setup.py`

 * *Files identical despite different names*

