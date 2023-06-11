# Comparing `tmp/financetoolkit-1.0.0.tar.gz` & `tmp/financetoolkit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financetoolkit-1.0.0.tar", max compression
+gzip compressed data, was "financetoolkit-1.0.1.tar", max compression
```

## Comparing `financetoolkit-1.0.0.tar` & `financetoolkit-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1069 2023-05-11 17:19:30.665832 financetoolkit-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0    15144 2023-05-31 12:09:31.687752 financetoolkit-1.0.0/README.md
--rw-r--r--   0        0        0      126 2023-05-31 11:54:14.444472 financetoolkit-1.0.0/financetoolkit/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 11:11:47.294669 financetoolkit-1.0.0/financetoolkit/base/__init__.py
--rw-r--r--   0        0        0     2050 2023-05-31 11:24:34.980993 financetoolkit-1.0.0/financetoolkit/base/helpers.py
--rw-r--r--   0        0        0        0 2023-05-15 11:11:47.296959 financetoolkit-1.0.0/financetoolkit/base/models/__init__.py
--rw-r--r--   0        0        0    10797 2023-05-31 11:56:11.886202 financetoolkit-1.0.0/financetoolkit/base/models/fundamentals_model.py
--rw-r--r--   0        0        0     4067 2023-05-15 16:09:01.630088 financetoolkit-1.0.0/financetoolkit/base/models/historical_model.py
--rw-r--r--   0        0        0     4267 2023-05-31 11:54:23.375640 financetoolkit-1.0.0/financetoolkit/base/models/normalization/README.md
--rw-r--r--   0        0        0     1813 2023-05-17 13:55:45.906209 financetoolkit-1.0.0/financetoolkit/base/models/normalization/balance.csv
--rw-r--r--   0        0        0     1364 2023-05-22 14:14:21.474129 financetoolkit-1.0.0/financetoolkit/base/models/normalization/cash.csv
--rw-r--r--   0        0        0     1119 2023-05-17 13:55:45.906558 financetoolkit-1.0.0/financetoolkit/base/models/normalization/income.csv
--rw-r--r--   0        0        0     4119 2023-05-22 13:38:39.982344 financetoolkit-1.0.0/financetoolkit/base/models/normalization_model.py
--rw-r--r--   0        0        0     2751 2023-05-31 11:56:07.209163 financetoolkit-1.0.0/financetoolkit/base/models_controller.py
--rw-r--r--   0        0        0    53898 2023-05-31 11:56:06.770771 financetoolkit-1.0.0/financetoolkit/base/ratios_controller.py
--rw-r--r--   0        0        0    17522 2023-05-31 11:55:53.562679 financetoolkit-1.0.0/financetoolkit/base/toolkit_controller.py
--rw-r--r--   0        0        0        0 2023-05-15 11:11:47.299347 financetoolkit-1.0.0/financetoolkit/historical/__init__.py
--rw-r--r--   0        0        0     2804 2023-05-15 11:11:47.299799 financetoolkit-1.0.0/financetoolkit/historical/price.py
--rw-r--r--   0        0        0        0 2023-05-11 14:54:28.954198 financetoolkit-1.0.0/financetoolkit/models/__init__.py
--rw-r--r--   0        0        0     5436 2023-05-31 11:56:10.551208 financetoolkit-1.0.0/financetoolkit/models/dupont.py
--rw-r--r--   0        0        0        0 2023-05-25 15:20:11.154442 financetoolkit-1.0.0/financetoolkit/portfolio/__init__.py
--rw-r--r--   0        0        0     5958 2023-05-11 17:58:02.180112 financetoolkit-1.0.0/financetoolkit/portfolio/portfolio.py
--rw-r--r--   0        0        0        0 2023-05-11 14:28:40.501711 financetoolkit-1.0.0/financetoolkit/ratios/__init__.py
--rw-r--r--   0        0        0     9590 2023-05-17 08:05:36.449227 financetoolkit-1.0.0/financetoolkit/ratios/efficiency.py
--rw-r--r--   0        0        0     5236 2023-05-17 08:05:36.439746 financetoolkit-1.0.0/financetoolkit/ratios/liquidity.py
--rw-r--r--   0        0        0    12600 2023-05-17 08:05:36.464750 financetoolkit-1.0.0/financetoolkit/ratios/profitability.py
--rw-r--r--   0        0        0     7090 2023-05-17 08:05:36.450598 financetoolkit-1.0.0/financetoolkit/ratios/solvency.py
--rw-r--r--   0        0        0    15285 2023-05-16 12:25:42.268831 financetoolkit-1.0.0/financetoolkit/ratios/valuation.py
--rw-r--r--   0        0        0     1769 2023-05-31 11:56:48.189557 financetoolkit-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    16286 1970-01-01 00:00:00.000000 financetoolkit-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 17:19:30.665832 financetoolkit-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0    15188 2023-06-11 09:18:37.060648 financetoolkit-1.0.1/README.md
+-rw-r--r--   0        0        0      126 2023-05-31 11:54:14.444472 financetoolkit-1.0.1/financetoolkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:11:47.294669 financetoolkit-1.0.1/financetoolkit/base/__init__.py
+-rw-r--r--   0        0        0     2018 2023-06-11 09:17:50.971134 financetoolkit-1.0.1/financetoolkit/base/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:11:47.296959 financetoolkit-1.0.1/financetoolkit/base/models/__init__.py
+-rw-r--r--   0        0        0    10651 2023-06-11 09:17:50.971389 financetoolkit-1.0.1/financetoolkit/base/models/fundamentals_model.py
+-rw-r--r--   0        0        0     4047 2023-06-11 09:17:50.971609 financetoolkit-1.0.1/financetoolkit/base/models/historical_model.py
+-rw-r--r--   0        0        0     4267 2023-05-31 11:54:23.375640 financetoolkit-1.0.1/financetoolkit/base/models/normalization/README.md
+-rw-r--r--   0        0        0     1813 2023-05-17 13:55:45.906209 financetoolkit-1.0.1/financetoolkit/base/models/normalization/balance.csv
+-rw-r--r--   0        0        0     1364 2023-05-22 14:14:21.474129 financetoolkit-1.0.1/financetoolkit/base/models/normalization/cash.csv
+-rw-r--r--   0        0        0     1119 2023-05-17 13:55:45.906558 financetoolkit-1.0.1/financetoolkit/base/models/normalization/income.csv
+-rw-r--r--   0        0        0     4071 2023-06-11 09:17:50.971830 financetoolkit-1.0.1/financetoolkit/base/models/normalization_model.py
+-rw-r--r--   0        0        0     2657 2023-06-11 09:17:50.972035 financetoolkit-1.0.1/financetoolkit/base/models_controller.py
+-rw-r--r--   0        0        0    53732 2023-06-11 09:17:50.972402 financetoolkit-1.0.1/financetoolkit/base/ratios_controller.py
+-rw-r--r--   0        0        0    17521 2023-06-11 09:17:50.972687 financetoolkit-1.0.1/financetoolkit/base/toolkit_controller.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:11:47.299347 financetoolkit-1.0.1/financetoolkit/historical/__init__.py
+-rw-r--r--   0        0        0     2635 2023-06-11 09:17:50.972933 financetoolkit-1.0.1/financetoolkit/historical/price.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:54:28.954198 financetoolkit-1.0.1/financetoolkit/models/__init__.py
+-rw-r--r--   0        0        0     5133 2023-06-11 09:17:50.973201 financetoolkit-1.0.1/financetoolkit/models/dupont.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:20:11.154442 financetoolkit-1.0.1/financetoolkit/portfolio/__init__.py
+-rw-r--r--   0        0        0     5632 2023-06-11 09:17:50.973438 financetoolkit-1.0.1/financetoolkit/portfolio/portfolio.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:28:40.501711 financetoolkit-1.0.1/financetoolkit/ratios/__init__.py
+-rw-r--r--   0        0        0     8587 2023-06-11 09:17:50.973751 financetoolkit-1.0.1/financetoolkit/ratios/efficiency.py
+-rw-r--r--   0        0        0     4658 2023-06-11 09:17:50.973973 financetoolkit-1.0.1/financetoolkit/ratios/liquidity.py
+-rw-r--r--   0        0        0    11177 2023-06-11 09:17:50.974232 financetoolkit-1.0.1/financetoolkit/ratios/profitability.py
+-rw-r--r--   0        0        0     6293 2023-06-11 09:17:50.974455 financetoolkit-1.0.1/financetoolkit/ratios/solvency.py
+-rw-r--r--   0        0        0    13584 2023-06-11 09:17:50.974710 financetoolkit-1.0.1/financetoolkit/ratios/valuation.py
+-rw-r--r--   0        0        0     1826 2023-06-11 09:17:50.974928 financetoolkit-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    16316 1970-01-01 00:00:00.000000 financetoolkit-1.0.1/PKG-INFO
```

### Comparing `financetoolkit-1.0.0/LICENSE.txt` & `financetoolkit-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.0/README.md` & `financetoolkit-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 ![FinanceToolkitCropped](https://github.com/JerBouma/FinanceToolkit/assets/46355364/198d47bd-e1b3-492d-acc4-5d9f02d1d009)
 
 [![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-Donate-brightgreen?logo=buymeacoffee)](https://www.buymeacoffee.com/jerbouma)
-[![Issues](https://img.shields.io/github/issues/jerbouma/FinanceToolkit)](https://github.com/JerBouma/FinanceToolkit/issues)
-[![Pull Requests](https://img.shields.io/github/issues-pr/JerBouma/FinanceToolkit?color=yellow)](https://github.com/JerBouma/FinanceToolkit/pulls)
+[![Website](https://img.shields.io/badge/Website-Learn%20more%20about%20me%20here-brightgreen?logo=ReadMe)](https://jeroenbouma.com/)
 [![PYPI Version](https://img.shields.io/pypi/v/FinanceToolkit)](https://pypi.org/project/FinanceToolkit/)
 [![PYPI Downloads](https://img.shields.io/pypi/dm/FinanceToolkit)](https://pypi.org/project/FinanceToolkit/)
 
+**NOTE: THIS VERSION HAS ALL TYPING REMOVED AND THUS SUPPORTS PYTHON VERSIONS LESS THAN PYTHON 3.10. THIS IS MERELY MEANT TO SUPPORT THOSE WHO HAVEN"T UPDATED YET AND WON"T BE MAINTAINED FURTHER. PLEASE VISIT THE LATEST BUILD AND UPDATE PYTHON ACCORDINGLY**
+
 While browsing a variety of websites, I kept finding that the same financial metric can greatly vary per source and so do the financial statements reported while little information is given how the metric was calculated.
 
 For example, Microsoft's Price-to-Earnings (PE) ratio on the 6th of May, 2023 is reported to be 28.93 (Stockopedia), 32.05 (Morningstar), 32.66 (Macrotrends), 33.09 (Finance Charts), 33.66 (Y Charts), 33.67 (Wall Street Journal), 33.80 (Yahoo Finance) and 34.4 (Companies Market Cap). All of these calculations are correct, however the method applied varies leading to different results. Therefore, collecting data from multiple sources can lead to wrong interpretation of the results given that one source could be applying a different calculation method than another. And that is, if it is even freely available. Often the calculation is hidden behind a paid subscription.
 
 **This is why I designed the FinanceToolkit**, this is an open-source toolkit in which all relevant financial ratios (50+), indicators and performance measurements are written down in the most simplistic way allowing for complete transparency of the calculation method. This allows you to not have to rely on metrics from other providers and, given a financial statement, allow for efficient manual calculations. This leads to one uniform method of calculation being applied that is available and understood by everyone.
 
 The Finance Toolkit is complimented very well with the [Finance Database 🌎](https://github.com/JerBouma/FinanceDatabase), a database that features 300.000+ symbols containing Equities, ETFs, Funds, Indices, Currencies, Cryptocurrencies and Money Markets. By utilising both, it is possible to do a fully-fledged competitive analysis with the tickers found from the FinanceDatabase inputted into the FinanceToolkit.
 
-**Disclaimer:** this package used to be called 'FundamentalAnalysis' but has since been renamed. This is a major update to the existent package which also justified a rename. The old package does remain available.
-
+ <img src="https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%205.%20Video%20Demo.gif?raw=true" alt="Finance Toolkit Illustration" width="100%"/>
+ 
 ---
 
 # Table of Contents
 
 1. [Installation](#installation)
 2. [Basic Usage](#basic-usage)
     1. [Using the Finance Toolkit](#using-the-finance-toolkit)
     2. [Working with other Datasets](#working-with-other-datasets)
     3. [Calling Functions Directly](#calling-functions-directly)
-4. [Questions & Answers](#questions--answers)
-6. [Contact](#contact)
+3. [Contact](#contact)
 
 # Installation
 
 To install the FinanceToolkit it simply requires the following:
 
 ```
 pip install financetoolkit
@@ -72,15 +72,15 @@
 - Historical market data (`historical_data`), which can be retrieved on a daily, weekly, monthly and yearly basis (from Yahoo Finance)
 - Balance Sheet Statements (`balance_sheet_statement`), Income Statements (`income_statement`) and Cash Flow Statements (`cash_flow_statement`), obtainable from FinancialModelingPrep or the source of your choosing through custom input. These functions are accompanied with a normalization function so that for any source, the same ratio analysis can be performed. Please see this Jupyter Notebook that explains how to use a custom source.
 - Efficiency ratios (`efficiency_ratios`), liquidity ratios (`liquidity_ratios`), profitability ratios (`profitability_ratios`), solvency ratios (`solvency_ratios`) and valuation ratios (`valuation_ratios`) functionality that automatically calculates the most important ratios based on the inputted balance sheet, income and cash flow statements.
 - Models (`models`) like DUPONT analysis that can be used to perform in-depth financial analysis through a single function.
 
 ## Using the Finance Toolkit
 
-A basic example of how to initialise the Finance Toolkit is shown below, also see [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%201.%20Getting%20Started.ipynb) for a detailed Getting Started guide as well as [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%202.%20Combining%20the%Finance%20Toolkit%20with%20the%20Finance%20Database.ipynb) that includes the [Finance Database 🌎](https://github.com/JerBouma/FinanceDatabase) and a proper financial analysis.
+A basic example of how to initialise the Finance Toolkit is shown below, also see [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%201.%20Getting%20Started.ipynb) for a detailed Getting Started guide as well as [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%202.%20Combining%20the%20Finance%20Toolkit%20with%20the%20Finance%20Database.ipynb) that includes the [Finance Database 🌎](https://github.com/JerBouma/FinanceDatabase) and a proper financial analysis.
 
 ````python
 from financetoolkit import Toolkit
 
 companies = Toolkit(['AAPL', 'MSFT'], api_key="FMP_KEY")
 
 # an Enterprise example
@@ -92,15 +92,15 @@
 # a Financial Statement example
 balance_sheet_statement = companies.get_balance_sheet_statement()
 
 # a Ratios example
 profitability_ratios = companies.ratios.collect_profitability_ratios()
 
 # Show the profitability ratios for Apple
-profitability_ratios.loc['AAPL]
+profitability_ratios.loc['AAPL']
 ````
 
 This returns the following output for `profitability_ratios.loc['AAPL]`. Omitting `.loc['AAPL']` will return the result for both AAPL and MSFT.
 
 
 |                                             |     2018 |     2019 |     2020 |     2021 |     2022 |
 |:--------------------------------------------|---------:|---------:|---------:|---------:|---------:|
```

### Comparing `financetoolkit-1.0.0/financetoolkit/base/helpers.py` & `financetoolkit-1.0.1/financetoolkit/base/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Helpers Module"""
 __docformat__ = "numpy"
 
 import pandas as pd
 
 
-def combine_dataframes(tickers: str | list[str], *args) -> pd.DataFrame:
+def combine_dataframes(tickers, *args):
     """
     Combine the dataframes from different companies of the same financial statement,
     e.g. the balance sheet statement, into a single dataframe.
 
     Args:
         **args: A dictionary of the same type of financial statement from multiple companies.
 
@@ -32,14 +32,15 @@
     Returns:
         function: The decorated function.
 
     Raises:
         KeyError: If an index name is missing in the provided financial statements.
         ValueError: If an error occurs while running the function, typically due to incomplete financial statements.
     """
+
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except KeyError as e:
             function_name = func.__name__
             print(
                 "There is an index name missing in the provided financial statements. "
```

### Comparing `financetoolkit-1.0.0/financetoolkit/base/models/fundamentals_model.py` & `financetoolkit-1.0.1/financetoolkit/base/models/fundamentals_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """Fundamentals Module"""
 __docformat__ = "numpy"
 
 
 import pandas as pd
 
+from typing import List
+
+
 from financetoolkit.base.models.normalization_model import (
     convert_financial_statements,
 )
 
 # pylint: disable=no-member
 
 
 def get_financial_statements(
-    tickers: str | list[str],
-    statement: str = "",
-    api_key: str = "",
+    tickers,
+    statement = "",
+    api_key = "",
     quarter: bool = False,
-    limit: int = 100,
-    statement_format: pd.DataFrame = pd.DataFrame(),
+    limit = 100,
+    statement_format = pd.DataFrame(),
 ):
     """
     Retrieves financial statements (balance, income, or cash flow statements) for one or multiple companies,
     and returns a DataFrame containing the data.
 
     Args:
         tickers (List[str]): List of company tickers.
@@ -96,15 +99,15 @@
     financial_statement_total = convert_financial_statements(
         financial_statement_total, statement_format, True
     )
 
     return financial_statement_total
 
 
-def get_profile(tickers: list[str] | str, api_key: str):
+def get_profile(tickers, api_key):
     """
     Description
     ----
     Gives information about the profile of a company which includes
     i.a. beta, company description, industry and sector.
     Input
     ----
@@ -120,28 +123,28 @@
     if isinstance(tickers, str):
         ticker_list = [tickers]
     elif isinstance(tickers, list):
         ticker_list = tickers
     else:
         raise ValueError(f"Type for the tickers ({type(tickers)}) variable is invalid.")
 
-    profile_dataframe: pd.DataFrame = pd.DataFrame()
+    profile_dataframe = pd.DataFrame()
 
     for ticker in ticker_list:
         try:
             profile_dataframe[ticker] = pd.read_json(
                 f"https://financialmodelingprep.com/api/v3/profile/{ticker}?apikey={api_key}"
             ).T
         except Exception as error:
             raise ValueError(error) from error
 
     return profile_dataframe
 
 
-def get_quote(tickers: list[str] | str, api_key: str):
+def get_quote(tickers, api_key):
     """
     Description
     ----
     Gives information about the quote of a company which includes i.a.
     high/low close prices, price-to-earning ratio and shares outstanding.
     Input
     ----
@@ -157,29 +160,29 @@
     if isinstance(tickers, str):
         ticker_list = [tickers]
     elif isinstance(tickers, list):
         ticker_list = tickers
     else:
         raise ValueError(f"Type for the tickers ({type(tickers)}) variable is invalid.")
 
-    quote_dataframe: pd.DataFrame = pd.DataFrame()
+    quote_dataframe = pd.DataFrame()
 
     for ticker in ticker_list:
         try:
             quote_dataframe[ticker] = pd.read_json(
                 f"https://financialmodelingprep.com/api/v3/quote/{ticker}?apikey={api_key}"
             ).T
         except Exception as error:
             raise ValueError(error) from error
 
     return quote_dataframe
 
 
 def get_enterprise(
-    tickers: list[str] | str, api_key: str, quarter: bool = False, limit: int = 100
+    tickers, api_key, quarter: bool = False, limit = 100
 ):
     """
     Description
     ----
     Gives information about the enterprise value of a company which includes
     i.a. market capitalisation, Cash & Cash Equivalents, total debt and enterprise value.
     Input
@@ -240,15 +243,15 @@
 
     if len(ticker_list) == 1:
         enterprise_dataframe = enterprise_dataframe.loc[ticker_list[0]]
 
     return enterprise_dataframe
 
 
-def get_rating(tickers: list[str] | str, api_key: str, limit: int = 100):
+def get_rating(tickers, api_key, limit = 100):
     """
     Description
     ----
     Gives information about the rating of a company which includes i.a. the company
     rating and recommendation as well as ratings based on a variety of ratios.
     Input
     ----
```

### Comparing `financetoolkit-1.0.0/financetoolkit/base/models/historical_model.py` & `financetoolkit-1.0.1/financetoolkit/base/models/historical_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Historical Module"""
 __docformat__ = "numpy"
 
 from datetime import datetime, timedelta
 
+from typing import List
+
+
 import pandas as pd
 
 
 def get_historical_data(
-    tickers: list[str] | str,
-    start: str = None,
-    end: str = None,
-    interval: str = "1d",
+    tickers,
+    start = None,
+    end = None,
+    interval = "1d",
 ):
     """
     Retrieves historical stock data for the given ticker(s) from Yahoo! Finance API for a specified period.
     If start and/or end date are not provided, it defaults to 10 years from the current date.
 
     Args:
         tickers (list of str): A list of one or more ticker symbols to retrieve data for.
@@ -86,15 +89,15 @@
 
     if yearly:
         historical_data = convert_daily_to_yearly(historical_data)
 
     return historical_data
 
 
-def convert_daily_to_yearly(daily_historical_data: pd.DataFrame):
+def convert_daily_to_yearly(daily_historical_data):
     """
     Converts daily historical data to yearly historical data.
 
     Args:
         daily_historical_data (pd.DataFrame): A DataFrame containing daily historical data.
 
     Returns:
```

### Comparing `financetoolkit-1.0.0/financetoolkit/base/models/normalization/README.md` & `financetoolkit-1.0.1/financetoolkit/base/models/normalization/README.md`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.0/financetoolkit/base/models/normalization/balance.csv` & `financetoolkit-1.0.1/financetoolkit/base/models/normalization/balance.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.0/financetoolkit/base/models/normalization/cash.csv` & `financetoolkit-1.0.1/financetoolkit/base/models/normalization/cash.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.0/financetoolkit/base/models/normalization/income.csv` & `financetoolkit-1.0.1/financetoolkit/base/models/normalization/income.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.0/financetoolkit/base/models/normalization_model.py` & `financetoolkit-1.0.1/financetoolkit/base/models/normalization_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import shutil
 from pathlib import Path
 
 import pandas as pd
 import pkg_resources
 
 
-def read_normalization_file(statement: str, format_location: str = ""):
+def read_normalization_file(statement, format_location = ""):
     """
     This function copies the normalization files as found inside the environment and saves them
     to a custom location defined by the user. This is designed to make it possible to edit these files
     and supply them to the financial statement functions and within the Analyzer class.
 
     Args:
         statement (string): the type of statement you wish to read (balance, income, or cash).
@@ -32,16 +32,16 @@
             __name__, f"normalization/{statement}.csv"
         ).name
 
     return pd.read_csv(file_location, index_col=[0]).iloc[:, 0]
 
 
 def convert_financial_statements(
-    financial_statements: pd.DataFrame,
-    statement_format: pd.DataFrame = pd.DataFrame(),
+    financial_statements,
+    statement_format = pd.DataFrame(),
     reverse_dates: bool = False,
 ):
     """
     Converts financial statements (balance, income, or cash flow statements) based on custom input
     and returns a DataFrame containing the data with the correct naming.
 
     Args:
@@ -75,16 +75,16 @@
     if reverse_dates:
         financial_statements = financial_statements[financial_statements.columns[::-1]]
 
     return financial_statements.sort_index(level=0, sort_remaining=False)
 
 
 def copy_normalization_files(
-    format_location: str = "",
-    save_location: str = Path(Path.home(), "Downloads"),
+    format_location = "",
+    save_location = Path(Path.home(), "Downloads"),
 ):
     """
     This function copies the normalization files as found inside the environment and saves them
     to a custom location defined by the user. This is designed to make it possible to edit these files
     and supply them to the financial statement functions and within the Analyzer class.
 
     Args:
```

### Comparing `financetoolkit-1.0.0/financetoolkit/base/models_controller.py` & `financetoolkit-1.0.1/financetoolkit/base/models_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 """Models Module"""
 __docformat__ = "numpy"
 
 import pandas as pd
 
+from typing import List
+
 from financetoolkit.base.helpers import handle_errors
 from financetoolkit.models.dupont import (
     get_dupont_analysis,
     get_extended_dupont_analysis,
 )
 
 
 class Models:
     """
     Models Controller Class
     """
 
     def __init__(
         self,
-        tickers: str | list[str],
-        balance: pd.DataFrame,
-        income: pd.DataFrame,
-        cash: pd.DataFrame,
+        tickers,
+        balance,
+        income,
+        cash,
     ):
         self._tickers = tickers
         self._balance_sheet_statement = balance
         self._income_statement = income
         self._cash_flow_statement = cash
 
         # Initialization of Model Variables
-        self._dupont_analysis: pd.DataFrame = pd.DataFrame()
-        self._extended_dupont_analysis: pd.DataFrame = pd.DataFrame()
+        self._dupont_analysis = pd.DataFrame()
+        self._extended_dupont_analysis = pd.DataFrame()
 
     @handle_errors
-    def get_dupont_analysis(self) -> pd.DataFrame:
+    def get_dupont_analysis(self):
         """
         Perform a Dupont analysis to breakdown the return on equity (ROE) into its components.
         """
         if self._dupont_analysis.empty:
             self._dupont_analysis = get_dupont_analysis(
                 self._income_statement.loc[:, "Net Income", :],
                 self._income_statement.loc[:, "Revenue", :],
@@ -48,15 +50,15 @@
 
         if len(self._tickers) == 1:
             return self._dupont_analysis.droplevel(level=0)
 
         return self._dupont_analysis
 
     @handle_errors
-    def get_extended_dupont_analysis(self) -> pd.DataFrame:
+    def get_extended_dupont_analysis(self):
         """
         Perform am Extended Dupont analysis to breakdown the return on equity (ROE) into its components.
         """
         if self._extended_dupont_analysis.empty:
             self._extended_dupont_analysis = get_extended_dupont_analysis(
                 self._income_statement.loc[:, "Income Before Tax", :],
                 self._income_statement.loc[:, "Operating Income", :],
```

### Comparing `financetoolkit-1.0.0/financetoolkit/base/ratios_controller.py` & `financetoolkit-1.0.1/financetoolkit/base/ratios_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Ratios Module"""
 __docformat__ = "numpy"
 
 import pandas as pd
 
+from typing import List
+
+
 from financetoolkit.base.helpers import handle_errors
 from financetoolkit.ratios import (
     efficiency,
     liquidity,
     profitability,
     solvency,
     valuation,
@@ -18,36 +21,36 @@
 class Ratios:
     """
     Ratios Controller Class
     """
 
     def __init__(
         self,
-        tickers: str | list[str],
-        historical: pd.DataFrame,
-        balance: pd.DataFrame,
-        income: pd.DataFrame,
-        cash: pd.DataFrame,
+        tickers,
+        historical,
+        balance,
+        income,
+        cash,
     ):
         self._tickers = tickers
         self._yearly_historical_data = historical
         self._balance_sheet_statement = balance
         self._income_statement = income
         self._cash_flow_statement = cash
 
         # Initialization of Fundamentals Variables
-        self._all_ratios: pd.DataFrame = pd.DataFrame()
-        self._efficiency_ratios: pd.DataFrame = pd.DataFrame()
-        self._liquidity_ratios: pd.DataFrame = pd.DataFrame()
-        self._profitability_ratios: pd.DataFrame = pd.DataFrame()
-        self._solvency_ratios: pd.DataFrame = pd.DataFrame()
-        self._valuation_ratios: pd.DataFrame = pd.DataFrame()
+        self._all_ratios = pd.DataFrame()
+        self._efficiency_ratios = pd.DataFrame()
+        self._liquidity_ratios = pd.DataFrame()
+        self._profitability_ratios = pd.DataFrame()
+        self._solvency_ratios = pd.DataFrame()
+        self._valuation_ratios = pd.DataFrame()
 
     def collect_all_ratios(
-        self, include_dividends: bool = False, diluted: bool = True, days: int = 365
+        self, include_dividends: bool = False, diluted: bool = True, days = 365
     ):
         """
         Calculates all Ratios based on the data provided.
         """
         if self._efficiency_ratios.empty:
             self.collect_efficiency_ratios(days=days)
         if self._liquidity_ratios.empty:
@@ -69,15 +72,15 @@
                 self._solvency_ratios,
                 self._valuation_ratios,
             ]
         )
 
         return self._all_ratios
 
-    def collect_efficiency_ratios(self, days: int = 365):
+    def collect_efficiency_ratios(self, days = 365):
         """
         Calculates all Efficiency Ratios based on the data provided.
         """
         if self._efficiency_ratios.empty:
             efficiency_ratios: dict = {}
 
             efficiency_ratios[
@@ -347,28 +350,28 @@
         return efficiency.get_inventory_turnover_ratio(
             self._income_statement.loc[:, "Cost of Goods Sold", :],
             self._balance_sheet_statement.loc[:, "Inventory", :].shift(axis=1),
             self._balance_sheet_statement.loc[:, "Inventory", :],
         )
 
     @handle_errors
-    def get_days_of_inventory_outstanding(self, days: int = 365):
+    def get_days_of_inventory_outstanding(self, days = 365):
         """
         Calculate the days sales in inventory ratio, an efficiency ratio that measures
         how long it takes a company to sell its inventory.
         """
         return efficiency.get_days_of_inventory_outstanding(
             self._balance_sheet_statement.loc[:, "Inventory", :].shift(axis=1),
             self._balance_sheet_statement.loc[:, "Inventory", :],
             self._income_statement.loc[:, "Cost of Goods Sold", :],
             days,
         )
 
     @handle_errors
-    def get_days_of_sales_outstanding(self, days: int = 365):
+    def get_days_of_sales_outstanding(self, days = 365):
         """
         Calculate the days of sales outstanding, an efficiency ratio that measures
         the average number of days it takes a company to collect payment on its
         credit sales.
         """
         return efficiency.get_days_of_sales_outstanding(
             self._balance_sheet_statement.loc[:, "Accounts Receivable", :].shift(
@@ -376,15 +379,15 @@
             ),
             self._balance_sheet_statement.loc[:, "Accounts Receivable", :],
             self._income_statement.loc[:, "Revenue", :],
             days,
         )
 
     @handle_errors
-    def get_operating_cycle(self, days: int = 365):
+    def get_operating_cycle(self, days = 365):
         """
         Calculate the operating cycle, an efficiency ratio that measures the average
         number of days it takes a company to turn its inventory into cash.
         """
         days_of_inventory = efficiency.get_days_of_inventory_outstanding(
             self._balance_sheet_statement.loc[:, "Inventory", :].shift(axis=1),
             self._balance_sheet_statement.loc[:, "Inventory", :],
@@ -411,28 +414,28 @@
         return efficiency.get_accounts_payables_turnover_ratio(
             self._income_statement.loc[:, "Cost of Goods Sold", :],
             self._balance_sheet_statement.loc[:, "Accounts Payable", :].shift(axis=1),
             self._balance_sheet_statement.loc[:, "Accounts Payable", :],
         )
 
     @handle_errors
-    def get_days_of_accounts_payable_outstanding(self, days: int = 365):
+    def get_days_of_accounts_payable_outstanding(self, days = 365):
         """
         Calculate the days payables outstanding, an efficiency ratio that measures the
         number of days it takes a company to pay its suppliers.
         """
         return efficiency.get_days_of_accounts_payable_outstanding(
             self._income_statement.loc[:, "Cost of Goods Sold", :],
             self._balance_sheet_statement.loc[:, "Accounts Payable", :].shift(axis=1),
             self._balance_sheet_statement.loc[:, "Accounts Payable", :],
             days,
         )
 
     @handle_errors
-    def get_cash_conversion_cycle(self, days: int = 365):
+    def get_cash_conversion_cycle(self, days = 365):
         """
         Calculate the Cash Conversion Cycle, which measures the amount of time it takes for a company to convert
         its investments in inventory and accounts receivable into cash, while considering the time it takes to pay
         its accounts payable.
         """
         days_of_inventory = efficiency.get_days_of_inventory_outstanding(
             self._balance_sheet_statement.loc[:, "Inventory", :].shift(axis=1),
```

### Comparing `financetoolkit-1.0.0/financetoolkit/base/toolkit_controller.py` & `financetoolkit-1.0.1/financetoolkit/base/toolkit_controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Toolkit Module"""
 __docformat__ = "numpy"
 
 
 import pandas as pd
 
+from warnings import warn
+
 from financetoolkit.base.models.fundamentals_model import (
     get_enterprise as _get_enterprise,
     get_financial_statements as _get_financial_statements,
     get_profile as _get_profile,
     get_quote as _get_quote,
     get_rating as _get_rating,
 )
@@ -36,20 +38,20 @@
     calculations. This leads to one uniform method of calculation being applied that
     is available and understood by everyone.
     """
 
     def __init__(
         self,
         tickers,
-        api_key: str = "",
-        historical: pd.DataFrame = pd.DataFrame(),
-        balance: pd.DataFrame = pd.DataFrame(),
-        income: pd.DataFrame = pd.DataFrame(),
-        cash: pd.DataFrame = pd.DataFrame(),
-        format_location: str = "",
+        api_key = "",
+        historical = pd.DataFrame(),
+        balance = pd.DataFrame(),
+        income = pd.DataFrame(),
+        cash = pd.DataFrame(),
+        format_location = "",
         reverse_dates: bool = False,
     ):
         """
         Initializes an Toolkit object with a ticker or a list of tickers.
 
         Args:
         tickers (str or list): A string or a list of strings containing the company ticker(s).
@@ -68,71 +70,77 @@
         else:
             raise TypeError("Tickers must be a string or a list of strings.")
 
         self._api_key = api_key
 
         if self._api_key:
             # Initialization of FinancialModelingPrep Variables
-            self._profile: pd.DataFrame = pd.DataFrame()
-            self._quote: pd.DataFrame = pd.DataFrame()
-            self._enterprise: pd.DataFrame = pd.DataFrame()
-            self._rating: pd.DataFrame = pd.DataFrame()
+            self._profile = pd.DataFrame()
+            self._quote = pd.DataFrame()
+            self._enterprise = pd.DataFrame()
+            self._rating = pd.DataFrame()
 
         # Initialization of Historical Variables
-        self._daily_historical_data: pd.DataFrame = (
+        self._daily_historical_data = (
             historical if not historical.empty else pd.DataFrame()
         )
-        self._weekly_historical_data: pd.DataFrame = pd.DataFrame()
-        self._monthly_historical_data: pd.DataFrame = pd.DataFrame()
-        self._yearly_historical_data: pd.DataFrame = (
+        self._weekly_historical_data = pd.DataFrame()
+        self._monthly_historical_data = pd.DataFrame()
+        self._yearly_historical_data = (
             _convert_daily_to_yearly(self._daily_historical_data)
             if not historical.empty
             else pd.DataFrame()
         )
 
         # Initialization of Normalization Variables
-        self._balance_sheet_statement_generic: pd.DataFrame = _read_normalization_file(
+        self._balance_sheet_statement_generic = _read_normalization_file(
             "balance", format_location
         )
-        self._income_statement_generic: pd.DataFrame = _read_normalization_file(
+        self._income_statement_generic = _read_normalization_file(
             "income", format_location
         )
-        self._cash_flow_statement_generic: pd.DataFrame = _read_normalization_file(
+        self._cash_flow_statement_generic = _read_normalization_file(
             "cash", format_location
         )
 
         # Initialization of Financial Statements
-        self._balance_sheet_statement: pd.DataFrame = (
+        self._balance_sheet_statement = (
             _convert_financial_statements(
                 balance, self._balance_sheet_statement_generic, reverse_dates
             )
             if not balance.empty
             else pd.DataFrame()
         )
-        self._income_statement: pd.DataFrame = (
+        self._income_statement = (
             _convert_financial_statements(
                 income, self._income_statement_generic, reverse_dates
             )
             if not income.empty
             else pd.DataFrame()
         )
-        self._cash_flow_statement: pd.DataFrame = (
+        self._cash_flow_statement = (
             _convert_financial_statements(
                 cash, self._cash_flow_statement_generic, reverse_dates
             )
             if not cash.empty
             else pd.DataFrame()
         )
 
+        warn(
+            "This version of the Finance Toolkit is deprecated. Finance Toolkit 1.0.2 and onwards require Python 3.10 and higher. Please update to the latest version of Python and the Finance Toolkit.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
     @property
     def ratios(self):
         """
         Gives access to financial ratios.
         """
-        empty_data: list = []
+        empty_data = []
 
         if not self._api_key and (
             self._balance_sheet_statement.empty
             or self._income_statement.empty
             or self._cash_flow_statement.empty
         ):
             raise ValueError(
@@ -167,15 +175,15 @@
         )
 
     @property
     def models(self):
         """
         Gives access to financial models.
         """
-        empty_data: list = []
+        empty_data = []
 
         if not self._api_key and (
             self._balance_sheet_statement.empty
             or self._income_statement.empty
             or self._cash_flow_statement.empty
         ):
             raise ValueError(
@@ -243,15 +251,15 @@
             )
 
         if self._quote.empty:
             self._quote = _get_quote(self._tickers, self._api_key)
 
         return self._quote
 
-    def get_enterprise(self, quarter: str = False, limit: str = 100):
+    def get_enterprise(self, quarter = False, limit = 100):
         """
         Returns a pandas dataframe containing the enterprise value information for the specified tickers.
 
         Args:
             quarter (str): The quarter for which the enterprise value is required. Defaults to False.
             limit (str): The number of results to return. Defaults to 100.
 
@@ -269,15 +277,15 @@
         if self._enterprise.empty:
             self._enterprise = _get_enterprise(
                 self._tickers, self._api_key, quarter, limit
             )
 
         return self._enterprise
 
-    def get_rating(self, limit: int = 100):
+    def get_rating(self, limit = 100):
         """
         Returns a pandas dataframe containing the stock rating information for the specified tickers.
 
         Args:
             limit (int): The number of results to return. Defaults to 100.
 
         Raises:
@@ -292,15 +300,15 @@
             )
 
         if self._rating.empty:
             self._rating = _get_rating(self._tickers, self._api_key, limit)
 
         return self._rating
 
-    def get_historical_data(self, start=None, end=None, period: str = "daily"):
+    def get_historical_data(self, start=None, end=None, period = "daily"):
         """
         Returns a pandas dataframe containing the historical data for the specified tickers.
 
         Args:
             start (str): The start date for the historical data. Defaults to None.
             end (str): The end date for the historical data. Defaults to None.
             period (str): The interval at which the historical data should be
@@ -368,15 +376,15 @@
         raise ValueError(
             "Please choose from daily, weekly, monthly or yearly as period."
         )
 
     def get_balance_sheet_statement(
         self,
         quarter=False,
-        limit: int = 100,
+        limit = 100,
         overwrite: bool = False,
     ):
         """
         Retrieves the balance sheet statement financial data for the company(s) from the specified source.
 
         Args:
             quarter (bool, optional): Flag to retrieve quarterly or annual data. Defaults to False.
@@ -403,15 +411,15 @@
             return self._balance_sheet_statement.loc[self._tickers[0]]
 
         return self._balance_sheet_statement
 
     def get_income_statement(
         self,
         quarter=False,
-        limit: int = 100,
+        limit = 100,
         overwrite: bool = False,
     ):
         """
         Retrieves the income statement financial data for the company(s) from the specified source.
 
         Args:
             quarter (bool, optional): Flag to retrieve quarterly or annual data. Defaults to False.
@@ -438,15 +446,15 @@
             return self._income_statement.loc[self._tickers[0]]
 
         return self._income_statement
 
     def get_cash_flow_statement(
         self,
         quarter=False,
-        limit: int = 100,
+        limit = 100,
         overwrite: bool = False,
     ):
         """
         Retrieves the cash flow statement financial data for the company(s) from the specified source.
 
         Args:
             quarter (bool, optional): Flag to retrieve quarterly or annual data. Defaults to False.
@@ -470,15 +478,15 @@
             )
 
         if len(self._tickers) == 1:
             return self._cash_flow_statement.loc[self._tickers[0]]
 
         return self._cash_flow_statement
 
-    def get_normalization_files(self, path: str = ""):
+    def get_normalization_files(self, path = ""):
         """
         Copies the normalization files to a folder based on path. By default, this is the path
         of the 'Downloads' folder.
 
         Args:
             path (str, optional): The path where to save the files to.
```

### Comparing `financetoolkit-1.0.0/financetoolkit/historical/price.py` & `financetoolkit-1.0.1/financetoolkit/historical/price.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """Price Module"""
 
 import pandas as pd
 
 
-def get_returns(historical_data: pd.Series) -> pd.Series:
+def get_returns(historical_data):
     """
     Calculate the returns of historical data for a given Series, with an option to include a rolling period.
 
     Args:
         historical_data (pd.Series): Series containing historical data.
 
     Returns:
         pd.Series: Series containing the calculated returns.
     """
     return historical_data.pct_change()
 
 
-def get_volatility(returns: pd.Series) -> pd.Series:
+def get_volatility(returns):
     """
     Calculate the volatility of returns over a rolling window.
 
     Args:
         returns (pd.Series): A Series of returns with time as index
         rolling (int): The size of the rolling window.
 
     Returns:
         pd.Series: A Series of volatility with time as index and assets as columns.
     """
     return returns.std()
 
 
 def get_sharpe_ratio(
-    returns: pd.Series, risk_free_rate: float | pd.Series
-) -> pd.Series:
+    returns, risk_free_rate
+):
     """
     Calculate the Sharpe ratio of returns over a rolling window.
 
     Args:
         returns (pd.Series): A Series of returns with time as index
         risk_free_rate (float or pd.Series): The annualized risk-free rate.
 
@@ -45,16 +45,16 @@
     """
     excess_returns = returns - risk_free_rate
 
     return excess_returns / returns.std()
 
 
 def get_sortino_ratio(
-    returns: pd.Series, risk_free_rate: float | pd.Series
-) -> pd.Series:
+    returns, risk_free_rate
+):
     """
     Calculate the Sortino ratio of returns over a rolling window.
 
     Args:
         returns (pd.Series): A Series of returns with time as index
         risk_free_rate (float or pd.Series): The annualized risk-free rate.
         rolling_window (int): The size of the rolling window.
@@ -64,15 +64,15 @@
     """
     excess_returns = returns - risk_free_rate
     downside_volatility = excess_returns[excess_returns < 0].std()
 
     return excess_returns / downside_volatility
 
 
-def get_beta(returns: pd.Series, benchmark_returns: pd.Series) -> pd.Series:
+def get_beta(returns, benchmark_returns):
     """
     Calculate the beta of returns with respect to a benchmark over a rolling window.
 
     Args:
         returns (pd.DataFrame): A DataFrame of returns with time as index and assets as columns.
         benchmark_returns (pd.DataFrame): A DataFrame of benchmark returns with time as index and a single column.
         rolling_window (int): The size of the rolling window.
```

### Comparing `financetoolkit-1.0.0/financetoolkit/models/dupont.py` & `financetoolkit-1.0.1/financetoolkit/models/dupont.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
     efficiency as _efficiency,
     profitability as _profitability,
     solvency as _solvency,
 )
 
 
 def get_dupont_analysis(
-    net_income: float | pd.Series,
-    total_revenue: float | pd.Series,
-    total_assets_begin: float | pd.Series,
-    total_assets_end: float | pd.Series,
-    total_equity_begin: float | pd.Series,
-    total_equity_end: float | pd.Series,
-) -> pd.DataFrame:
+    net_income,
+    total_revenue,
+    total_assets_begin,
+    total_assets_end,
+    total_equity_begin,
+    total_equity_end,
+):
     """
     Perform a Dupont analysis to breakdown the return on equity (ROE) into its components.
 
     Args:
         net_income (float or pd.Series): Net profit of the company.
         total_revenue (float or pd.Series): Total revenue of the company.
         total_assets_begin (float or pd.Series): Total assets of the company at the beginning of the period.
@@ -63,29 +63,29 @@
             .sort_index(level=0, sort_remaining=False)
         )
 
     return pd.DataFrame.from_dict(components, orient="index")
 
 
 def get_extended_dupont_analysis(
-    operating_income: float | pd.Series,
-    income_before_tax: float | pd.Series,
-    net_income: float | pd.Series,
-    total_revenue: float | pd.Series,
-    total_assets_begin: float | pd.Series,
-    total_assets_end: float | pd.Series,
-    total_equity_begin: float | pd.Series,
-    total_equity_end: float | pd.Series,
-) -> pd.DataFrame:
+    operating_income,
+    income_before_tax,
+    net_income,
+    total_revenue,
+    total_assets_begin,
+    total_assets_end,
+    total_equity_begin,
+    total_equity_end,
+):
     """
     Perform am Extended Dupont analysis to breakdown the return on equity (ROE) into its components.
 
     Args:
         operating_income (float or pd.Series): Operating income of the company.
-        interest_expense (float or pd.Series): Interest expense of the company.
+        interest_expense (float or pd.Series)erest expense of the company.
         income_before_tax (float or pd.Series): Income before taxes of the company.
         net_income (float or pd.Series): Net profit of the company.
         total_revenue (float or pd.Series): Total revenue of the company.
         total_assets_begin (float or pd.Series): Total assets of the company at the beginning of the period.
         total_assets_end (float or pd.Series): Total assets of the company at the end of the period.
         total_equity_begin (float or pd.Series): Total equity of the company at the beginning of the period.
         total_equity_end (float or pd.Series): Total equity of the company at the end of the period.
```

### Comparing `financetoolkit-1.0.0/financetoolkit/portfolio/portfolio.py` & `financetoolkit-1.0.1/financetoolkit/portfolio/portfolio.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,46 +2,46 @@
 __docformat__ = "numpy"
 
 import numpy as np
 import pandas as pd
 
 
 def get_tracking_error(
-    portfolio_returns: pd.Series, benchmark_returns: pd.Series
-) -> pd.Series:
+    portfolio_returns, benchmark_returns
+):
     """
     Calculate the tracking error, a measure of the deviation of a portfolio's returns
     from its benchmark.
 
     Args:
         portfolio_returns (pd.Series): A pandas series of portfolio returns.
         benchmark_returns (pd.Series): A pandas series of benchmark returns.
     Returns:
         pd.Series: A pandas series of tracking error.
     """
     return np.std(portfolio_returns - benchmark_returns)
 
 
-def get_payoff_ratio(returns: pd.Series) -> float | pd.Series:
+def get_payoff_ratio(returns) :
     """
     Calculate the Payoff Ratio, a ratio that measures the ability of a trading strategy
     to generate profits relative to its losses.
 
     Args:
         returns (pd.Series): A series of returns.
 
     Returns:
-        float | pd.Series: The Payoff Ratio value.
+        float : The Payoff Ratio value.
     """
     return np.sum(returns.where(returns > 0, 0)) / -np.sum(
         returns.where(returns < 0, 0)
     )
 
 
-def get_profit_factor(returns: pd.Series) -> pd.Series:
+def get_profit_factor(returns):
     """
     Calculate the profit factor, which measures the gross profit of winning trades
     divided by the gross loss of losing trades. A value greater than 1 indicates
     profitability, while a value less than 1 indicates unprofitability.
 
     Args:
         returns (pd.Series): Series of returns.
@@ -51,18 +51,18 @@
     Returns:
         pd.Series: Series of profit factor values.
     """
     return returns[returns > 0].sum() / abs(returns[returns < 0].sum())
 
 
 def get_jensens_alpha(
-    returns: pd.Series,
-    benchmark_returns: pd.Series,
-    risk_free_rate: float | pd.Series = 0.0,
-) -> pd.Series:
+    returns,
+    benchmark_returns,
+    risk_free_rate = 0.0,
+):
     """
     Calculates the Jensen's alpha for the given returns series relative to the given benchmark returns series.
 
     Args:
         returns (pd.Series): A series of asset returns.
         benchmark_returns (pd.Series): A series of benchmark returns.
         risk_free_rate (float or pd.Series): The annual risk-free rate, defaults to 0.0.
@@ -75,29 +75,29 @@
     excess_benchmark_returns = benchmark_returns - (risk_free_rate / 252)
 
     _, alpha = np.polyfit(excess_benchmark_returns, excess_returns, 1)
 
     return alpha
 
 
-def get_gain_to_pain_ratio(returns: pd.Series) -> pd.Series:
+def get_gain_to_pain_ratio(returns):
     """
     Calculate the gain to pain ratio, a risk-adjusted return ratio that measures the
     return of an investment relative to the drawdown experienced over the same period.
 
     Args:
         returns (pd.Series): A pandas series of returns.
 
     Returns:
         pd.Series: A pandas series of gain to pain ratio.
     """
     return returns.sum() / np.abs(returns[returns < 0].sum())
 
 
-def get_max_drawdown(returns: pd.Series) -> pd.Series:
+def get_max_drawdown(returns):
     """
     The maximum drawdown is a measure of the largest loss from
     a peak to a through of a portfolio, expressed as a percentage.
 
     Args:
         returns (pd.Series): A pandas series of returns.
 
@@ -108,43 +108,43 @@
     peak = np.maximum.accumulate(cum_returns)
     drawdown = (cum_returns - peak) / peak
     max_drawdown = np.min(drawdown)
 
     return max_drawdown
 
 
-def get_tail_ratio(returns: pd.Series) -> pd.Series:
+def get_tail_ratio(returns):
     """
     Calculate the tail ratio, a measure of the ratio of the average of the positive
     returns to the absolute value of the average of the negative returns.
 
     Args:
         returns (pd.Series): A pandas series of returns.
 
     Returns:
         pd.Series: A pandas series of tail ratio.
     """
     return np.mean(returns[returns > 0]) / np.abs(np.mean(returns[returns < 0]))
 
 
-def get_common_sense_ratio(returns: pd.Series) -> pd.Series:
+def get_common_sense_ratio(returns):
     """
     Calculate the common sense ratio, a risk-adjusted return ratio that measures the
     return of an investment relative to its maximum drawdown.
 
     Args:
         returns (pd.Series): A pandas series of returns.
 
     Returns:
         pd.Series: A pandas series of common sense ratio.
     """
     return returns.sum() / np.abs(returns.min())
 
 
-def get_calmar_ratio(returns: pd.Series) -> pd.Series:
+def get_calmar_ratio(returns):
     """
     The Calmar Ratio is a measure of risk-adjusted performance
     of an investment strategy. It is calculated by dividing the average
     annual rate of return by the maximum drawdown over a specified period.
 
     Args:
         returns (pd.Series): A series of asset returns.
@@ -160,16 +160,16 @@
             "Calmar ratio can not be calculated due to zero negative returns."
         )
 
     return average_return / maximum_drawdown
 
 
 def get_kelly_criterion(
-    win_probability: float | pd.Series, win_loss_ratio: float | pd.Series
-) -> pd.Series:
+    win_probability, win_loss_ratio
+):
     """
     Calculates the Kelly criterion for the given win and loss probabilities.
 
     The win/loss ratio rpresents the ratio of the amount won on a winning
     bet to the amount lost on a losing bet.
 
     The Kelly Criterion is a decimal value between 0 and 1, which
```

### Comparing `financetoolkit-1.0.0/financetoolkit/ratios/profitability.py` & `financetoolkit-1.0.1/financetoolkit/ratios/profitability.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,351 +1,351 @@
 """Profitability Module"""
 __docformat__ = "numpy"
 
 import pandas as pd
 
 
 def get_gross_margin(
-    revenue: float | pd.Series, cost_of_goods_sold: float | pd.Series
-) -> float | pd.Series:
+    revenue, cost_of_goods_sold
+) :
     """
     Calculate the gross margin, a profitability ratio that measures the percentage of
     revenue that exceeds the cost of goods sold.
 
     Args:
         revenue (float or pd.Series): Total revenue of the company.
         cost_of_goods_sold (float or pd.Series): Total cost of goods sold of the company.
 
     Returns:
-        float | pd.Series: The gross margin percentage value.
+        float : The gross margin percentage value.
     """
     return (revenue - cost_of_goods_sold) / revenue
 
 
 def get_operating_margin(
-    operating_income: float | pd.Series, revenue: float | pd.Series
-) -> float | pd.Series:
+    operating_income, revenue
+) :
     """
     Calculate the operating margin, a profitability ratio that measures the percentage of
     revenue that remains after deducting operating expenses.
 
     Args:
         operating_income (float or pd.Series): Operating income of the company.
         revenue (float or pd.Series): Total revenue of the company.
 
     Returns:
-        float | pd.Series: The operating margin percentage value.
+        float : The operating margin percentage value.
     """
     return operating_income / revenue
 
 
 def get_net_profit_margin(
-    net_income: float | pd.Series, revenue: float | pd.Series
-) -> float | pd.Series:
+    net_income, revenue
+) :
     """
     Calculate the net profit margin, a profitability ratio that measures the percentage
     of profit a company earns per dollar of revenue.
 
     Args:
         net_income (float or pd.Series): Net income of the company.
         revenue (float or pd.Series): Revenue of the company.
 
     Returns:
-        float | pd.Series: The net profit margin value as a percentage.
+        float : The net profit margin value as a percentage.
     """
     return net_income / revenue
 
 
 def get_interest_coverage_ratio(
-    operating_income: float | pd.Series, interest_expense: float | pd.Series
-) -> float | pd.Series:
+    operating_income, interest_expense
+) :
     """
     Compute the Interest Coverage Ratio, a metric that reveals a company's
     ability to cover its interest expenses with its pre-tax profits.
     This ratio measures how many times the operating income covers the
     interest payments of operain required and is crucial in determining a
     company's financial health.
 
     Args:
         operating_income (float or pd.Series): Operating income of the company.
-        interest_expense (float or pd.Series): Interest expense of the company.
+        interest_expense (float or pd.Series)erest expense of the company.
 
     Returns:
-        float | pd.Series: The Interest Coverage Ratio
+        float : The Interest Coverage Ratio
     """
     return operating_income / interest_expense
 
 
 def get_interest_burden_ratio(
-    income_before_tax: float | pd.Series, operating_income: float | pd.Series
-) -> float | pd.Series:
+    income_before_tax, operating_income
+) :
     """
     Compute the Interest Burden Ratio, a metric that reveals a company's
     ability to cover its interest expenses with its pre-tax profits.
     This ratio measures how many times the operating income covers the
     interest payments of operain required and is crucial in determining a
     company's financial health.
 
     Args:
         income_before_tax (float or pd.Series): Income before tax of the company.
         operating_income (float or pd.Series): Operating income of the company.
 
     Returns:
-        float | pd.Series: The Interest Burden Ratio
+        float : The Interest Burden Ratio
     """
     return income_before_tax / operating_income
 
 
 def get_income_before_tax_profit_margin(
-    income_before_tax: float | pd.Series, revenue: float | pd.Series
-) -> float | pd.Series:
+    income_before_tax, revenue
+) :
     """
     Calculate the Pretax Profit Margin, which is the ratio of a company's pre-tax profit to its revenue,
     indicating how much profit a company makes before paying taxes on its earnings.
 
     Args:
         income_before_tax (float or pd.Series): Income before tax of the company.
         revenue (float or pd.Series): Revenue of the company.
 
     Returns:
-        float | pd.Series: The Pretax Profit Margin value.
+        float : The Pretax Profit Margin value.
     """
     return income_before_tax / revenue
 
 
 def get_effective_tax_rate(
-    income_tax_expense: float | pd.Series, income_before_tax: float | pd.Series
-) -> float | pd.Series:
+    income_tax_expense, income_before_tax
+) :
     """
     Calculate the effective tax rate, a financial ratio that measures the percentage of pretax income
     that is paid as taxes.
 
     Args:
         income_tax_expense (float or pd.Series): The amount of income tax paid by the company.
         income_before_tax (float or pd.Series): The company's income before taxes.
 
     Returns:
-        float | pd.Series: The effective tax rate value.
+        float : The effective tax rate value.
     """
     return income_tax_expense / income_before_tax
 
 
 def get_return_on_assets(
-    net_income: float | pd.Series, total_assets: float | pd.Series
-) -> float | pd.Series:
+    net_income, total_assets
+) :
     """
     Calculate the return on assets (ROA), a profitability ratio that measures how
     efficiently a company uses its assets to generate profits.
 
     Args:
         net_income (float or pd.Series): Net income of the company.
         total_assets (float or pd.Series): Total assets of the company.
 
     Returns:
-        float | pd.Series: The ROA percentage value.
+        float : The ROA percentage value.
     """
     return net_income / total_assets
 
 
 def get_return_on_equity(
-    net_income: float | pd.Series,
-    total_equity_begin: float | pd.Series,
-    total_equity_end: float | pd.Series,
-) -> float | pd.Series:
+    net_income,
+    total_equity_begin,
+    total_equity_end,
+) :
     """
     Calculate the return on equity (ROE), a profitability ratio that measures how
     efficiently a company generates profits using its shareholders' equity.
 
     Args:
         net_income (float or pd.Series): Net income of the company.
         total_equity_begin (float or pd.Series): Total equity at the beginning of the period.
         total_equity_end (float or pd.Series): Total equity at the end of the period.
 
     Returns:
-        float | pd.Series: The ROE percentage value.
+        float : The ROE percentage value.
     """
     return net_income / ((total_equity_begin + total_equity_end) / 2)
 
 
 def get_return_on_invested_capital(
-    net_income: float | pd.Series,
-    dividends: float | pd.Series,
-    effective_tax_rate: float | pd.Series,
-    total_equity: float | pd.Series,
-    total_debt: float | pd.Series,
-) -> float | pd.Series:
+    net_income,
+    dividends,
+    effective_tax_rate,
+    total_equity,
+    total_debt,
+) :
     """
     Calculate the return on invested capital, a financial ratio that measures the company's return on
     the capital invested in it, including both equity and debt.
 
     Args:
         net_income (float or pd.Series): The company's net income.
         dividends (float or pd.Series): The dividends paid by the company.
         effective_tax_rate (float or pd.Series): The effective tax rate of the company.
         total_equity (float or pd.Series): The total equity of the company.
         total_debt (float or pd.Series): The total debt of the company.
 
     Returns:
-        float | pd.Series: The return on invested capital value.
+        float : The return on invested capital value.
     """
     return ((net_income - dividends) * (1 - effective_tax_rate)) / (
         total_equity + total_debt
     )
 
 
 def get_income_quality_ratio(
-    cash_flow_from_operating_activities: float | pd.Series,
-    net_income: float | pd.Series,
-) -> float | pd.Series:
+    cash_flow_from_operating_activities,
+    net_income,
+) :
     """
     Calculates the income quality ratio, which measures the cash flow from operating
     activities relative to the net income of the company.
 
     Args:
         cash_flow_from_operating_activities (float or pd.Series): Cash flow from operating activities
             of the company.
         net_income (float or pd.Series): Net income of the company.
 
     Returns:
-        float | pd.Series: The income quality ratio.
+        float : The income quality ratio.
     """
     return cash_flow_from_operating_activities / net_income
 
 
 def get_return_on_tangible_assets(
-    net_income: float | pd.Series,
-    total_assets: float | pd.Series,
-    intangible_assets: float | pd.Series,
-    total_liabilities: float | pd.Series,
-) -> float | pd.Series:
+    net_income,
+    total_assets,
+    intangible_assets,
+    total_liabilities,
+) :
     """
     Calculate the return on tangible assets, which measures the amount of profit
     generated by a company's tangible assets.
 
     Args:
         net_income (float or pd.Series): The net income of the company.
         interest_expense (float or pd.Series): The interest expense of the company.
         total_assets (float or pd.Series): The total assets of the company.
         total_liabilities (float or pd.Series): The total liabilities of the company.
 
     Returns:
-        float | pd.Series: The return on tangible assets value.
+        float : The return on tangible assets value.
     """
     tangible_assets = total_assets - intangible_assets - total_liabilities
 
     return net_income / tangible_assets
 
 
 def get_return_on_capital_employed(
-    net_income: float | pd.Series,
-    interest_expense: float | pd.Series,
-    tax_expense: float | pd.Series,
-    total_assets: float | pd.Series,
-    total_current_liabilities: float | pd.Series,
-) -> float | pd.Series:
+    net_income,
+    interest_expense,
+    tax_expense,
+    total_assets,
+    total_current_liabilities,
+) :
     """
     Calculate the return on capital employed (ROCE), a profitability ratio that measures
     the amount of return a company generates from the capital it has invested in the business.
 
     Args:
         net_income (float or pd.Series): Net income of the company.
-        interest_expense (float or pd.Series): Interest expense of the company.
+        interest_expense (float or pd.Series)erest expense of the company.
         tax_expense (float or pd.Series): Tax expense of the company.
         total_assets (float or pd.Series): Total assets of the company.
         total_current_liabilities (float or pd.Series): Total current liabilities of the company.
 
     Returns:
-        float | pd.Series: The ROCE value.
+        float : The ROCE value.
     """
     return (net_income + interest_expense + tax_expense) / (
         total_assets - total_current_liabilities
     )
 
 
 def get_net_income_per_ebt(
-    net_income: float | pd.Series, income_tax_expense: float | pd.Series
-) -> float | pd.Series:
+    net_income, income_tax_expense
+) :
     """
     Calculate the net income per earnings before taxes (EBT), a profitability ratio that
     measures the net income generated for each dollar of EBT.
 
     Args:
         net_income (float or pd.Series): Net income of the company.
         income_tax_expense (float or pd.Series): Income tax expense of the company.
 
     Returns:
-        float | pd.Series: The net income per EBT value.
+        float : The net income per EBT value.
     """
     return net_income / (net_income + income_tax_expense)
 
 
 def get_free_cash_flow_operating_cash_flow_ratio(
-    free_cash_flow: float | pd.Series, operating_cash_flow: float | pd.Series
-) -> float | pd.Series:
+    free_cash_flow, operating_cash_flow
+) :
     """
     Calculate the free cash flow to operating cash flow ratio, a profitability
     ratio that measures the amount of free cash flow a company generates
     for every dollar of operating cash flow.
 
     Args:
         free_cash_flow (float or pd.Series): Free cash flow of the company.
         operating_cash_flow (float or pd.Series): Operating cash flow of the company.
 
     Returns:
-        float | pd.Series: The free cash flow to operating cash flow ratio value.
+        float : The free cash flow to operating cash flow ratio value.
     """
     return free_cash_flow / operating_cash_flow
 
 
 def get_tax_burden_ratio(
-    net_income: float | pd.Series, income_before_tax: float | pd.Series
-) -> float | pd.Series:
+    net_income, income_before_tax
+) :
     """
     Calculate the tax burden ratio, which is the ratio of a company's
     net income to its income before tax, indicating how much of a
     company's income is retained after taxes.
 
     Args:
         net_income (float or pd.Series): Net income of the company.
         income_before_tax (float or pd.Series): Income before tax of the company.
 
     Returns:
-        float | pd.Series: The NIperEBT value.
+        float : The NIperEBT value.
     """
     return net_income / income_before_tax
 
 
 def get_EBT_to_EBIT(
-    earnings_before_tax: float | pd.Series,
-    earnings_before_interest_and_taxes: float | pd.Series,
-) -> float | pd.Series:
+    earnings_before_tax,
+    earnings_before_interest_and_taxes,
+) :
     """
     Calculate the EBT to EBIT, which is the ratio of a company's earnings before tax to its earnings before
     interest and taxes, indicating how much of a company's earnings are generated before paying interest on debt.
 
     Args:
         earnings_before_tax (float or pd.Series): Earnings before tax of the company.
         earnings_before_interest_and_taxes (float or pd.Series): Earnings before interest and taxes of the company.
 
     Returns:
-        float | pd.Series: The EBTperEBIT value.
+        float : The EBTperEBIT value.
     """
     return earnings_before_tax / earnings_before_interest_and_taxes
 
 
 def get_EBIT_to_revenue(
-    earnings_before_interest_and_taxes: float | pd.Series, revenue: float | pd.Series
-) -> float | pd.Series:
+    earnings_before_interest_and_taxes, revenue
+) :
     """
     Calculate the EBITperRevenue, which is the ratio of a company's earnings
     before interest and taxes to its revenue, indicating how much profit a
     company generates from its operations before paying interest on debt
     and taxes on its earnings.
 
     Args:
         earnings_before_interest_and_taxes (float or pd.Series): Earnings before interest and taxes of the company.
         revenue (float or pd.Series): Revenue of the company.
 
     Returns:
-        float | pd.Series: The EBITperRevenue value.
+        float : The EBITperRevenue value.
     """
     return earnings_before_interest_and_taxes / revenue
```

### Comparing `financetoolkit-1.0.0/financetoolkit/ratios/valuation.py` & `financetoolkit-1.0.1/financetoolkit/ratios/valuation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 """Valuation Module"""
 __docformat__ = "numpy"
 
 import pandas as pd
 
 
 def get_earnings_per_share(
-    net_income: float | pd.Series,
-    preferred_dividends: float | pd.Series,
-    average_outstanding_shares: float | pd.Series,
-) -> float | pd.Series:
+    net_income,
+    preferred_dividends,
+    average_outstanding_shares,
+) :
     """
     Calculate the earnings per share (EPS), a valuation ratio that measures the
     amount of net income earned per share of outstanding common stock.
 
     Args:
         net_income (float or pd.Series): Net income of the company.
         preferred_dividends (float or pd.Series): Preferred dividends of the company.
         average_outstanding_shares (float or pd.Series): Average outstanding shares of the company.
 
     Returns:
-        float | pd.Series: The EPS value.
+        float : The EPS value.
     """
     return (net_income - preferred_dividends) / average_outstanding_shares
 
 
 def get_revenue_per_share(
-    total_revenue: float | pd.Series, shares_outstanding: float | pd.Series
-) -> float | pd.Series:
+    total_revenue, shares_outstanding
+) :
     """
     Calculate the revenue per share, a valuation ratio that measures the amount of
     revenue generated per outstanding share of a company's stock.
 
     Args:
         total_revenue (float or pd.Series): Total revenue of the company.
         shares_outstanding (float or pd.Series): Total number of outstanding shares of the company.
 
     Returns:
-        float | pd.Series: The revenue per share value.
+        float : The revenue per share value.
     """
     return total_revenue / shares_outstanding
 
 
 def get_price_earnings_ratio(
-    stock_price: float | pd.Series, earnings_per_share: float | pd.Series
-) -> float | pd.Series:
+    stock_price, earnings_per_share
+) :
     """
     Calculate the price earnings ratio (P/E), a valuation ratio that compares a company's
     stock price to its earnings per share.
 
     Args:
         stock_price (float or pd.Series): Stock price of the company.
         earnings_per_share (float or pd.Series): Earnings per share of the company.
 
     Returns:
-        float | pd.Series: The P/E ratio value.
+        float : The P/E ratio value.
     """
     return stock_price / earnings_per_share
 
 
 def get_earnings_per_share_growth(
-    earnings_per_share: pd.Series | pd.DataFrame,
-) -> pd.Series | pd.DataFrame:
+    earnings_per_share,
+):
     """
     Calculate the earnings per share growth.
 
     Args:
         net_income (pd.Series): The net income of the company.
 
     Returns:
@@ -75,184 +75,184 @@
     if isinstance(earnings_per_share, pd.DataFrame):
         return earnings_per_share.pct_change(axis="columns")
 
     raise TypeError("earnings_per_share must be a pd.Series or pd.DataFrame object.")
 
 
 def get_price_to_earnings_growth_ratio(
-    price_earnings: float | pd.Series, earnings_per_share_growth: float | pd.Series
-) -> float | pd.Series:
+    price_earnings, earnings_per_share_growth
+) :
     """
     Calculate the price earnings to growth (PEG) ratio, a valuation metric that measures the ratio
     of the price-to-earnings ratio to earnings growth rate.
 
     Args:
         price_earnings (float or pd.Series): The company's price-to-earnings ratio.
         earnings_growth (float or pd.Series): The earnings per share growth rate of the company.
 
     Returns:
-        float | pd.Series: The PEG ratio value.
+        float : The PEG ratio value.
     """
     return price_earnings / earnings_per_share_growth
 
 
 def get_book_value_per_share(
-    total_shareholder_equity: float | pd.Series,
-    preferred_equity: float | pd.Series,
-    common_shares_outstanding: float | pd.Series,
-) -> float | pd.Series:
+    total_shareholder_equity,
+    preferred_equity,
+    common_shares_outstanding,
+) :
     """
     Calculate the book value per share, a valuation ratio that measures the amount of
     common equity value per share outstanding.
 
     Args:
         total_shareholder_equity (float or pd.Series): Total equity of the company.
         preferred_equity (float or pd.Series): Preferred equity of the company.
         common_shares_outstanding (float or pd.Series): Common shares outstanding of the company.
 
     Returns:
-        float | pd.Series: The book value per share value.
+        float : The book value per share value.
     """
     return (total_shareholder_equity - preferred_equity) / common_shares_outstanding
 
 
 def get_price_to_book_ratio(
-    price_per_share: float | pd.Series, book_value_per_share: float | pd.Series
-) -> float | pd.Series:
+    price_per_share, book_value_per_share
+) :
     """
     Calculate the price to book ratio, a valuation ratio that compares a company's market
     price to its book value per share.
 
     Args:
         price_per_share (float or pd.Series): Price per share of the company.
         book_value_per_share (float or pd.Series): Book value per share of the company.
 
     Returns:
-        float | pd.Series: The price to book ratio value.
+        float : The price to book ratio value.
     """
     return price_per_share / book_value_per_share
 
 
 def get_interest_debt_per_share(
-    interest_expense: float | pd.Series,
-    total_debt: float | pd.Series,
-    shares_outstanding: float | pd.Series,
-) -> float | pd.Series:
+    interest_expense,
+    total_debt,
+    shares_outstanding,
+) :
     """
     Calculate the interest debt per share, a valuation ratio that measures the
     amount of interest expense incurred per outstanding share of a company's stock.
 
     Args:
-        interest_expense (float or pd.Series): Interest expense of the company.
+        interest_expense (float or pd.Series)erest expense of the company.
         total_debt (float or pd.Series): Total debt of the company.
         shares_outstanding (float or pd.Series): Total number of outstanding shares of the company.
 
     Returns:
-        float | pd.Series: The interest debt per share value.
+        float : The interest debt per share value.
     """
     return (interest_expense / total_debt) * shares_outstanding
 
 
 def get_capex_per_share(
-    capital_expenditures: float | pd.Series, shares_outstanding: float | pd.Series
-) -> float | pd.Series:
+    capital_expenditures, shares_outstanding
+) :
     """
     Calculate the capex per share, a valuation ratio that measures the amount of
     capital expenditures made per outstanding share of a company's stock.
 
     Args:
         capital_expenditures (float or pd.Series): Total capital expenditures made by the company.
         shares_outstanding (float or pd.Series): Total number of outstanding shares of the company.
 
     Returns:
-        float | pd.Series: The capex per share value.
+        float : The capex per share value.
     """
     return capital_expenditures / shares_outstanding
 
 
 def get_dividend_yield(
-    dividends_paid: float | pd.Series,
-    shares_outstanding: float | pd.Series,
-    stock_price: float | pd.Series,
-) -> float | pd.Series:
+    dividends_paid,
+    shares_outstanding,
+    stock_price,
+) :
     """
     Calculate the dividend yield ratio, a valuation ratio that measures the amount of
     dividends distributed per share of stock relative to the stock's price.
 
     Args:
         dividends_paid (float or pd.Series): Dividend per share of the company.
         shares_outstanding (float or pd.Series): Total number of outstanding shares of the company.
         stock_price (float or pd.Series): Stock price of the company.
 
     Returns:
-        float | pd.Series: The dividend yield percentage value.
+        float : The dividend yield percentage value.
     """
     return (dividends_paid / shares_outstanding) / stock_price
 
 
 def get_price_to_cash_flow_ratio(
-    market_cap: float | pd.Series, operations_cash_flow: float | pd.Series
-) -> float | pd.Series:
+    market_cap, operations_cash_flow
+) :
     """
     Calculate the price to cash flow ratio, a valuation ratio that compares a company's market
     price to its cash flow per share.
 
     Args:
         market_cap (float or pd.Series): Market capitalization of the company.
         operations_cash_flow (float or pd.Series): Operations cash flow of the company.
 
     Returns:
-        float | pd.Series: The price to cash flow ratio value.
+        float : The price to cash flow ratio value.
     """
     return market_cap / operations_cash_flow
 
 
 def get_price_to_free_cash_flow_ratio(
-    market_cap: float | pd.Series, free_cash_flow: float | pd.Series
-) -> float | pd.Series:
+    market_cap, free_cash_flow
+) :
     """
     Calculate the price to free cash flow ratio, a valuation ratio that compares a company's market
     price to its free cash flow per share.
 
     Args:
         market_cap (float or pd.Series): Market capitalization of the company.
         free_cash_flow (float or pd.Series): Free cash flow of the company
 
     Returns:
-        float | pd.Series: The price to free cash flow ratio value.
+        float : The price to free cash flow ratio value.
     """
     return market_cap / free_cash_flow
 
 
 def get_market_cap(
-    share_price: float | pd.Series,
-    total_shares_outstanding: float | pd.Series,
-) -> float | pd.Series:
+    share_price,
+    total_shares_outstanding,
+) :
     """
     Calculates the market capitalization of the company.
 
     Note: All the inputs must be in the same currency and unit for accurate calculations.
 
     Args:
-        share_price (float | pd.Series): The share price of the company.
-        total_shares_outstanding (float | pd.Series): The total number of shares outstanding of the company.
+        share_price (float ): The share price of the company.
+        total_shares_outstanding (float ): The total number of shares outstanding of the company.
 
     Returns:
-        float | pd.Series: The market capitalization of the company.
+        float : The market capitalization of the company.
     """
     return share_price * total_shares_outstanding
 
 
 def get_enterprise_value(
-    market_cap: float | pd.Series,
-    total_debt: float | pd.Series,
-    minority_interest: float | pd.Series,
-    preferred_equity: float | pd.Series,
-    cash_and_cash_equivalents: float | pd.Series,
-) -> float | pd.Series:
+    market_cap,
+    total_debt,
+    minority_interest,
+    preferred_equity,
+    cash_and_cash_equivalents,
+) :
     """
     Calculates the Enterprise Value (EV) of a company. The Enterprise Value (EV)
     is a measure of a company's total value, often used as a more comprehensive
     alternative to market capitalization. It is calculated as the sum of a company's
     market capitalization, outstanding debt, minority interest, and
     preferred equity, minus the cash and cash equivalents.
 
@@ -262,164 +262,164 @@
         market_cap (float or pd.Series): The market capitalization of the company.
         total_debt (float or pd.Series): The total debt of the company.
         minority_interest (float or pd.Series): The value of minority interest in the company.
         preferred_equity (float or pd.Series): The value of the preferred equity in the company.
         cash_and_cash_equivalents (float or pd.Series): The value of cash and cash equivalents of the company.
 
     Returns:
-        float | pd.Series: The Enterprise Value (EV) of the company.
+        float : The Enterprise Value (EV) of the company.
     """
     return (
         market_cap
         + total_debt
         + minority_interest
         + preferred_equity
         - cash_and_cash_equivalents
     )
 
 
 def get_ev_to_sales_ratio(
-    enterprise_value: float | pd.Series, total_revenue: float | pd.Series
-) -> float | pd.Series:
+    enterprise_value, total_revenue
+) :
     """
     Calculate the EV to sales ratio, a valuation ratio that compares a company's enterprise value
     (EV) to its total revenue.
 
     Args:
         enterprise_value (float or pd.Series): Enterprise value of the company.
         total_revenue (float or pd.Series): Total revenue of the company.
 
     Returns:
-        float | pd.Series: The EV to sales ratio value.
+        float : The EV to sales ratio value.
     """
     return enterprise_value / total_revenue
 
 
 def get_ev_to_ebitda_ratio(
-    enterprise_value: float | pd.Series,
-    operating_income: float | pd.Series,
-    depreciation_and_amortization: float | pd.Series,
-) -> float | pd.Series:
+    enterprise_value,
+    operating_income,
+    depreciation_and_amortization,
+) :
     """
     Calculates the enterprise value over EBITDA ratio, which is a valuation ratio
     that measures a company's total value (including debt and equity) relative to its
     EBITDA.
 
     Args:
         enterprise_value (float or pd.Series): The total value of a company (market capitalization
             plus debt minus cash and cash equivalents).
         operating_income (float or pd.Series): The operating income of the company.
         depreciation_and_amortization (float or pd.Series): The depreciation and amortization of the company.
 
     Returns:
-        float | pd.Series: The enterprise value over EBITDA ratio.
+        float : The enterprise value over EBITDA ratio.
     """
     return enterprise_value / (operating_income + depreciation_and_amortization)
 
 
 def get_ev_to_operating_cashflow_ratio(
-    enterprise_value: float | pd.Series, operating_cashflow: float | pd.Series
-) -> float | pd.Series:
+    enterprise_value, operating_cashflow
+) :
     """
     Calculates the enterprise value over operating cash flow ratio, which is a valuation ratio
     that measures a company's total value (including debt and equity) relative to its
     operating cash flow.
 
     Args:
         enterprise_value (float or pd.Series): The total value of a company (market capitalization
             plus debt minus cash and cash equivalents).
         operating_cashflow (float or pd.Series): The cash generated by the company's operations.
 
     Returns:
-        float | pd.Series: The enterprise value over operating cash flow ratio.
+        float : The enterprise value over operating cash flow ratio.
     """
     return enterprise_value / operating_cashflow
 
 
 def get_earnings_yield(
-    earnings_per_share: float | pd.Series, market_price_per_share: float | pd.Series
-) -> float | pd.Series:
+    earnings_per_share, market_price_per_share
+) :
     """
     Calculates the earnings yield ratio, which measures the earnings per share relative
     to the market price per share.
 
     Args:
         earnings_per_share (float or pd.Series): Earnings per share of the company.
         market_price_per_share (float or pd.Series): Market price per share of the company.
 
     Returns:
-        float | pd.Series: The earnings yield ratio.
+        float : The earnings yield ratio.
     """
     return earnings_per_share / market_price_per_share
 
 
 def get_payout_ratio(
-    dividends: float | pd.Series, net_income: float | pd.Series
-) -> float | pd.Series:
+    dividends, net_income
+) :
     """
     Calculates the payout ratio, which measures the proportion of net income paid out as
     dividends to shareholders.
 
     Args:
         dividends (float or pd.Series): Dividends paid by the company.
         net_income (float or pd.Series): Net income of the company.
 
     Returns:
-        float | pd.Series: The payout ratio.
+        float : The payout ratio.
     """
     return abs(dividends) / net_income
 
 
 def get_tangible_asset_value(
-    total_assets: float | pd.Series,
-    total_liabilities: float | pd.Series,
-    goodwill: float | pd.Series,
-) -> float | pd.Series:
+    total_assets,
+    total_liabilities,
+    goodwill,
+) :
     """
     Calculate the tangible asset value, which represents the total value of a company's assets
     that can be used to generate revenue.
 
     Args:
         total_assets (float or pd.Series): The total assets of the company.
         total_liabilities (float or pd.Series): The total liabilities of the company.
         goodwill (float or pd.Series): The goodwill of the company.
 
     Returns:
-        float | pd.Series: The tangible asset value.
+        float : The tangible asset value.
     """
     return total_assets - total_liabilities - goodwill
 
 
 def get_net_current_asset_value(
-    total_current_assets: float | pd.Series,
-    total_current_liabilities: float | pd.Series,
-) -> float | pd.Series:
+    total_current_assets,
+    total_current_liabilities,
+) :
     """
     Calculate the net current asset value, which is the total value of a company's current assets
     minus its current liabilities.
 
     Args:
         total_current_assets (float or pd.Series): The current assets of the company.
         total_current_liabilities (float or pd.Series): The current liabilities of the company.
 
     Returns:
-        float | pd.Series: The net current asset value.
+        float : The net current asset value.
     """
     return total_current_assets - total_current_liabilities
 
 
 def get_ev_to_ebit(
-    enterprise_value: float | pd.Series,
-    earnings_before_interest_and_taxes: float | pd.Series,
-) -> float | pd.Series:
+    enterprise_value,
+    earnings_before_interest_and_taxes,
+) :
     """
     Calculate the enterprise value multiplier, a financial ratio that measures the total value of a
     company's operations (including debt and equity) relative to its earnings before interest and taxes.
 
     Args:
         enterprise_value (float or pd.Series): The total value of a company's operations.
         earnings_before_interest_and_taxes (float or pd.Series): The company's earnings before interest and taxes.
 
     Returns:
-        float | pd.Series: The enterprise value multiplier value.
+        float : The enterprise value multiplier value.
     """
     return enterprise_value / earnings_before_interest_and_taxes
```

### Comparing `financetoolkit-1.0.0/pyproject.toml` & `financetoolkit-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "financetoolkit"
-version = "1.0.0"
+version = "1.0.1"
 description = "Transparent and Efficient Financial Analysis"
 license = "MIT"
 authors = ["Jeroen Bouma"]
 packages = [
     { include = "financetoolkit" },
 ]
 include = ['normalization/*.csv']
 readme = "README.md"
+homepage = "https://www.jeroenbouma.com/"
 repository = "https://github.com/JerBouma/FinanceToolkit"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Financial and Insurance Industry",
     "Topic :: Office/Business :: Financial :: Investment",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -40,27 +41,27 @@
 line-length = 122
 select = ["E", "W", "F", "Q", "W", "S", "UP", "I", "PD", "SIM", "PLC", "PLE", "PLR", "PLW"]
 ignore = ["S105", "S106", "S107", "PLR0913", "PLR0912", "PLR0911"]
 exclude = ["conftest.py"]
 
 [tool.pylint]
 max-line-length = 122
-disable = ["R0913", "W1514", "R0911", "R0912", "R0915", "R0801", "W0221", "C0103"]
+disable = ["R0913", "W1514", "R0911", "R0912", "R0915", "R0801", "W0221", "C0103", "E1131"]
 
 [tool.ruff.isort]
 combine-as-imports = true
 force-wrap-aliases = true
 
 [tool.isort]
 profile = "black"
 line_length = 122
 skip_gitignore = true
 combine_as_imports = true
 
 [tool.codespell]
-ignore-words-list = 'zar,profund,basf,applicatio,ser,mone,vie,wew,ist,tre,ue'
+ignore-words-list = 'zar,profund,basf,applicatio,ser,mone,vie,wew,ist,tre,ue,nd,fo'
 skip = '*.json,./.git,pyproject.toml'
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::pytest.PytestAssertRewriteWarning:",
 ]
```

### Comparing `financetoolkit-1.0.0/PKG-INFO` & `financetoolkit-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: financetoolkit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Transparent and Efficient Financial Analysis
-Home-page: https://github.com/JerBouma/FinanceToolkit
+Home-page: https://www.jeroenbouma.com/
 License: MIT
 Author: Jeroen Bouma
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
@@ -23,40 +23,40 @@
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Project-URL: Repository, https://github.com/JerBouma/FinanceToolkit
 Description-Content-Type: text/markdown
 
 ![FinanceToolkitCropped](https://github.com/JerBouma/FinanceToolkit/assets/46355364/198d47bd-e1b3-492d-acc4-5d9f02d1d009)
 
 [![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-Donate-brightgreen?logo=buymeacoffee)](https://www.buymeacoffee.com/jerbouma)
-[![Issues](https://img.shields.io/github/issues/jerbouma/FinanceToolkit)](https://github.com/JerBouma/FinanceToolkit/issues)
-[![Pull Requests](https://img.shields.io/github/issues-pr/JerBouma/FinanceToolkit?color=yellow)](https://github.com/JerBouma/FinanceToolkit/pulls)
+[![Website](https://img.shields.io/badge/Website-Learn%20more%20about%20me%20here-brightgreen?logo=ReadMe)](https://jeroenbouma.com/)
 [![PYPI Version](https://img.shields.io/pypi/v/FinanceToolkit)](https://pypi.org/project/FinanceToolkit/)
 [![PYPI Downloads](https://img.shields.io/pypi/dm/FinanceToolkit)](https://pypi.org/project/FinanceToolkit/)
 
+**NOTE: THIS VERSION HAS ALL TYPING REMOVED AND THUS SUPPORTS PYTHON VERSIONS LESS THAN PYTHON 3.10. THIS IS MERELY MEANT TO SUPPORT THOSE WHO HAVEN"T UPDATED YET AND WON"T BE MAINTAINED FURTHER. PLEASE VISIT THE LATEST BUILD AND UPDATE PYTHON ACCORDINGLY**
+
 While browsing a variety of websites, I kept finding that the same financial metric can greatly vary per source and so do the financial statements reported while little information is given how the metric was calculated.
 
 For example, Microsoft's Price-to-Earnings (PE) ratio on the 6th of May, 2023 is reported to be 28.93 (Stockopedia), 32.05 (Morningstar), 32.66 (Macrotrends), 33.09 (Finance Charts), 33.66 (Y Charts), 33.67 (Wall Street Journal), 33.80 (Yahoo Finance) and 34.4 (Companies Market Cap). All of these calculations are correct, however the method applied varies leading to different results. Therefore, collecting data from multiple sources can lead to wrong interpretation of the results given that one source could be applying a different calculation method than another. And that is, if it is even freely available. Often the calculation is hidden behind a paid subscription.
 
 **This is why I designed the FinanceToolkit**, this is an open-source toolkit in which all relevant financial ratios (50+), indicators and performance measurements are written down in the most simplistic way allowing for complete transparency of the calculation method. This allows you to not have to rely on metrics from other providers and, given a financial statement, allow for efficient manual calculations. This leads to one uniform method of calculation being applied that is available and understood by everyone.
 
 The Finance Toolkit is complimented very well with the [Finance Database 🌎](https://github.com/JerBouma/FinanceDatabase), a database that features 300.000+ symbols containing Equities, ETFs, Funds, Indices, Currencies, Cryptocurrencies and Money Markets. By utilising both, it is possible to do a fully-fledged competitive analysis with the tickers found from the FinanceDatabase inputted into the FinanceToolkit.
 
-**Disclaimer:** this package used to be called 'FundamentalAnalysis' but has since been renamed. This is a major update to the existent package which also justified a rename. The old package does remain available.
-
+ <img src="https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%205.%20Video%20Demo.gif?raw=true" alt="Finance Toolkit Illustration" width="100%"/>
+ 
 ---
 
 # Table of Contents
 
 1. [Installation](#installation)
 2. [Basic Usage](#basic-usage)
     1. [Using the Finance Toolkit](#using-the-finance-toolkit)
     2. [Working with other Datasets](#working-with-other-datasets)
     3. [Calling Functions Directly](#calling-functions-directly)
-4. [Questions & Answers](#questions--answers)
-6. [Contact](#contact)
+3. [Contact](#contact)
 
 # Installation
 
 To install the FinanceToolkit it simply requires the following:
 
 ```
 pip install financetoolkit
@@ -98,15 +98,15 @@
 - Historical market data (`historical_data`), which can be retrieved on a daily, weekly, monthly and yearly basis (from Yahoo Finance)
 - Balance Sheet Statements (`balance_sheet_statement`), Income Statements (`income_statement`) and Cash Flow Statements (`cash_flow_statement`), obtainable from FinancialModelingPrep or the source of your choosing through custom input. These functions are accompanied with a normalization function so that for any source, the same ratio analysis can be performed. Please see this Jupyter Notebook that explains how to use a custom source.
 - Efficiency ratios (`efficiency_ratios`), liquidity ratios (`liquidity_ratios`), profitability ratios (`profitability_ratios`), solvency ratios (`solvency_ratios`) and valuation ratios (`valuation_ratios`) functionality that automatically calculates the most important ratios based on the inputted balance sheet, income and cash flow statements.
 - Models (`models`) like DUPONT analysis that can be used to perform in-depth financial analysis through a single function.
 
 ## Using the Finance Toolkit
 
-A basic example of how to initialise the Finance Toolkit is shown below, also see [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%201.%20Getting%20Started.ipynb) for a detailed Getting Started guide as well as [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%202.%20Combining%20the%Finance%20Toolkit%20with%20the%20Finance%20Database.ipynb) that includes the [Finance Database 🌎](https://github.com/JerBouma/FinanceDatabase) and a proper financial analysis.
+A basic example of how to initialise the Finance Toolkit is shown below, also see [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%201.%20Getting%20Started.ipynb) for a detailed Getting Started guide as well as [this notebook](https://github.com/JerBouma/FinanceToolkit/blob/main/examples/Finance%20Toolkit%20-%202.%20Combining%20the%20Finance%20Toolkit%20with%20the%20Finance%20Database.ipynb) that includes the [Finance Database 🌎](https://github.com/JerBouma/FinanceDatabase) and a proper financial analysis.
 
 ````python
 from financetoolkit import Toolkit
 
 companies = Toolkit(['AAPL', 'MSFT'], api_key="FMP_KEY")
 
 # an Enterprise example
@@ -118,15 +118,15 @@
 # a Financial Statement example
 balance_sheet_statement = companies.get_balance_sheet_statement()
 
 # a Ratios example
 profitability_ratios = companies.ratios.collect_profitability_ratios()
 
 # Show the profitability ratios for Apple
-profitability_ratios.loc['AAPL]
+profitability_ratios.loc['AAPL']
 ````
 
 This returns the following output for `profitability_ratios.loc['AAPL]`. Omitting `.loc['AAPL']` will return the result for both AAPL and MSFT.
 
 
 |                                             |     2018 |     2019 |     2020 |     2021 |     2022 |
 |:--------------------------------------------|---------:|---------:|---------:|---------:|---------:|
```

