# Comparing `tmp/PyTrial-0.0.5.tar.gz` & `tmp/PyTrial-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyTrial-0.0.5.tar", last modified: Tue Apr 25 16:40:29 2023, max compression
+gzip compressed data, was "dist/PyTrial-0.0.6.tar", last modified: Sun Jun 11 21:42:17 2023, max compression
```

## Comparing `PyTrial-0.0.5.tar` & `PyTrial-0.0.6.tar`

### file list

```diff
@@ -1,139 +1,141 @@
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1316 2023-01-18 21:29:45.000000 PyTrial-0.0.5/LICENSE
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6746 2023-04-25 16:40:29.000000 PyTrial-0.0.5/PKG-INFO
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/PyTrial.egg-info/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6746 2023-04-25 16:40:29.000000 PyTrial-0.0.5/PyTrial.egg-info/PKG-INFO
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4711 2023-04-25 16:40:29.000000 PyTrial-0.0.5/PyTrial.egg-info/SOURCES.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        1 2023-04-25 16:40:29.000000 PyTrial-0.0.5/PyTrial.egg-info/dependency_links.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      264 2023-04-25 16:40:29.000000 PyTrial-0.0.5/PyTrial.egg-info/requires.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        8 2023-04-25 16:40:29.000000 PyTrial-0.0.5/PyTrial.egg-info/top_level.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6009 2023-03-06 23:05:32.000000 PyTrial-0.0.5/README.md
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      302 2023-04-25 16:40:15.000000 PyTrial-0.0.5/pytrial/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/data/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/data/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10898 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/data/demo_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        3 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/data/drug_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15741 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/data/patient_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21943 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/data/site_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13918 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/data/trial_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2804 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/data/utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1324 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/data/vocab_data.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/model_utils/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/model_utils/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5257 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/model_utils/bert.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    19288 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/model_utils/drug.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11508 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/model_utils/icd.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/causal/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/causal/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/confidence/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/confidence/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3485 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1757 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/losses.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2342 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/metrics.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      128 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11365 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21022 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/dipole.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13626 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/raim.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10887 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/retain.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13497 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/rnn.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15633 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/stagenet.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      174 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10018 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    46325 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5848 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7436 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/mlp.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11151 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/transtab.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7509 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/xgboost.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1563 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/indiv_outcome/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       80 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4575 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8666 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5913 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/losses.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3023 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/metrics.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8185 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/pgentropy.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3659 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/site_selection/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      147 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      830 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2335 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2167 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/evaluation.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    41581 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/hint.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5262 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/logistic_regression.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9120 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/mlp.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7751 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/data_structure.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2934 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/data_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7158 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/dataloader.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4047 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8303 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3857 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/module.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12827 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5784 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/protocol_encode.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8295 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/topic_discovery.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6727 2023-01-18 22:50:10.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    33283 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/spot.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5454 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_outcome/xgboost.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      384 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4166 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4590 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/losses.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7234 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    27438 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/compose.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24519 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/deepenroll.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4455 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_patient_match/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      191 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1775 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1223 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/losses.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      552 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/metrics.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/models/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/models/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7238 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/models/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/models/bm25.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8652 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/models/doc2vec.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    39578 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/models/trial2vec.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15813 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_search/models/whiten_bert.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4125 2023-04-19 17:00:00.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4986 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/losses.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      136 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12108 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16604 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/eva.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21137 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/evaluation.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9448 2023-03-10 18:11:27.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/knn.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7669 2023-01-27 05:51:39.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/promptehr.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16617 2023-03-08 22:14:32.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/rnn_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24355 2023-03-08 22:16:42.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/synteg.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      154 2023-03-06 23:05:32.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3742 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    14843 2023-03-06 23:05:32.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/copula_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8207 2023-03-06 23:05:32.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/ct_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7208 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/evaluation.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3781 2023-03-06 23:05:32.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15310 2023-04-25 16:39:29.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/med_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9470 2023-03-06 23:05:32.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/tvae.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13937 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/tasks/trial_simulation/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 16:40:29.000000 PyTrial-0.0.5/pytrial/utils/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      146 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/utils/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3089 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/utils/check.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    20404 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/utils/mimic_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10434 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/utils/parallel.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15561 2023-04-21 19:25:57.000000 PyTrial-0.0.5/pytrial/utils/tabular_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    17977 2023-04-21 00:55:39.000000 PyTrial-0.0.5/pytrial/utils/trainer.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12797 2023-01-18 21:29:45.000000 PyTrial-0.0.5/pytrial/utils/trial_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       38 2023-04-25 16:40:29.000000 PyTrial-0.0.5/setup.cfg
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1271 2023-04-25 16:40:09.000000 PyTrial-0.0.5/setup.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1316 2023-01-18 21:29:45.000000 PyTrial-0.0.6/LICENSE
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6769 2023-06-11 21:42:17.000000 PyTrial-0.0.6/PKG-INFO
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/PyTrial.egg-info/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6769 2023-06-11 21:42:17.000000 PyTrial-0.0.6/PyTrial.egg-info/PKG-INFO
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4797 2023-06-11 21:42:17.000000 PyTrial-0.0.6/PyTrial.egg-info/SOURCES.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        1 2023-06-11 21:42:17.000000 PyTrial-0.0.6/PyTrial.egg-info/dependency_links.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      275 2023-06-11 21:42:17.000000 PyTrial-0.0.6/PyTrial.egg-info/requires.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        8 2023-06-11 21:42:17.000000 PyTrial-0.0.6/PyTrial.egg-info/top_level.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6032 2023-06-11 21:40:37.000000 PyTrial-0.0.6/README.md
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      302 2023-06-11 21:41:34.000000 PyTrial-0.0.6/pytrial/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/data/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/data/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10893 2023-06-11 21:40:37.000000 PyTrial-0.0.6/pytrial/data/demo_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        3 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/data/drug_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15741 2023-04-21 19:25:57.000000 PyTrial-0.0.6/pytrial/data/patient_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    22007 2023-06-11 21:40:37.000000 PyTrial-0.0.6/pytrial/data/site_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13918 2023-04-21 19:25:57.000000 PyTrial-0.0.6/pytrial/data/trial_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2804 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/data/utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1324 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/data/vocab_data.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/model_utils/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/model_utils/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5257 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/model_utils/bert.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    19288 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/model_utils/drug.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11508 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/model_utils/icd.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/causal/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/causal/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/confidence/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/confidence/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3485 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1757 2023-03-10 18:11:27.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/losses.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2342 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/metrics.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/sequence/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      128 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/sequence/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11365 2023-03-10 18:11:27.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/sequence/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21022 2023-03-10 18:11:27.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/sequence/dipole.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13626 2023-03-10 18:11:27.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/sequence/raim.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10887 2023-03-10 18:11:27.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/sequence/retain.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13497 2023-03-10 18:11:27.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/sequence/rnn.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15633 2023-03-10 18:11:27.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/sequence/stagenet.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/tabular/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      174 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/tabular/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10018 2023-03-10 18:11:27.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/tabular/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    46325 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5848 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7436 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/tabular/mlp.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11151 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/tabular/transtab.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7509 2023-03-10 18:11:27.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/tabular/xgboost.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1563 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/indiv_outcome/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/site_selection/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       80 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/site_selection/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4575 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/site_selection/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8739 2023-06-11 21:40:37.000000 PyTrial-0.0.6/pytrial/tasks/site_selection/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    18343 2023-06-11 21:40:37.000000 PyTrial-0.0.6/pytrial/tasks/site_selection/framm.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5941 2023-06-11 21:40:37.000000 PyTrial-0.0.6/pytrial/tasks/site_selection/losses.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3023 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/site_selection/metrics.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8185 2023-04-21 19:25:57.000000 PyTrial-0.0.6/pytrial/tasks/site_selection/pgentropy.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3659 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/site_selection/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      147 2023-04-21 19:25:57.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      830 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2335 2023-04-21 19:25:57.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2167 2023-04-21 19:25:57.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/evaluation.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    41581 2023-04-21 19:25:57.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/hint.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5262 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/logistic_regression.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9120 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/mlp.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7751 2023-04-21 19:25:57.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/data_structure.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2934 2023-04-21 19:25:57.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/data_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7158 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/dataloader.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4047 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8303 2023-04-21 19:25:57.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3857 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/module.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12827 2023-04-21 19:25:57.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5784 2023-04-21 19:25:57.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/protocol_encode.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8295 2023-04-21 19:25:57.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/topic_discovery.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6727 2023-01-18 22:50:10.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    33283 2023-04-21 19:25:57.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/spot.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5454 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_outcome/xgboost.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/trial_patient_match/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      384 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_patient_match/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4166 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_patient_match/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4590 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_patient_match/losses.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/trial_patient_match/models/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_patient_match/models/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7234 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_patient_match/models/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    27438 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_patient_match/models/compose.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24519 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_patient_match/models/deepenroll.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4455 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_patient_match/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/trial_search/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      191 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_search/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1775 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_search/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1223 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_search/losses.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      552 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_search/metrics.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/trial_search/models/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_search/models/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7238 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_search/models/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_search/models/bm25.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8652 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_search/models/doc2vec.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    39578 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_search/models/trial2vec.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15813 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_search/models/whiten_bert.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4125 2023-04-19 17:00:00.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4986 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/losses.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      159 2023-06-11 21:40:37.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12108 2023-06-11 21:40:37.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16604 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/eva.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21137 2023-03-10 18:11:27.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/evaluation.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9448 2023-03-10 18:11:27.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/knn.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7669 2023-06-06 03:21:11.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/promptehr.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16617 2023-03-08 22:14:32.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/rnn_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24355 2023-03-08 22:16:42.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/synteg.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    35501 2023-06-11 21:40:37.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/twin.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      154 2023-03-06 23:05:32.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3742 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    14843 2023-03-06 23:05:32.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/copula_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8207 2023-03-06 23:05:32.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/ct_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7208 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/evaluation.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3781 2023-03-06 23:05:32.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15310 2023-04-25 16:39:29.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/med_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9470 2023-03-06 23:05:32.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/tvae.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13937 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/tasks/trial_simulation/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-11 21:42:17.000000 PyTrial-0.0.6/pytrial/utils/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      146 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/utils/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3089 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/utils/check.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    20404 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/utils/mimic_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10434 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/utils/parallel.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16479 2023-06-11 21:40:37.000000 PyTrial-0.0.6/pytrial/utils/tabular_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    17977 2023-04-21 00:55:39.000000 PyTrial-0.0.6/pytrial/utils/trainer.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12797 2023-01-18 21:29:45.000000 PyTrial-0.0.6/pytrial/utils/trial_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       38 2023-06-11 21:42:17.000000 PyTrial-0.0.6/setup.cfg
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1271 2023-06-11 21:41:25.000000 PyTrial-0.0.6/setup.py
```

### Comparing `PyTrial-0.0.5/LICENSE` & `PyTrial-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/PKG-INFO` & `PyTrial-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTrial
-Version: 0.0.5
+Version: 0.0.6
 Summary: PyTrial: A Python Package for Artificial Intelligence in Drug Development
 Home-page: https://github.com/RyanWangZf/pytrial
 Author: Zifeng Wang, Brandon Theodoru, Tianfan Fu, Jimeng Sun
 Author-email: zifengw2@illinois.edu
 Keywords: drug development,clinical trial,artificial intelligence,deep learning,machine learning
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -140,19 +140,19 @@
 
 
 ## :smiley: Citing 
 
 If you use PyTrial in a scientific publication, we would appreciate citations to:
 
 ```bibtex
-@misc{pytrial2022,
-    title = {PyTrial: A Python Package for Artificial Intelligence in Drug Development},
-    author = {Wang, Zifeng and Theodorou, Brandon and Fu, Tianfan and Sun, Jimeng},
-    year = {2022},
-    month = {11},
+@misc{pytrial2023,
+    title = {PyTrial: A Comprehensive Platform for Artificial Intelligence for Drug Development},
+    author = {Wang, Zifeng and Theodorou, Brandon and Fu, Tianfan and Xiao, Cao and Sun, Jimeng},
+    year = {2023},
+    month = {06},
     organization = {SunLab, UIUC},
     url = {https://pytrial.readthedocs.io/en/latest/},
 }
 ```
```

### Comparing `PyTrial-0.0.5/PyTrial.egg-info/PKG-INFO` & `PyTrial-0.0.6/PyTrial.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTrial
-Version: 0.0.5
+Version: 0.0.6
 Summary: PyTrial: A Python Package for Artificial Intelligence in Drug Development
 Home-page: https://github.com/RyanWangZf/pytrial
 Author: Zifeng Wang, Brandon Theodoru, Tianfan Fu, Jimeng Sun
 Author-email: zifengw2@illinois.edu
 Keywords: drug development,clinical trial,artificial intelligence,deep learning,machine learning
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -140,19 +140,19 @@
 
 
 ## :smiley: Citing 
 
 If you use PyTrial in a scientific publication, we would appreciate citations to:
 
 ```bibtex
-@misc{pytrial2022,
-    title = {PyTrial: A Python Package for Artificial Intelligence in Drug Development},
-    author = {Wang, Zifeng and Theodorou, Brandon and Fu, Tianfan and Sun, Jimeng},
-    year = {2022},
-    month = {11},
+@misc{pytrial2023,
+    title = {PyTrial: A Comprehensive Platform for Artificial Intelligence for Drug Development},
+    author = {Wang, Zifeng and Theodorou, Brandon and Fu, Tianfan and Xiao, Cao and Sun, Jimeng},
+    year = {2023},
+    month = {06},
     organization = {SunLab, UIUC},
     url = {https://pytrial.readthedocs.io/en/latest/},
 }
 ```
```

### Comparing `PyTrial-0.0.5/PyTrial.egg-info/SOURCES.txt` & `PyTrial-0.0.6/PyTrial.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 pytrial/tasks/indiv_outcome/tabular/logistic_regression.py
 pytrial/tasks/indiv_outcome/tabular/mlp.py
 pytrial/tasks/indiv_outcome/tabular/transtab.py
 pytrial/tasks/indiv_outcome/tabular/xgboost.py
 pytrial/tasks/site_selection/__init__.py
 pytrial/tasks/site_selection/base.py
 pytrial/tasks/site_selection/data.py
+pytrial/tasks/site_selection/framm.py
 pytrial/tasks/site_selection/losses.py
 pytrial/tasks/site_selection/metrics.py
 pytrial/tasks/site_selection/pgentropy.py
 pytrial/tasks/site_selection/trainer.py
 pytrial/tasks/trial_outcome/__init__.py
 pytrial/tasks/trial_outcome/base.py
 pytrial/tasks/trial_outcome/data.py
@@ -94,14 +95,15 @@
 pytrial/tasks/trial_simulation/sequence/base.py
 pytrial/tasks/trial_simulation/sequence/eva.py
 pytrial/tasks/trial_simulation/sequence/evaluation.py
 pytrial/tasks/trial_simulation/sequence/knn.py
 pytrial/tasks/trial_simulation/sequence/promptehr.py
 pytrial/tasks/trial_simulation/sequence/rnn_gan.py
 pytrial/tasks/trial_simulation/sequence/synteg.py
+pytrial/tasks/trial_simulation/sequence/twin.py
 pytrial/tasks/trial_simulation/tabular/__init__.py
 pytrial/tasks/trial_simulation/tabular/base.py
 pytrial/tasks/trial_simulation/tabular/copula_gan.py
 pytrial/tasks/trial_simulation/tabular/ct_gan.py
 pytrial/tasks/trial_simulation/tabular/evaluation.py
 pytrial/tasks/trial_simulation/tabular/gaussian_copula.py
 pytrial/tasks/trial_simulation/tabular/med_gan.py
```

### Comparing `PyTrial-0.0.5/README.md` & `PyTrial-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -123,19 +123,19 @@
 
 
 ## :smiley: Citing 
 
 If you use PyTrial in a scientific publication, we would appreciate citations to:
 
 ```bibtex
-@misc{pytrial2022,
-    title = {PyTrial: A Python Package for Artificial Intelligence in Drug Development},
-    author = {Wang, Zifeng and Theodorou, Brandon and Fu, Tianfan and Sun, Jimeng},
-    year = {2022},
-    month = {11},
+@misc{pytrial2023,
+    title = {PyTrial: A Comprehensive Platform for Artificial Intelligence for Drug Development},
+    author = {Wang, Zifeng and Theodorou, Brandon and Fu, Tianfan and Xiao, Cao and Sun, Jimeng},
+    year = {2023},
+    month = {06},
     organization = {SunLab, UIUC},
     url = {https://pytrial.readthedocs.io/en/latest/},
 }
 ```
```

### Comparing `PyTrial-0.0.5/pytrial/data/demo_data.py` & `PyTrial-0.0.6/pytrial/data/demo_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         x['feature'] = x['feature'][:n_sample]
 
     return x
 
 
 def load_mimic_ehr_sequence(input_dir=None, n_sample=None):
     '''
-    Load real EHR patient sequence data, which needs to be accessed via https://physionet.org/content/mimiciii/1.4/.
+    Load EHR patient sequence data, which needs to be accessed via https://physionet.org/content/mimiciii/1.4/.
 
     Parameters
     ----------
     input_dir: str
         The folder that stores the demo data. If None, we will look for the demo data in
         './demo_data/demo_patient_sequence/ehr'.
```

### Comparing `PyTrial-0.0.5/pytrial/data/patient_data.py` & `PyTrial-0.0.6/pytrial/data/patient_data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/data/site_data.py` & `PyTrial-0.0.6/pytrial/data/site_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,15 +452,18 @@
     enroll_hist = None
     eth_label = None
     max_visit = None
     max_trial = None
     visit_voc_size = None
 
     metadata = {
-        'voc': {},
+        'voc': {
+            'dx': 100,
+            'rx': 100
+            },
         
         'feature':{
             'mode': 'tensor',
             },
         
         'visit':{
             'mode': 'tensor',
@@ -481,27 +484,27 @@
         # get input data
         self._parse_inputdata(inputs=data)
 
     def __getitem__(self, index):
         return_data = {}
         if self.dx_hist is not None:
             dx_hist = self.dx_hist[index]
-            if self.metadata['dx']['mode'] == 'tensor':
-                dx_ts, dx_len = self._dense_visit_to_tensor(dx_hist, self.metadata['dx']['voc'])
+            if self.metadata['visit']['mode'] == 'tensor':
+                dx_ts, dx_len = self._dense_visit_to_tensor(dx_hist, self.metadata['voc']['dx'])
                 return_data['dx'] = dx_ts
                 return_data['dx_lens'] = dx_len
             else:
                 visit_dict, dx_len = self._tensor_visit_to_dense(dx_hist)
                 return_data['dx'] = visit_dict
                 return_data['dx_lens'] = dx_len
                 
         if self.rx_hist is not None:
             rx_hist = self.rx_hist[index]
-            if self.metadata['rx']['mode'] == 'tensor':
-                rx_ts, rx_len = self._dense_visit_to_tensor(rx_hist, self.metadata['rx']['voc'])
+            if self.metadata['visit']['mode'] == 'tensor':
+                rx_ts, rx_len = self._dense_visit_to_tensor(rx_hist, self.metadata['voc']['rx'])
                 return_data['rx'] = rx_ts
                 return_data['rx_lens'] = rx_len
             else:
                 visit_dict, rx_len = self._tensor_visit_to_dense(rx_hist)
                 return_data['rx'] = visit_dict
                 return_data['rx_lens'] = rx_len
```

### Comparing `PyTrial-0.0.5/pytrial/data/trial_data.py` & `PyTrial-0.0.6/pytrial/data/trial_data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/data/utils.py` & `PyTrial-0.0.6/pytrial/data/utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/data/vocab_data.py` & `PyTrial-0.0.6/pytrial/data/vocab_data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/model_utils/bert.py` & `PyTrial-0.0.6/pytrial/model_utils/bert.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/model_utils/drug.py` & `PyTrial-0.0.6/pytrial/model_utils/drug.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/model_utils/icd.py` & `PyTrial-0.0.6/pytrial/model_utils/icd.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/data.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/losses.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/losses.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/metrics.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/metrics.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/base.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/sequence/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/dipole.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/sequence/dipole.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/raim.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/sequence/raim.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/retain.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/sequence/retain.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/rnn.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/sequence/rnn.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/sequence/stagenet.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/sequence/stagenet.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/base.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/tabular/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/mlp.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/tabular/mlp.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/transtab.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/tabular/transtab.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/tabular/xgboost.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/tabular/xgboost.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/indiv_outcome/trainer.py` & `PyTrial-0.0.6/pytrial/tasks/indiv_outcome/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/site_selection/base.py` & `PyTrial-0.0.6/pytrial/tasks/site_selection/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/site_selection/data.py` & `PyTrial-0.0.6/pytrial/tasks/site_selection/data.py`

 * *Files 18% similar despite different names*

```diff
@@ -63,26 +63,27 @@
         self.trials = TrialDatasetStructured(trial_data)
 
     def __len__(self):
         return len(self.trials)
 
     def __getitem__(self, idx):
         sitesPerTrial = self.mappings[idx]
-        siteFeatures = [self.sites[sites] for sites in sitesPerTrial]
-        sample = {"trial": self.trial_features[idx], 
+        siteFeatures = [self.sites[trialSites] for trialSites in sitesPerTrial]
+        siteFeatures = {k: np.stack([d[k] for d in siteFeatures]) for k in siteFeatures[0]}
+        sample = {"trial": self.trials[idx], 
                   "label": self.enrollments[idx], 
                   "eth_label": siteFeatures['eth_label'],
                   "inv_static": siteFeatures['x'],
-                  "inv_dx": siteFeatures['dx'],
-                  "inv_dx_len": siteFeatures['dx_lens'],
-                  "inv_rx": siteFeatures['rx'],
-                  "inv_rx_len": siteFeatures['rx_lens'],
-                  "inv_enroll": siteFeatures['hist'],
-                  "inv_enroll_len": siteFeatures['hist_lens'],
-                  "inv_mask": np.ones((len(sitesPerTrial), max([len(s) for s in sitesPerTrial], 4)), dtype=np.int8)
+                  "dx": siteFeatures['dx'],
+                  "dx_len": siteFeatures['dx_lens'],
+                  "rx": siteFeatures['rx'],
+                  "rx_len": siteFeatures['rx_lens'],
+                  "enroll_hist": siteFeatures['hist'],
+                  "enroll_hist_len": siteFeatures['hist_lens'],
+                  "inv_mask": np.zeros((len(sitesPerTrial), 4), dtype=np.int8)
                  }
         return sample
 
 class SiteSelectionBaseCollator:
     '''
     support make collation of unequal sized list of batch for densely stored
     sequential visits data.
@@ -175,15 +176,15 @@
     def __init__(self, config=None):
         if config is not None:
             self.config.update(config)
             
         if self.config['visit_mode'] == 'tensor': self.is_tensor_visit = True
         else: self.is_tensor_visit = False
 
-        if self.config['trial_model'] == 'tensor': self.is_tensor_trial = True
+        if self.config['trial_mode'] == 'tensor': self.is_tensor_trial = True
         else: self.is_tensor_trial = False
         
         if self.config['has_demographics'] == 'true': self.has_demographics = True
         else: self.has_demographics = False
 
     def __call__(self, inputs):
         '''
@@ -194,25 +195,25 @@
             
             'label': list[list[int]],
             
             'eth_label' None or list[list[np.ndarray]]
             
             'inv_static': list[list[np.ndarray]]
             
-            'inv_dx': list[list[np.ndarray]]
+            'dx': list[list[np.ndarray]]
             
-            'inv_dx_len': list[list[int]]
+            'dx_len': list[list[int]]
             
-            'inv_rx': list[list[np.ndarray]]
+            'rx': list[list[np.ndarray]]
             
-            'inv_rx_len': list[list[int]]
+            'rx_len': list[list[int]]
             
-            'inv_enroll': list[list[np.ndarray]]
+            'enroll_hist': list[list[np.ndarray]]
             
-            'inv_enroll_len': list[list[int]]
+            'enroll_hist_len': list[list[int]]
             
             'inv_mask': list[list[np.ndarray]]
         }
 
         Returns
         -------
         outputs = {
@@ -220,42 +221,44 @@
             
             'label': tensor,
             
             'eth_label' None or tensor,
             
             'inv_static': tensor
             
-            'inv_dx': tensor
+            'dx': tensor
             
-            'inv_dx_len': tensor
+            'dx_len': tensor
             
-            'inv_rx': tensor
+            'rx': tensor
             
-            'inv_rx_len': tensor
+            'rx_len': tensor
             
-            'inv_enroll': tensor
+            'enroll_hist': tensor
             
-            'inv_enroll_len': tensor
+            'enroll_hist_len': tensor
             
             'inv_mask': tensor
         }
         '''
         
         # init output dict
         return_data = defaultdict(list)
         
+        inputs = {k: np.stack([d[k] for d in inputs]) for k in inputs[0]}
+        
         return_data['trial'] = torch.FloatTensor(np.array(inputs['trial']))
         return_data['label'] = torch.FloatTensor(np.array(inputs['label']))
         return_data['inv_static'] = torch.FloatTensor(np.array(inputs['inv_static']))
-        return_data['inv_dx'] = torch.FloatTensor(np.array(inputs['inv_dx']))
-        return_data['inv_dx_len'] = torch.IntTensor(np.array(inputs['inv_dx_len']))
-        return_data['inv_rx'] = torch.FloatTensor(np.array(inputs['inv_rx']))
-        return_data['inv_rx_len'] = torch.IntTensor(np.array(inputs['inv_rx_len']))
-        return_data['inv_enroll'] = torch.FloatTensor(np.array(inputs['inv_enroll']))
-        return_data['inv_enroll_len'] = torch.IntTensor(np.array(inputs['inv_enroll_len']))
-        return_data['inv_mask'] = torch.IntTensor(np.array(inputs['inv_mask']))
+        return_data['dx'] = torch.FloatTensor(np.array(inputs['dx']))
+        return_data['dx_len'] = torch.LongTensor(np.array(inputs['dx_len']))
+        return_data['rx'] = torch.FloatTensor(np.array(inputs['rx']))
+        return_data['rx_len'] = torch.LongTensor(np.array(inputs['rx_len']))
+        return_data['enroll_hist'] = torch.FloatTensor(np.array(inputs['enroll_hist']))
+        return_data['enroll_hist_len'] = torch.LongTensor(np.array(inputs['enroll_hist_len']))
+        return_data['inv_mask'] = torch.LongTensor(np.array(inputs['inv_mask']))
 
         # processing all
         if self.has_demographics:
             return_data['eth_label'] = torch.FloatTensor(np.array(inputs['eth_label']))
         
         return return_data
```

### Comparing `PyTrial-0.0.5/pytrial/tasks/site_selection/losses.py` & `PyTrial-0.0.6/pytrial/tasks/site_selection/losses.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,52 +52,52 @@
 #######
 
 # score = bs * M
 # relevance = bs * M
 # eth_list = bs * M * num_cat
 # rank_samples = bs * MC * M
 def loss_function(score, relevance, eth_list, lam, K):	
-	num_MC_samples = 25
-	M = len(score[0])
-	score = F.softmax(score, dim=1)
-
-	rank_samples = torch.stack([torch.multinomial(score, num_samples=M, replacement=False).to(score.device) for _ in range(num_MC_samples)], axis=1)
-
-	importance_prob_values = compute_log_prob(rank_samples, score, num_MC_samples, K)
-	delta_values = ranking_loss(rank_samples, relevance, num_MC_samples, K)
-	delta_f_values = fairness_loss(rank_samples, eth_list, relevance, num_MC_samples, K)
-	rewards = delta_values + lam*delta_f_values
-	loss = -1 * torch.sum(importance_prob_values * rewards, 1)
-	return loss/num_MC_samples #, torch.mean(rewards), torch.mean(delta_values), torch.mean(delta_f_values)
+		num_MC_samples = 25
+		M = len(score[0])
+		score = F.softmax(score, dim=1)
+
+		rank_samples = torch.stack([torch.multinomial(score, num_samples=M, replacement=False).to(score.device) for _ in range(num_MC_samples)], axis=1)
+
+		importance_prob_values = compute_log_prob(rank_samples, score, num_MC_samples, K)
+		delta_values = ranking_loss(rank_samples, relevance, num_MC_samples, K)
+		delta_f_values = fairness_loss(rank_samples, eth_list, relevance, num_MC_samples, K)
+		rewards = delta_values + lam*delta_f_values
+		loss = -1 * torch.sum(importance_prob_values * rewards, 1)
+		return loss/num_MC_samples #, torch.mean(rewards), torch.mean(delta_values), torch.mean(delta_f_values)
 
 def loss_function_enrollment(score, relevance, K):	
-	num_MC_samples = 25
-	M = len(score[0])
-	score = F.softmax(score, dim=1)
-
-	rank_samples = torch.stack([torch.multinomial(score, num_samples=M, replacement=False).to(score.device) for _ in range(num_MC_samples)], axis=1)
-
-	importance_prob_values = compute_log_prob(rank_samples, score, num_MC_samples, K)
-	delta_values = ranking_loss(rank_samples, relevance, num_MC_samples, K)
-	rewards = delta_values
-	loss = -1 * torch.sum(importance_prob_values * rewards, 1)
-	return loss/num_MC_samples #, torch.mean(rewards), torch.mean(delta_values)
+		num_MC_samples = 25
+		M = len(score[0])
+		score = F.softmax(score, dim=1)
+
+		rank_samples = torch.stack([torch.multinomial(score, num_samples=M, replacement=False).to(score.device) for _ in range(num_MC_samples)], axis=1)
+
+		importance_prob_values = compute_log_prob(rank_samples, score, num_MC_samples, K)
+		delta_values = ranking_loss(rank_samples, relevance, num_MC_samples, K)
+		rewards = delta_values
+		loss = -1 * torch.sum(importance_prob_values * rewards, 1)
+		return loss/num_MC_samples #, torch.mean(rewards), torch.mean(delta_values)
 
 def loss_function_fairness(score, relevance, eth_list, K):
-	num_MC_samples = 25
-	M = len(score[0])
-	score = F.softmax(score, dim=1)
-
-	rank_samples = torch.stack([torch.multinomial(score,num_samples=M, replacement=False).to(score.device) for _ in range(num_MC_samples)], axis=1)
-	
-	importance_prob_values = compute_log_prob(rank_samples, score, num_MC_samples, K)
-	delta_f_values = fairness_loss(rank_samples, eth_list, relevance, num_MC_samples, K)
+		num_MC_samples = 25
+		M = len(score[0])
+		score = F.softmax(score, dim=1)
+
+		rank_samples = torch.stack([torch.multinomial(score,num_samples=M, replacement=False).to(score.device) for _ in range(num_MC_samples)], axis=1)
+		
+		importance_prob_values = compute_log_prob(rank_samples, score, num_MC_samples, K)
+		delta_f_values = fairness_loss(rank_samples, eth_list, relevance, num_MC_samples, K)
 
-	loss = -1 * torch.sum(importance_prob_values * (delta_f_values), 1)
-	return loss/num_MC_samples
+		loss = -1 * torch.sum(importance_prob_values * (delta_f_values), 1)
+		return loss/num_MC_samples
 
 class PolicyGradientLossEnrollment(nn.Module):
     def __init__(self, model, K) -> None:
         super().__init__()
         self.model = model
         self.K = K
         self.loss = loss_function_enrollment
```

### Comparing `PyTrial-0.0.5/pytrial/tasks/site_selection/metrics.py` & `PyTrial-0.0.6/pytrial/tasks/site_selection/metrics.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/site_selection/pgentropy.py` & `PyTrial-0.0.6/pytrial/tasks/site_selection/pgentropy.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/site_selection/trainer.py` & `PyTrial-0.0.6/pytrial/tasks/site_selection/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/base.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/data.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/evaluation.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/evaluation.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/hint.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/hint.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/logistic_regression.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/mlp.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/mlp.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/data_structure.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/data_structure.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/data_utils.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/dataloader.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/module.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/module.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/protocol_encode.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/protocol_encode.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/topic_discovery.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/topic_discovery.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/model_utils/utils.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/model_utils/utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/spot.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/spot.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_outcome/xgboost.py` & `PyTrial-0.0.6/pytrial/tasks/trial_outcome/xgboost.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_patient_match/data.py` & `PyTrial-0.0.6/pytrial/tasks/trial_patient_match/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_patient_match/losses.py` & `PyTrial-0.0.6/pytrial/tasks/trial_patient_match/losses.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/base.py` & `PyTrial-0.0.6/pytrial/tasks/trial_patient_match/models/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/compose.py` & `PyTrial-0.0.6/pytrial/tasks/trial_patient_match/models/compose.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_patient_match/models/deepenroll.py` & `PyTrial-0.0.6/pytrial/tasks/trial_patient_match/models/deepenroll.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_patient_match/trainer.py` & `PyTrial-0.0.6/pytrial/tasks/trial_patient_match/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_search/data.py` & `PyTrial-0.0.6/pytrial/tasks/trial_search/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_search/losses.py` & `PyTrial-0.0.6/pytrial/tasks/trial_search/losses.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_search/metrics.py` & `PyTrial-0.0.6/pytrial/tasks/trial_search/metrics.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_search/models/base.py` & `PyTrial-0.0.6/pytrial/tasks/trial_search/models/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_search/models/doc2vec.py` & `PyTrial-0.0.6/pytrial/tasks/trial_search/models/doc2vec.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_search/models/trial2vec.py` & `PyTrial-0.0.6/pytrial/tasks/trial_search/models/trial2vec.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_search/models/whiten_bert.py` & `PyTrial-0.0.6/pytrial/tasks/trial_search/models/whiten_bert.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/data.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/losses.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/losses.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/base.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     def _compute_n_per_sample(self, n_test_sample, n=None, n_per_sample=None):
         if n_per_sample is not None:
             n_total = n_test_sample*n_per_sample
             if n is not None:
                 n_total = min(n_total, n)
             return n_total, n_per_sample
         else:
-            return n, math.ceil(n_test_sample / n)
+            return n, math.ceil(n / n_test_sample)
 
     def _get_num_visit(self, data, idx):
         visits = data['v']
         num_visit_list = []
         for k,v in visits.items():
             num_visit_list.append(len(v[idx]))
```

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/eva.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/eva.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/evaluation.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/evaluation.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/knn.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/knn.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/promptehr.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/promptehr.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/rnn_gan.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/rnn_gan.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/sequence/synteg.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/sequence/synteg.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/base.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/copula_gan.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/copula_gan.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/ct_gan.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/ct_gan.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/evaluation.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/evaluation.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/med_gan.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/med_gan.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/tabular/tvae.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/tabular/tvae.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/tasks/trial_simulation/trainer.py` & `PyTrial-0.0.6/pytrial/tasks/trial_simulation/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/utils/check.py` & `PyTrial-0.0.6/pytrial/utils/check.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/utils/mimic_utils.py` & `PyTrial-0.0.6/pytrial/utils/mimic_utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/utils/parallel.py` & `PyTrial-0.0.6/pytrial/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/utils/tabular_utils.py` & `PyTrial-0.0.6/pytrial/utils/tabular_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,38 +47,57 @@
         max values seen during ``fit``. Defaults to ``False``.
 
     learn_rounding_scheme (bool):
         Whether or not to learn what place to round to based on the data seen during ``fit``.
         If ``True``, the data returned by ``reverse_transform`` will be rounded to that place.
         Defaults to ``False``.
 
+    missing_value_generation (str or None):
+        The way missing values are being handled. There are three strategies:
+
+            * ``random``: Randomly generates missing values based on the percentage of
+                missing values.
+            * ``from_column``: Creates a binary column that describes whether the original
+                value was missing. Then use it to recreate missing values.
+            * ``None``: Do nothing with the missing values on the reverse transform. Simply
+                pass whatever data we get through.
+
+    computer_representation (dtype):
+        Accepts ``'Int8'``, ``'Int16'``, ``'Int32'``, ``'Int64'``, ``'UInt8'``, ``'UInt16'``,
+        ``'UInt32'``, ``'UInt64'``, ``'Float'``.
+        Defaults to ``'Float'``.
+
     model_missing_values (bool):
-        Whether to create a new column to indicate which values were null or not. The column
+        **Deprecated** Whether to create a new column to indicate which values were null or not. The column
         will be created only if there are null values. If ``True``, create the new column if
         there are null values. If ``False``, do not create the new column even if there
         are null values. Defaults to ``False``.
     '''
     _dtype = None
     _min_value = None
     _max_value = None
     random_states = None
 
     def __init__(self,
         missing_value_replacement=None,
         enforce_min_max_values=False,
         learn_rounding_scheme=False,
+        computer_representation='Float',
+        missing_value_generation="random",
         model_missing_values=None,
-        computer_representation='Float'
         ):
         self.output_properties = {None: {'sdtype': 'float', 'next_transformer': None}}
-        self.missing_value_replacement = missing_value_replacement
-        self.enforce_min_max_values=enforce_min_max_values
-        self.learn_rounding_scheme=learn_rounding_scheme
-        self.model_missing_values = model_missing_values
-        self.computer_representation = computer_representation
+        super().__init__(
+            missing_value_replacement=missing_value_replacement,
+            model_missing_values=model_missing_values,
+            learn_rounding_scheme=learn_rounding_scheme,
+            enforce_min_max_values=enforce_min_max_values,
+            computer_representation=computer_representation,
+            missing_value_generation=missing_value_generation,
+        )
         self.standard_transformer = sk_standardscaler()
 
     def _fit(self, data):
         '''
         Fit the transformer to the data.
 
         Parameters
```

### Comparing `PyTrial-0.0.5/pytrial/utils/trainer.py` & `PyTrial-0.0.6/pytrial/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/pytrial/utils/trial_utils.py` & `PyTrial-0.0.6/pytrial/utils/trial_utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.5/setup.py` & `PyTrial-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # read the contents of requirements.txt
 with open(os.path.join(this_directory, 'requirements.txt'),
           encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name = 'PyTrial',
-    version = '0.0.5',
+    version = '0.0.6',
     author = 'Zifeng Wang, Brandon Theodoru, Tianfan Fu, Jimeng Sun',
     author_email = 'zifengw2@illinois.edu',
     description = 'PyTrial: A Python Package for Artificial Intelligence in Drug Development',
     url = 'https://github.com/RyanWangZf/pytrial',
     keywords=['drug development', 'clinical trial', 'artificial intelligence', 'deep learning', 'machine learning'],
     long_description=long_description,
     long_description_content_type='text/markdown',
```

