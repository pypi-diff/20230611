# Comparing `tmp/evodflow-0.1.7.0.tar.gz` & `tmp/evodflow-0.1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evodflow-0.1.7.0.tar", last modified: Thu Jun  8 11:51:34 2023, max compression
+gzip compressed data, was "evodflow-0.1.9.0.tar", last modified: Sun Jun 11 18:12:59 2023, max compression
```

## Comparing `evodflow-0.1.7.0.tar` & `evodflow-0.1.9.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.597224 evodflow-0.1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-08 11:51:34.597224 evodflow-0.1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.585224 evodflow-0.1.7.0/evodflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-08 11:51:34.000000 evodflow-0.1.7.0/evodflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-08 11:51:34.000000 evodflow-0.1.7.0/evodflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:51:34.000000 evodflow-0.1.7.0/evodflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-08 11:51:34.000000 evodflow-0.1.7.0/evodflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-08 11:51:34.000000 evodflow-0.1.7.0/evodflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 11:51:34.000000 evodflow-0.1.7.0/evodflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.589223 evodflow-0.1.7.0/evoflow/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/__info__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.589223 evodflow-0.1.7.0/evoflow/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/controller/common_step_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.589223 evodflow-0.1.7.0/evoflow/controller/data_manipulate/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/controller/data_manipulate/PdfFileOperator.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/controller/data_manipulate/PptxFileOperator.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/controller/data_manipulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/controller/data_manipulate/data_manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/controller/data_manipulate/excel_file_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/controller/data_manipulate/file_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/controller/data_manipulate/image_file_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/controller/log_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/controller/visualize_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.589223 evodflow-0.1.7.0/evoflow/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.589223 evodflow-0.1.7.0/evoflow/entities/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.589223 evodflow-0.1.7.0/evoflow/entities/common/step/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/common/step/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.589223 evodflow-0.1.7.0/evoflow/entities/common/step/browser/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/common/step/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/common/step/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.589223 evodflow-0.1.7.0/evoflow/entities/common/step/file_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/common/step/file_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/common/step/open_excel_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.593224 evodflow-0.1.7.0/evoflow/entities/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/core/base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/core/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/core/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/core/step_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/core/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.593224 evodflow-0.1.7.0/evoflow/entities/data_manipulate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/data_manipulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/data_manipulate/abstract_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.593224 evodflow-0.1.7.0/evoflow/entities/data_manipulate/file_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/data_manipulate/file_operator/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/data_manipulate/file_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/data_manipulate/file_operator/dataframe_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/data_manipulate/file_operator/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/data_manipulate/file_operator/image_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/data_manipulate/file_operator/pdf_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/data_manipulate/file_operator/pptx_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.593224 evodflow-0.1.7.0/evoflow/entities/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/exceptions/base_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/exceptions/evo_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/entities/global_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.593224 evodflow-0.1.7.0/evoflow/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/operators/base_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/operators/empty_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/operators/python_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.593224 evodflow-0.1.7.0/evoflow/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/services/abstract_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.597224 evodflow-0.1.7.0/evoflow/services/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/services/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/services/ocr/easy_ocr_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/services/ocr/ocr_service.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/services/ocr/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/services/ocr/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/services/service_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.597224 evodflow-0.1.7.0/evoflow/services/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/services/templates/item.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.597224 evodflow-0.1.7.0/evoflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/utils/create_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/utils/ultilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/evoflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:51:34.597224 evodflow-0.1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:34.597224 evodflow-0.1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 11:51:20.000000 evodflow-0.1.7.0/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.435241 evodflow-0.1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-11 18:12:59.435241 evodflow-0.1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.431241 evodflow-0.1.9.0/evodflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-11 18:12:59.000000 evodflow-0.1.9.0/evodflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-11 18:12:59.000000 evodflow-0.1.9.0/evodflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:12:59.000000 evodflow-0.1.9.0/evodflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-11 18:12:59.000000 evodflow-0.1.9.0/evodflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-11 18:12:59.000000 evodflow-0.1.9.0/evodflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 18:12:59.000000 evodflow-0.1.9.0/evodflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.431241 evodflow-0.1.9.0/evoflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.431241 evodflow-0.1.9.0/evoflow/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/controller/common_step_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.431241 evodflow-0.1.9.0/evoflow/controller/data_manipulate/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/controller/data_manipulate/PdfFileOperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/controller/data_manipulate/PptxFileOperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/controller/data_manipulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/controller/data_manipulate/data_manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/controller/data_manipulate/excel_file_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/controller/data_manipulate/file_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/controller/data_manipulate/image_file_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/controller/log_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/controller/visualize_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.431241 evodflow-0.1.9.0/evoflow/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.431241 evodflow-0.1.9.0/evoflow/entities/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.431241 evodflow-0.1.9.0/evoflow/entities/common/step/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/common/step/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.431241 evodflow-0.1.9.0/evoflow/entities/common/step/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/common/step/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/common/step/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.431241 evodflow-0.1.9.0/evoflow/entities/common/step/file_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/common/step/file_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/common/step/open_excel_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.435241 evodflow-0.1.9.0/evoflow/entities/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/core/base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/core/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/core/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/core/step_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/core/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.435241 evodflow-0.1.9.0/evoflow/entities/data_manipulate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/data_manipulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/data_manipulate/abstract_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.435241 evodflow-0.1.9.0/evoflow/entities/data_manipulate/file_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/data_manipulate/file_operator/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/data_manipulate/file_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/data_manipulate/file_operator/dataframe_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/data_manipulate/file_operator/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/data_manipulate/file_operator/image_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/data_manipulate/file_operator/pdf_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/data_manipulate/file_operator/pptx_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.435241 evodflow-0.1.9.0/evoflow/entities/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/exceptions/base_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/exceptions/evo_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/entities/global_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.435241 evodflow-0.1.9.0/evoflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/operators/base_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/operators/empty_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/operators/python_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.435241 evodflow-0.1.9.0/evoflow/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/services/abstract_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.435241 evodflow-0.1.9.0/evoflow/services/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/services/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/services/ocr/easy_ocr_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/services/ocr/ocr_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/services/ocr/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/services/ocr/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/services/service_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.435241 evodflow-0.1.9.0/evoflow/services/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/services/templates/item.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.435241 evodflow-0.1.9.0/evoflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/utils/create_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/utils/ultilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/evoflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 18:12:59.435241 evodflow-0.1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:59.435241 evodflow-0.1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-11 18:12:51.000000 evodflow-0.1.9.0/tests/test_base.py
```

### Comparing `evodflow-0.1.7.0/LICENSE` & `evodflow-0.1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/PKG-INFO` & `evodflow-0.1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodflow
-Version: 0.1.7.0
+Version: 0.1.9.0
 Summary: Awesome evoflow created by maycuatroi
 Home-page: https://github.com/maycuatroi/evo-flow/
 Author: maycuatroi
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `evodflow-0.1.7.0/README.md` & `evodflow-0.1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evodflow.egg-info/PKG-INFO` & `evodflow-0.1.9.0/evodflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodflow
-Version: 0.1.7.0
+Version: 0.1.9.0
 Summary: Awesome evoflow created by maycuatroi
 Home-page: https://github.com/maycuatroi/evo-flow/
 Author: maycuatroi
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `evodflow-0.1.7.0/evodflow.egg-info/SOURCES.txt` & `evodflow-0.1.9.0/evodflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/__init__.py` & `evodflow-0.1.9.0/evoflow/__init__.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/cli.py` & `evodflow-0.1.9.0/evoflow/cli.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/controller/data_manipulate/PdfFileOperator.py` & `evodflow-0.1.9.0/evoflow/controller/data_manipulate/PdfFileOperator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/controller/data_manipulate/PptxFileOperator.py` & `evodflow-0.1.9.0/evoflow/controller/data_manipulate/PptxFileOperator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/controller/data_manipulate/excel_file_operator.py` & `evodflow-0.1.9.0/evoflow/controller/data_manipulate/excel_file_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/controller/data_manipulate/file_operator.py` & `evodflow-0.1.9.0/evoflow/controller/data_manipulate/file_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/controller/data_manipulate/image_file_operator.py` & `evodflow-0.1.9.0/evoflow/controller/data_manipulate/image_file_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/controller/log_controller.py` & `evodflow-0.1.9.0/evoflow/controller/log_controller.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/entities/common/step/__init__.py` & `evodflow-0.1.9.0/evoflow/entities/common/step/__init__.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/entities/common/step/browser/__init__.py` & `evodflow-0.1.9.0/evoflow/entities/common/step/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/entities/common/step/downloader.py` & `evodflow-0.1.9.0/evoflow/entities/common/step/downloader.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/entities/common/step/open_excel_file.py` & `evodflow-0.1.9.0/evoflow/entities/common/step/open_excel_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/entities/core/base_object.py` & `evodflow-0.1.9.0/evoflow/entities/core/base_object.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/entities/core/condition.py` & `evodflow-0.1.9.0/evoflow/entities/core/condition.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/entities/core/job.py` & `evodflow-0.1.9.0/evoflow/entities/core/job.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 import importlib
 import inspect
 import json
 import os
 import sys
+import typing
+from time import sleep
 
+from rich.columns import Columns
+from rich.live import Live
+from rich.panel import Panel
+from rich.progress import Progress
+from rich.spinner import Spinner
+from rich.text import Text
+from rich.tree import Tree
 from tqdm import tqdm
 
 from evoflow.controller.log_controller import logger, pretty_dict
 from evoflow.entities.core.base_object import BaseObject
 from evoflow.entities.core.step import Step
+from evoflow.entities.core.step_list import StepList
 from evoflow.entities.core.transaction import Transaction
 
 
 class Job(BaseObject):
     """
     Job : Các bot sẽ được tạo dưới dạng các Job.
 
@@ -39,57 +49,77 @@
 
     def kill(self, **kwargs):
         pass
 
     def finish(self, **kwargs):
         logger.info(f"Finish job: {self.name}")
 
-    def __step_generator(self):
+    def __step_generator(self) -> typing.Generator:
         self.stacks = [self.start_step]
         while len(self.stacks) > 0:
-            step_i = self.stacks.pop()
-            self.current_step = step_i
-            yield step_i
+            for i, step in enumerate(self.stacks):
+                if step.is_ready():
+                    self.current_step = step
+                    self.stacks.pop(i)
+                    yield step
+            sleep(0.1)
 
     def run(self, **kwargs):
+        with Live(
+            Panel(Columns([]), title=f"Running {self.name}"),
+            refresh_per_second=20,
+        ) as live:
+            # live.update(Panel(spinners, title="Panel 2"))
+
+            # add
+            while True:
+                # do self.__run by new thread
+                self.__run(live=live, **kwargs)
+
+    def __run(self, live=None, **kwargs):
+        self.compile()
         logger.info(f"Running job: {self.name}")
         self.params_pool = kwargs
         step_generator = self.__step_generator()
 
-        for step in tqdm(step_generator, unit="step"):
-            log_string = f"Running step : {step.name}"
+        for step in step_generator:
+            log_string = f"Running step : {step}"
             logger.info(log_string)
-
             step.prepare(**self.params_pool)
+            if live is not None:
+                self.__update_live(live)
             try:
                 action_params = inspect.getfullargspec(step.action).args
                 build_params = {}
                 for param in action_params:
                     if param == "self":
                         continue
                     build_params[param] = step.__dict__.get(param)
                 last_result = step.action(**build_params)
-            except AttributeError:
+            except AttributeError as e:
                 logger.error(f"Current Job params: {pretty_dict(self.params_pool)}")
+                step.set_error(e)
                 raise
             step.end(**kwargs)
 
             if last_result is not None:
                 self.params_pool = {**self.params_pool, **last_result}
             step.set_all_params(self.params_pool)
             self.stacks += step.get_next_steps(self.params_pool)
 
         self.finish()
 
         return last_result
 
     def __init__(self, name=None, start_step: Step = None, **kwargs):
         self.current_step = None
-        self.__start_step = start_step
+        self.__start_step: Step = start_step
         self.params_pool = {}
+        self.__steps = []
+        self.__running_steps = []
         if name is None:
             name = os.getenv("JOB_NAME")
         super().__init__(name=name, **kwargs)
 
     @property
     def start_step(self):
         return self.__start_step
@@ -194,7 +224,42 @@
         return data
 
     def __enter__(self, *args, **kwargs):
         return self
 
     def __exit__(self, *args, **kwargs):
         self.finish()
+
+    def find_previous_steps(self, step, all_steps):
+        previous_steps = []
+        for step_i in all_steps:
+            if step in step_i.get_next_steps():
+                previous_steps.append(step_i)
+        return previous_steps
+
+    def compile(self):
+        self.__steps = self.get_all_steps()
+        for step in self.__steps:
+            step.job = self
+
+    def add_running_step(self, step):
+        self.__running_steps.append(step)
+
+    def remove_running_step(self, step):
+        self.__running_steps.remove(step)
+
+    def __update_live(self, live):
+        tree = Tree(self.name)
+        for step in self.__running_steps:
+            is_step_list = isinstance(step, StepList)
+            if is_step_list:
+                remaining_steps = len(step.get_remaining_step())
+                total_step = len(step.steps)
+                step_title = f"{step.name} {total_step-remaining_steps}/{total_step}"
+            else:
+                step_title = step.name
+            spinner = Spinner("material", text=Text(step_title, style="green"))
+            step_live = tree.add(spinner)
+            if isinstance(step, StepList):
+                for sub_step in step.steps:
+                    step_live.add(Spinner("material", text=Text(sub_step.name, style="blue")))
+        live.update(Panel(tree, title=f"Running {self.name}"))
```

### Comparing `evodflow-0.1.7.0/evoflow/entities/core/step.py` & `evodflow-0.1.9.0/evoflow/entities/core/step.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 
 
 class Step(BaseObject):
     """
     Step is a cells of jobs
     """
 
+    STATUS_PENDING = "pending"  # waiting to run
+    STATUS_RUNNING = "running"  # running
+    STATUS_SUCCESS = "success"  # success
+    STATUS_FAILED = "failed"  # failed
+    STATUS_SKIPPED = "skipped"  # skipped by condition
+    STATUS_READY = "ready"  # ready to run
+
     def __call__(self, func) -> "Step":
         """
 
         :return: Step object
         :rtype: Step
         """
 
@@ -40,50 +47,71 @@
             return wrapper_action
 
         return step_decorator(func)
 
     def __init__(self, name=None, transactions=None, **kwargs):
         """
 
-        @param name: Name of the step
-        @param kwargs:
+        Args:
+            name: Name of the step
+            transactions: List of transactions
+            **kwargs:
         """
         self.is_start = kwargs.get("is_start")
         self.is_end = kwargs.get("is_end")
         if transactions is None:
             self.transactions = []
         else:
             self.transactions = transactions
 
         if name is None:
             name = self.__class__.__name__
 
         self.params = {"name": name}
+        self.previous_steps = []
+        self.error = None
+        self.status = self.STATUS_PENDING
+        self.job = None
         super().__init__(name=name, **kwargs)
 
     @abc.abstractmethod
     def action(self, **kwargs):
         """
         Performs the function of step
         """
         pass
 
+    def do_action(self, **kwargs):
+        """
+        Performs the function of step
+        """
+
+        return self.action(**kwargs)
+
+    def set_error(self, error):
+        self.status = self.STATUS_FAILED
+        self.error = error
+
     def end(self, **kwargs) -> dict:
         """
         Kết thúc step, kill các object không cần thiết để giải phóng bộ nhớ
         """
-        # Global.caa.start_command('clear history')
+        self.status = self.STATUS_SUCCESS
+        self.job.remove_running_step(self)
+        return self.params
 
     def prepare(self, **kwargs):
         """
         Chuẩn bị cho action, hàm prepare giúp chuẩn bị input để đẩy vào action()
         """
         for k, v in kwargs.items():
             setattr(self, k, v)
         self.params = kwargs
+        self.job.add_running_step(self)
+        self.status = self.STATUS_RUNNING
 
     def __str__(self):
         return self.name
 
     def get_next_steps(self, params=None):
         next_steps = []
 
@@ -118,7 +146,17 @@
         # connect to other step
         if isinstance(other, Step) or isinstance(other, StepList):
             return other.next(self)
         elif isinstance(other, list):
             step_list = StepList(other)
             return step_list.next(self)
         raise Exception("Invalid step")
+
+    def is_ready(self):
+        """
+        Check if step is ready to run
+        """
+        for step in self.previous_steps:
+            if step.status != self.STATUS_SUCCESS:
+                return False
+            self.status = self.STATUS_READY
+        return True
```

### Comparing `evodflow-0.1.7.0/evoflow/entities/core/step_list.py` & `evodflow-0.1.9.0/evoflow/entities/core/step_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 import typing
 from concurrent.futures import ThreadPoolExecutor
-
-from tqdm import tqdm
-
 from evoflow.entities.core.step import Step
 
 
 class StepList(Step):
     def __init__(self, steps=None, transactions=None, **kwargs):
         super().__init__(**kwargs)
         self.steps = steps or []
@@ -45,14 +42,11 @@
 
     def action(self, **kwargs):
         """
         Performs the function of step
         """
         kwargs = {**self.params, **kwargs}
         with ThreadPoolExecutor(max_workers=10) as executor:
-            list(
-                tqdm(
-                    executor.map(lambda step: step.action(**kwargs), self.steps),
-                    total=len(self.steps),
-                    desc=self.name,
-                )
-            )
+            list(executor.map(lambda step: step.action(**kwargs), self.steps))
+
+    def get_remaining_step(self):
+        return [step for step in self.steps if step.status != Step.STATUS_SUCCESS]
```

### Comparing `evodflow-0.1.7.0/evoflow/entities/core/transaction.py` & `evodflow-0.1.9.0/evoflow/entities/core/transaction.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 class Transaction(BaseObject):
     def __init__(self, step: Step, to: Step, condition="always"):
         self.id = str(step.id) + "-" + str(to.id)
         self.to = to
         self.__from_step__ = step
         self.condition = Condition(condition)
         self.__from_step__.transactions.append(self)
+        self.to.previous_steps.append(self.__from_step__)
 
     def validate(self, **kwargs):
         if type(self.condition.condition_function) == str:
             if self.condition.condition_function == "always":
                 return True
-            return self.build_condition_from_string(
-                self.condition.condition_function, self.__from_step__.params
-            )
+            return self.build_condition_from_string(self.condition.condition_function, self.__from_step__.params)
         return bool(self.condition.condition_function(**kwargs))
 
     def build_condition_from_string(self, condition_function_string, params):
         """
         @param condition_function_string: Ex - select_condition == 3
         @return:
         """
```

### Comparing `evodflow-0.1.7.0/evoflow/entities/core/workflow.py` & `evodflow-0.1.9.0/evoflow/entities/core/workflow.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/entities/data_manipulate/abstract_data.py` & `evodflow-0.1.9.0/evoflow/entities/data_manipulate/abstract_data.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/entities/data_manipulate/file_operator/dataframe_file.py` & `evodflow-0.1.9.0/evoflow/entities/data_manipulate/file_operator/dataframe_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/entities/data_manipulate/file_operator/file.py` & `evodflow-0.1.9.0/evoflow/entities/data_manipulate/file_operator/file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/entities/data_manipulate/file_operator/image_file.py` & `evodflow-0.1.9.0/evoflow/entities/data_manipulate/file_operator/image_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/entities/data_manipulate/file_operator/pdf_file.py` & `evodflow-0.1.9.0/evoflow/entities/data_manipulate/file_operator/pdf_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/entities/data_manipulate/file_operator/pptx_file.py` & `evodflow-0.1.9.0/evoflow/entities/data_manipulate/file_operator/pptx_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/entities/global_vars.py` & `evodflow-0.1.9.0/evoflow/entities/global_vars.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/operators/base_operator.py` & `evodflow-0.1.9.0/evoflow/operators/base_operator.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,23 +4,31 @@
 class BaseOperator(Step):
     def __init__(self, op_args=None, op_kwargs=None, **kwargs):
         super().__init__(**kwargs)
         self.task_id = kwargs.get("task_id", None)
         self.name = self.task_id
         self.op_args = op_args or []
         self.__op_kwargs = op_kwargs or {}
+        self.__op_kwargs = {
+            **self.__op_kwargs,
+            **{
+                "ti": self,
+                "task_instance": self,
+            },
+            **kwargs
+        }
 
     @property
     def op_kwargs(self):
-        return {**self.__op_kwargs, **{"ti": self}}
+        return self.__op_kwargs
 
     def __str__(self):
         return f"{self.__class__.__name__} {self.task_id}"
 
     def __repr__(self):
         return f"{self.__class__.__name__} {self.task_id}"
 
     def xcom_push(self, key, value):
         self.params[key] = value
 
     def xcom_pull(self, key, **kwargs):
-        return self.params[key]
+        return self.params[key]
```

### Comparing `evodflow-0.1.7.0/evoflow/operators/empty_operator.py` & `evodflow-0.1.9.0/evoflow/operators/empty_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/operators/python_operator.py` & `evodflow-0.1.9.0/evoflow/operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/services/ocr/easy_ocr_engine.py` & `evodflow-0.1.9.0/evoflow/services/ocr/easy_ocr_engine.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/services/ocr/ocr_service.py` & `evodflow-0.1.9.0/evoflow/services/ocr/ocr_service.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/services/ocr/result.py` & `evodflow-0.1.9.0/evoflow/services/ocr/result.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/services/service_controller.py` & `evodflow-0.1.9.0/evoflow/services/service_controller.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.7.0/evoflow/utils/ultilities.py` & `evodflow-0.1.9.0/evoflow/utils/ultilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,18 @@
     download_file_name = url.split("/")[-1]
     opener = urllib.request.URLopener(proxies=proxies_list)
     opener.addheader("User-Agent", "evoflow")
     filename, _ = opener.retrieve(url, f"{des_path}/{download_file_name}")
     Archive(filename).extractall(des_path)
     os.remove(filename)
 
+def unarchive(file_path: str, des_path: str):
+    pathlib.Path(des_path).mkdir(parents=True, exist_ok=True)
+    Archive(file_path).extractall(des_path)
+
 
 if __name__ == "__main__":
     import os
 
     proxies = {
         "http": "fsoft-proxy:8080",
     }
```

### Comparing `evodflow-0.1.7.0/setup.py` & `evodflow-0.1.9.0/setup.py`

 * *Files identical despite different names*

