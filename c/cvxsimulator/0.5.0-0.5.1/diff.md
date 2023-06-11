# Comparing `tmp/cvxsimulator-0.5.0.tar.gz` & `tmp/cvxsimulator-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.5.0.tar", max compression
+gzip compressed data, was "cvxsimulator-0.5.1.tar", max compression
```

## Comparing `cvxsimulator-0.5.0.tar` & `cvxsimulator-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11375 2023-06-06 05:24:40.839610 cvxsimulator-0.5.0/LICENSE
--rw-r--r--   0        0        0     5052 2023-06-06 05:24:40.839610 cvxsimulator-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-06-06 05:24:40.915611 cvxsimulator-0.5.0/cvx/simulator/__init__.py
--rw-r--r--   0        0        0    16264 2023-06-06 05:24:40.915611 cvxsimulator-0.5.0/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1613 2023-06-06 05:24:40.915611 cvxsimulator-0.5.0/cvx/simulator/grid.py
--rw-r--r--   0        0        0     1209 2023-06-06 05:24:40.915611 cvxsimulator-0.5.0/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1457 2023-06-06 05:24:40.915611 cvxsimulator-0.5.0/cvx/simulator/month.py
--rw-r--r--   0        0        0    19295 2023-06-06 05:24:40.915611 cvxsimulator-0.5.0/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      795 2023-06-06 05:24:40.915611 cvxsimulator-0.5.0/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      608 2023-06-06 05:25:06.343972 cvxsimulator-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5639 1970-01-01 00:00:00.000000 cvxsimulator-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-06-11 21:28:16.366250 cvxsimulator-0.5.1/LICENSE
+-rw-r--r--   0        0        0     5051 2023-06-11 21:28:16.366250 cvxsimulator-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 21:28:16.458251 cvxsimulator-0.5.1/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    16264 2023-06-11 21:28:16.458251 cvxsimulator-0.5.1/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1613 2023-06-11 21:28:16.458251 cvxsimulator-0.5.1/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1209 2023-06-11 21:28:16.458251 cvxsimulator-0.5.1/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1457 2023-06-11 21:28:16.458251 cvxsimulator-0.5.1/cvx/simulator/month.py
+-rw-r--r--   0        0        0    19295 2023-06-11 21:28:16.458251 cvxsimulator-0.5.1/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      795 2023-06-11 21:28:16.458251 cvxsimulator-0.5.1/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      633 2023-06-11 21:28:52.266601 cvxsimulator-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5643 1970-01-01 00:00:00.000000 cvxsimulator-0.5.1/PKG-INFO
```

### Comparing `cvxsimulator-0.5.0/LICENSE` & `cvxsimulator-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.0/README.md` & `cvxsimulator-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,14 @@
 from cvx.simulator.portfolio import EquityPortfolio
 
 prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
 stocks = pd.read_csv(Path("resources") / "stock.csv", index_col=0, parse_dates=True, header=0)
 portfolio = EquityPortfolio(prices=prices, stocks=stocks, initial_cash=1e6)
 ```
 
-
 ## Poetry
 
 We assume you share already the love for [Poetry](https://python-poetry.org). Once you have installed poetry you can perform
 
 ```bash
 poetry install
 ```
```

### Comparing `cvxsimulator-0.5.0/cvx/simulator/builder.py` & `cvxsimulator-0.5.1/cvx/simulator/builder.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.0/cvx/simulator/grid.py` & `cvxsimulator-0.5.1/cvx/simulator/grid.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.0/cvx/simulator/metrics.py` & `cvxsimulator-0.5.1/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.0/cvx/simulator/month.py` & `cvxsimulator-0.5.1/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.0/cvx/simulator/portfolio.py` & `cvxsimulator-0.5.1/cvx/simulator/portfolio.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.0/cvx/simulator/trading_costs.py` & `cvxsimulator-0.5.1/cvx/simulator/trading_costs.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.0/pyproject.toml` & `cvxsimulator-0.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.5.0"
+version = "v0.5.1"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8"
+python = ">=3.8,<4.0"
 numpy = "*"
 pandas = "*"   # unfortunately crash with quantstats for pandas >= 2.0.0
 
 [tool.poetry.dev-dependencies]
 pytest = "7.2.0"
-pytest-cov = "4.0.0"
+pytest-cov = "*"
 yfinance = "*"
 quantstats = "*"
 plotly = "*"
 cvxpy = "*"
 jupyterlab = "*"
+jupyter-book = "0.15.1"
 loguru = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cvxsimulator-0.5.0/PKG-INFO` & `cvxsimulator-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.5.0
+Version: 0.5.1
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy
 Requires-Dist: pandas
@@ -133,15 +133,14 @@
 from cvx.simulator.portfolio import EquityPortfolio
 
 prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
 stocks = pd.read_csv(Path("resources") / "stock.csv", index_col=0, parse_dates=True, header=0)
 portfolio = EquityPortfolio(prices=prices, stocks=stocks, initial_cash=1e6)
 ```
 
-
 ## Poetry
 
 We assume you share already the love for [Poetry](https://python-poetry.org). Once you have installed poetry you can perform
 
 ```bash
 poetry install
 ```
```

