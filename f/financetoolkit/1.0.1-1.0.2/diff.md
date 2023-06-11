# Comparing `tmp/financetoolkit-1.0.1.tar.gz` & `tmp/financetoolkit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financetoolkit-1.0.1.tar", max compression
+gzip compressed data, was "financetoolkit-1.0.2.tar", max compression
```

## Comparing `financetoolkit-1.0.1.tar` & `financetoolkit-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1069 2023-05-11 17:19:30.665832 financetoolkit-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0    15188 2023-06-11 09:18:37.060648 financetoolkit-1.0.1/README.md
--rw-r--r--   0        0        0      126 2023-05-31 11:54:14.444472 financetoolkit-1.0.1/financetoolkit/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 11:11:47.294669 financetoolkit-1.0.1/financetoolkit/base/__init__.py
--rw-r--r--   0        0        0     2018 2023-06-11 09:17:50.971134 financetoolkit-1.0.1/financetoolkit/base/helpers.py
--rw-r--r--   0        0        0        0 2023-05-15 11:11:47.296959 financetoolkit-1.0.1/financetoolkit/base/models/__init__.py
--rw-r--r--   0        0        0    10651 2023-06-11 09:17:50.971389 financetoolkit-1.0.1/financetoolkit/base/models/fundamentals_model.py
--rw-r--r--   0        0        0     4047 2023-06-11 09:17:50.971609 financetoolkit-1.0.1/financetoolkit/base/models/historical_model.py
--rw-r--r--   0        0        0     4267 2023-05-31 11:54:23.375640 financetoolkit-1.0.1/financetoolkit/base/models/normalization/README.md
--rw-r--r--   0        0        0     1813 2023-05-17 13:55:45.906209 financetoolkit-1.0.1/financetoolkit/base/models/normalization/balance.csv
--rw-r--r--   0        0        0     1364 2023-05-22 14:14:21.474129 financetoolkit-1.0.1/financetoolkit/base/models/normalization/cash.csv
--rw-r--r--   0        0        0     1119 2023-05-17 13:55:45.906558 financetoolkit-1.0.1/financetoolkit/base/models/normalization/income.csv
--rw-r--r--   0        0        0     4071 2023-06-11 09:17:50.971830 financetoolkit-1.0.1/financetoolkit/base/models/normalization_model.py
--rw-r--r--   0        0        0     2657 2023-06-11 09:17:50.972035 financetoolkit-1.0.1/financetoolkit/base/models_controller.py
--rw-r--r--   0        0        0    53732 2023-06-11 09:17:50.972402 financetoolkit-1.0.1/financetoolkit/base/ratios_controller.py
--rw-r--r--   0        0        0    17521 2023-06-11 09:17:50.972687 financetoolkit-1.0.1/financetoolkit/base/toolkit_controller.py
--rw-r--r--   0        0        0        0 2023-05-15 11:11:47.299347 financetoolkit-1.0.1/financetoolkit/historical/__init__.py
--rw-r--r--   0        0        0     2635 2023-06-11 09:17:50.972933 financetoolkit-1.0.1/financetoolkit/historical/price.py
--rw-r--r--   0        0        0        0 2023-05-11 14:54:28.954198 financetoolkit-1.0.1/financetoolkit/models/__init__.py
--rw-r--r--   0        0        0     5133 2023-06-11 09:17:50.973201 financetoolkit-1.0.1/financetoolkit/models/dupont.py
--rw-r--r--   0        0        0        0 2023-05-25 15:20:11.154442 financetoolkit-1.0.1/financetoolkit/portfolio/__init__.py
--rw-r--r--   0        0        0     5632 2023-06-11 09:17:50.973438 financetoolkit-1.0.1/financetoolkit/portfolio/portfolio.py
--rw-r--r--   0        0        0        0 2023-05-11 14:28:40.501711 financetoolkit-1.0.1/financetoolkit/ratios/__init__.py
--rw-r--r--   0        0        0     8587 2023-06-11 09:17:50.973751 financetoolkit-1.0.1/financetoolkit/ratios/efficiency.py
--rw-r--r--   0        0        0     4658 2023-06-11 09:17:50.973973 financetoolkit-1.0.1/financetoolkit/ratios/liquidity.py
--rw-r--r--   0        0        0    11177 2023-06-11 09:17:50.974232 financetoolkit-1.0.1/financetoolkit/ratios/profitability.py
--rw-r--r--   0        0        0     6293 2023-06-11 09:17:50.974455 financetoolkit-1.0.1/financetoolkit/ratios/solvency.py
--rw-r--r--   0        0        0    13584 2023-06-11 09:17:50.974710 financetoolkit-1.0.1/financetoolkit/ratios/valuation.py
--rw-r--r--   0        0        0     1826 2023-06-11 09:17:50.974928 financetoolkit-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    16316 1970-01-01 00:00:00.000000 financetoolkit-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 17:19:30.665832 financetoolkit-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0    15189 2023-06-11 09:30:13.783101 financetoolkit-1.0.2/README.md
+-rw-r--r--   0        0        0      126 2023-05-31 11:54:14.444472 financetoolkit-1.0.2/financetoolkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:11:47.294669 financetoolkit-1.0.2/financetoolkit/base/__init__.py
+-rw-r--r--   0        0        0     2018 2023-06-11 09:28:16.773832 financetoolkit-1.0.2/financetoolkit/base/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:11:47.296959 financetoolkit-1.0.2/financetoolkit/base/models/__init__.py
+-rw-r--r--   0        0        0    10608 2023-06-11 09:29:06.929029 financetoolkit-1.0.2/financetoolkit/base/models/fundamentals_model.py
+-rw-r--r--   0        0        0     4015 2023-06-11 09:29:06.926373 financetoolkit-1.0.2/financetoolkit/base/models/historical_model.py
+-rw-r--r--   0        0        0     4267 2023-05-31 11:54:23.375640 financetoolkit-1.0.2/financetoolkit/base/models/normalization/README.md
+-rw-r--r--   0        0        0     1813 2023-05-17 13:55:45.906209 financetoolkit-1.0.2/financetoolkit/base/models/normalization/balance.csv
+-rw-r--r--   0        0        0     1364 2023-05-22 14:14:21.474129 financetoolkit-1.0.2/financetoolkit/base/models/normalization/cash.csv
+-rw-r--r--   0        0        0     1119 2023-05-17 13:55:45.906558 financetoolkit-1.0.2/financetoolkit/base/models/normalization/income.csv
+-rw-r--r--   0        0        0     4063 2023-06-11 09:28:43.320884 financetoolkit-1.0.2/financetoolkit/base/models/normalization_model.py
+-rw-r--r--   0        0        0     2633 2023-06-11 09:29:06.925766 financetoolkit-1.0.2/financetoolkit/base/models_controller.py
+-rw-r--r--   0        0        0    53693 2023-06-11 09:29:06.937124 financetoolkit-1.0.2/financetoolkit/base/ratios_controller.py
+-rw-r--r--   0        0        0    17494 2023-06-11 09:29:44.868171 financetoolkit-1.0.2/financetoolkit/base/toolkit_controller.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:11:47.299347 financetoolkit-1.0.2/financetoolkit/historical/__init__.py
+-rw-r--r--   0        0        0     2603 2023-06-11 09:29:06.924471 financetoolkit-1.0.2/financetoolkit/historical/price.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:54:28.954198 financetoolkit-1.0.2/financetoolkit/models/__init__.py
+-rw-r--r--   0        0        0     5133 2023-06-11 09:28:16.777418 financetoolkit-1.0.2/financetoolkit/models/dupont.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:20:11.154442 financetoolkit-1.0.2/financetoolkit/portfolio/__init__.py
+-rw-r--r--   0        0        0     5597 2023-06-11 09:29:06.925477 financetoolkit-1.0.2/financetoolkit/portfolio/portfolio.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:28:40.501711 financetoolkit-1.0.2/financetoolkit/ratios/__init__.py
+-rw-r--r--   0        0        0     8531 2023-06-11 09:29:06.926754 financetoolkit-1.0.2/financetoolkit/ratios/efficiency.py
+-rw-r--r--   0        0        0     4607 2023-06-11 09:29:06.926071 financetoolkit-1.0.2/financetoolkit/ratios/liquidity.py
+-rw-r--r--   0        0        0    11067 2023-06-11 09:29:06.925787 financetoolkit-1.0.2/financetoolkit/ratios/profitability.py
+-rw-r--r--   0        0        0     6233 2023-06-11 09:29:06.925953 financetoolkit-1.0.2/financetoolkit/ratios/solvency.py
+-rw-r--r--   0        0        0    13497 2023-06-11 09:28:43.345005 financetoolkit-1.0.2/financetoolkit/ratios/valuation.py
+-rw-r--r--   0        0        0     1826 2023-06-11 09:33:58.332333 financetoolkit-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    16317 1970-01-01 00:00:00.000000 financetoolkit-1.0.2/PKG-INFO
```

### Comparing `financetoolkit-1.0.1/LICENSE.txt` & `financetoolkit-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.1/README.md` & `financetoolkit-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![FinanceToolkitCropped](https://github.com/JerBouma/FinanceToolkit/assets/46355364/198d47bd-e1b3-492d-acc4-5d9f02d1d009)
 
 [![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-Donate-brightgreen?logo=buymeacoffee)](https://www.buymeacoffee.com/jerbouma)
 [![Website](https://img.shields.io/badge/Website-Learn%20more%20about%20me%20here-brightgreen?logo=ReadMe)](https://jeroenbouma.com/)
 [![PYPI Version](https://img.shields.io/pypi/v/FinanceToolkit)](https://pypi.org/project/FinanceToolkit/)
 [![PYPI Downloads](https://img.shields.io/pypi/dm/FinanceToolkit)](https://pypi.org/project/FinanceToolkit/)
 
-**NOTE: THIS VERSION HAS ALL TYPING REMOVED AND THUS SUPPORTS PYTHON VERSIONS LESS THAN PYTHON 3.10. THIS IS MERELY MEANT TO SUPPORT THOSE WHO HAVEN"T UPDATED YET AND WON"T BE MAINTAINED FURTHER. PLEASE VISIT THE LATEST BUILD AND UPDATE PYTHON ACCORDINGLY**
+**NOTE: THIS VERSION HAS ALL TYPING REMOVED AND THUS SUPPORTS PYTHON VERSIONS LESS THAN PYTHON 3.10. THIS IS MERELY MEANT TO SUPPORT THOSE WHO HAVEN'T UPDATED YET AND WON'T BE MAINTAINED FURTHER. PLEASE VISIT THE LATEST BUILD AND UPDATE PYTHON ACCORDINGLY.**
 
 While browsing a variety of websites, I kept finding that the same financial metric can greatly vary per source and so do the financial statements reported while little information is given how the metric was calculated.
 
 For example, Microsoft's Price-to-Earnings (PE) ratio on the 6th of May, 2023 is reported to be 28.93 (Stockopedia), 32.05 (Morningstar), 32.66 (Macrotrends), 33.09 (Finance Charts), 33.66 (Y Charts), 33.67 (Wall Street Journal), 33.80 (Yahoo Finance) and 34.4 (Companies Market Cap). All of these calculations are correct, however the method applied varies leading to different results. Therefore, collecting data from multiple sources can lead to wrong interpretation of the results given that one source could be applying a different calculation method than another. And that is, if it is even freely available. Often the calculation is hidden behind a paid subscription.
 
 **This is why I designed the FinanceToolkit**, this is an open-source toolkit in which all relevant financial ratios (50+), indicators and performance measurements are written down in the most simplistic way allowing for complete transparency of the calculation method. This allows you to not have to rely on metrics from other providers and, given a financial statement, allow for efficient manual calculations. This leads to one uniform method of calculation being applied that is available and understood by everyone.
```

### Comparing `financetoolkit-1.0.1/financetoolkit/base/helpers.py` & `financetoolkit-1.0.2/financetoolkit/base/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.1/financetoolkit/base/models/fundamentals_model.py` & `financetoolkit-1.0.2/financetoolkit/base/models/fundamentals_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """Fundamentals Module"""
 __docformat__ = "numpy"
 
 
-import pandas as pd
-
-from typing import List
 
+import pandas as pd
 
 from financetoolkit.base.models.normalization_model import (
     convert_financial_statements,
 )
 
 # pylint: disable=no-member
 
 
 def get_financial_statements(
     tickers,
-    statement = "",
-    api_key = "",
+    statement="",
+    api_key="",
     quarter: bool = False,
-    limit = 100,
-    statement_format = pd.DataFrame(),
+    limit=100,
+    statement_format=pd.DataFrame(),
 ):
     """
     Retrieves financial statements (balance, income, or cash flow statements) for one or multiple companies,
     and returns a DataFrame containing the data.
 
     Args:
         tickers (List[str]): List of company tickers.
@@ -173,17 +171,15 @@
             ).T
         except Exception as error:
             raise ValueError(error) from error
 
     return quote_dataframe
 
 
-def get_enterprise(
-    tickers, api_key, quarter: bool = False, limit = 100
-):
+def get_enterprise(tickers, api_key, quarter: bool = False, limit=100):
     """
     Description
     ----
     Gives information about the enterprise value of a company which includes
     i.a. market capitalisation, Cash & Cash Equivalents, total debt and enterprise value.
     Input
     ----
@@ -243,15 +239,15 @@
 
     if len(ticker_list) == 1:
         enterprise_dataframe = enterprise_dataframe.loc[ticker_list[0]]
 
     return enterprise_dataframe
 
 
-def get_rating(tickers, api_key, limit = 100):
+def get_rating(tickers, api_key, limit=100):
     """
     Description
     ----
     Gives information about the rating of a company which includes i.a. the company
     rating and recommendation as well as ratings based on a variety of ratios.
     Input
     ----
```

### Comparing `financetoolkit-1.0.1/financetoolkit/base/models/historical_model.py` & `financetoolkit-1.0.2/financetoolkit/base/models/historical_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """Historical Module"""
 __docformat__ = "numpy"
 
 from datetime import datetime, timedelta
 
-from typing import List
-
-
 import pandas as pd
 
 
 def get_historical_data(
     tickers,
-    start = None,
-    end = None,
-    interval = "1d",
+    start=None,
+    end=None,
+    interval="1d",
 ):
     """
     Retrieves historical stock data for the given ticker(s) from Yahoo! Finance API for a specified period.
     If start and/or end date are not provided, it defaults to 10 years from the current date.
 
     Args:
         tickers (list of str): A list of one or more ticker symbols to retrieve data for.
```

### Comparing `financetoolkit-1.0.1/financetoolkit/base/models/normalization/README.md` & `financetoolkit-1.0.2/financetoolkit/base/models/normalization/README.md`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.1/financetoolkit/base/models/normalization/balance.csv` & `financetoolkit-1.0.2/financetoolkit/base/models/normalization/balance.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.1/financetoolkit/base/models/normalization/cash.csv` & `financetoolkit-1.0.2/financetoolkit/base/models/normalization/cash.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.1/financetoolkit/base/models/normalization/income.csv` & `financetoolkit-1.0.2/financetoolkit/base/models/normalization/income.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.1/financetoolkit/base/models/normalization_model.py` & `financetoolkit-1.0.2/financetoolkit/base/models/normalization_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import shutil
 from pathlib import Path
 
 import pandas as pd
 import pkg_resources
 
 
-def read_normalization_file(statement, format_location = ""):
+def read_normalization_file(statement, format_location=""):
     """
     This function copies the normalization files as found inside the environment and saves them
     to a custom location defined by the user. This is designed to make it possible to edit these files
     and supply them to the financial statement functions and within the Analyzer class.
 
     Args:
         statement (string): the type of statement you wish to read (balance, income, or cash).
@@ -33,15 +33,15 @@
         ).name
 
     return pd.read_csv(file_location, index_col=[0]).iloc[:, 0]
 
 
 def convert_financial_statements(
     financial_statements,
-    statement_format = pd.DataFrame(),
+    statement_format=pd.DataFrame(),
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
-    format_location = "",
-    save_location = Path(Path.home(), "Downloads"),
+    format_location="",
+    save_location=Path(Path.home(), "Downloads"),
 ):
     """
     This function copies the normalization files as found inside the environment and saves them
     to a custom location defined by the user. This is designed to make it possible to edit these files
     and supply them to the financial statement functions and within the Analyzer class.
 
     Args:
```

### Comparing `financetoolkit-1.0.1/financetoolkit/base/models_controller.py` & `financetoolkit-1.0.2/financetoolkit/base/models_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Models Module"""
 __docformat__ = "numpy"
 
-import pandas as pd
 
-from typing import List
+import pandas as pd
 
 from financetoolkit.base.helpers import handle_errors
 from financetoolkit.models.dupont import (
     get_dupont_analysis,
     get_extended_dupont_analysis,
 )
```

### Comparing `financetoolkit-1.0.1/financetoolkit/base/ratios_controller.py` & `financetoolkit-1.0.2/financetoolkit/base/ratios_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Ratios Module"""
 __docformat__ = "numpy"
 
-import pandas as pd
-
-from typing import List
 
+import pandas as pd
 
 from financetoolkit.base.helpers import handle_errors
 from financetoolkit.ratios import (
     efficiency,
     liquidity,
     profitability,
     solvency,
@@ -42,15 +40,15 @@
         self._efficiency_ratios = pd.DataFrame()
         self._liquidity_ratios = pd.DataFrame()
         self._profitability_ratios = pd.DataFrame()
         self._solvency_ratios = pd.DataFrame()
         self._valuation_ratios = pd.DataFrame()
 
     def collect_all_ratios(
-        self, include_dividends: bool = False, diluted: bool = True, days = 365
+        self, include_dividends: bool = False, diluted: bool = True, days=365
     ):
         """
         Calculates all Ratios based on the data provided.
         """
         if self._efficiency_ratios.empty:
             self.collect_efficiency_ratios(days=days)
         if self._liquidity_ratios.empty:
@@ -72,15 +70,15 @@
                 self._solvency_ratios,
                 self._valuation_ratios,
             ]
         )
 
         return self._all_ratios
 
-    def collect_efficiency_ratios(self, days = 365):
+    def collect_efficiency_ratios(self, days=365):
         """
         Calculates all Efficiency Ratios based on the data provided.
         """
         if self._efficiency_ratios.empty:
             efficiency_ratios: dict = {}
 
             efficiency_ratios[
@@ -350,28 +348,28 @@
         return efficiency.get_inventory_turnover_ratio(
             self._income_statement.loc[:, "Cost of Goods Sold", :],
             self._balance_sheet_statement.loc[:, "Inventory", :].shift(axis=1),
             self._balance_sheet_statement.loc[:, "Inventory", :],
         )
 
     @handle_errors
-    def get_days_of_inventory_outstanding(self, days = 365):
+    def get_days_of_inventory_outstanding(self, days=365):
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
-    def get_days_of_sales_outstanding(self, days = 365):
+    def get_days_of_sales_outstanding(self, days=365):
         """
         Calculate the days of sales outstanding, an efficiency ratio that measures
         the average number of days it takes a company to collect payment on its
         credit sales.
         """
         return efficiency.get_days_of_sales_outstanding(
             self._balance_sheet_statement.loc[:, "Accounts Receivable", :].shift(
@@ -379,15 +377,15 @@
             ),
             self._balance_sheet_statement.loc[:, "Accounts Receivable", :],
             self._income_statement.loc[:, "Revenue", :],
             days,
         )
 
     @handle_errors
-    def get_operating_cycle(self, days = 365):
+    def get_operating_cycle(self, days=365):
         """
         Calculate the operating cycle, an efficiency ratio that measures the average
         number of days it takes a company to turn its inventory into cash.
         """
         days_of_inventory = efficiency.get_days_of_inventory_outstanding(
             self._balance_sheet_statement.loc[:, "Inventory", :].shift(axis=1),
             self._balance_sheet_statement.loc[:, "Inventory", :],
@@ -414,28 +412,28 @@
         return efficiency.get_accounts_payables_turnover_ratio(
             self._income_statement.loc[:, "Cost of Goods Sold", :],
             self._balance_sheet_statement.loc[:, "Accounts Payable", :].shift(axis=1),
             self._balance_sheet_statement.loc[:, "Accounts Payable", :],
         )
 
     @handle_errors
-    def get_days_of_accounts_payable_outstanding(self, days = 365):
+    def get_days_of_accounts_payable_outstanding(self, days=365):
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
-    def get_cash_conversion_cycle(self, days = 365):
+    def get_cash_conversion_cycle(self, days=365):
         """
         Calculate the Cash Conversion Cycle, which measures the amount of time it takes for a company to convert
         its investments in inventory and accounts receivable into cash, while considering the time it takes to pay
         its accounts payable.
         """
         days_of_inventory = efficiency.get_days_of_inventory_outstanding(
             self._balance_sheet_statement.loc[:, "Inventory", :].shift(axis=1),
```

### Comparing `financetoolkit-1.0.1/financetoolkit/base/toolkit_controller.py` & `financetoolkit-1.0.2/financetoolkit/base/toolkit_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Toolkit Module"""
 __docformat__ = "numpy"
 
 
-import pandas as pd
-
 from warnings import warn
 
+import pandas as pd
+
 from financetoolkit.base.models.fundamentals_model import (
     get_enterprise as _get_enterprise,
     get_financial_statements as _get_financial_statements,
     get_profile as _get_profile,
     get_quote as _get_quote,
     get_rating as _get_rating,
 )
@@ -38,20 +38,20 @@
     calculations. This leads to one uniform method of calculation being applied that
     is available and understood by everyone.
     """
 
     def __init__(
         self,
         tickers,
-        api_key = "",
-        historical = pd.DataFrame(),
-        balance = pd.DataFrame(),
-        income = pd.DataFrame(),
-        cash = pd.DataFrame(),
-        format_location = "",
+        api_key="",
+        historical=pd.DataFrame(),
+        balance=pd.DataFrame(),
+        income=pd.DataFrame(),
+        cash=pd.DataFrame(),
+        format_location="",
         reverse_dates: bool = False,
     ):
         """
         Initializes an Toolkit object with a ticker or a list of tickers.
 
         Args:
         tickers (str or list): A string or a list of strings containing the company ticker(s).
@@ -122,15 +122,15 @@
                 cash, self._cash_flow_statement_generic, reverse_dates
             )
             if not cash.empty
             else pd.DataFrame()
         )
 
         warn(
-            "This version of the Finance Toolkit is deprecated. Finance Toolkit 1.0.2 and onwards require Python 3.10 and higher. Please update to the latest version of Python and the Finance Toolkit.",
+            "This version of the Finance Toolkit is depreciated. Finance Toolkit 1.0.3 and onwards require Python 3.10 and higher. Please update to the latest version of Python and the Finance Toolkit.",
             DeprecationWarning,
             stacklevel=2,
         )
 
     @property
     def ratios(self):
         """
@@ -251,15 +251,15 @@
             )
 
         if self._quote.empty:
             self._quote = _get_quote(self._tickers, self._api_key)
 
         return self._quote
 
-    def get_enterprise(self, quarter = False, limit = 100):
+    def get_enterprise(self, quarter=False, limit=100):
         """
         Returns a pandas dataframe containing the enterprise value information for the specified tickers.
 
         Args:
             quarter (str): The quarter for which the enterprise value is required. Defaults to False.
             limit (str): The number of results to return. Defaults to 100.
 
@@ -277,15 +277,15 @@
         if self._enterprise.empty:
             self._enterprise = _get_enterprise(
                 self._tickers, self._api_key, quarter, limit
             )
 
         return self._enterprise
 
-    def get_rating(self, limit = 100):
+    def get_rating(self, limit=100):
         """
         Returns a pandas dataframe containing the stock rating information for the specified tickers.
 
         Args:
             limit (int): The number of results to return. Defaults to 100.
 
         Raises:
@@ -300,15 +300,15 @@
             )
 
         if self._rating.empty:
             self._rating = _get_rating(self._tickers, self._api_key, limit)
 
         return self._rating
 
-    def get_historical_data(self, start=None, end=None, period = "daily"):
+    def get_historical_data(self, start=None, end=None, period="daily"):
         """
         Returns a pandas dataframe containing the historical data for the specified tickers.
 
         Args:
             start (str): The start date for the historical data. Defaults to None.
             end (str): The end date for the historical data. Defaults to None.
             period (str): The interval at which the historical data should be
@@ -376,15 +376,15 @@
         raise ValueError(
             "Please choose from daily, weekly, monthly or yearly as period."
         )
 
     def get_balance_sheet_statement(
         self,
         quarter=False,
-        limit = 100,
+        limit=100,
         overwrite: bool = False,
     ):
         """
         Retrieves the balance sheet statement financial data for the company(s) from the specified source.
 
         Args:
             quarter (bool, optional): Flag to retrieve quarterly or annual data. Defaults to False.
@@ -411,15 +411,15 @@
             return self._balance_sheet_statement.loc[self._tickers[0]]
 
         return self._balance_sheet_statement
 
     def get_income_statement(
         self,
         quarter=False,
-        limit = 100,
+        limit=100,
         overwrite: bool = False,
     ):
         """
         Retrieves the income statement financial data for the company(s) from the specified source.
 
         Args:
             quarter (bool, optional): Flag to retrieve quarterly or annual data. Defaults to False.
@@ -446,15 +446,15 @@
             return self._income_statement.loc[self._tickers[0]]
 
         return self._income_statement
 
     def get_cash_flow_statement(
         self,
         quarter=False,
-        limit = 100,
+        limit=100,
         overwrite: bool = False,
     ):
         """
         Retrieves the cash flow statement financial data for the company(s) from the specified source.
 
         Args:
             quarter (bool, optional): Flag to retrieve quarterly or annual data. Defaults to False.
@@ -478,15 +478,15 @@
             )
 
         if len(self._tickers) == 1:
             return self._cash_flow_statement.loc[self._tickers[0]]
 
         return self._cash_flow_statement
 
-    def get_normalization_files(self, path = ""):
+    def get_normalization_files(self, path=""):
         """
         Copies the normalization files to a folder based on path. By default, this is the path
         of the 'Downloads' folder.
 
         Args:
             path (str, optional): The path where to save the files to.
```

### Comparing `financetoolkit-1.0.1/financetoolkit/historical/price.py` & `financetoolkit-1.0.2/financetoolkit/historical/price.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Price Module"""
 
-import pandas as pd
 
 
 def get_returns(historical_data):
     """
     Calculate the returns of historical data for a given Series, with an option to include a rolling period.
 
     Args:
@@ -26,17 +25,15 @@
 
     Returns:
         pd.Series: A Series of volatility with time as index and assets as columns.
     """
     return returns.std()
 
 
-def get_sharpe_ratio(
-    returns, risk_free_rate
-):
+def get_sharpe_ratio(returns, risk_free_rate):
     """
     Calculate the Sharpe ratio of returns over a rolling window.
 
     Args:
         returns (pd.Series): A Series of returns with time as index
         risk_free_rate (float or pd.Series): The annualized risk-free rate.
 
@@ -44,17 +41,15 @@
         pd.Series: A Series of Sharpe ratios with time as index and assets as columns.
     """
     excess_returns = returns - risk_free_rate
 
     return excess_returns / returns.std()
 
 
-def get_sortino_ratio(
-    returns, risk_free_rate
-):
+def get_sortino_ratio(returns, risk_free_rate):
     """
     Calculate the Sortino ratio of returns over a rolling window.
 
     Args:
         returns (pd.Series): A Series of returns with time as index
         risk_free_rate (float or pd.Series): The annualized risk-free rate.
         rolling_window (int): The size of the rolling window.
```

### Comparing `financetoolkit-1.0.1/financetoolkit/models/dupont.py` & `financetoolkit-1.0.2/financetoolkit/models/dupont.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.0.1/financetoolkit/portfolio/portfolio.py` & `financetoolkit-1.0.2/financetoolkit/portfolio/portfolio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 """Portfolio Module"""
 __docformat__ = "numpy"
 
 import numpy as np
-import pandas as pd
 
 
-def get_tracking_error(
-    portfolio_returns, benchmark_returns
-):
+def get_tracking_error(portfolio_returns, benchmark_returns):
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
 
 
-def get_payoff_ratio(returns) :
+def get_payoff_ratio(returns):
     """
     Calculate the Payoff Ratio, a ratio that measures the ability of a trading strategy
     to generate profits relative to its losses.
 
     Args:
         returns (pd.Series): A series of returns.
 
@@ -53,15 +50,15 @@
     """
     return returns[returns > 0].sum() / abs(returns[returns < 0].sum())
 
 
 def get_jensens_alpha(
     returns,
     benchmark_returns,
-    risk_free_rate = 0.0,
+    risk_free_rate=0.0,
 ):
     """
     Calculates the Jensen's alpha for the given returns series relative to the given benchmark returns series.
 
     Args:
         returns (pd.Series): A series of asset returns.
         benchmark_returns (pd.Series): A series of benchmark returns.
@@ -159,17 +156,15 @@
         raise ValueError(
             "Calmar ratio can not be calculated due to zero negative returns."
         )
 
     return average_return / maximum_drawdown
 
 
-def get_kelly_criterion(
-    win_probability, win_loss_ratio
-):
+def get_kelly_criterion(win_probability, win_loss_ratio):
     """
     Calculates the Kelly criterion for the given win and loss probabilities.
 
     The win/loss ratio rpresents the ratio of the amount won on a winning
     bet to the amount lost on a losing bet.
 
     The Kelly Criterion is a decimal value between 0 and 1, which
```

### Comparing `financetoolkit-1.0.1/financetoolkit/ratios/efficiency.py` & `financetoolkit-1.0.2/financetoolkit/ratios/efficiency.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """Efficncy Module"""
 __docformat__ = "numpy"
 
-import pandas as pd
 
 
-def get_asset_turnover_ratio(
-    sales, total_assets_begin, total_assets_end
-) :
+def get_asset_turnover_ratio(sales, total_assets_begin, total_assets_end):
     """
     Calculate the asset turnover ratio, an efficiency ratio that measures how
     efficiently a company uses its assets to generate sales.
 
     Args:
         sales (float or pd.Series): Total sales of the company.
         total_assets_begin (float or pd.Series): Total assets at the beginning of the period.
@@ -22,15 +19,15 @@
     return sales / ((total_assets_begin + total_assets_end) / 2)
 
 
 def get_inventory_turnover_ratio(
     cost_of_goods_sold,
     inventory_begin,
     inventory_end,
-) :
+):
     """
     Calculate the inventory turnover ratio, an efficiency ratio that measures
     how quickly a company sells its inventory.
 
     Args:
         cost_of_goods_sold (float or pd.Series): Total cost of goods sold of the company.
         beginning_inventory (float or pd.Series): Beginning inventory of the company.
@@ -42,16 +39,16 @@
     return cost_of_goods_sold / ((inventory_begin + inventory_end) / 2)
 
 
 def get_days_of_inventory_outstanding(
     inventory_begin,
     inventory_end,
     cost_of_goods_sold,
-    days = 365,
-) :
+    days=365,
+):
     """
     Calculate the days sales in inventory ratio, an efficiency ratio that measures
     how long it takes a company to sell its inventory.
 
     Args:
         inventory_begin (float or pd.Series): Beginning inventory of the company.
         inventory_end (float or pd.Series): Ending inventory of the company.
@@ -64,16 +61,16 @@
     return ((inventory_begin + inventory_end) / 2) / cost_of_goods_sold * days
 
 
 def get_days_of_sales_outstanding(
     accounts_receivable_begin,
     accounts_receivable_end,
     net_credit_sales,
-    days = 365,
-) :
+    days=365,
+):
     """
     Calculate the days of sales outstanding, an efficiency ratio that measures
     the average number of days it takes a company to collect payment on its
     credit sales.
 
     Args:
         accounts_receivable_begin (float or pd.Series): Beginning accounts receivable of the company.
@@ -87,17 +84,15 @@
     return (
         ((accounts_receivable_begin + accounts_receivable_end) / 2)
         / net_credit_sales
         * days
     )
 
 
-def get_operating_cycle(
-    days_of_inventory, days_of_sales_outstanding
-) :
+def get_operating_cycle(days_of_inventory, days_of_sales_outstanding):
     """
     Calculate the operating cycle, an efficiency ratio that measures the average
     number of days it takes a company to turn its inventory into cash.
 
     Args:
         days_of_inventory (float or pd.Series): Days of inventory of the company.
         days_of_sales_outstanding (float or pd.Series): Days of sales outstanding of the company.
@@ -109,15 +104,15 @@
     return days_of_inventory + days_of_sales_outstanding
 
 
 def get_accounts_payables_turnover_ratio(
     cost_of_goods_sold,
     accounts_payable_begin,
     accounts_payable_end,
-) :
+):
     """
     Calculate the accounts payable turnover ratio is an efficiency ratio that measures how
     quickly a company pays its suppliers.
 
     Args:
         cost_of_goods_sold (float or pd.Series): Total Costs of Goods Sold of the company.
         accounts_payable_begin (float or pd.Series): Beginning accounts payable of the company.
@@ -129,16 +124,16 @@
     return cost_of_goods_sold / ((accounts_payable_begin + accounts_payable_end) / 2)
 
 
 def get_days_of_accounts_payable_outstanding(
     cost_of_goods_sold,
     accounts_payable_begin,
     accounts_payable_end,
-    days = 365,
-) :
+    days=365,
+):
     """
     Calculate the days payables outstanding, an efficiency ratio that measures the
     number of days it takes a company to pay its suppliers.
 
     Args:
         cost_of_goods_sold (float or pd.Series): Total Costs of Goods Sold of the company.
         accounts_payable_begin (float or pd.Series): Beginning accounts payable of the company.
@@ -155,15 +150,15 @@
     )
 
 
 def get_cash_conversion_cycle(
     days_inventory,
     days_sales_outstanding,
     days_payables_outstanding,
-) :
+):
     """
     Calculate the Cash Conversion Cycle, which measures the amount of time it takes for a company to convert
     its investments in inventory and accounts receivable into cash, while considering the time it takes to pay
     its accounts payable.
 
     Args:
         days_inventory (float or pd.Series): Average number of days that inventory is held before being sold.
@@ -176,15 +171,15 @@
     return days_inventory + days_sales_outstanding - days_payables_outstanding
 
 
 def get_receivables_turnover(
     accounts_receivable_begin,
     accounts_receivable_end,
     net_credit_sales,
-) :
+):
     """
     Calculate the receivables turnover, a ratio that measures how efficiently a
     company uses its assets by comparing the amount of credit extended to customers to
     the amount of sales generated.
 
     Args:
         account_receivables (float or pd.Series): The average amount of receivables during the period.
@@ -194,17 +189,15 @@
         float : The receivables turnover value.
     """
     return (
         (accounts_receivable_begin + accounts_receivable_end) / 2
     ) / net_credit_sales
 
 
-def get_sga_to_revenue_ratio(
-    sga_expenses, revenue
-) :
+def get_sga_to_revenue_ratio(sga_expenses, revenue):
     """
     Calculates the sales, general, and administrative (SG&A) expenses to revenue ratio,
     which measures the SG&A expenses relative to the revenue of the company.
 
     Args:
         sga_expenses (float or pd.Series): SG&A expenses of the company.
         revenue (float or pd.Series): Revenue of the company.
@@ -215,15 +208,15 @@
     return sga_expenses / revenue
 
 
 def get_fixed_asset_turnover(
     net_sales,
     net_fixed_assets_begin,
     net_fixed_assets_end,
-) :
+):
     """
     Calculate the Fixed Asset Turnover ratio, an efficiency ratio that
     measures how efficiently a company uses its fixed assets to generate sales.
 
     Args:
         net_sales (float or pd.Series): Total sales of the company.
         net_fixed_assets_begin (float or pd.Series): Net fixed assets of the company.
@@ -235,15 +228,15 @@
     return net_sales / ((net_fixed_assets_begin + net_fixed_assets_end) / 2)
 
 
 def get_operating_ratio(
     operating_expenses,
     cost_of_goods_sold,
     revenue,
-) :
+):
     """
     Calculate the operating ratio, a financial metric that measures the efficiency
     of a company's operations by comparing its operating expenses to its revenue.
 
     Args:
         operating_expenses (float or pd.Series): Total operating expenses of the company.
         cost_of_goods_sold (float or pd.Series): Total cost of goods sold of the company.
```

### Comparing `financetoolkit-1.0.1/financetoolkit/ratios/liquidity.py` & `financetoolkit-1.0.2/financetoolkit/ratios/liquidity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """Liquidity Module"""
 __docformat__ = "numpy"
 
-import pandas as pd
 
 
-def get_current_ratio(
-    current_assets, current_liabilities
-) :
+def get_current_ratio(current_assets, current_liabilities):
     """
     Calculate the current ratio, a liquidity ratio that measures a company's ability
     to pay off its short-term liabilities with its current assets.
 
     This can also be called the working capital ratio.
 
     Args:
@@ -24,15 +21,15 @@
 
 
 def get_quick_ratio(
     cash_and_equivalents,
     accounts_receivable,
     marketable_securities,
     current_liabilities,
-) :
+):
     """
     Calculate the quick ratio (also known as the acid-test ratio), a more stringent
     measure of liquidity that excludes inventory from current assets.
 
     This ratio is also referred to as the Acid Test Ratio.
 
     Args:
@@ -49,15 +46,15 @@
     ) / current_liabilities
 
 
 def get_cash_ratio(
     cash_and_equivalents,
     marketable_securities,
     current_liabilities,
-) :
+):
     """
     Calculate the cash ratio, a liquidity ratio that measures a company's ability
     to pay off its short-term liabilities with its cash and cash equivalents.
 
     Args:
         cash_and_equivalents (float or pd.Series): Total cash and cash equivalents of the company.
         marketable_securities (float or pd.Series): Total marketable securities of the company.
@@ -65,51 +62,45 @@
 
     Returns:
         float : The cash ratio value.
     """
     return (cash_and_equivalents + marketable_securities) / current_liabilities
 
 
-def get_working_capital(
-    current_assets, current_liabilities
-) :
+def get_working_capital(current_assets, current_liabilities):
     """
     Calculate the working capital, which is the difference between a company's current assets
     and current liabilities.
 
     Args:
         current_assets (float or pd.Series): The current assets of the company.
         current_liabilities (float or pd.Series): The current liabilities of the company.
 
     Returns:
         float : The working capital value.
     """
     return current_assets - current_liabilities
 
 
-def get_operating_cash_flow_ratio(
-    operating_cash_flow, current_liabilities
-) :
+def get_operating_cash_flow_ratio(operating_cash_flow, current_liabilities):
     """
     Calculate the operating cash flow ratio, a liquidity ratio that measures a company's
     ability to pay off its current liabilities with its operating cash flow.
 
     Args:
         operating_cash_flow (float or pd.Series): Operating cash flow of the company.
         current_liabilities (float or pd.Series): Current liabilities of the company.
 
     Returns:
         float : The operating cash flow ratio value.
     """
     return operating_cash_flow / current_liabilities
 
 
-def get_operating_cash_flow_sales_ratio(
-    operating_cash_flow, revenue
-) :
+def get_operating_cash_flow_sales_ratio(operating_cash_flow, revenue):
     """
     Calculate the operating cash flow to sales ratio, a liquidity ratio that measures the ability of a company to generate
     cash from its sales.
 
     Args:
         operating_cash_flow (float or pd.Series): Operating cash flow of the company.
         revenue (float or pd.Series): Sales of the company.
@@ -121,15 +112,15 @@
 
 
 def get_short_term_coverage_ratio(
     operating_cash_flow,
     accounts_receivable,
     inventory,
     accounts_payable,
-) :
+):
     """
     Calculate the short term coverage ratio, a liquidity ratio that measures a company's ability to pay off its
     short-term obligations with its operating cash flow.
 
     Args:
         operating_cash_flow (float or pd.Series): Operating cash flow of the company.
         accounts_receivable (float or pd.Series): Accounts receivable of the company.
```

### Comparing `financetoolkit-1.0.1/financetoolkit/ratios/profitability.py` & `financetoolkit-1.0.2/financetoolkit/ratios/profitability.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,67 +1,58 @@
 """Profitability Module"""
 __docformat__ = "numpy"
 
-import pandas as pd
 
 
-def get_gross_margin(
-    revenue, cost_of_goods_sold
-) :
+def get_gross_margin(revenue, cost_of_goods_sold):
     """
     Calculate the gross margin, a profitability ratio that measures the percentage of
     revenue that exceeds the cost of goods sold.
 
     Args:
         revenue (float or pd.Series): Total revenue of the company.
         cost_of_goods_sold (float or pd.Series): Total cost of goods sold of the company.
 
     Returns:
         float : The gross margin percentage value.
     """
     return (revenue - cost_of_goods_sold) / revenue
 
 
-def get_operating_margin(
-    operating_income, revenue
-) :
+def get_operating_margin(operating_income, revenue):
     """
     Calculate the operating margin, a profitability ratio that measures the percentage of
     revenue that remains after deducting operating expenses.
 
     Args:
         operating_income (float or pd.Series): Operating income of the company.
         revenue (float or pd.Series): Total revenue of the company.
 
     Returns:
         float : The operating margin percentage value.
     """
     return operating_income / revenue
 
 
-def get_net_profit_margin(
-    net_income, revenue
-) :
+def get_net_profit_margin(net_income, revenue):
     """
     Calculate the net profit margin, a profitability ratio that measures the percentage
     of profit a company earns per dollar of revenue.
 
     Args:
         net_income (float or pd.Series): Net income of the company.
         revenue (float or pd.Series): Revenue of the company.
 
     Returns:
         float : The net profit margin value as a percentage.
     """
     return net_income / revenue
 
 
-def get_interest_coverage_ratio(
-    operating_income, interest_expense
-) :
+def get_interest_coverage_ratio(operating_income, interest_expense):
     """
     Compute the Interest Coverage Ratio, a metric that reveals a company's
     ability to cover its interest expenses with its pre-tax profits.
     This ratio measures how many times the operating income covers the
     interest payments of operain required and is crucial in determining a
     company's financial health.
 
@@ -71,17 +62,15 @@
 
     Returns:
         float : The Interest Coverage Ratio
     """
     return operating_income / interest_expense
 
 
-def get_interest_burden_ratio(
-    income_before_tax, operating_income
-) :
+def get_interest_burden_ratio(income_before_tax, operating_income):
     """
     Compute the Interest Burden Ratio, a metric that reveals a company's
     ability to cover its interest expenses with its pre-tax profits.
     This ratio measures how many times the operating income covers the
     interest payments of operain required and is crucial in determining a
     company's financial health.
 
@@ -91,51 +80,45 @@
 
     Returns:
         float : The Interest Burden Ratio
     """
     return income_before_tax / operating_income
 
 
-def get_income_before_tax_profit_margin(
-    income_before_tax, revenue
-) :
+def get_income_before_tax_profit_margin(income_before_tax, revenue):
     """
     Calculate the Pretax Profit Margin, which is the ratio of a company's pre-tax profit to its revenue,
     indicating how much profit a company makes before paying taxes on its earnings.
 
     Args:
         income_before_tax (float or pd.Series): Income before tax of the company.
         revenue (float or pd.Series): Revenue of the company.
 
     Returns:
         float : The Pretax Profit Margin value.
     """
     return income_before_tax / revenue
 
 
-def get_effective_tax_rate(
-    income_tax_expense, income_before_tax
-) :
+def get_effective_tax_rate(income_tax_expense, income_before_tax):
     """
     Calculate the effective tax rate, a financial ratio that measures the percentage of pretax income
     that is paid as taxes.
 
     Args:
         income_tax_expense (float or pd.Series): The amount of income tax paid by the company.
         income_before_tax (float or pd.Series): The company's income before taxes.
 
     Returns:
         float : The effective tax rate value.
     """
     return income_tax_expense / income_before_tax
 
 
-def get_return_on_assets(
-    net_income, total_assets
-) :
+def get_return_on_assets(net_income, total_assets):
     """
     Calculate the return on assets (ROA), a profitability ratio that measures how
     efficiently a company uses its assets to generate profits.
 
     Args:
         net_income (float or pd.Series): Net income of the company.
         total_assets (float or pd.Series): Total assets of the company.
@@ -146,15 +129,15 @@
     return net_income / total_assets
 
 
 def get_return_on_equity(
     net_income,
     total_equity_begin,
     total_equity_end,
-) :
+):
     """
     Calculate the return on equity (ROE), a profitability ratio that measures how
     efficiently a company generates profits using its shareholders' equity.
 
     Args:
         net_income (float or pd.Series): Net income of the company.
         total_equity_begin (float or pd.Series): Total equity at the beginning of the period.
@@ -168,15 +151,15 @@
 
 def get_return_on_invested_capital(
     net_income,
     dividends,
     effective_tax_rate,
     total_equity,
     total_debt,
-) :
+):
     """
     Calculate the return on invested capital, a financial ratio that measures the company's return on
     the capital invested in it, including both equity and debt.
 
     Args:
         net_income (float or pd.Series): The company's net income.
         dividends (float or pd.Series): The dividends paid by the company.
@@ -191,15 +174,15 @@
         total_equity + total_debt
     )
 
 
 def get_income_quality_ratio(
     cash_flow_from_operating_activities,
     net_income,
-) :
+):
     """
     Calculates the income quality ratio, which measures the cash flow from operating
     activities relative to the net income of the company.
 
     Args:
         cash_flow_from_operating_activities (float or pd.Series): Cash flow from operating activities
             of the company.
@@ -212,15 +195,15 @@
 
 
 def get_return_on_tangible_assets(
     net_income,
     total_assets,
     intangible_assets,
     total_liabilities,
-) :
+):
     """
     Calculate the return on tangible assets, which measures the amount of profit
     generated by a company's tangible assets.
 
     Args:
         net_income (float or pd.Series): The net income of the company.
         interest_expense (float or pd.Series): The interest expense of the company.
@@ -237,15 +220,15 @@
 
 def get_return_on_capital_employed(
     net_income,
     interest_expense,
     tax_expense,
     total_assets,
     total_current_liabilities,
-) :
+):
     """
     Calculate the return on capital employed (ROCE), a profitability ratio that measures
     the amount of return a company generates from the capital it has invested in the business.
 
     Args:
         net_income (float or pd.Series): Net income of the company.
         interest_expense (float or pd.Series)erest expense of the company.
@@ -257,34 +240,30 @@
         float : The ROCE value.
     """
     return (net_income + interest_expense + tax_expense) / (
         total_assets - total_current_liabilities
     )
 
 
-def get_net_income_per_ebt(
-    net_income, income_tax_expense
-) :
+def get_net_income_per_ebt(net_income, income_tax_expense):
     """
     Calculate the net income per earnings before taxes (EBT), a profitability ratio that
     measures the net income generated for each dollar of EBT.
 
     Args:
         net_income (float or pd.Series): Net income of the company.
         income_tax_expense (float or pd.Series): Income tax expense of the company.
 
     Returns:
         float : The net income per EBT value.
     """
     return net_income / (net_income + income_tax_expense)
 
 
-def get_free_cash_flow_operating_cash_flow_ratio(
-    free_cash_flow, operating_cash_flow
-) :
+def get_free_cash_flow_operating_cash_flow_ratio(free_cash_flow, operating_cash_flow):
     """
     Calculate the free cash flow to operating cash flow ratio, a profitability
     ratio that measures the amount of free cash flow a company generates
     for every dollar of operating cash flow.
 
     Args:
         free_cash_flow (float or pd.Series): Free cash flow of the company.
@@ -292,17 +271,15 @@
 
     Returns:
         float : The free cash flow to operating cash flow ratio value.
     """
     return free_cash_flow / operating_cash_flow
 
 
-def get_tax_burden_ratio(
-    net_income, income_before_tax
-) :
+def get_tax_burden_ratio(net_income, income_before_tax):
     """
     Calculate the tax burden ratio, which is the ratio of a company's
     net income to its income before tax, indicating how much of a
     company's income is retained after taxes.
 
     Args:
         net_income (float or pd.Series): Net income of the company.
@@ -313,32 +290,30 @@
     """
     return net_income / income_before_tax
 
 
 def get_EBT_to_EBIT(
     earnings_before_tax,
     earnings_before_interest_and_taxes,
-) :
+):
     """
     Calculate the EBT to EBIT, which is the ratio of a company's earnings before tax to its earnings before
     interest and taxes, indicating how much of a company's earnings are generated before paying interest on debt.
 
     Args:
         earnings_before_tax (float or pd.Series): Earnings before tax of the company.
         earnings_before_interest_and_taxes (float or pd.Series): Earnings before interest and taxes of the company.
 
     Returns:
         float : The EBTperEBIT value.
     """
     return earnings_before_tax / earnings_before_interest_and_taxes
 
 
-def get_EBIT_to_revenue(
-    earnings_before_interest_and_taxes, revenue
-) :
+def get_EBIT_to_revenue(earnings_before_interest_and_taxes, revenue):
     """
     Calculate the EBITperRevenue, which is the ratio of a company's earnings
     before interest and taxes to its revenue, indicating how much profit a
     company generates from its operations before paying interest on debt
     and taxes on its earnings.
 
     Args:
```

### Comparing `financetoolkit-1.0.1/financetoolkit/ratios/solvency.py` & `financetoolkit-1.0.2/financetoolkit/ratios/solvency.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """Solvency Module"""
 __docformat__ = "numpy"
 
-import pandas as pd
 
 
-def get_debt_to_assets_ratio(
-    total_debt , total_assets
-):
+def get_debt_to_assets_ratio(total_debt, total_assets):
     """
     Calculate the debt to assets ratio, a solvency ratio that measures the proportion of a
     company's assets that are financed by debt.
 
     This ratio is also known as the debt ratio.
 
     Args:
@@ -19,17 +16,15 @@
 
     Returns:
         float : The debt ratio value.
     """
     return total_debt / total_assets
 
 
-def get_debt_to_equity_ratio(
-    total_debt, total_equity
-) :
+def get_debt_to_equity_ratio(total_debt, total_equity):
     """
     Calculate the debt to equity ratio, a solvency ratio that measures the
     proportion of a company's equity that is financed by debt.
 
     Args:
         total_debt (float or pd.Series): Total debt of the company.
         total_equity (float or pd.Series): Total equity of the company.
@@ -40,15 +35,15 @@
     return total_debt / total_equity
 
 
 def get_interest_coverage_ratio(
     operating_income,
     depreciation_and_amortization,
     interest_expense,
-) :
+):
     """
     Calculate the interest coverage ratio, a solvency ratio that measures a company's
     ability to pay its interest expenses on outstanding debt.
 
     Args:
         operating_income (float or pd.Series): Operating income of the company.
         depreciation_and_amortization (float or pd.Series): Depreciation and amortization of the company.
@@ -56,17 +51,15 @@
 
     Returns:
         float : The interest coverage ratio value.
     """
     return (operating_income + depreciation_and_amortization) / interest_expense
 
 
-def get_debt_service_coverage_ratio(
-    operating_income, current_liabilities
-) :
+def get_debt_service_coverage_ratio(operating_income, current_liabilities):
     """
     Calculate the debt service coverage ratio, a solvency ratio that measures a company's
     ability to service its debt with its net operating income.
 
     Args:
         net_operating_income (float or pd.Series): Net operating income of the company.
         current_liabilities (float or pd.Series): Total debt service of the company.
@@ -78,15 +71,15 @@
 
 
 def get_equity_multiplier(
     total_assets_begin,
     total_assets_end,
     total_equity_begin,
     total_equity_end,
-) :
+):
     """
     Calculate the equity multiplier, a solvency ratio that measures the degree to which a company
     uses borrowed money (debt) to finance its operations and growth.
 
     This is also referred to as the company financial leverage.
 
     Args:
@@ -99,17 +92,15 @@
         float : The equity multiplier.
     """
     return ((total_assets_begin + total_assets_end) / 2) / (
         (total_equity_begin + total_equity_end) / 2
     )
 
 
-def get_free_cash_flow_yield(
-    free_cash_flow, market_capitalization
-) :
+def get_free_cash_flow_yield(free_cash_flow, market_capitalization):
     """
     Calculates the free cash flow yield ratio, which measures the free cash flow
     relative to the market capitalization of the company.
 
     Args:
         free_cash_flow (float or pd.Series): Free cash flow of the company.
         market_capitalization (float or pd.Series): Market capitalization of the company.
@@ -120,15 +111,15 @@
     return free_cash_flow / market_capitalization
 
 
 def get_net_debt_to_ebitda_ratio(
     operating_income,
     depreciation_and_amortization,
     net_debt,
-) :
+):
     """
     Calculates the net debt to EBITDA ratio, which measures the net debt of the company
     relative to its EBITDA.
 
     Args:
         operating_income (float or pd.Series): Operating income of the company.
         depreciation_and_amortization (float or pd.Series): Depreciation and amortization of the company.
@@ -139,32 +130,30 @@
     """
     return net_debt / (operating_income + depreciation_and_amortization)
 
 
 def get_cash_flow_coverage_ratio(
     operating_cash_flow,
     total_debt,
-) :
+):
     """
     Calculate the cash flow coverage ratio, a solvency ratio that measures a company's ability to pay off its debt
     with its operating cash flow.
 
     Args:
         operating_cash_flow (float or pd.Series): Operating cash flow of the company.
         total_debt (float or pd.Series): Total debt of the company.
 
     Returns:
         float : The cash flow coverage ratio value.
     """
     return operating_cash_flow / total_debt
 
 
-def get_capex_coverage_ratio(
-    cash_flow_from_operations, capital_expenditure
-) :
+def get_capex_coverage_ratio(cash_flow_from_operations, capital_expenditure):
     """
     Calculate the capital expenditure coverage ratio, a solvency ratio that
     measures a company's ability to cover its capital expenditures with its
     cash flow from operations.
 
     Args:
         cash_flow_from_operations (float or pd.Series): Cash flow from operations of the company.
@@ -176,15 +165,15 @@
     return cash_flow_from_operations / capital_expenditure
 
 
 def get_dividend_capex_coverage_ratio(
     cash_flow_from_operations,
     capital_expenditure,
     dividends,
-) :
+):
     """
     Calculate the dividend paid and capex coverage ratio, a solvency ratio that
     measures a company's ability to cover both its capital expenditures and
     dividend payments with its cash flow from operations.
 
     Args:
         cash_flow_from_operations (float or pd.Series): Cash flow from operations of the company.
```

### Comparing `financetoolkit-1.0.1/financetoolkit/ratios/valuation.py` & `financetoolkit-1.0.2/financetoolkit/ratios/valuation.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pandas as pd
 
 
 def get_earnings_per_share(
     net_income,
     preferred_dividends,
     average_outstanding_shares,
-) :
+):
     """
     Calculate the earnings per share (EPS), a valuation ratio that measures the
     amount of net income earned per share of outstanding common stock.
 
     Args:
         net_income (float or pd.Series): Net income of the company.
         preferred_dividends (float or pd.Series): Preferred dividends of the company.
@@ -20,34 +20,30 @@
 
     Returns:
         float : The EPS value.
     """
     return (net_income - preferred_dividends) / average_outstanding_shares
 
 
-def get_revenue_per_share(
-    total_revenue, shares_outstanding
-) :
+def get_revenue_per_share(total_revenue, shares_outstanding):
     """
     Calculate the revenue per share, a valuation ratio that measures the amount of
     revenue generated per outstanding share of a company's stock.
 
     Args:
         total_revenue (float or pd.Series): Total revenue of the company.
         shares_outstanding (float or pd.Series): Total number of outstanding shares of the company.
 
     Returns:
         float : The revenue per share value.
     """
     return total_revenue / shares_outstanding
 
 
-def get_price_earnings_ratio(
-    stock_price, earnings_per_share
-) :
+def get_price_earnings_ratio(stock_price, earnings_per_share):
     """
     Calculate the price earnings ratio (P/E), a valuation ratio that compares a company's
     stock price to its earnings per share.
 
     Args:
         stock_price (float or pd.Series): Stock price of the company.
         earnings_per_share (float or pd.Series): Earnings per share of the company.
@@ -74,17 +70,15 @@
         return earnings_per_share.pct_change()
     if isinstance(earnings_per_share, pd.DataFrame):
         return earnings_per_share.pct_change(axis="columns")
 
     raise TypeError("earnings_per_share must be a pd.Series or pd.DataFrame object.")
 
 
-def get_price_to_earnings_growth_ratio(
-    price_earnings, earnings_per_share_growth
-) :
+def get_price_to_earnings_growth_ratio(price_earnings, earnings_per_share_growth):
     """
     Calculate the price earnings to growth (PEG) ratio, a valuation metric that measures the ratio
     of the price-to-earnings ratio to earnings growth rate.
 
     Args:
         price_earnings (float or pd.Series): The company's price-to-earnings ratio.
         earnings_growth (float or pd.Series): The earnings per share growth rate of the company.
@@ -95,15 +89,15 @@
     return price_earnings / earnings_per_share_growth
 
 
 def get_book_value_per_share(
     total_shareholder_equity,
     preferred_equity,
     common_shares_outstanding,
-) :
+):
     """
     Calculate the book value per share, a valuation ratio that measures the amount of
     common equity value per share outstanding.
 
     Args:
         total_shareholder_equity (float or pd.Series): Total equity of the company.
         preferred_equity (float or pd.Series): Preferred equity of the company.
@@ -111,17 +105,15 @@
 
     Returns:
         float : The book value per share value.
     """
     return (total_shareholder_equity - preferred_equity) / common_shares_outstanding
 
 
-def get_price_to_book_ratio(
-    price_per_share, book_value_per_share
-) :
+def get_price_to_book_ratio(price_per_share, book_value_per_share):
     """
     Calculate the price to book ratio, a valuation ratio that compares a company's market
     price to its book value per share.
 
     Args:
         price_per_share (float or pd.Series): Price per share of the company.
         book_value_per_share (float or pd.Series): Book value per share of the company.
@@ -132,15 +124,15 @@
     return price_per_share / book_value_per_share
 
 
 def get_interest_debt_per_share(
     interest_expense,
     total_debt,
     shares_outstanding,
-) :
+):
     """
     Calculate the interest debt per share, a valuation ratio that measures the
     amount of interest expense incurred per outstanding share of a company's stock.
 
     Args:
         interest_expense (float or pd.Series)erest expense of the company.
         total_debt (float or pd.Series): Total debt of the company.
@@ -148,17 +140,15 @@
 
     Returns:
         float : The interest debt per share value.
     """
     return (interest_expense / total_debt) * shares_outstanding
 
 
-def get_capex_per_share(
-    capital_expenditures, shares_outstanding
-) :
+def get_capex_per_share(capital_expenditures, shares_outstanding):
     """
     Calculate the capex per share, a valuation ratio that measures the amount of
     capital expenditures made per outstanding share of a company's stock.
 
     Args:
         capital_expenditures (float or pd.Series): Total capital expenditures made by the company.
         shares_outstanding (float or pd.Series): Total number of outstanding shares of the company.
@@ -169,15 +159,15 @@
     return capital_expenditures / shares_outstanding
 
 
 def get_dividend_yield(
     dividends_paid,
     shares_outstanding,
     stock_price,
-) :
+):
     """
     Calculate the dividend yield ratio, a valuation ratio that measures the amount of
     dividends distributed per share of stock relative to the stock's price.
 
     Args:
         dividends_paid (float or pd.Series): Dividend per share of the company.
         shares_outstanding (float or pd.Series): Total number of outstanding shares of the company.
@@ -185,34 +175,30 @@
 
     Returns:
         float : The dividend yield percentage value.
     """
     return (dividends_paid / shares_outstanding) / stock_price
 
 
-def get_price_to_cash_flow_ratio(
-    market_cap, operations_cash_flow
-) :
+def get_price_to_cash_flow_ratio(market_cap, operations_cash_flow):
     """
     Calculate the price to cash flow ratio, a valuation ratio that compares a company's market
     price to its cash flow per share.
 
     Args:
         market_cap (float or pd.Series): Market capitalization of the company.
         operations_cash_flow (float or pd.Series): Operations cash flow of the company.
 
     Returns:
         float : The price to cash flow ratio value.
     """
     return market_cap / operations_cash_flow
 
 
-def get_price_to_free_cash_flow_ratio(
-    market_cap, free_cash_flow
-) :
+def get_price_to_free_cash_flow_ratio(market_cap, free_cash_flow):
     """
     Calculate the price to free cash flow ratio, a valuation ratio that compares a company's market
     price to its free cash flow per share.
 
     Args:
         market_cap (float or pd.Series): Market capitalization of the company.
         free_cash_flow (float or pd.Series): Free cash flow of the company
@@ -222,15 +208,15 @@
     """
     return market_cap / free_cash_flow
 
 
 def get_market_cap(
     share_price,
     total_shares_outstanding,
-) :
+):
     """
     Calculates the market capitalization of the company.
 
     Note: All the inputs must be in the same currency and unit for accurate calculations.
 
     Args:
         share_price (float ): The share price of the company.
@@ -244,15 +230,15 @@
 
 def get_enterprise_value(
     market_cap,
     total_debt,
     minority_interest,
     preferred_equity,
     cash_and_cash_equivalents,
-) :
+):
     """
     Calculates the Enterprise Value (EV) of a company. The Enterprise Value (EV)
     is a measure of a company's total value, often used as a more comprehensive
     alternative to market capitalization. It is calculated as the sum of a company's
     market capitalization, outstanding debt, minority interest, and
     preferred equity, minus the cash and cash equivalents.
 
@@ -273,17 +259,15 @@
         + total_debt
         + minority_interest
         + preferred_equity
         - cash_and_cash_equivalents
     )
 
 
-def get_ev_to_sales_ratio(
-    enterprise_value, total_revenue
-) :
+def get_ev_to_sales_ratio(enterprise_value, total_revenue):
     """
     Calculate the EV to sales ratio, a valuation ratio that compares a company's enterprise value
     (EV) to its total revenue.
 
     Args:
         enterprise_value (float or pd.Series): Enterprise value of the company.
         total_revenue (float or pd.Series): Total revenue of the company.
@@ -294,15 +278,15 @@
     return enterprise_value / total_revenue
 
 
 def get_ev_to_ebitda_ratio(
     enterprise_value,
     operating_income,
     depreciation_and_amortization,
-) :
+):
     """
     Calculates the enterprise value over EBITDA ratio, which is a valuation ratio
     that measures a company's total value (including debt and equity) relative to its
     EBITDA.
 
     Args:
         enterprise_value (float or pd.Series): The total value of a company (market capitalization
@@ -312,17 +296,15 @@
 
     Returns:
         float : The enterprise value over EBITDA ratio.
     """
     return enterprise_value / (operating_income + depreciation_and_amortization)
 
 
-def get_ev_to_operating_cashflow_ratio(
-    enterprise_value, operating_cashflow
-) :
+def get_ev_to_operating_cashflow_ratio(enterprise_value, operating_cashflow):
     """
     Calculates the enterprise value over operating cash flow ratio, which is a valuation ratio
     that measures a company's total value (including debt and equity) relative to its
     operating cash flow.
 
     Args:
         enterprise_value (float or pd.Series): The total value of a company (market capitalization
@@ -331,34 +313,30 @@
 
     Returns:
         float : The enterprise value over operating cash flow ratio.
     """
     return enterprise_value / operating_cashflow
 
 
-def get_earnings_yield(
-    earnings_per_share, market_price_per_share
-) :
+def get_earnings_yield(earnings_per_share, market_price_per_share):
     """
     Calculates the earnings yield ratio, which measures the earnings per share relative
     to the market price per share.
 
     Args:
         earnings_per_share (float or pd.Series): Earnings per share of the company.
         market_price_per_share (float or pd.Series): Market price per share of the company.
 
     Returns:
         float : The earnings yield ratio.
     """
     return earnings_per_share / market_price_per_share
 
 
-def get_payout_ratio(
-    dividends, net_income
-) :
+def get_payout_ratio(dividends, net_income):
     """
     Calculates the payout ratio, which measures the proportion of net income paid out as
     dividends to shareholders.
 
     Args:
         dividends (float or pd.Series): Dividends paid by the company.
         net_income (float or pd.Series): Net income of the company.
@@ -369,15 +347,15 @@
     return abs(dividends) / net_income
 
 
 def get_tangible_asset_value(
     total_assets,
     total_liabilities,
     goodwill,
-) :
+):
     """
     Calculate the tangible asset value, which represents the total value of a company's assets
     that can be used to generate revenue.
 
     Args:
         total_assets (float or pd.Series): The total assets of the company.
         total_liabilities (float or pd.Series): The total liabilities of the company.
@@ -388,15 +366,15 @@
     """
     return total_assets - total_liabilities - goodwill
 
 
 def get_net_current_asset_value(
     total_current_assets,
     total_current_liabilities,
-) :
+):
     """
     Calculate the net current asset value, which is the total value of a company's current assets
     minus its current liabilities.
 
     Args:
         total_current_assets (float or pd.Series): The current assets of the company.
         total_current_liabilities (float or pd.Series): The current liabilities of the company.
@@ -406,15 +384,15 @@
     """
     return total_current_assets - total_current_liabilities
 
 
 def get_ev_to_ebit(
     enterprise_value,
     earnings_before_interest_and_taxes,
-) :
+):
     """
     Calculate the enterprise value multiplier, a financial ratio that measures the total value of a
     company's operations (including debt and equity) relative to its earnings before interest and taxes.
 
     Args:
         enterprise_value (float or pd.Series): The total value of a company's operations.
         earnings_before_interest_and_taxes (float or pd.Series): The company's earnings before interest and taxes.
```

### Comparing `financetoolkit-1.0.1/pyproject.toml` & `financetoolkit-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "financetoolkit"
-version = "1.0.1"
+version = "1.0.2"
 description = "Transparent and Efficient Financial Analysis"
 license = "MIT"
 authors = ["Jeroen Bouma"]
 packages = [
     { include = "financetoolkit" },
 ]
 include = ['normalization/*.csv']
```

### Comparing `financetoolkit-1.0.1/PKG-INFO` & `financetoolkit-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financetoolkit
-Version: 1.0.1
+Version: 1.0.2
 Summary: Transparent and Efficient Financial Analysis
 Home-page: https://www.jeroenbouma.com/
 License: MIT
 Author: Jeroen Bouma
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 ![FinanceToolkitCropped](https://github.com/JerBouma/FinanceToolkit/assets/46355364/198d47bd-e1b3-492d-acc4-5d9f02d1d009)
 
 [![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-Donate-brightgreen?logo=buymeacoffee)](https://www.buymeacoffee.com/jerbouma)
 [![Website](https://img.shields.io/badge/Website-Learn%20more%20about%20me%20here-brightgreen?logo=ReadMe)](https://jeroenbouma.com/)
 [![PYPI Version](https://img.shields.io/pypi/v/FinanceToolkit)](https://pypi.org/project/FinanceToolkit/)
 [![PYPI Downloads](https://img.shields.io/pypi/dm/FinanceToolkit)](https://pypi.org/project/FinanceToolkit/)
 
-**NOTE: THIS VERSION HAS ALL TYPING REMOVED AND THUS SUPPORTS PYTHON VERSIONS LESS THAN PYTHON 3.10. THIS IS MERELY MEANT TO SUPPORT THOSE WHO HAVEN"T UPDATED YET AND WON"T BE MAINTAINED FURTHER. PLEASE VISIT THE LATEST BUILD AND UPDATE PYTHON ACCORDINGLY**
+**NOTE: THIS VERSION HAS ALL TYPING REMOVED AND THUS SUPPORTS PYTHON VERSIONS LESS THAN PYTHON 3.10. THIS IS MERELY MEANT TO SUPPORT THOSE WHO HAVEN'T UPDATED YET AND WON'T BE MAINTAINED FURTHER. PLEASE VISIT THE LATEST BUILD AND UPDATE PYTHON ACCORDINGLY.**
 
 While browsing a variety of websites, I kept finding that the same financial metric can greatly vary per source and so do the financial statements reported while little information is given how the metric was calculated.
 
 For example, Microsoft's Price-to-Earnings (PE) ratio on the 6th of May, 2023 is reported to be 28.93 (Stockopedia), 32.05 (Morningstar), 32.66 (Macrotrends), 33.09 (Finance Charts), 33.66 (Y Charts), 33.67 (Wall Street Journal), 33.80 (Yahoo Finance) and 34.4 (Companies Market Cap). All of these calculations are correct, however the method applied varies leading to different results. Therefore, collecting data from multiple sources can lead to wrong interpretation of the results given that one source could be applying a different calculation method than another. And that is, if it is even freely available. Often the calculation is hidden behind a paid subscription.
 
 **This is why I designed the FinanceToolkit**, this is an open-source toolkit in which all relevant financial ratios (50+), indicators and performance measurements are written down in the most simplistic way allowing for complete transparency of the calculation method. This allows you to not have to rely on metrics from other providers and, given a financial statement, allow for efficient manual calculations. This leads to one uniform method of calculation being applied that is available and understood by everyone.
```

