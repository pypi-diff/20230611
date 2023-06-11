# Comparing `tmp/pcdl-3.1.5.tar.gz` & `tmp/pcdl-3.1.6.tar.gz`

## Comparing `pcdl-3.1.5.tar` & `pcdl-3.1.6.tar`

### file list

```diff
@@ -1,24 +1,190 @@
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/__init__.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/pdplt.py
--rw-r--r--   0        0        0    55191 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/pyMCDS.py
--rw-r--r--   0        0        0    18951 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/pyMCDSts.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/ALL_CITATIONS.txt
--rw-r--r--   0        0        0    16071 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/PhysiCell_settings.xml
--rw-r--r--   0        0        0   230391 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/initial.svg
--rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/initial.xml
--rw-r--r--   0        0        0   135425 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/initial_attached_cells_graph.txt
--rw-r--r--   0        0        0   135425 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/initial_cell_neighbor_graph.txt
--rw-r--r--   0        0        0 14507089 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/initial_cells.mat
--rw-r--r--   0        0        0    42616 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/initial_mesh0.mat
--rw-r--r--   0        0        0    63935 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/initial_microenvironment0.mat
--rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/output00000000.xml
--rw-r--r--   0        0        0   135425 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/output00000000_attached_cells_graph.txt
--rw-r--r--   0        0        0   135425 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/output00000000_cell_neighbor_graph.txt
--rw-r--r--   0        0        0 14507089 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/output00000000_cells.mat
--rw-r--r--   0        0        0    63935 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/output00000000_microenvironment0.mat
--rw-r--r--   0        0        0   230391 2020-02-02 00:00:00.000000 pcdl-3.1.5/pcdl/data_timeseries_3d/snapshot00000000.svg
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pcdl-3.1.5/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 pcdl-3.1.5/LICENSE
--rw-r--r--   0        0        0     8481 2020-02-02 00:00:00.000000 pcdl-3.1.5/README.md
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 pcdl-3.1.5/pyproject.toml
--rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 pcdl-3.1.5/PKG-INFO
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/__init__.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/pdplt.py
+-rw-r--r--   0        0        0    55191 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/pyMCDS.py
+-rw-r--r--   0        0        0    18951 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/pyMCDSts.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/ALL_CITATIONS.txt
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/PhysiCell_settings.xml
+-rw-r--r--   0        0        0   313850 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/final.svg
+-rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/final.xml
+-rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/final_attached_cells_graph.txt
+-rw-r--r--   0        0        0    17815 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/final_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   685801 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/final_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/final_microenvironment0.mat
+-rw-r--r--   0        0        0   254328 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/initial.svg
+-rw-r--r--   0        0        0     8243 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/initial.xml
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/initial_attached_cells_graph.txt
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/initial_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   554761 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/initial_cells.mat
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/initial_mesh0.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/initial_microenvironment0.mat
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/legend.svg
+-rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000000.xml
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000000_attached_cells_graph.txt
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000000_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   554761 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000000_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000000_microenvironment0.mat
+-rw-r--r--   0        0        0     8272 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000001.xml
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000001_attached_cells_graph.txt
+-rw-r--r--   0        0        0    10443 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000001_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   560377 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000001_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000001_microenvironment0.mat
+-rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000002.xml
+-rw-r--r--   0        0        0     5319 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000002_attached_cells_graph.txt
+-rw-r--r--   0        0        0    10669 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000002_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   564745 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000002_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000002_microenvironment0.mat
+-rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000003.xml
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000003_attached_cells_graph.txt
+-rw-r--r--   0        0        0    10877 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000003_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   570985 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000003_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000003_microenvironment0.mat
+-rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000004.xml
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000004_attached_cells_graph.txt
+-rw-r--r--   0        0        0    11006 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000004_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   574729 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000004_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000004_microenvironment0.mat
+-rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000005.xml
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000005_attached_cells_graph.txt
+-rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000005_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   577849 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000005_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000005_microenvironment0.mat
+-rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000006.xml
+-rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000006_attached_cells_graph.txt
+-rw-r--r--   0        0        0    11322 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000006_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   582217 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000006_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000006_microenvironment0.mat
+-rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000007.xml
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000007_attached_cells_graph.txt
+-rw-r--r--   0        0        0    11561 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000007_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   586585 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000007_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000007_microenvironment0.mat
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000008.xml
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000008_attached_cells_graph.txt
+-rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000008_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   594697 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000008_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000008_microenvironment0.mat
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000009.xml
+-rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000009_attached_cells_graph.txt
+-rw-r--r--   0        0        0    12262 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000009_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   601561 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000009_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000009_microenvironment0.mat
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000010.xml
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000010_attached_cells_graph.txt
+-rw-r--r--   0        0        0    12613 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000010_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   607801 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000010_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000010_microenvironment0.mat
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000011.xml
+-rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000011_attached_cells_graph.txt
+-rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000011_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   615289 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000011_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000011_microenvironment0.mat
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000012.xml
+-rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000012_attached_cells_graph.txt
+-rw-r--r--   0        0        0    13228 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000012_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   619033 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000012_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000012_microenvironment0.mat
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000013.xml
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000013_attached_cells_graph.txt
+-rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000013_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   624649 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000013_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000013_microenvironment0.mat
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000014.xml
+-rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000014_attached_cells_graph.txt
+-rw-r--r--   0        0        0    13994 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000014_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   632137 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000014_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000014_microenvironment0.mat
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000015.xml
+-rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000015_attached_cells_graph.txt
+-rw-r--r--   0        0        0    14046 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000015_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   634009 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000015_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000015_microenvironment0.mat
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000016.xml
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000016_attached_cells_graph.txt
+-rw-r--r--   0        0        0    14441 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000016_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   639625 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000016_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000016_microenvironment0.mat
+-rw-r--r--   0        0        0     8275 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000017.xml
+-rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000017_attached_cells_graph.txt
+-rw-r--r--   0        0        0    14602 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000017_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   642745 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000017_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000017_microenvironment0.mat
+-rw-r--r--   0        0        0     8275 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000018.xml
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000018_attached_cells_graph.txt
+-rw-r--r--   0        0        0    15119 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000018_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   650857 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000018_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000018_microenvironment0.mat
+-rw-r--r--   0        0        0     8275 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000019.xml
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000019_attached_cells_graph.txt
+-rw-r--r--   0        0        0    15489 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000019_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   655849 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000019_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000019_microenvironment0.mat
+-rw-r--r--   0        0        0     8275 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000020.xml
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000020_attached_cells_graph.txt
+-rw-r--r--   0        0        0    15921 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000020_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   661465 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000020_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000020_microenvironment0.mat
+-rw-r--r--   0        0        0     8275 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000021.xml
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000021_attached_cells_graph.txt
+-rw-r--r--   0        0        0    16246 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000021_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   665833 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000021_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000021_microenvironment0.mat
+-rw-r--r--   0        0        0     8275 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000022.xml
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000022_attached_cells_graph.txt
+-rw-r--r--   0        0        0    16633 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000022_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   670201 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000022_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000022_microenvironment0.mat
+-rw-r--r--   0        0        0     8275 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000023.xml
+-rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000023_attached_cells_graph.txt
+-rw-r--r--   0        0        0    16918 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000023_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   675817 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000023_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000023_microenvironment0.mat
+-rw-r--r--   0        0        0     8275 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000024.xml
+-rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000024_attached_cells_graph.txt
+-rw-r--r--   0        0        0    17808 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000024_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0   685801 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000024_cells.mat
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/output00000024_microenvironment0.mat
+-rw-r--r--   0        0        0   254328 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000000.svg
+-rw-r--r--   0        0        0   257071 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000001.svg
+-rw-r--r--   0        0        0   259013 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000002.svg
+-rw-r--r--   0        0        0   261847 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000003.svg
+-rw-r--r--   0        0        0   263541 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000004.svg
+-rw-r--r--   0        0        0   264942 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000005.svg
+-rw-r--r--   0        0        0   266956 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000006.svg
+-rw-r--r--   0        0        0   268880 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000007.svg
+-rw-r--r--   0        0        0   272540 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000008.svg
+-rw-r--r--   0        0        0   275696 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000009.svg
+-rw-r--r--   0        0        0   278516 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000010.svg
+-rw-r--r--   0        0        0   281847 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000011.svg
+-rw-r--r--   0        0        0   283560 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000012.svg
+-rw-r--r--   0        0        0   286112 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000013.svg
+-rw-r--r--   0        0        0   289482 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000014.svg
+-rw-r--r--   0        0        0   290340 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000015.svg
+-rw-r--r--   0        0        0   292888 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000016.svg
+-rw-r--r--   0        0        0   294281 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000017.svg
+-rw-r--r--   0        0        0   298014 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000018.svg
+-rw-r--r--   0        0        0   300295 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000019.svg
+-rw-r--r--   0        0        0   302842 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000020.svg
+-rw-r--r--   0        0        0   304767 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000021.svg
+-rw-r--r--   0        0        0   306732 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000022.svg
+-rw-r--r--   0        0        0   309307 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000023.svg
+-rw-r--r--   0        0        0   313853 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_2d/snapshot00000024.svg
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/ALL_CITATIONS.txt
+-rw-r--r--   0        0        0    16071 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/PhysiCell_settings.xml
+-rw-r--r--   0        0        0   230391 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/initial.svg
+-rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/initial.xml
+-rw-r--r--   0        0        0   135425 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/initial_attached_cells_graph.txt
+-rw-r--r--   0        0        0   135425 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/initial_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0 14507089 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/initial_cells.mat
+-rw-r--r--   0        0        0    42616 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/initial_mesh0.mat
+-rw-r--r--   0        0        0    63935 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/initial_microenvironment0.mat
+-rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/output00000000.xml
+-rw-r--r--   0        0        0   135425 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/output00000000_attached_cells_graph.txt
+-rw-r--r--   0        0        0   135425 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/output00000000_cell_neighbor_graph.txt
+-rw-r--r--   0        0        0 14507089 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/output00000000_cells.mat
+-rw-r--r--   0        0        0    63935 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/output00000000_microenvironment0.mat
+-rw-r--r--   0        0        0   230391 2020-02-02 00:00:00.000000 pcdl-3.1.6/pcdl/data_timeseries_3d/snapshot00000000.svg
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pcdl-3.1.6/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 pcdl-3.1.6/LICENSE
+-rw-r--r--   0        0        0     8481 2020-02-02 00:00:00.000000 pcdl-3.1.6/README.md
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 pcdl-3.1.6/pyproject.toml
+-rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 pcdl-3.1.6/PKG-INFO
```

### Comparing `pcdl-3.1.5/pcdl/pdplt.py` & `pcdl-3.1.6/pcdl/pdplt.py`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/pyMCDS.py` & `pcdl-3.1.6/pcdl/pyMCDS.py`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/pyMCDSts.py` & `pcdl-3.1.6/pcdl/pyMCDSts.py`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/ALL_CITATIONS.txt` & `pcdl-3.1.6/pcdl/data_timeseries_3d/ALL_CITATIONS.txt`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/PhysiCell_settings.xml` & `pcdl-3.1.6/pcdl/data_timeseries_3d/PhysiCell_settings.xml`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/initial.svg` & `pcdl-3.1.6/pcdl/data_timeseries_3d/initial.svg`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/initial.xml` & `pcdl-3.1.6/pcdl/data_timeseries_3d/initial.xml`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/initial_attached_cells_graph.txt` & `pcdl-3.1.6/pcdl/data_timeseries_3d/initial_attached_cells_graph.txt`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/initial_cell_neighbor_graph.txt` & `pcdl-3.1.6/pcdl/data_timeseries_3d/initial_cell_neighbor_graph.txt`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/initial_cells.mat` & `pcdl-3.1.6/pcdl/data_timeseries_3d/initial_cells.mat`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/initial_mesh0.mat` & `pcdl-3.1.6/pcdl/data_timeseries_3d/initial_mesh0.mat`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/initial_microenvironment0.mat` & `pcdl-3.1.6/pcdl/data_timeseries_3d/initial_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/output00000000.xml` & `pcdl-3.1.6/pcdl/data_timeseries_3d/output00000000.xml`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/output00000000_attached_cells_graph.txt` & `pcdl-3.1.6/pcdl/data_timeseries_3d/output00000000_attached_cells_graph.txt`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/output00000000_cell_neighbor_graph.txt` & `pcdl-3.1.6/pcdl/data_timeseries_3d/output00000000_cell_neighbor_graph.txt`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/output00000000_cells.mat` & `pcdl-3.1.6/pcdl/data_timeseries_3d/output00000000_cells.mat`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/output00000000_microenvironment0.mat` & `pcdl-3.1.6/pcdl/data_timeseries_3d/output00000000_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pcdl/data_timeseries_3d/snapshot00000000.svg` & `pcdl-3.1.6/pcdl/data_timeseries_3d/snapshot00000000.svg`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/LICENSE` & `pcdl-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/README.md` & `pcdl-3.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pcdl-3.1.5/pyproject.toml` & `pcdl-3.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 build-backend = "hatchling.build"
 
 [project]
 # name of the project
 # pip install pcdl
 # import pcdl
 name = "pcdl"  # Required
-version = "3.1.5" # Required
+version = "3.1.6" # Required
 
 description = "physicell data loader (pcdl) provides a platform independent, python3 based, pip installable interface to load output, generated with the PhysiCell agent based modeling framework, into python3."  # Optional
 readme = "README.md"
 
 requires-python = ">=3.6, <4"
 
 license = "BSD-3-Clause"
@@ -74,18 +74,18 @@
 Documentation = "https://github.com/elmbeech/physicelldataloader/tree/master/man"
 Issues = "https://github.com/elmbeech/physicelldataloader/issues"
 Source = "https://github.com/elmbeech/physicelldataloader"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/pcdl",
+    "/pcdl/data_timeseries_2d",
     "/pcdl/data_timeseries_3d",
 ]
 exclude = [
-    "/pcdl/data_timeseries_2d",
     "/.pytest_cache",
     "/test",
 ]
 
 # setuptool
 #[tool.setuptools.packages.find]
 #include = ["pcdl"]
```

### Comparing `pcdl-3.1.5/PKG-INFO` & `pcdl-3.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdl
-Version: 3.1.5
+Version: 3.1.6
 Summary: physicell data loader (pcdl) provides a platform independent, python3 based, pip installable interface to load output, generated with the PhysiCell agent based modeling framework, into python3.
 Project-URL: Homepage lab, http://www.mathcancer.org/
 Project-URL: Homepage project, http://physicell.org/
 Project-URL: Hompage, https://github.com/elmbeech/physicelldataloader
 Project-URL: Documentation, https://github.com/elmbeech/physicelldataloader/tree/master/man
 Project-URL: Issues, https://github.com/elmbeech/physicelldataloader/issues
 Project-URL: Source, https://github.com/elmbeech/physicelldataloader
```

