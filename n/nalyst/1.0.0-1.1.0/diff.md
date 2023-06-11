# Comparing `tmp/nalyst-1.0.0.tar.gz` & `tmp/nalyst-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-1.0.0.tar", last modified: Sat May  6 07:29:50 2023, max compression
+gzip compressed data, was "nalyst-1.1.0.tar", last modified: Sun Jun 11 13:11:42 2023, max compression
```

## Comparing `nalyst-1.0.0.tar` & `nalyst-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 07:29:50.157330 nalyst-1.0.0/
--rw-rw-rw-   0        0        0       49 2023-05-06 07:29:02.000000 nalyst-1.0.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4156 2023-05-06 07:29:50.155829 nalyst-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3039 2023-05-06 07:01:11.000000 nalyst-1.0.0/README.md
--rw-rw-rw-   0        0        0     1369 2023-05-06 07:00:07.000000 nalyst-1.0.0/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:29:50.152839 nalyst-1.0.0/nalyst/
--rw-rw-rw-   0        0        0      824 2023-04-21 15:26:54.000000 nalyst-1.0.0/nalyst/BetaFive.py
--rw-rw-rw-   0        0        0     1111 2023-04-21 14:56:18.000000 nalyst-1.0.0/nalyst/BetaMax.py
--rw-rw-rw-   0        0        0     2899 2023-05-02 15:50:18.000000 nalyst-1.0.0/nalyst/CorrelationAnalysis.py
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-1.0.0/nalyst/DecisionTree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-1.0.0/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3010 2023-04-21 15:26:24.000000 nalyst-1.0.0/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-1.0.0/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-1.0.0/nalyst/MaxAbsScaler.py
--rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-1.0.0/nalyst/MinMaxScaler.py
--rw-rw-rw-   0        0        0     1324 2023-04-21 15:49:00.000000 nalyst-1.0.0/nalyst/MonteCarloSimulator.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-1.0.0/nalyst/PCA.py
--rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-1.0.0/nalyst/RegressionPlot.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-1.0.0/nalyst/StandardScaler.py
--rw-rw-rw-   0        0        0     3285 2023-05-06 06:46:38.000000 nalyst-1.0.0/nalyst/StockAnalyzer.py
--rw-rw-rw-   0        0        0     2341 2023-05-02 16:29:32.000000 nalyst-1.0.0/nalyst/StockVolatility.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-1.0.0/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-1.0.0/nalyst/ThresholdClassifier.py
--rw-rw-rw-   0        0        0     2771 2023-05-02 15:46:55.000000 nalyst-1.0.0/nalyst/TrendAnalyst.py
--rw-rw-rw-   0        0        0     1369 2023-05-06 07:00:18.000000 nalyst-1.0.0/nalyst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:29:50.155829 nalyst-1.0.0/nalyst.egg-info/
--rw-rw-rw-   0        0        0     4156 2023-05-06 07:29:50.000000 nalyst-1.0.0/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      681 2023-05-06 07:29:50.000000 nalyst-1.0.0/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 07:29:50.000000 nalyst-1.0.0/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-05-06 07:29:50.000000 nalyst-1.0.0/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-06 07:29:50.000000 nalyst-1.0.0/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 07:29:50.157330 nalyst-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1553 2023-05-06 07:29:36.000000 nalyst-1.0.0/setup.py
--rw-rw-rw-   0        0        0       19 2023-05-06 07:28:38.000000 nalyst-1.0.0/version.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:11:42.064716 nalyst-1.1.0/
+-rw-rw-rw-   0        0        0      100 2023-06-11 13:11:00.000000 nalyst-1.1.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4249 2023-06-11 13:11:42.064716 nalyst-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3130 2023-06-11 13:11:24.000000 nalyst-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1486 2023-06-11 13:09:47.000000 nalyst-1.1.0/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:11:42.049767 nalyst-1.1.0/nalyst/
+-rw-rw-rw-   0        0        0      824 2023-04-21 15:26:54.000000 nalyst-1.1.0/nalyst/BetaFive.py
+-rw-rw-rw-   0        0        0     1111 2023-04-21 14:56:18.000000 nalyst-1.1.0/nalyst/BetaMax.py
+-rw-rw-rw-   0        0        0     2899 2023-05-02 15:50:18.000000 nalyst-1.1.0/nalyst/CorrelationAnalysis.py
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-1.1.0/nalyst/DecisionTree.py
+-rw-rw-rw-   0        0        0      614 2023-06-11 13:06:18.000000 nalyst-1.1.0/nalyst/EMA.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-1.1.0/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3010 2023-04-21 15:26:24.000000 nalyst-1.1.0/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-1.1.0/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-1.1.0/nalyst/MaxAbsScaler.py
+-rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-1.1.0/nalyst/MinMaxScaler.py
+-rw-rw-rw-   0        0        0     1324 2023-04-21 15:49:00.000000 nalyst-1.1.0/nalyst/MonteCarloSimulator.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-1.1.0/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     1980 2023-04-21 13:25:37.000000 nalyst-1.1.0/nalyst/RegressionPlot.py
+-rw-rw-rw-   0        0        0      560 2023-06-11 13:05:17.000000 nalyst-1.1.0/nalyst/SMA.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-1.1.0/nalyst/StandardScaler.py
+-rw-rw-rw-   0        0        0     3285 2023-05-06 06:46:38.000000 nalyst-1.1.0/nalyst/StockAnalyzer.py
+-rw-rw-rw-   0        0        0     2341 2023-05-02 16:29:32.000000 nalyst-1.1.0/nalyst/StockVolatility.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-1.1.0/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0     2217 2023-04-21 11:44:13.000000 nalyst-1.1.0/nalyst/ThresholdClassifier.py
+-rw-rw-rw-   0        0        0     2771 2023-05-02 15:46:55.000000 nalyst-1.1.0/nalyst/TrendAnalyst.py
+-rw-rw-rw-   0        0        0     1486 2023-06-11 13:09:37.000000 nalyst-1.1.0/nalyst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 13:11:42.063720 nalyst-1.1.0/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     4249 2023-06-11 13:11:41.000000 nalyst-1.1.0/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2023-06-11 13:11:41.000000 nalyst-1.1.0/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 13:11:41.000000 nalyst-1.1.0/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-06-11 13:11:41.000000 nalyst-1.1.0/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-11 13:11:41.000000 nalyst-1.1.0/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-11 13:11:42.068703 nalyst-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1553 2023-06-11 13:10:10.000000 nalyst-1.1.0/setup.py
+-rw-rw-rw-   0        0        0       19 2023-06-11 13:10:04.000000 nalyst-1.1.0/version.py
```

### Comparing `nalyst-1.0.0/PKG-INFO` & `nalyst-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 1.0.0
+Version: 1.1.0
 Summary: Packages for quantative analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa, Kiran Basnet
 Author-email: hemantthapa1998@gmail.com, kiransbasnet@gmail.com
 License: Proprietary License
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
@@ -88,14 +88,16 @@
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
 from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
 from nalyst.StockVolatility import stock_volatility
 from nalyst.StockAnalyzer import StockAnalyzer
+from nalyst.SMA import SimpleMovingAverage
+from nalyst.EMA import ExponentialMovingAverage
 ```
 
 6. SUPPORT
 
 If you need help or have any questions, please feel free to reach out and text to Integrated audio architecture dosen't support google collab or cloud system. 
 
 7. COMMUNICATION
```

### Comparing `nalyst-1.0.0/README.md` & `nalyst-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,16 @@
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
 from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
 from nalyst.StockVolatility import stock_volatility
 from nalyst.StockAnalyzer import StockAnalyzer
+from nalyst.SMA import SimpleMovingAverage
+from nalyst.EMA import ExponentialMovingAverage
 ```
 
 6. SUPPORT
 
 If you need help or have any questions, please feel free to reach out and text to Integrated audio architecture dosen't support google collab or cloud system. 
 
 7. COMMUNICATION
```

### Comparing `nalyst-1.0.0/__init__.py` & `nalyst-1.1.0/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
 from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
 from nalyst.StockVolatility import stock_volatility
 from nalyst.StockAnalyzer import StockAnalyzer
+from nalyst.SMA import SimpleMovingAverage
+from nalyst.EMA import ExponentialMovingAverage
 
 __all__ = [
     "LinearRegression",
     "DecisionTree",
     "KMeans",
     "PCA",
     "LogisticRegression",
@@ -32,8 +34,10 @@
     "BetaMax",
     "SharpRatio",
     "ThresholdClassifier",
     "LinearCorrelationVisualizer",
     "LinearRegressionVisualizer",
     "StockVolatility",
     "StockAnalyzer",
+    "SMA",
+    "EMA",
 ]
```

### Comparing `nalyst-1.0.0/nalyst/BetaFive.py` & `nalyst-1.1.0/nalyst/BetaFive.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/BetaMax.py` & `nalyst-1.1.0/nalyst/BetaMax.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/CorrelationAnalysis.py` & `nalyst-1.1.0/nalyst/CorrelationAnalysis.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/DecisionTree.py` & `nalyst-1.1.0/nalyst/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/KMeans.py` & `nalyst-1.1.0/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/LinearRegression.py` & `nalyst-1.1.0/nalyst/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/LogisticRegression.py` & `nalyst-1.1.0/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/MaxAbsScaler.py` & `nalyst-1.1.0/nalyst/MaxAbsScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/MinMaxScaler.py` & `nalyst-1.1.0/nalyst/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/MonteCarloSimulator.py` & `nalyst-1.1.0/nalyst/MonteCarloSimulator.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/PCA.py` & `nalyst-1.1.0/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/RegressionPlot.py` & `nalyst-1.1.0/nalyst/RegressionPlot.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/StandardScaler.py` & `nalyst-1.1.0/nalyst/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/StockAnalyzer.py` & `nalyst-1.1.0/nalyst/StockAnalyzer.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/StockVolatility.py` & `nalyst-1.1.0/nalyst/StockVolatility.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/TestTrainSplit.py` & `nalyst-1.1.0/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/ThresholdClassifier.py` & `nalyst-1.1.0/nalyst/ThresholdClassifier.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/TrendAnalyst.py` & `nalyst-1.1.0/nalyst/TrendAnalyst.py`

 * *Files identical despite different names*

### Comparing `nalyst-1.0.0/nalyst/__init__.py` & `nalyst-1.1.0/nalyst/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
 from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
 from nalyst.StockVolatility import stock_volatility
 from nalyst.StockAnalyzer import StockAnalyzer
+from nalyst.SMA import SimpleMovingAverage
+from nalyst.EMA import ExponentialMovingAverage
 
 __all__ = [
     "LinearRegression",
     "DecisionTree",
     "KMeans",
     "PCA",
     "LogisticRegression",
@@ -32,8 +34,10 @@
     "BetaMax",
     "SharpRatio",
     "ThresholdClassifier",
     "LinearCorrelationVisualizer",
     "LinearRegressionVisualizer",
     "StockVolatility",
     "StockAnalyzer",
+    "SMA",
+    "EMA",
 ]
```

### Comparing `nalyst-1.0.0/nalyst.egg-info/PKG-INFO` & `nalyst-1.1.0/nalyst.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 1.0.0
+Version: 1.1.0
 Summary: Packages for quantative analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa, Kiran Basnet
 Author-email: hemantthapa1998@gmail.com, kiransbasnet@gmail.com
 License: Proprietary License
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
@@ -88,14 +88,16 @@
 from nalyst.BetaMax import calculate_beta_max
 from nalyst.ThresholdClassifier import ThresholdClassifier, ThresholdPlot
 from nalyst.RegressionPlot import RegressionPlot
 from nalyst.CorrelationAnalysis import LinearCorrelationVisualizer
 from nalyst.TrendAnalyst import LinearRegressionVisualizer
 from nalyst.StockVolatility import stock_volatility
 from nalyst.StockAnalyzer import StockAnalyzer
+from nalyst.SMA import SimpleMovingAverage
+from nalyst.EMA import ExponentialMovingAverage
 ```
 
 6. SUPPORT
 
 If you need help or have any questions, please feel free to reach out and text to Integrated audio architecture dosen't support google collab or cloud system. 
 
 7. COMMUNICATION
```

### Comparing `nalyst-1.0.0/nalyst.egg-info/SOURCES.txt` & `nalyst-1.1.0/nalyst.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 CHANGELOG.txt
 MANIFEST.in
 README.md
 __init__.py
 pyproject.toml
+setup.cfg
 setup.py
 version.py
 nalyst/BetaFive.py
 nalyst/BetaMax.py
 nalyst/CorrelationAnalysis.py
 nalyst/DecisionTree.py
+nalyst/EMA.py
 nalyst/KMeans.py
 nalyst/LinearRegression.py
 nalyst/LogisticRegression.py
 nalyst/MaxAbsScaler.py
 nalyst/MinMaxScaler.py
 nalyst/MonteCarloSimulator.py
 nalyst/PCA.py
 nalyst/RegressionPlot.py
+nalyst/SMA.py
 nalyst/StandardScaler.py
 nalyst/StockAnalyzer.py
 nalyst/StockVolatility.py
 nalyst/TestTrainSplit.py
 nalyst/ThresholdClassifier.py
 nalyst/TrendAnalyst.py
 nalyst/__init__.py
```

### Comparing `nalyst-1.0.0/setup.py` & `nalyst-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 with io.open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="nalyst",
-    version="1.0.0",
+    version="1.1.0",
     author="Hemant Thapa, Kiran Basnet",
     author_email="hemantthapa1998@gmail.com, kiransbasnet@gmail.com",
     description="Packages for quantative analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/harryworlds/nalyst",
     packages=find_packages(),
```

