# Comparing `tmp/smart_data_science-0.1.1.tar.gz` & `tmp/smart_data_science-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_data_science-0.1.1.tar", max compression
+gzip compressed data, was "smart_data_science-0.1.2.tar", max compression
```

## Comparing `smart_data_science-0.1.1.tar` & `smart_data_science-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,53 @@
--rwxr-xr-x   0        0        0     1078 2023-01-06 19:11:15.664337 smart_data_science-0.1.1/LICENSE
--rw-r--r--   0        0        0     2719 2023-05-20 17:54:55.102523 smart_data_science-0.1.1/README.md
--rw-r--r--   0        0        0     4770 2023-05-20 17:54:55.114523 smart_data_science-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      735 2023-05-20 17:54:55.114523 smart_data_science-0.1.1/src/smart_data_science/__init__.py
--rw-r--r--   0        0        0    11347 2023-05-20 17:54:55.114523 smart_data_science-0.1.1/src/smart_data_science/analysis/info.py
--rw-r--r--   0        0        0     3555 2023-05-20 17:54:55.114523 smart_data_science-0.1.1/src/smart_data_science/analysis/info_advanced.py
--rw-r--r--   0        0        0     2210 2023-05-20 17:54:55.114523 smart_data_science-0.1.1/src/smart_data_science/analysis/plot.py
--rw-r--r--   0        0        0    12669 2023-05-20 17:54:55.114523 smart_data_science-0.1.1/src/smart_data_science/cloud/gcp.py
--rw-r--r--   0        0        0      579 2023-05-20 17:54:55.114523 smart_data_science-0.1.1/src/smart_data_science/core/data_samples/README.md
--rw-r--r--   0        0        0   684858 2023-05-20 17:54:55.122523 smart_data_science-0.1.1/src/smart_data_science/core/data_samples/churn_bank.csv
--rw-r--r--   0        0        0  4516899 2023-05-20 17:54:55.146523 smart_data_science-0.1.1/src/smart_data_science/core/data_samples/sales_supermarkets.parquet
--rw-r--r--   0        0        0  1443761 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/core/data_samples/shipping_logs.csv
--rw-r--r--   0        0        0     1931 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/core/data_samples_module.py
--rw-r--r--   0        0        0     5196 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/core/io.py
--rw-r--r--   0        0        0     4764 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/core/logger.py
--rw-r--r--   0        0        0     6505 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/core/system.py
--rw-r--r--   0        0        0     3874 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/dev/modelling/ml_classifier_old_format/prediction.py
--rw-r--r--   0        0        0     5326 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/graph_data/network_graph.py
--rwxr-xr-x   0        0        0    22447 2023-05-20 18:18:17.728691 smart_data_science-0.1.1/src/smart_data_science/llm/assistant.py
--rwxr-xr-x   0        0        0    22651 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/ml/ml_base.py
--rwxr-xr-x   0        0        0    20443 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/ml/ml_classifier.py
--rwxr-xr-x   0        0        0     9454 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/ml/ml_contributions.py
--rwxr-xr-x   0        0        0     5292 2023-05-20 18:18:47.316460 smart_data_science-0.1.1/src/smart_data_science/ml/ml_intervals.py
--rwxr-xr-x   0        0        0    18556 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/ml/ml_regressor.py
--rwxr-xr-x   0        0        0     2040 2023-05-20 18:18:28.580603 smart_data_science-0.1.1/src/smart_data_science/ml/ml_tune.py
--rwxr-xr-x   0        0        0    17470 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/ml/ml_utils.py
--rwxr-xr-x   0        0        0     3364 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/ml/plot_classifier.py
--rwxr-xr-x   0        0        0     5936 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/ml/plot_contributions.py
--rwxr-xr-x   0        0        0     3045 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/ml/plot_general.py
--rwxr-xr-x   0        0        0     2919 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/ml/plot_intervals.py
--rwxr-xr-x   0        0        0     2206 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/ml/plot_regressor.py
--rw-r--r--   0        0        0    27360 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/nlp/semantic_search.py
--rw-r--r--   0        0        0     4605 2023-05-20 18:25:42.323494 smart_data_science-0.1.1/src/smart_data_science/optimization/sequence.py
--rw-r--r--   0        0        0    12896 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/process/clean.py
--rw-r--r--   0        0        0     1709 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/process/etl.py
--rw-r--r--   0        0        0     3893 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/process/transform.py
--rw-r--r--   0        0        0       48 2023-01-06 19:11:15.664337 smart_data_science-0.1.1/src/smart_data_science/smart_data_science.py
--rw-r--r--   0        0        0     5641 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/time_series/date_time.py
--rw-r--r--   0        0        0     5093 2023-05-20 17:54:55.154523 smart_data_science-0.1.1/src/smart_data_science/ui/table_definitions.py
--rw-r--r--   0        0        0     7857 2023-05-20 17:54:55.158523 smart_data_science-0.1.1/src/smart_data_science/ui/ui_info.py
--rw-r--r--   0        0        0     8144 2023-05-20 17:54:55.158523 smart_data_science-0.1.1/src/smart_data_science/ui/ui_io.py
--rw-r--r--   0        0        0     4169 2023-05-20 17:54:55.158523 smart_data_science-0.1.1/src/smart_data_science/ui/ui_template.py
--rw-r--r--   0        0        0     5496 1970-01-01 00:00:00.000000 smart_data_science-0.1.1/setup.py
--rw-r--r--   0        0        0     5266 1970-01-01 00:00:00.000000 smart_data_science-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1078 2023-06-11 19:15:17.816588 smart_data_science-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2719 2023-06-11 19:15:17.816588 smart_data_science-0.1.2/README.md
+-rw-r--r--   0        0        0     4965 2023-06-11 20:08:55.679194 smart_data_science-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      802 2023-06-11 19:15:17.826588 smart_data_science-0.1.2/src/smart_data_science/__init__.py
+-rw-r--r--   0        0        0    11506 2023-06-11 19:15:17.826588 smart_data_science-0.1.2/src/smart_data_science/analysis/info.py
+-rw-r--r--   0        0        0     3555 2023-06-11 19:15:17.826588 smart_data_science-0.1.2/src/smart_data_science/analysis/info_advanced.py
+-rw-r--r--   0        0        0     2210 2023-06-11 19:15:17.826588 smart_data_science-0.1.2/src/smart_data_science/analysis/plot.py
+-rw-r--r--   0        0        0    12756 2023-06-11 19:15:17.826588 smart_data_science-0.1.2/src/smart_data_science/cloud/gcp.py
+-rw-r--r--   0        0        0     7553 2023-06-11 19:15:17.826588 smart_data_science-0.1.2/src/smart_data_science/core/io.py
+-rw-r--r--   0        0        0     4852 2023-06-11 19:15:17.826588 smart_data_science-0.1.2/src/smart_data_science/core/logger.py
+-rw-r--r--   0        0        0     1005 2023-06-11 19:15:17.826588 smart_data_science-0.1.2/src/smart_data_science/core/samples_data/README.md
+-rw-r--r--   0        0        0   684858 2023-06-11 19:15:17.826588 smart_data_science-0.1.2/src/smart_data_science/core/samples_data/churn_bank.csv
+-rw-r--r--   0        0        0  5557107 2023-06-11 19:15:17.856588 smart_data_science-0.1.2/src/smart_data_science/core/samples_data/electric_motor_50k.parquet
+-rw-r--r--   0        0        0  1474796 2023-06-11 19:15:17.866588 smart_data_science-0.1.2/src/smart_data_science/core/samples_data/energy_building.parquet
+-rw-r--r--   0        0        0  4516899 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/core/samples_data/supermarket_sales.parquet
+-rw-r--r--   0        0        0  1443761 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/core/samples_data/supply_chain.csv
+-rw-r--r--   0        0        0     3137 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/core/samples_data_module.py
+-rw-r--r--   0        0        0     2675 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/core/samples_scenario/scenario_electric_motor.py
+-rw-r--r--   0        0        0     3820 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/core/samples_scenario/scenario_energy_building.py
+-rw-r--r--   0        0        0     2685 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/core/samples_scenario/scenario_supermarket_sales.py
+-rw-r--r--   0        0        0     2764 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/core/samples_scenario/scenario_supply_chain.py
+-rw-r--r--   0        0        0     2176 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/core/samples_scenario_module.py
+-rw-r--r--   0        0        0     5345 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/core/scenario_base.py
+-rw-r--r--   0        0        0     6614 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/core/system.py
+-rw-r--r--   0        0        0     3874 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/dev/modelling/ml_classifier_old_format/prediction.py
+-rw-r--r--   0        0        0     5326 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/graph_data/network_graph.py
+-rwxr-xr-x   0        0        0    32623 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/llm/assistant.py
+-rwxr-xr-x   0        0        0    24272 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/ml/ml_base.py
+-rwxr-xr-x   0        0        0    20429 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/ml/ml_classifier.py
+-rwxr-xr-x   0        0        0     9454 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/ml/ml_contributions.py
+-rwxr-xr-x   0        0        0     5292 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/ml/ml_intervals.py
+-rwxr-xr-x   0        0        0    18577 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/ml/ml_regressor.py
+-rwxr-xr-x   0        0        0     2040 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/ml/ml_tune.py
+-rwxr-xr-x   0        0        0    17538 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/ml/ml_utils.py
+-rwxr-xr-x   0        0        0     3364 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/ml/plot_classifier.py
+-rwxr-xr-x   0        0        0     5936 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/ml/plot_contributions.py
+-rwxr-xr-x   0        0        0     3045 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/ml/plot_general.py
+-rwxr-xr-x   0        0        0     2919 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/ml/plot_intervals.py
+-rwxr-xr-x   0        0        0     2200 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/ml/plot_regressor.py
+-rw-r--r--   0        0        0    27360 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/nlp/semantic_search.py
+-rw-r--r--   0        0        0     4603 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/optimization/sequence.py
+-rw-r--r--   0        0        0    12896 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/process/clean.py
+-rw-r--r--   0        0        0     1709 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/process/etl.py
+-rw-r--r--   0        0        0     3893 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/process/transform.py
+-rw-r--r--   0        0        0       48 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/smart_data_science.py
+-rw-r--r--   0        0        0     5641 2023-06-11 19:15:17.896588 smart_data_science-0.1.2/src/smart_data_science/time_series/date_time.py
+-rw-r--r--   0        0        0     5476 2023-06-11 19:15:17.906588 smart_data_science-0.1.2/src/smart_data_science/ui/ui_assistant.py
+-rw-r--r--   0        0        0     8145 2023-06-11 19:15:17.906588 smart_data_science-0.1.2/src/smart_data_science/ui/ui_info.py
+-rw-r--r--   0        0        0     8144 2023-06-11 19:15:17.906588 smart_data_science-0.1.2/src/smart_data_science/ui/ui_io.py
+-rw-r--r--   0        0        0     6234 2023-06-11 19:15:17.906588 smart_data_science-0.1.2/src/smart_data_science/ui/ui_table_definition.py
+-rw-r--r--   0        0        0     4142 2023-06-11 19:15:17.906588 smart_data_science-0.1.2/src/smart_data_science/ui/ui_template.py
+-rw-r--r--   0        0        0     5600 1970-01-01 00:00:00.000000 smart_data_science-0.1.2/setup.py
+-rw-r--r--   0        0        0     5383 1970-01-01 00:00:00.000000 smart_data_science-0.1.2/PKG-INFO
```

### Comparing `smart_data_science-0.1.1/LICENSE` & `smart_data_science-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/README.md` & `smart_data_science-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/pyproject.toml` & `smart_data_science-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Note: Ths file is generated by the cookiecutter template and modify with poetry commands. It's not neccessary to
 # edit it manually (advanced).
 # The pyproject.toml file with Poetry: https://python-poetry.org/docs/pyproject/
 # Fast Reference: https://py-pkgs.org/03-how-to-package-a-python#summary-and-next-steps
 
 [tool.poetry]
 name = "smart_data_science"
-version = "0.1.1"
+version = "0.1.2"
 description = "Personal side project to streamline the most common tasks of data science solutions in an efficient manner. This project is based on my experience as a lead data scientist in the industry and financial services sectors, where I have gained expertise in delivering effective data-driven insights and solutions"
 authors = ["Angel Martinez-Tenor <angelmtenor@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
@@ -52,36 +52,42 @@
 pandas-profiling = { version = ">=3.4.0", python = ">=3.10,<3.11", optional = true }
 streamlit = { version = ">=1.15.0", python = ">=3.10,<4.0", optional = true }
 sentence-transformers = { version = ">=2.2.2", python = ">=3.10,<4.0", optional = true }
 # google-cloud-storage = { version = ">=2.6.0", python = ">=3.10,<4.0", optional = true }
 # google-cloud-bigquery = { version = ">=3.4.0", python = ">=3.10,<4.0", optional = true }
 # networkx = { version = ">=2.8.8", optional = true}
 uvicorn = { version = ">=0.20.0", optional = true }
+
+openai = { version = ">=0.27.6", optional = true }
+google-cloud-aiplatform = { version = ">=1.25.0", optional = true }
+
 gunicorn = ">=20.1.0"
 fastapi = ">=0.93.0"
-graphviz = "^0.20.1"
-chart-studio = "^1.1.0"
-ua-parser = "^0.16.1"
-openai = "^0.27.6"
-python-dotenv = "^1.0.0"
+graphviz = ">=0.20.1"
+chart-studio = ">=1.1.0"
+ua-parser = ">=0.16.1"
+python-dotenv = ">=1.0.0"
+langchain = ">=0.0.186"
+tabulate = ">=0.9.0"
 
 [tool.poetry.extras]
 full = [
     "scikit-learn",
     "lightgbm",
     "shap",
     "flask-simplelogin",
     "explainerdashboard",
     "mapie",
     "plotly",
     "pandas-profiling",
     "streamlit",
     "sentence-transformers",
     "networkx",
-
+    "openai",
+    "google-cloud-aiplatform",
     # "google-cloud-storage",
     # "google-cloud-bigquery",
 ] # poetry install --extras full  ;  pip install utils_tabular_data[full]
 ml = [
     "scikit-learn",
     "scikit-optimize",
     "lightgbm",
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/__init__.py` & `smart_data_science-0.1.2/src/smart_data_science/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """ Python Package init file """
 # pylint: disable=unused-import, wrong-import-position
+# isort:skip_file
 import warnings
 from importlib.metadata import version  # read version from installed package
 
 from numba.core.errors import NumbaDeprecationWarning  # shap issue
 
 warnings.simplefilter("ignore", category=NumbaDeprecationWarning)
 
-
+from .process.clean import optimize_schema  # noqa: F401, E402
 from .analysis.info import info_data  # noqa: F401, E402
 from .core import logger  # io, system  # noqa: F401, E402
-from .core.data_samples_module import load_sample  # noqa: F401, E402
+from .core.samples_data_module import load_sample  # noqa: F401, E402
 from .core.system import info_system  # noqa: F401, E402
+
+# Must be the last one to avoid circular imports
 from .ml.ml_regressor import SmartRegressor  # noqa: F401, E402
-from .process.clean import optimize_schema  # noqa: F401, E402
 
 __version__ = version("smart_data_science")
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/analysis/info.py` & `smart_data_science-0.1.2/src/smart_data_science/analysis/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,17 @@
     """
     if table_name:
         log.info(Markdown(f"## {table_name}"))
     log.info(f"{df.shape[0]:,} samples and {df.shape[1]:,} variables  ({get_memory_usage(df)} MB)")
     if var_names:
         log.info(f"{list(df)}")
     if unique:
+        if exclude_unique is None:
+            # exclude numerical variables
+            exclude_unique = df.select_dtypes(include=np.number).columns.tolist()
         fig_unique = show_unique(df, plot=plot, exclude=exclude_unique)
         if fig_unique:
             fig_unique.show()
     if missing:
         fig_missing = show_missing(df, plot=plot)
         if fig_missing:
             fig_missing.show()
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/analysis/info_advanced.py` & `smart_data_science-0.1.2/src/smart_data_science/analysis/info_advanced.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/analysis/plot.py` & `smart_data_science-0.1.2/src/smart_data_science/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/cloud/gcp.py` & `smart_data_science-0.1.2/src/smart_data_science/cloud/gcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from pathlib import Path
 from typing import Dict
 
 import pandas as pd
 from google.cloud import aiplatform  # pylint: disable=import-error, no-name-in-module
 from google.cloud import bigquery, storage  # type: ignore # pylint: disable=import-error, no-name-in-module
 from google.protobuf import json_format  # pylint: disable=import-error, no-name-in-module
+from google.protobuf.json_format import MessageToDict
 from google.protobuf.struct_pb2 import Value  # pylint: disable=import-error, no-name-in-module
 
 from smart_data_science import logger
 
 log = logger.get_logger(__name__)
 
 global_client_storage = None
@@ -191,15 +192,15 @@
     instance = json_format.ParseDict(instance_dict, Value())
     instances = [instance]
     parameters_dict: dict = {}
     parameters = json_format.ParseDict(parameters_dict, Value())
     endpoint = client.endpoint_path(project=project, location=location, endpoint=endpoint_id)
     response = client.predict(endpoint=endpoint, instances=instances, parameters=parameters)
     predictions = response.predictions
-    return dict(predictions[0])  # Only one prediction is returned
+    return MessageToDict(predictions[0])  # dict(predictions[0])  # Only one prediction is returned
 
 
 # def get_from_bigquery() -> pd.DataFrame:
 #     """Get the normalized dataframe from BigQuery
 #     Returns:
 #         pd.DataFrame: Normalized dataframe
 #     """
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/core/data_samples/README.md` & `smart_data_science-0.1.2/src/smart_data_science/core/samples_data/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,14 @@
 ## Acknowledgments
 
 - `shipping_logs` is based on a sample in Amazon SageMaker for Supply chain delivery. The full description and the original dataset can be found [here](https://catalog.us-east-1.prod.workshops.aws/workshops/80ba0ea5-7cf9-4b8c-9d3f-1cd988b6c071/en-US/7-supply-chain/).
 
+- `sales_supermarket` description and original dataset from [Kaggle](https://www.kaggle.com/datasets/yasserh/walmart-dataset)
+
 - `churn_bank` description and original dataset from [Kaggle](https://www.kaggle.com/datasets/sonalidasgupta95/churn-prediction-of-bank-customers)
 
-- `mpm` description and original dataset from [Kaggle](https://www.kaggle.com/datasets/shivamb/machine-predictive-maintenance-classification)
+- `electric_motor_50k.parquet` description and original dataset from [Kaggle](https://www.kaggle.com/datasets/wkirgsn/electric-motor-temperature)
+
+- 'energy_building.parquet' description and original dataset from [UCI](https://archive.ics.uci.edu/ml/datasets/Appliances+energy+prediction)
+
+<!--
+- `mpm` description and original dataset from [Kaggle](https://www.kaggle.com/datasets/shivamb/machine-predictive-maintenance-classification) -->
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/core/data_samples/churn_bank.csv` & `smart_data_science-0.1.2/src/smart_data_science/core/samples_data/churn_bank.csv`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/core/data_samples/sales_supermarkets.parquet` & `smart_data_science-0.1.2/src/smart_data_science/core/samples_data/supermarket_sales.parquet`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/core/data_samples/shipping_logs.csv` & `smart_data_science-0.1.2/src/smart_data_science/core/samples_data/supply_chain.csv`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/core/io.py` & `smart_data_science-0.1.2/src/smart_data_science/core/io.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,26 +5,102 @@
 - Dev Date:         2017 - 2022
 
 - Status:           Planning
 """
 
 from __future__ import annotations
 
+import importlib.util
 import time
 from datetime import datetime
 from pathlib import Path
 
 import pandas as pd
 
 from smart_data_science import logger
 
 log = logger.get_logger(__name__)
 
 
-def load_datafile(filepath: str | Path, usecols: list[str] = None, cache=False) -> pd.DataFrame:
+def get_files(path: str | Path, template: str = "*"):
+    """
+    Get a list of all files in the specified path that match the specified template.
+
+    Args:
+        path: Path to the folder containing the files.
+        template : Template for the filenames.
+
+    Returns:
+        List[str]: Filenames that match the template, or None if the specified path doesn't exist or there are no
+        files with the specified template.
+    """
+    path = Path(path)
+    if not path.exists():
+        log.warning(f"Path '{path}' doesn't exist.")
+        return None
+    files = list(path.glob(template))
+    if not files:
+        log.warning(f"No files found in '{path}' with template '{template}'.")
+        return None
+    return files
+
+
+def import_custom_module(module_path):
+    """
+    Import the specified Python module. e.g.: used for importing scenario modules.
+
+    Args:
+        module_path (str): Path to the module file.
+
+    Returns:
+        module: Imported module.
+    """
+    module_name = Path(module_path).stem
+    spec = importlib.util.spec_from_file_location(module_name, module_path)
+    module = importlib.util.module_from_spec(spec)
+    spec.loader.exec_module(module)
+    return module
+
+
+def format_prefixed_name(name, prefix="", separator="_", capitalize=True):
+    """
+    Convert a name in the format "<prefix><name1_name2_ ...>" to a more readable format.
+
+    Args:
+        name (str): Name in the format "<prefix><name>".
+        prefix (str): Prefix to remove from the name. Default is "".
+        separator (str): Separator between words in the name. Default is "_".
+        capitalize (bool): Whether to capitalize the first letter of each word. Default is True.
+
+    Returns:
+        str: Formatted name, or the input string if it doesn't start with the prefix.
+
+    Examples:
+        >>> format_prefixed_name("scenario_supermarket_sales", "scenario_")
+        'Supermarket Sales'
+    """
+    if not name.startswith(prefix):
+        return name
+
+    name = str(Path(name).stem)
+
+    # Remove the prefix and split the name into words
+    words = name[len(prefix) :].split(separator)  # noqa: E203
+
+    # Format the words
+    if capitalize:
+        words = [word.capitalize() for word in words]
+
+    # Join the words with spaces
+    formatted_name = " ".join(words)
+
+    return formatted_name
+
+
+def load_datafile(filepath: str | Path, usecols: list[str] = None, cache=False) -> pd.DataFrame | None:
     """Read a parquet, csv or excel (first sheet) table and return it as a dataframe
     If no extension is given, it will try to get source files in this order: .parquet > .csv  > .xlsx
     Args:
         filepath (str|Path): Path of the source File (extension not needed)
         usecols (list[str], optional): List of columns to load. Defaults to None (all columns).
     Returns:
         pd.DataFrame: Loaded table
@@ -115,15 +191,15 @@
         filepath_list = target_path.glob(f"{match_string}{suffix}")
         dict_filepaths.update({Path(filepath).stem: filepath for filepath in filepath_list})
     if show_output:
         log.info(f"Data Files found in {target_path}: {dict_filepaths.keys()}")
     return dict_filepaths
 
 
-def get_creation_date(filepath: str | Path) -> datetime:
+def get_creation_date(filepath: str | Path) -> datetime | None:
     """
     Return the creation date of the file found in filepath (return None if not found)
     Args:
         filepath: The path to the file to get the creation date of
     Returns:
         pd.datetime: The creation date of the file in datetime format
     """
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/core/logger.py` & `smart_data_science-0.1.2/src/smart_data_science/core/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 TIMESTAMP_REDUCED = "%H:%M:%S"
 TIMESTAMP_FILENAME = "%Y-%m-%d %H-%M-%S"
 
 global_dict: dict = {"logger": None}  # mutable global variable to store the logger
 
 
 def init(
-    logger_name=APP_LOGGER_NAME,
-    filepath=None,
-    level=logging.INFO,
+    logger_name: str = APP_LOGGER_NAME,
+    filepath: Path | str = None,  # type: ignore
+    level: str | int = logging.INFO,
     simple_format: bool = True,
     subfolder: Path | str | None = None,
     filename_modifier: str = "",
-    save_log=False,
+    save_log: bool = False,
 ) -> logging.Logger:
     """Initialize the logger for a high-level application.
     Args:
         logger_name (str): Name of the logger. Default: APP_LOGGER_NAME
         filepath (pathlib.Path): Path of the log file. Default: None (default LOG_PATH / filename)
         level (int): Logging level: 10:'DEBUG', 20:'INFO', 30:'WARNING', 40:'ERROR', 50:'CRITICAL'. Default: 20 (INFO)
         simple_format (bool): If True (default) , use a simple format for the log messages (simple timestamp + message)
@@ -61,14 +61,15 @@
     if filename_modifier:
         filename_prefix += f"_{filename_modifier}"
     filename = f"{filename_prefix}.log"
 
     if not filepath:
         filepath = LOG_PATH / Path(subfolder) / Path(filename) if subfolder else LOG_PATH / Path(filename)
 
+    filepath = Path(filepath)
     filepath.parent.mkdir(exist_ok=True, parents=True)
     logger = logging.getLogger(logger_name)
     logger.setLevel(level)
     if simple_format:
         formatter = logging.Formatter("%(asctime)s - %(levelname)s \t %(message)s", TIMESTAMP_REDUCED)
     else:
         formatter = logging.Formatter("%(asctime)s - %(name)s  \t %(levelname)s - %(message)s", TIMESTAMP_COMPLETE)
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/core/system.py` & `smart_data_science-0.1.2/src/smart_data_science/core/system.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,23 +74,26 @@
     current_path = Path.cwd()
     if current_path != target_path:
         os.chdir(target_path)
         if show_info:
             log.info(f"Working Path changed to {Path().absolute()}")
 
 
-def change_dir_to_parent(target_path: Path | str, show_info=False) -> None:
+def change_dir_to_parent(target_path: Path | str = None, show_info=False) -> None:
     """Change the current working directory to the parent one. If a target_path is given, the current working is checked
     against it and forced to the parent if not found.
     Used to execute notebooks located in subfolders. For a more general solution, see 'change_dir' function
 
     Args:
         execution_path (Path or str): Execution path. e.g.: 'my-cloned-repo/'
         show_info (bool, optional): Show info about the change of execution path. Defaults to False.
     """
+    if target_path is None:
+        target_path = get_root("src")  # default to parent of src folder
+
     target_path = Path(target_path)
     desired_folder = target_path.stem
     current_folder = Path().absolute().stem
     if current_folder != desired_folder:
         app_dir = Path().absolute() / target_path
         os.chdir(app_dir)
         current_folder = Path().absolute().stem
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/dev/modelling/ml_classifier_old_format/prediction.py` & `smart_data_science-0.1.2/src/smart_data_science/dev/modelling/ml_classifier_old_format/prediction.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/graph_data/network_graph.py` & `smart_data_science-0.1.2/src/smart_data_science/graph_data/network_graph.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ml/ml_base.py` & `smart_data_science-0.1.2/src/smart_data_science/ml/ml_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import shap
 from explainerdashboard import RegressionExplainer  # ExplainerDashboard
 from IPython.display import display  # import display (for notebooks)
 from sklearn.model_selection import cross_validate
 from sklearn.pipeline import Pipeline
 
 from smart_data_science.core import logger
+from smart_data_science.core.scenario_base import ScenarioBase
 from smart_data_science.ml import ml_contributions, ml_intervals, ml_tune, ml_utils  # ml_counterfactual
 from smart_data_science.ml.plot_contributions import plot_contributions_summary  # plot_interval_predictions
 
 # from .info_advanced import find_similar_samples
 
 # from .transform import multi_to_single_index
 
@@ -67,56 +68,81 @@
         numerical_features (list(str)): numerical features
         categorical_features (list(str)): categorical features
         pipeline (sklearn Pipeline): Pipeline
         input_ml_model (sklearn-type estimator): ML model (the trained one will be saved in the pipeline)
         path_ml_pipeline (str): path to save/load the ML pipeline
         description (str): description of the Object / ML pipeline
         chronological_split (bool): if True, the split between train and test is done chronologically
-        grouped_col (str): auxiliary column to plot the result grouped by this column
+        group_col (str): auxiliary column to plot the result grouped by this column
         target_units (str): units of the target variable
         dashboard_title (str): title of the dashboard
         model_folder (str): folder where the model is saved
         dict_metrics (dict): dictionary with the metrics to be used
         dict_metrics_type (dict): dictionary with the type of metrics (minimize or maximize)
         dict_metrics_scoring (dict): dictionary with the scoring to be used
         model_type (ModelType): type of model (classifier or regressor)  # leave blank to be inferred
     """
 
-    df: pd.DataFrame
-    target: str
+    df: pd.DataFrame = None
+    target: str = None
     numerical_features: list[str] = None
     categorical_features: list[str] = None
+
     pipeline: Pipeline = None
     input_ml_model: object = None
+    input_ml_params = None
+    model_folder: str | Path = None  # folder where the model is saved
+
     path_ml_pipeline: str = DEFAULT_PATH_ML_PIPELINE
     description: str = None
     chronological_split: bool = False
-    grouped_col: str = None  # auxiliary column to plot the result grouped by this column
+    group_col: str = None  # auxiliary column to plot the result grouped by this column
     target_units: str = None  # units of the target variable
     dashboard_title: str = None  # title of the dashboard
-    model_folder: str = None  # folder where the model is saved
     dict_metrics: dict = None
     dict_metrics_type: dict = None
     dict_metrics_scoring: dict = None
     model_type: ml_utils.ModelType = None
     default_ml_model = None
+    scenario: ScenarioBase = None
 
-    def __post_init__(self) -> None:
+    def __post_init__(self) -> None:  # noqa: R0915 # pylint: disable=too-many-statements
         """Post initialization"""
-        processed_dict = ml_utils.preprocess_input_data(
-            self.df, self.target, self.numerical_features, self.categorical_features, self.model_type
-        )
 
-        ml_utils.info_ml_data(processed_dict)
+        self.features: list[str] = None
+
+        if self.scenario is not None:
+            log.info(f"Loading Parameters from Scenario {self.scenario.label}")
+            self.df = self.scenario.df
+            self.target = self.scenario.target
+            self.features = self.scenario.features
+            self.numerical_features = self.scenario.numerical_features
+            self.categorical_features = self.scenario.categorical_features
+            self.group_col = self.scenario.group_col
+
+            self.input_ml_model = self.scenario.input_ml_model
+            self.input_ml_params = self.scenario.input_ml_params
+            self.model_folder = self.scenario.model_folder
+            self.chronological_split = self.scenario.chronological_split
 
-        self.df = processed_dict["df"]
-        self.target = processed_dict["target"]
-        self.features = processed_dict["features"]
-        self.numerical_features = processed_dict["numerical_features"]
-        self.categorical_features = processed_dict["categorical_features"]
+            self.dashboard_title = self.scenario.label  # TODO remove dashboard_title
+            self.target_units = self.scenario.target_units
+
+        else:
+            processed_dict = ml_utils.preprocess_input_data(
+                self.df, self.target, self.numerical_features, self.categorical_features, self.model_type
+            )
+
+            ml_utils.info_ml_data(processed_dict)
+
+            self.df = processed_dict["df"]
+            self.target = processed_dict["target"]
+            self.features = processed_dict["features"]
+            self.numerical_features = processed_dict["numerical_features"]
+            self.categorical_features = processed_dict["categorical_features"]
 
         self.x = self.df[self.features].copy()
         self.y = self.df[self.target].copy()
 
         # Initialize empty variables
 
         self.scores: dict = {}
@@ -141,16 +167,16 @@
         self.df_contributions: pd.DataFrame = None
         self.df_last_predictions: pd.DataFrame = None
         self.df_last_contributions: pd.DataFrame = None
         self.test_size: float = None
         self.random_state: int = None
         self.default_param_grid: dict = None
         self.df_contributions_summary: pd.DataFrame = None
-        self.pipeline_lower = None
-        self.pipeline_upper = None
+        self.pipeline_lower: Pipeline = None
+        self.pipeline_upper: Pipeline = None
 
         self.build_pipeline(input_ml_model=self.input_ml_model)
 
     def build_pipeline(self, input_ml_model=None, preprocess: bool = True) -> Pipeline:
         """Return a production scikit-learn Pipeline (transformer + estimator)
         (usually already tuned and validated)
 
@@ -256,18 +282,17 @@
         self.y_train = y_train
         self.y_test = y_test
         self.test_size = test_size
         self.random_state = random_state
 
         return x_train, x_test, y_train, y_test
 
-    def fit(self, plot: bool = False, cv: int = 10) -> None:  # TO IMPROVE: Move to ML utils?
+    def fit(self, cv: int = 10) -> None:  # TO IMPROVE: Move to ML utils?
         """Train & evaluate a ML pipeline
         Args:
-            plot (bool, optional): if True, plot the results. Defaults to False.
             cv (int, optional): Number of folds for cross validation.
         """
 
         start_time = time.time()
 
         if self.x_train is None:
             x_train, x_test, y_train, y_test = self.split_data(chronological_split=self.chronological_split)
@@ -307,21 +332,19 @@
         self.df_pred = df_pred.join(y_test)
 
         end_time = time.time()
         log.info(f"Total Training (CV) and evaluation time: {end_time - start_time:.0f} seconds")
 
         log.info(self.get_summary())
         display(self.display_scores())
-        if self.grouped_col:
-            display(self.get_scores_grouped(self.df_pred, self.grouped_col))
-
-        if plot and self.model_type.is_regressor():
-            self.plot_predictions_vs_target()  # TODO: REMOVE OBSOLETE
+        if self.group_col:
+            display(self.get_scores_grouped(self.df_pred, self.group_col))
 
-        # TO IMPROVE: Retrain removing features with very low global contribution
+        # TO IMPROVE: Retrain removing features with very low global contribution (via LLM with feature engineering or
+        #  Rule based)
 
     def evaluate(self, x_test: pd.DataFrame, y_test: pd.DataFrame | pd.Series):
         """Show the R2 score and MAD
         Args:
             x_test (pd.DataFrame): Test features
             y_test (pd.DataFrame | pd.Series): Test target
         """
@@ -387,59 +410,78 @@
         if df is None:
             df = self.df_contributions_summary.copy()
 
         fig = plot_contributions_summary(df, title=title)
 
         return fig
 
-    def get_summary(self) -> str:
-        """Return a summary string of the model"""
+    def get_summary(self) -> dict:  # TODO: improve this
+        """Return a summary dict of the model"""
+
+        summary_dict = {}
+        if self.scenario is not None:
+            summary_dict = self.scenario.summary_dict
+
+        summary_dict.update(
+            {
+                "target": self.target,
+                "numerical_features": self.numerical_features,
+                "categorical_features": self.categorical_features,
+                "model": self.pipeline["ml_model"].__class__.__name__,
+                "ml_params": ml_utils.remove_null_params(ml_utils.get_ml_params(self.pipeline)),
+                "training_samples": self.df_train.shape[0],
+                "test_samples": self.df_test.shape[0],
+                "test_size": self.test_size,
+                "random_state": self.random_state,
+                "results": self.scores,
+            }
+        )
+        if self.df_contributions_summary is not None:
+            dict_contributions = self.df_contributions_summary.to_dict()
+            # force all the values to 3 decimals
+            dict_contributions = {k: round(v, 3) for k, v in dict_contributions.items()}
+
+            summary_dict.update({"global_contributions_to_predictions": dict_contributions})
+
         summary_dict = {
-            "Target": self.target,
-            "Numerical Features": self.numerical_features,
-            "Categorical Features": self.categorical_features,
-            "Model": self.pipeline["ml_model"].__class__.__name__,
-            "Model Parameters": ml_utils.remove_null_params(ml_utils.get_ml_params(self.pipeline)),
-            "Training Samples": self.df_train.shape[0],
-            "Test Samples": self.df_test.shape[0],
-            "Test Size": self.test_size,
-            "Random State": self.random_state,
-            "Results": self.scores,
+            k: v for k, v in summary_dict.items() if v is not None and v is not False  # and k != "description"
         }
 
-        summary_str = "SUMMARY:\n\n"
-        for key, value in summary_dict.items():
-            if isinstance(value, list):
-                value = ", ".join(value)
-            elif isinstance(value, dict):
-                plain_str = ""
-                for k, v in value.items():
-                    # if isinstance(v, str):
-                    plain_str += f"\n- {k:<22} {v}"
-                    # else:
-                    #     plain_str += f"{k}: {v}, "
-                value = plain_str
-            key = f"{key}:"
-            summary_str += f"{key:<22} {value}\n"
-        return summary_str
+        # summary_str = "SUMMARY:\n\n"
+        # for key, value in summary_dict.items():
+        #     if isinstance(value, list):
+        #         value = ", ".join(value)
+        #     elif isinstance(value, dict):
+        #         plain_str = ""
+        #         for k, v in value.items():
+        #             # if isinstance(v, str):
+        #             plain_str += f"\n- {k:<22} {v}"
+        #             # else:
+        #             #     plain_str += f"{k}: {v}, "
+        #         value = plain_str
+        #     key = f"{key}:"
+        #     summary_str += f"{key:<22} {value}\n"
+        return summary_dict  # summary_str
 
     def generate_shap_explainer(self):
         """Generate the SHAP explainer"""
         assert self.pipeline is not None, "Pipeline is not fitted yet. Please fit the pipeline first"
         self.explainer = ml_contributions.generate_shap_explainer(self.pipeline)
 
-    def get_contributions(self, df: pd.DataFrame = None, plot=True, save=False) -> pd.DataFrame:
+    def get_contributions(self, df: pd.DataFrame = None, save=False) -> pd.DataFrame:
         """Get the contributions of each feature to the prediction (SHAP)
         Args:
             df (pd.DataFrame): Data to predict
-            plot (bool, optional): Plot the contributions. Defaults to True.
             save_explainer (bool, optional): Save the explainer and contributions to the object. Defaults to False.
 
         Returns:
             pd.DataFrame: contributions to the prediction (SHAP)
+
+        To plot: fig = self.plot_contributions_summary(self.df_contributions_summary)
+
         """
         # shap.initjs()
         if self.explainer is None:
             self.generate_shap_explainer()
 
         if df is None:
             df = self.df_pred.copy()
@@ -453,24 +495,22 @@
             shap_values, feature_names_transformed, self.categorical_features, df
         )
         # explainer = shap.TreeExplainer(ml_model, feature_perturbation="tree_path_dependent")
 
         # df_contributions_summary = (
         #     df_contributions.apply(abs).mean().sort_values(ascending=False).astype("float32").round(3)
         # )
-        if plot:
-            pass
-            # fig = self.plot_contributions_summary(df_contributions_summary)  # TODO Remove (obsolete)
 
         if save:
             self.df_contributions = df_contributions
             self.x_transformed = x_transformed
             self.feature_names_transformed = feature_names_transformed
             self.df_contributions_summary = df_contributions_summary
             self.shap_values = shap_values
+
         return df_contributions
 
     def fit_intervals(self, confidence: float = None):
         """Generate prediction intervals model
         Args:
             confidence (float, optional): Confidence interval.
         """
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ml/ml_classifier.py` & `smart_data_science-0.1.2/src/smart_data_science/ml/ml_classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         numerical_features (list(str)): numerical features
         categorical_features (list(str)): categorical features
         pipeline (sklearn Pipeline): Pipeline
         input_ml_model (sklearn-type estimator): ML model (the trained one will be saved in the pipeline)
         path_ml_pipeline (str): path to save/load the ML pipeline
         description (str): description of the Object / ML pipeline
         chronological_split (bool): if True, the split between train and test is done chronologically
-        grouped_col (str): auxiliary column to plot the result grouped by this column
+        group_col (str): auxiliary column to plot the result grouped by this column
         target_units (str): units of the target variable
         dashboard_title (str): title of the dashboard
         model_folder (str): folder where the model is saved
     """
 
     default_ml_model: LGBMClassifier = DEFAULT_ML_MODEL
     # default_param_grid: dict = DEFAULT_PARAM_GRID
@@ -273,15 +273,15 @@
 
             # df_pred["predicted_interval_%"] = 100 * df_pred["predicted_interval_diff"] / df_pred["predicted"]
 
         # Generate contributions
         if contributions:
             if logs:
                 log.info("Getting contributions ...")
-            df_contributions = self.get_contributions(x, plot=False, save=save)
+            df_contributions = self.get_contributions(x, save=save)
         else:
             df_contributions = None
 
         self.df_last_predictions = df_pred.copy()
         self.df_last_contributions = df_contributions.copy()
 
         # numeric_cols = [col for col in df_pred.columns if df_pred[col].dtype not in ["object", "category"]]
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ml/ml_contributions.py` & `smart_data_science-0.1.2/src/smart_data_science/ml/ml_contributions.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ml/ml_intervals.py` & `smart_data_science-0.1.2/src/smart_data_science/ml/ml_intervals.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ml/ml_regressor.py` & `smart_data_science-0.1.2/src/smart_data_science/ml/ml_regressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 log = logger.get_logger(__name__)
 
 MODEL_TYPE = ModelType(ModelType.REGRESSOR)
 
 DEFAULT_PATH_OBJECT = "model/smart_regressor.pkl"
 CONFIDENCE_INTERVAL = 0.95  # used for Interval Prediction. 95% by default (alpha = 0.05)
 
-DEFAULT_ML_PARAMS = {"max_depth": 7, "n_estimators": 250, "n_jobs": -1}
+DEFAULT_ML_PARAMS = {"max_depth": 7, "n_estimators": 150, "n_jobs": -1}  # down from 250 to 150 (faster demos)
 DEFAULT_ML_MODEL = LGBMRegressor(**DEFAULT_ML_PARAMS)
 
 DEFAULT_PARAM_GRID = {  # used for Bayesian optimization/tunning (BayesSearchCV)
     "ml_model__colsample_bytree": [None],
     "ml_model__max_depth": [7, 9, 11, 13, 15, 17],
     "ml_model__n_estimators": [30, 50, 70, 100, 250, 400, 600],
     "ml_model__learning_rate": [0.01, 0.05, 0.1, 0.2, 0.3, 0.5],
@@ -97,15 +97,15 @@
         numerical_features (list(str)): numerical features
         categorical_features (list(str)): categorical features
         pipeline (sklearn Pipeline): Pipeline
         input_ml_model (sklearn-type estimator): ML model (the trained one will be saved in the pipeline)
         path_ml_pipeline (str): path to save/load the ML pipeline
         description (str): description of the Object / ML pipeline
         chronological_split (bool): if True, the split between train and test is done chronologically
-        grouped_col (str): auxiliary column to plot the result grouped by this column
+        group_col (str): auxiliary column to plot the result grouped by this column
         target_units (str): units of the target variable
         dashboard_title (str): title of the dashboard
         model_folder (str): folder where the model is saved
     """
 
     default_ml_model: LGBMRegressor = DEFAULT_ML_MODEL
     # default_param_grid: dict = DEFAULT_PARAM_GRID
@@ -199,15 +199,15 @@
 
             df_pred["predicted_interval_%"] = 100 * df_pred["predicted_interval_diff"] / df_pred["predicted"]
 
         # Generate contributions
         if contributions:
             if logs:
                 log.info("Getting contributions ...")
-            df_contributions = self.get_contributions(x, plot=False, save=save)
+            df_contributions = self.get_contributions(x, save=save)
         else:
             df_contributions = None
 
         self.df_last_predictions = df_pred.copy()
         self.df_last_contributions = df_contributions.copy()
 
         # numeric_cols = [col for col in df_pred.columns if df_pred[col].dtype not in ["object", "category"]]
@@ -399,15 +399,15 @@
         Plot the Predicted vs True Target
         Args:
             df: dataframe with predictions. If None, the current self.df_pred is used
         """
 
         if df is None:
             df = self.df_pred
-        fig = plot_predictions_vs_target(df, self.target, grouped_col=self.grouped_col)
+        fig = plot_predictions_vs_target(df, self.target, group_col=self.group_col)
         return fig
 
     def plot_interval_predictions(self, df: pd.DataFrame):
         """
         Plot the interval Predictions along with the Predicted & True Target
         Args:
             df: dataframe with predictions. If None, the current 100 samples self.df_pred with sorted index is used
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ml/ml_tune.py` & `smart_data_science-0.1.2/src/smart_data_science/ml/ml_tune.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ml/ml_utils.py` & `smart_data_science-0.1.2/src/smart_data_science/ml/ml_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,18 +162,18 @@
         transformers=[
             ("num", numerical_transformer, numerical_features),
             ("cat", categorical_transformer, categorical_features),
         ],
         sparse_threshold=0,
     )
 
-    pipeline = Pipeline(steps=[("preprocessor", preprocessor), ("ml_model", ml_model)])
+    pipeline = Pipeline(steps=[("preprocessor", preprocessor), ("ml_model", ml_model)])  # memory=cache_dir)
 
     if not preprocess:
-        pipeline = Pipeline(steps=[("ml_model", ml_model)])
+        pipeline = Pipeline(steps=[("ml_model", ml_model)])  # memory=cache_dir) To Improve: add cache_dir
 
     info_model(pipeline)
 
     return pipeline
 
 
 def split_data(
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ml/plot_classifier.py` & `smart_data_science-0.1.2/src/smart_data_science/ml/plot_classifier.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ml/plot_contributions.py` & `smart_data_science-0.1.2/src/smart_data_science/ml/plot_contributions.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ml/plot_general.py` & `smart_data_science-0.1.2/src/smart_data_science/ml/plot_general.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ml/plot_intervals.py` & `smart_data_science-0.1.2/src/smart_data_science/ml/plot_intervals.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ml/plot_regressor.py` & `smart_data_science-0.1.2/src/smart_data_science/ml/plot_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 
 pd.options.plotting.backend = "plotly"
 
 
 log = logger.get_logger(__name__)
 
 
-def plot_predictions_vs_target(df: pd.DataFrame, target: str, predicted="predicted", grouped_col=None) -> go.Figure:
+def plot_predictions_vs_target(df: pd.DataFrame, target: str, predicted="predicted", group_col=None) -> go.Figure:
     """
     Creates a plot with the predictions using Plotly -Regression Only
     Args:
         df: pandas DataFrame with the data.
         target: string with the name of the target variable.
         predicted: string with the name of the predicted variable.
-        grouped_col: string with the name of the column to group by.
+        group_col: string with the name of the column to group by.
 
     """
 
     fig = df.plot(
-        kind="scatter", x=target, y=predicted, color=grouped_col, title=f"Prediction vs. Actual {target} (test set)"
+        kind="scatter", x=target, y=predicted, color=group_col, title=f"Prediction vs. Actual {target} (test set)"
     )
     return fig
 
 
 # def regressor_eval(reg, x_test, y_test, plotly_fig=True, show_plot=True):
 #     """Show the evaluation of a ML regressor (tested on tree-based sklearn models)"""
 #     y_pred = reg.predict(x_test)
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/nlp/semantic_search.py` & `smart_data_science-0.1.2/src/smart_data_science/nlp/semantic_search.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/optimization/sequence.py` & `smart_data_science-0.1.2/src/smart_data_science/optimization/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 log = logger.get_logger(__name__)
 
 
 MAX_NODES = 50  # Max number of nodes to optimize. This is a limitation to avoid excessive computing in OR-Tools library
 
 
-# TODO: Add force start node
+# TODO: Add force end node
 
 
 def execute(  # pylint: disable=too-many-statements
     df: pd.DataFrame,
     start_node: str = None,
 ) -> tuple[list, float, float]:
     """Execute the sequence optimizer (SP)
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/process/clean.py` & `smart_data_science-0.1.2/src/smart_data_science/process/clean.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/process/etl.py` & `smart_data_science-0.1.2/src/smart_data_science/process/etl.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/process/transform.py` & `smart_data_science-0.1.2/src/smart_data_science/process/transform.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/time_series/date_time.py` & `smart_data_science-0.1.2/src/smart_data_science/time_series/date_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 dict_weekday = {0: "Monday", 1: "Tuesday", 2: "Wednesday", 3: "Thursday", 4: "Friday", 5: "Saturday", 6: "Sunday"}
 
 # Dicts used to parse the text schedules of the custom designation table:
 int2weekday = {0: "Mon", 1: "Tue", 2: "Wed", 3: "Thu", 4: "Fri", 5: "Sat", 6: "Sun"}
 weekday2int = {v: k for k, v in int2weekday.items()}
 
 months = [
-    "january",
-    "february",
-    "march",
-    "april",
-    "may",
-    "june",
-    "july",
-    "august",
-    "september",
-    "october",
-    "november",
-    "december",
+    "January",
+    "February",
+    "March",
+    "April",
+    "May",
+    "June",
+    "July",
+    "August",
+    "September",
+    "October",
+    "November",
+    "December",
 ]
 months_short = [i[:3] for i in months]
 
 
 def next_sunday(input_datetime: datetime.date) -> datetime.date:
     """
     Return a datetime.date object with the next Sunday of the input_datetime
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ui/ui_info.py` & `smart_data_science-0.1.2/src/smart_data_science/ui/ui_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         for i in numerical:
             col1.write(f"**- {i}**")
 
         col2.write("Non Numerical Variables")
         for i in non_numerical:
             col2.write(f"**- {i}**")
 
-    show_summary_distinct_missing = st.checkbox("Show Distinct & Missing Values", value=default_on)
+    show_summary_distinct_missing = st.checkbox("Show Distinct & Missing Values", value=False)
     if show_summary_distinct_missing:
         col1, _, col2 = st.columns([3, 1, 3])  # 1, 3, 1, 3])
         col1.write(info.show_unique(df))
         missing_plot = info.show_missing(df)
         if missing_plot is not None:
             col2.write(info.show_missing(df))
         else:
@@ -212,7 +212,18 @@
 
 
 def show_result_header():
     """Custom result header to display in all the function sections"""
     st.write("_" * 30)
     st.markdown("### Results:")
     st.write("")
+
+
+def show_dict_as_table(input_dict: dict, label: str) -> None:
+    """Show a dictionary as a table
+    Args:
+        input_dict (dict): dictionary to show
+        label (str): label of the table (header)
+    """
+    series = pd.Series(input_dict)
+    series.name = label
+    st.table(series)
```

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ui/ui_io.py` & `smart_data_science-0.1.2/src/smart_data_science/ui/ui_io.py`

 * *Files identical despite different names*

### Comparing `smart_data_science-0.1.1/src/smart_data_science/ui/ui_template.py` & `smart_data_science-0.1.2/src/smart_data_science/ui/ui_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from smart_data_science import info_system, load_sample, logger
 from smart_data_science.ui.ui_info import explore_elements_of_frame, perform_query, ui_info_data
 
 # from smart_data_science.ui.ui_io import load_image
 
 # PATH_LOGO = "logo.jpg"
 
-SCENARIO_LABEL = "Utils Tabular Data"
+LABEL = "Utils Tabular Data"
 APP_PASSWORD = "AI_2023"
 
 MAX_SAMPLES_SHOWN_IN_TABLES = 20000  # Max samples shown in each table to avoid overload in UI
 
 # Streamlit Content
 SECTION_EXPLORE = " Explore"
 
@@ -63,15 +63,15 @@
 current_date_string = current_date.strftime("%Y_%m_%d")
 
 
 start_time = time.time()
 
 
 # set page title
-st.set_page_config(page_title=f"{SCENARIO_LABEL}", layout="wide")  # , page_icon='')
+st.set_page_config(page_title=f"{LABEL}", layout="wide")  # , page_icon='')
 
 # Hide Menu button & Footer
 st.markdown(
     """ <style>
 #MainMenu {visibility: hidden;}
 footer {visibility: hidden;}
 </style> """,
@@ -114,15 +114,15 @@
 
 # Streamlit Entrypoint
 
 # logo = ui_io.load_image(PATH_LOGO)
 # if logo:
 #     st.sidebar.image(logo)
 
-st.sidebar.title(SCENARIO_LABEL)
+st.sidebar.title(LABEL)
 st.sidebar.header("Exploration App for Utils Tabular Data")
 # st.sidebar.write(f"Template:\n{UI_TEMPLATE}")
 selected_section = st.sidebar.selectbox(label="", options=(SECTIONS), index=0)
 
 if st.session_state["access_granted"] is None:
     # log.debug("Requesting password")
     st.write("### Enter the Password:")
```

### Comparing `smart_data_science-0.1.1/setup.py` & `smart_data_science-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,54 +5,58 @@
 {'': 'src'}
 
 packages = \
 ['smart_data_science',
  'smart_data_science.analysis',
  'smart_data_science.cloud',
  'smart_data_science.core',
+ 'smart_data_science.core.samples_scenario',
  'smart_data_science.dev.modelling.ml_classifier_old_format',
  'smart_data_science.graph_data',
  'smart_data_science.llm',
  'smart_data_science.ml',
  'smart_data_science.nlp',
  'smart_data_science.optimization',
  'smart_data_science.process',
  'smart_data_science.time_series',
  'smart_data_science.ui']
 
 package_data = \
-{'': ['*'], 'smart_data_science.core': ['data_samples/*']}
+{'': ['*'], 'smart_data_science.core': ['samples_data/*']}
 
 install_requires = \
-['chart-studio>=1.1.0,<2.0.0',
+['chart-studio>=1.1.0',
  'fastapi>=0.93.0',
- 'graphviz>=0.20.1,<0.21.0',
+ 'graphviz>=0.20.1',
  'gunicorn>=20.1.0',
  'ipython>=8.10',
  'jupyter-contrib-nbextensions>=0.7.0',
  'jupyter>=1.0.0',
- 'openai>=0.27.6,<0.28.0',
+ 'langchain>=0.0.186',
  'pandarallel>=1.6.3',
  'pandas>=1.5.0',
  'pandera>=0.13.4',
  'psutil>=5.9.4',
  'py-cpuinfo>=9.0.0',
  'pyarrow>=9.0.0',
- 'python-dotenv>=1.0.0,<2.0.0',
+ 'python-dotenv>=1.0.0',
+ 'tabulate>=0.9.0',
  'tqdm>=4.64.1',
- 'ua-parser>=0.16.1,<0.17.0']
+ 'ua-parser>=0.16.1']
 
 extras_require = \
 {'full': ['scikit-learn>=1.2.0',
           'lightgbm>=3.3.4',
           'explainerdashboard>=0.4.2.1',
           'flask-simplelogin>=0.1.2',
           'mapie>=0.6.4',
           'shap>=0.41.0',
-          'plotly>=5.10.0'],
+          'plotly>=5.10.0',
+          'openai>=0.27.6',
+          'google-cloud-aiplatform>=1.25.0'],
  'full:python_version >= "3.10" and python_version < "3.11"': ['pandas-profiling>=3.4.0'],
  'full:python_version >= "3.10" and python_version < "4.0"': ['streamlit>=1.15.0',
                                                               'sentence-transformers>=2.2.2'],
  'ml': ['scikit-learn>=1.2.0',
         'lightgbm>=3.3.4',
         'xgboost>=1.7.3',
         'scikit-optimize>=0.9.0',
@@ -60,15 +64,15 @@
         'mapie>=0.6.4',
         'shap>=0.41.0'],
  'plot': ['plotly>=5.10.0', 'matplotlib>=3.6.3', 'seaborn>=0.12.2'],
  'ui:python_version >= "3.10" and python_version < "4.0"': ['streamlit>=1.15.0']}
 
 setup_kwargs = {
     'name': 'smart-data-science',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Personal side project to streamline the most common tasks of data science solutions in an efficient manner. This project is based on my experience as a lead data scientist in the industry and financial services sectors, where I have gained expertise in delivering effective data-driven insights and solutions',
     'long_description': '# smart_data_science\n\nPersonal side project to streamline the most common tasks of data science solutions in an efficient manner. This project is based on my experience as a lead data scientist in the industry and financial services sectors, where I have gained expertise in delivering effective data-driven insights and solutions\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)<br>\n\n## Installation in Dev / Editor mode\n\nNote: A Debian/Ubuntu Machine, VM or container is highly recommended\n\n\n**Step 0: One-time Machine setup only valid for all Data Science Projects**\n\nCreate or use a Machine with Conda, Git and Poetry as closely as defined in `.devcontainer/Dockerfile`:\n\n- This Dockerfile contains a non-root user so the same configuration can be applied to a WSL Ubuntu Machine and any Debian/Ubuntu CLoud Machine (Vertex AI workbench, Azure VM ...)\n- In case of having an Ubuntu/Debian machine with non-root user (e.g.: Ubuntu in WSL, Vertex AI VM ...), just install the tools from  "non-root user" (no sudo) section of the Dockerfile  (sudo apt-get install \\<software\\> may be required)\n- A pre-configured Cloud VM usually has Git and Conda pre-installed, those steps can be skipped\n- The development container defined in `.devcontainer/Dockerfile` can be directly used for a fast setup (Docker required).  With Visual Studio Code, just open the root folder of this repo, press `F1` and select the option **Dev Containers: Open Workspace in Container**. The container will open the same workspace after the Docker Image is built.\n\n\n**Step 1**. Enter to the root path of the repo and use or create a new conda environment for development:\n\n```bash\n$ conda create -n dev python=3.10 -y && conda activate dev\n```\n\n**Step 2**. Install all the Dependencies and the package in editor mode:\n\n```bash\n$ make setup\n```\n\n## Installation for Production/Usage (Not published in PyPi yet)\n```bash\n$ conda create -n smart python=3.10 -y && conda activate smart\n$ pip install dist/smart-data-science-0.1.1-py3-none-any.whl\n```\n\n## Installation for Production/Usage (after the package is published in PyPi)\n\n```bash\n$ pip install smart_data_science\n```\n\n\n## Usage\n\n- Still under development. Please refer to the notebooks and examples folders for usage examples\n\n## Contributing\n\nCheck out the contributing guidelines\n\n## License\n\n`smart_data_science` was created by Angel Martinez-Tenor. It is licensed under the terms of the MIT license.\n\n## Credits\n\n`smart_data_science` was created from a Data Science Template developed by Angel Martinez-Tenor. The template was built upon `py-pkgs-cookiecutter` [template] (https://github.com/py-pkgs/py-pkgs-cookiecutter)\n',
     'author': 'Angel Martinez-Tenor',
     'author_email': 'angelmtenor@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `smart_data_science-0.1.1/PKG-INFO` & `smart_data_science-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 Metadata-Version: 2.1
 Name: smart-data-science
-Version: 0.1.1
+Version: 0.1.2
 Summary: Personal side project to streamline the most common tasks of data science solutions in an efficient manner. This project is based on my experience as a lead data scientist in the industry and financial services sectors, where I have gained expertise in delivering effective data-driven insights and solutions
 License: MIT
 Author: Angel Martinez-Tenor
 Author-email: angelmtenor@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: full
 Provides-Extra: ml
 Provides-Extra: plot
 Provides-Extra: ui
-Requires-Dist: chart-studio (>=1.1.0,<2.0.0)
+Requires-Dist: chart-studio (>=1.1.0)
 Requires-Dist: explainerdashboard (>=0.4.2.1); extra == "full" or extra == "ml"
 Requires-Dist: fastapi (>=0.93.0)
 Requires-Dist: flask-simplelogin (>=0.1.2); extra == "full"
-Requires-Dist: graphviz (>=0.20.1,<0.21.0)
+Requires-Dist: google-cloud-aiplatform (>=1.25.0); extra == "full"
+Requires-Dist: graphviz (>=0.20.1)
 Requires-Dist: gunicorn (>=20.1.0)
 Requires-Dist: ipython (>=8.10)
 Requires-Dist: jupyter (>=1.0.0)
 Requires-Dist: jupyter-contrib-nbextensions (>=0.7.0)
+Requires-Dist: langchain (>=0.0.186)
 Requires-Dist: lightgbm (>=3.3.4); extra == "full" or extra == "ml"
 Requires-Dist: mapie (>=0.6.4); extra == "full" or extra == "ml"
 Requires-Dist: matplotlib (>=3.6.3); extra == "plot"
-Requires-Dist: openai (>=0.27.6,<0.28.0)
+Requires-Dist: openai (>=0.27.6); extra == "full"
 Requires-Dist: pandarallel (>=1.6.3)
 Requires-Dist: pandas (>=1.5.0)
 Requires-Dist: pandas-profiling (>=3.4.0); (python_version >= "3.10" and python_version < "3.11") and (extra == "full")
 Requires-Dist: pandera (>=0.13.4)
 Requires-Dist: plotly (>=5.10.0); extra == "full" or extra == "plot"
 Requires-Dist: psutil (>=5.9.4)
 Requires-Dist: py-cpuinfo (>=9.0.0)
 Requires-Dist: pyarrow (>=9.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.0)
 Requires-Dist: scikit-learn (>=1.2.0); extra == "full" or extra == "ml"
 Requires-Dist: scikit-optimize (>=0.9.0); extra == "ml"
 Requires-Dist: seaborn (>=0.12.2); extra == "plot"
 Requires-Dist: sentence-transformers (>=2.2.2); (python_version >= "3.10" and python_version < "4.0") and (extra == "full")
 Requires-Dist: shap (>=0.41.0); extra == "full" or extra == "ml"
 Requires-Dist: streamlit (>=1.15.0); (python_version >= "3.10" and python_version < "4.0") and (extra == "full" or extra == "ui")
+Requires-Dist: tabulate (>=0.9.0)
 Requires-Dist: tqdm (>=4.64.1)
-Requires-Dist: ua-parser (>=0.16.1,<0.17.0)
+Requires-Dist: ua-parser (>=0.16.1)
 Requires-Dist: uvicorn (>=0.20.0)
 Requires-Dist: xgboost (>=1.7.3); extra == "ml"
 Description-Content-Type: text/markdown
 
 # smart_data_science
 
 Personal side project to streamline the most common tasks of data science solutions in an efficient manner. This project is based on my experience as a lead data scientist in the industry and financial services sectors, where I have gained expertise in delivering effective data-driven insights and solutions
```

