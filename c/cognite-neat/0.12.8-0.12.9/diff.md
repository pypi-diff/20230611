# Comparing `tmp/cognite_neat-0.12.8.tar.gz` & `tmp/cognite_neat-0.12.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.12.8.tar", max compression
+gzip compressed data, was "cognite_neat-0.12.9.tar", max compression
```

## Comparing `cognite_neat-0.12.8.tar` & `cognite_neat-0.12.9.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0    11351 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/LICENSE
--rw-r--r--   0        0        0     8765 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/README.md
--rw-r--r--   0        0        0       23 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/__init__.py
--rw-r--r--   0        0        0      761 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2652 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/app.py
--rw-r--r--   0        0        0     1344 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0      408 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/data_classes/__init__.py
--rw-r--r--   0        0        0     4775 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/data_classes/config.py
--rw-r--r--   0        0        0     8132 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/data_classes/rules.py
--rw-r--r--   0        0        0    30296 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/data_classes/transformation_rules.py
--rw-r--r--   0        0        0        0 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     1520 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/data_stores/metrics.py
--rw-r--r--   0        0        0     9436 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0      646 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     5449 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/extractors/graph_sheet_to_graph.py
--rw-r--r--   0        0        0     2250 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/extractors/labels.py
--rw-r--r--   0        0        0    37510 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/extractors/rdf_to_assets.py
--rw-r--r--   0        0        0    17870 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/extractors/rdf_to_relationships.py
--rw-r--r--   0        0        0     5400 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
--rw-r--r--   0        0        0     6700 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/extractors/rules_to_graphql.py
--rw-r--r--   0        0        0      138 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0      938 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/loader/graph_capturing_sheet.py
--rw-r--r--   0        0        0    10647 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0      913 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/loader/rules.py
--rw-r--r--   0        0        0        0 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    10373 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0    15303 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/modeler.py
--rw-r--r--   0        0        0      110 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/parser/__init__.py
--rw-r--r--   0        0        0     1727 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/parser/transformation_rules.py
--rw-r--r--   0        0        0       73 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9595 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0    11914 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0     6092 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/utils.py
--rw-r--r--   0        0        0     2559 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      311 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    18503 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17764 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0     6200 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     4103 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0      781 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     6648 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0      286 2023-06-09 09:11:49.188747 cognite_neat-0.12.8/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
--rw-r--r--   0        0        0    94607 2023-06-09 09:11:49.192747 cognite_neat-0.12.8/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
--rw-r--r--   0        0        0    79580 2023-06-09 09:11:49.192747 cognite_neat-0.12.8/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    77438 2023-06-09 09:11:49.192747 cognite_neat-0.12.8/cognite/neat/examples/rules/power-grid-example.xlsx
--rw-r--r--   0        0        0    75865 2023-06-09 09:11:49.192747 cognite_neat-0.12.8/cognite/neat/examples/rules/rules-template.xlsx
--rw-r--r--   0        0        0    52178 2023-06-09 09:11:49.192747 cognite_neat-0.12.8/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    79427 2023-06-09 09:11:49.192747 cognite_neat-0.12.8/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1461 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1782 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15632 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6774 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0     3630 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
--rw-r--r--   0        0        0     2573 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
--rw-r--r--   0        0        0    11477 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4792 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0    16421 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
--rw-r--r--   0        0        0     8083 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
--rw-r--r--   0        0        0    13784 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6025 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0    11867 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
--rw-r--r--   0        0        0     6837 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
--rw-r--r--   0        0        0        0 2023-06-09 09:11:49.236748 cognite_neat-0.12.8/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 09:11:49.236748 cognite_neat-0.12.8/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1013 2023-06-09 09:11:49.236748 cognite_neat-0.12.8/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    21517 2023-06-09 09:11:49.236748 cognite_neat-0.12.8/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-06-09 09:11:49.236748 cognite_neat-0.12.8/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-06-09 09:11:49.236748 cognite_neat-0.12.8/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4003 2023-06-09 09:11:49.236748 cognite_neat-0.12.8/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2023-06-09 09:11:49.196747 cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1359583 2023-06-09 09:11:49.204747 cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js
--rw-r--r--   0        0        0     2667 2023-06-09 09:11:49.204747 cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.LICENSE.txt
--rw-r--r--   0        0        0  5853485 2023-06-09 09:11:49.232748 cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.map
--rw-r--r--   0        0        0     2633 2023-06-09 09:11:49.232748 cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-06-09 09:11:49.236748 cognite_neat-0.12.8/cognite/neat/main.py
--rw-r--r--   0        0        0        0 2023-06-09 09:11:49.236748 cognite_neat-0.12.8/cognite/neat/migration/__init__.py
--rw-r--r--   0        0        0     1581 2023-06-09 09:11:49.236748 cognite_neat-0.12.8/cognite/neat/migration/wf_manifests.py
--rw-r--r--   0        0        0     2471 2023-06-09 09:11:49.632753 cognite_neat-0.12.8/pyproject.toml
--rw-r--r--   0        0        0    10241 1970-01-01 00:00:00.000000 cognite_neat-0.12.8/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/LICENSE
+-rw-r--r--   0        0        0     8765 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/README.md
+-rw-r--r--   0        0        0       23 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/constants.py
+-rw-r--r--   0        0        0        0 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/__init__.py
+-rw-r--r--   0        0        0     2652 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/app.py
+-rw-r--r--   0        0        0     1344 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/configuration.py
+-rw-r--r--   0        0        0      408 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/data_classes/__init__.py
+-rw-r--r--   0        0        0     4775 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/data_classes/config.py
+-rw-r--r--   0        0        0     8132 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/data_classes/rules.py
+-rw-r--r--   0        0        0    30296 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/data_classes/transformation_rules.py
+-rw-r--r--   0        0        0        0 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/data_stores/__init__.py
+-rw-r--r--   0        0        0     1520 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/data_stores/metrics.py
+-rw-r--r--   0        0        0     9436 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0      646 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/extractors/__init__.py
+-rw-r--r--   0        0        0     5449 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/extractors/graph_sheet_to_graph.py
+-rw-r--r--   0        0        0     2250 2023-06-11 12:15:28.876066 cognite_neat-0.12.9/cognite/neat/core/extractors/labels.py
+-rw-r--r--   0        0        0    37477 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/extractors/rdf_to_assets.py
+-rw-r--r--   0        0        0    17870 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/extractors/rdf_to_relationships.py
+-rw-r--r--   0        0        0     5400 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
+-rw-r--r--   0        0        0     6700 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/extractors/rules_to_graphql.py
+-rw-r--r--   0        0        0      138 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/loader/__init__.py
+-rw-r--r--   0        0        0      711 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/loader/config.py
+-rw-r--r--   0        0        0     1210 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/loader/graph.py
+-rw-r--r--   0        0        0      938 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/loader/graph_capturing_sheet.py
+-rw-r--r--   0        0        0    10647 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/loader/graph_store.py
+-rw-r--r--   0        0        0      913 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/loader/rules.py
+-rw-r--r--   0        0        0        0 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/mocks/__init__.py
+-rw-r--r--   0        0        0    10373 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/mocks/graph.py
+-rw-r--r--   0        0        0    15303 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/modeler.py
+-rw-r--r--   0        0        0      110 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/parser/__init__.py
+-rw-r--r--   0        0        0     1727 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/parser/transformation_rules.py
+-rw-r--r--   0        0        0       73 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/query_generator/__init__.py
+-rw-r--r--   0        0        0     9595 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/query_generator/sparql.py
+-rw-r--r--   0        0        0    11914 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/transformer.py
+-rw-r--r--   0        0        0     6092 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/utils.py
+-rw-r--r--   0        0        0     2559 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/validator.py
+-rw-r--r--   0        0        0      311 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/__init__.py
+-rw-r--r--   0        0        0    18503 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/base.py
+-rw-r--r--   0        0        0    17764 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/cdf_store.py
+-rw-r--r--   0        0        0     6200 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/manager.py
+-rw-r--r--   0        0        0     4103 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/model.py
+-rw-r--r--   0        0        0      781 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/tasks.py
+-rw-r--r--   0        0        0     6648 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/core/workflow/utils.py
+-rw-r--r--   0        0        0      286 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
+-rw-r--r--   0        0        0    94607 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
+-rw-r--r--   0        0        0    79580 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    77438 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/examples/rules/power-grid-example.xlsx
+-rw-r--r--   0        0        0    75865 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/examples/rules/rules-template.xlsx
+-rw-r--r--   0        0        0    52178 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    79427 2023-06-11 12:15:28.880066 cognite_neat-0.12.9/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1461 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1782 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15632 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6774 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0     3630 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
+-rw-r--r--   0        0        0     2573 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
+-rw-r--r--   0        0        0    11477 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4792 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0    16421 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
+-rw-r--r--   0        0        0     8083 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
+-rw-r--r--   0        0        0    13784 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6025 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0    11867 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
+-rw-r--r--   0        0        0     6837 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/explorer/data_classes/__init__.py
+-rw-r--r--   0        0        0     1013 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/explorer/data_classes/rest.py
+-rw-r--r--   0        0        0    21517 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/explorer/explorer.py
+-rw-r--r--   0        0        0        0 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/explorer/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/explorer/utils/data_mapping.py
+-rw-r--r--   0        0        0     4003 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/explorer/utils/query_templates.py
+-rw-r--r--   0        0        0       16 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/index.html
+-rw-r--r--   0        0        0      312 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2023-06-11 12:15:28.888066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1359583 2023-06-11 12:15:28.896066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js
+-rw-r--r--   0        0        0     2667 2023-06-11 12:15:28.896066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.LICENSE.txt
+-rw-r--r--   0        0        0  5853485 2023-06-11 12:15:28.924066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.map
+-rw-r--r--   0        0        0     2633 2023-06-11 12:15:28.924066 cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      358 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/main.py
+-rw-r--r--   0        0        0        0 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/migration/__init__.py
+-rw-r--r--   0        0        0     1581 2023-06-11 12:15:28.932066 cognite_neat-0.12.9/cognite/neat/migration/wf_manifests.py
+-rw-r--r--   0        0        0     2471 2023-06-11 12:15:29.380070 cognite_neat-0.12.9/pyproject.toml
+-rw-r--r--   0        0        0    10241 1970-01-01 00:00:00.000000 cognite_neat-0.12.9/PKG-INFO
```

### Comparing `cognite_neat-0.12.8/LICENSE` & `cognite_neat-0.12.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/README.md` & `cognite_neat-0.12.9/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/constants.py` & `cognite_neat-0.12.9/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/app.py` & `cognite_neat-0.12.9/cognite/neat/core/app.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/configuration.py` & `cognite_neat-0.12.9/cognite/neat/core/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/data_classes/config.py` & `cognite_neat-0.12.9/cognite/neat/core/data_classes/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/data_classes/rules.py` & `cognite_neat-0.12.9/cognite/neat/core/data_classes/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/data_classes/transformation_rules.py` & `cognite_neat-0.12.9/cognite/neat/core/data_classes/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/data_stores/metrics.py` & `cognite_neat-0.12.9/cognite/neat/core/data_stores/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.12.9/cognite/neat/core/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/extractors/__init__.py` & `cognite_neat-0.12.9/cognite/neat/core/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/extractors/graph_sheet_to_graph.py` & `cognite_neat-0.12.9/cognite/neat/core/extractors/graph_sheet_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/extractors/labels.py` & `cognite_neat-0.12.9/cognite/neat/core/extractors/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/extractors/rdf_to_assets.py` & `cognite_neat-0.12.9/cognite/neat/core/extractors/rdf_to_assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -968,27 +968,28 @@
 @overload
 def remove_non_existing_labels(
     client: CogniteClient, assets: dict[str, Asset | dict[str, Any]]
 ) -> dict[str, Asset] | dict[str, Any]:
     ...
 
 
-def remove_non_existing_labels(
-    client: CogniteClient, assets: Sequence[Asset | dict[str, Any]] | dict[str, Asset | dict[str, Any]]
-) -> Sequence[Asset | dict[str, Any]] | dict[str, Asset | dict[str, Any]]:
+AssetLike = Sequence[Asset | dict[str, Any]] | dict[str, Asset | dict[str, Any]]
+
+
+def remove_non_existing_labels(client: CogniteClient, assets: AssetLike) -> AssetLike:
     cdf_labels = client.labels.list(limit=-1)
     if not cdf_labels:
         # No labels, nothing to check.
         return assets
 
     available_labels = {label.external_id for label in cdf_labels}
 
     def clean_asset_labels(asset: Asset | dict[str, Any]) -> Asset | dict[str, Any]:
         if isinstance(asset, Asset):
-            asset.labels = [label for label in asset.labels if label.external_id in available_labels] or None
+            asset.labels = [label for label in (asset.labels or []) if label.external_id in available_labels] or None
         elif isinstance(asset, dict) and "labels" in asset:
             asset["labels"] = [label for label in asset["labels"] if label in available_labels]
         return asset
 
     if isinstance(assets, Sequence):
         return [clean_asset_labels(a) for a in assets]
```

### Comparing `cognite_neat-0.12.8/cognite/neat/core/extractors/rdf_to_relationships.py` & `cognite_neat-0.12.9/cognite/neat/core/extractors/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py` & `cognite_neat-0.12.9/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/extractors/rules_to_graphql.py` & `cognite_neat-0.12.9/cognite/neat/core/extractors/rules_to_graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/loader/config.py` & `cognite_neat-0.12.9/cognite/neat/core/loader/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/loader/graph.py` & `cognite_neat-0.12.9/cognite/neat/core/loader/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/loader/graph_capturing_sheet.py` & `cognite_neat-0.12.9/cognite/neat/core/loader/graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.12.9/cognite/neat/core/loader/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/loader/rules.py` & `cognite_neat-0.12.9/cognite/neat/core/loader/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.12.9/cognite/neat/core/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/modeler.py` & `cognite_neat-0.12.9/cognite/neat/core/modeler.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/parser/transformation_rules.py` & `cognite_neat-0.12.9/cognite/neat/core/parser/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.12.9/cognite/neat/core/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/transformer.py` & `cognite_neat-0.12.9/cognite/neat/core/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/utils.py` & `cognite_neat-0.12.9/cognite/neat/core/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/validator.py` & `cognite_neat-0.12.9/cognite/neat/core/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/workflow/base.py` & `cognite_neat-0.12.9/cognite/neat/core/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.12.9/cognite/neat/core/workflow/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.12.9/cognite/neat/core/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/workflow/model.py` & `cognite_neat-0.12.9/cognite/neat/core/workflow/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.12.9/cognite/neat/core/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.12.9/cognite/neat/core/workflow/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx` & `cognite_neat-0.12.9/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.12.9/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/rules/power-grid-example.xlsx` & `cognite_neat-0.12.9/cognite/neat/examples/rules/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/rules/rules-template.xlsx` & `cognite_neat-0.12.9/cognite/neat/examples/rules/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.12.9/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.12.9/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.12.9/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.12.9/cognite/neat/examples/workflows/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.12.9/cognite/neat/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.12.9/cognite/neat/examples/workflows/default/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.12.9/cognite/neat/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py` & `cognite_neat-0.12.9/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml` & `cognite_neat-0.12.9/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_db_import/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py` & `cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml` & `cognite_neat-0.12.9/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/workflows/sheet2cdf/workflow.py` & `cognite_neat-0.12.9/cognite/neat/examples/workflows/sheet2cdf/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.12.9/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/workflows/sme_graph_capture/workflow.py` & `cognite_neat-0.12.9/cognite/neat/examples/workflows/sme_graph_capture/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml` & `cognite_neat-0.12.9/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/explorer/data_classes/rest.py` & `cognite_neat-0.12.9/cognite/neat/explorer/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/explorer/explorer.py` & `cognite_neat-0.12.9/cognite/neat/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.12.9/cognite/neat/explorer/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js` & `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.LICENSE.txt` & `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.map` & `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.12.9/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/cognite/neat/migration/wf_manifests.py` & `cognite_neat-0.12.9/cognite/neat/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.8/pyproject.toml` & `cognite_neat-0.12.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.12.8"
+version = "0.12.9"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 packages = [
```

### Comparing `cognite_neat-0.12.8/PKG-INFO` & `cognite_neat-0.12.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.12.8
+Version: 0.12.9
 Summary: Knowledge graph transformation
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

