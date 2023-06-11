# Comparing `tmp/shihua-roshareclient-0.1.1.tar.gz` & `tmp/shihua-roshareclient-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shihua-roshareclient-0.1.1.tar", last modified: Sun Jun 11 08:15:26 2023, max compression
+gzip compressed data, was "shihua-roshareclient-0.1.2.tar", last modified: Sun Jun 11 14:16:32 2023, max compression
```

## Comparing `shihua-roshareclient-0.1.1.tar` & `shihua-roshareclient-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 shihua    (1000) shihua    (1000)        0 2023-06-11 08:15:26.819666 shihua-roshareclient-0.1.1/
--rw-rw-r--   0 shihua    (1000) shihua    (1000)      111 2023-06-09 15:31:55.000000 shihua-roshareclient-0.1.1/MANIFEST.in
--rw-rw-r--   0 shihua    (1000) shihua    (1000)     2151 2023-06-11 08:15:26.819666 shihua-roshareclient-0.1.1/PKG-INFO
--rw-rw-r--   0 shihua    (1000) shihua    (1000)     1837 2023-06-10 15:45:21.000000 shihua-roshareclient-0.1.1/README.md
-drwxrwxr-x   0 shihua    (1000) shihua    (1000)        0 2023-06-11 08:15:26.819666 shihua-roshareclient-0.1.1/roshareclient/
--rw-rw-r--   0 shihua    (1000) shihua    (1000)        0 2023-06-07 14:41:09.000000 shihua-roshareclient-0.1.1/roshareclient/__init__.py
-drwxrwxr-x   0 shihua    (1000) shihua    (1000)        0 2023-06-11 08:15:26.819666 shihua-roshareclient-0.1.1/roshareclient/client/
--rw-rw-r--   0 shihua    (1000) shihua    (1000)        0 2023-06-07 14:41:09.000000 shihua-roshareclient-0.1.1/roshareclient/client/__init__.py
--rw-rw-r--   0 shihua    (1000) shihua    (1000)     6666 2023-06-09 15:11:00.000000 shihua-roshareclient-0.1.1/roshareclient/client/api.py
--rw-rw-r--   0 shihua    (1000) shihua    (1000)    11509 2023-06-09 15:12:04.000000 shihua-roshareclient-0.1.1/roshareclient/client/cons.py
-drwxrwxr-x   0 shihua    (1000) shihua    (1000)        0 2023-06-11 08:15:26.819666 shihua-roshareclient-0.1.1/roshareclient/test/
--rw-rw-r--   0 shihua    (1000) shihua    (1000)    10948 2023-06-09 15:12:32.000000 shihua-roshareclient-0.1.1/roshareclient/test/test_dataapi.py
--rw-rw-r--   0 shihua    (1000) shihua    (1000)       38 2023-06-11 08:15:26.819666 shihua-roshareclient-0.1.1/setup.cfg
--rw-rw-r--   0 shihua    (1000) shihua    (1000)     1299 2023-06-11 08:13:40.000000 shihua-roshareclient-0.1.1/setup.py
-drwxrwxr-x   0 shihua    (1000) shihua    (1000)        0 2023-06-11 08:15:26.819666 shihua-roshareclient-0.1.1/shihua_roshareclient.egg-info/
--rw-rw-r--   0 shihua    (1000) shihua    (1000)     2151 2023-06-11 08:15:26.000000 shihua-roshareclient-0.1.1/shihua_roshareclient.egg-info/PKG-INFO
--rw-rw-r--   0 shihua    (1000) shihua    (1000)      357 2023-06-11 08:15:26.000000 shihua-roshareclient-0.1.1/shihua_roshareclient.egg-info/SOURCES.txt
--rw-rw-r--   0 shihua    (1000) shihua    (1000)        1 2023-06-11 08:15:26.000000 shihua-roshareclient-0.1.1/shihua_roshareclient.egg-info/dependency_links.txt
--rw-rw-r--   0 shihua    (1000) shihua    (1000)       14 2023-06-11 08:15:26.000000 shihua-roshareclient-0.1.1/shihua_roshareclient.egg-info/top_level.txt
+drwxrwxr-x   0 shihua    (1000) shihua    (1000)        0 2023-06-11 14:16:32.691756 shihua-roshareclient-0.1.2/
+-rw-rw-r--   0 shihua    (1000) shihua    (1000)      111 2023-06-09 15:31:55.000000 shihua-roshareclient-0.1.2/MANIFEST.in
+-rw-rw-r--   0 shihua    (1000) shihua    (1000)     2151 2023-06-11 14:16:32.691756 shihua-roshareclient-0.1.2/PKG-INFO
+-rw-rw-r--   0 shihua    (1000) shihua    (1000)     1837 2023-06-10 15:45:21.000000 shihua-roshareclient-0.1.2/README.md
+drwxrwxr-x   0 shihua    (1000) shihua    (1000)        0 2023-06-11 14:16:32.691756 shihua-roshareclient-0.1.2/roshareclient/
+-rw-rw-r--   0 shihua    (1000) shihua    (1000)        0 2023-06-07 14:41:09.000000 shihua-roshareclient-0.1.2/roshareclient/__init__.py
+drwxrwxr-x   0 shihua    (1000) shihua    (1000)        0 2023-06-11 14:16:32.691756 shihua-roshareclient-0.1.2/roshareclient/client/
+-rw-rw-r--   0 shihua    (1000) shihua    (1000)        0 2023-06-07 14:41:09.000000 shihua-roshareclient-0.1.2/roshareclient/client/__init__.py
+-rw-rw-r--   0 shihua    (1000) shihua    (1000)     6666 2023-06-09 15:11:00.000000 shihua-roshareclient-0.1.2/roshareclient/client/api.py
+-rw-rw-r--   0 shihua    (1000) shihua    (1000)    11554 2023-06-11 14:03:24.000000 shihua-roshareclient-0.1.2/roshareclient/client/cons.py
+drwxrwxr-x   0 shihua    (1000) shihua    (1000)        0 2023-06-11 14:16:32.691756 shihua-roshareclient-0.1.2/roshareclient/test/
+-rw-rw-r--   0 shihua    (1000) shihua    (1000)    10948 2023-06-11 14:06:40.000000 shihua-roshareclient-0.1.2/roshareclient/test/test_dataapi.py
+-rw-rw-r--   0 shihua    (1000) shihua    (1000)       38 2023-06-11 14:16:32.691756 shihua-roshareclient-0.1.2/setup.cfg
+-rw-rw-r--   0 shihua    (1000) shihua    (1000)     1300 2023-06-11 14:15:12.000000 shihua-roshareclient-0.1.2/setup.py
+drwxrwxr-x   0 shihua    (1000) shihua    (1000)        0 2023-06-11 14:16:32.691756 shihua-roshareclient-0.1.2/shihua_roshareclient.egg-info/
+-rw-rw-r--   0 shihua    (1000) shihua    (1000)     2151 2023-06-11 14:16:32.000000 shihua-roshareclient-0.1.2/shihua_roshareclient.egg-info/PKG-INFO
+-rw-rw-r--   0 shihua    (1000) shihua    (1000)      357 2023-06-11 14:16:32.000000 shihua-roshareclient-0.1.2/shihua_roshareclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 shihua    (1000) shihua    (1000)        1 2023-06-11 14:16:32.000000 shihua-roshareclient-0.1.2/shihua_roshareclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 shihua    (1000) shihua    (1000)       14 2023-06-11 14:16:32.000000 shihua-roshareclient-0.1.2/shihua_roshareclient.egg-info/top_level.txt
```

### Comparing `shihua-roshareclient-0.1.1/PKG-INFO` & `shihua-roshareclient-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shihua-roshareclient
-Version: 0.1.1
+Version: 0.1.2
 Summary: RoShareClient is a python sdk with chinese stock data client
 Home-page: https://github.com/redblue0216/RoShare
 Author: shihua
 Author-email: 15021408795@163.com
 License: MIT
 Requires-Python: >=3.9.13
 Description-Content-Type: text/markdown
```

### Comparing `shihua-roshareclient-0.1.1/README.md` & `shihua-roshareclient-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `shihua-roshareclient-0.1.1/roshareclient/client/api.py` & `shihua-roshareclient-0.1.2/roshareclient/client/api.py`

 * *Files identical despite different names*

### Comparing `shihua-roshareclient-0.1.1/roshareclient/client/cons.py` & `shihua-roshareclient-0.1.2/roshareclient/client/cons.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 ### 2.添加基础路由
 ### 3.加入到API字典
 
 
 
 ### 基础组件参数管理，为所有数据服务接口的基础
 REQUEST_PROTOCOL = {'http':'http'}
-REQUEST_HOST = {'local':'127.0.0.1'}
+REQUEST_HOST = {'local':'127.0.0.1','aliyun':'139.196.234.152'}
 REQUEST_PORT = {'default':'11911'}
 DATAAPI = {'tushare':'tushare'}
 OPERATOR = {'get_tushare_stock_basic':'get_tushare_stock_basic',
             'get_tushare_stock_company':'get_tushare_stock_company',
             'get_tushare_daily':'get_tushare_daily',
             'get_tushare_weekly':'get_tushare_weekly',
             'get_tushare_monthly':'get_tushare_monthly',
@@ -73,134 +73,134 @@
             }
 
 
 
 ### 具体接口路由管理，由基础组件拼接而成
 ### 沪深股票--基础数据--股票列表
 GET_TUSHARE_STOCK_BASIC = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_stock_basic'] + \
                                 '?'
 ### 沪深股票--基础数据--上市公司基本信息
 GET_TUSHARE_STOCK_COMPANY = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_stock_company'] + \
                                 '?'
 ### 沪深股票--行情数据--日线行情
 GET_TUSHARE_DAILY = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_daily'] + \
                                 '?'
 ### 沪深股票--行情数据--周线行情
 GET_TUSHARE_WEEKLY = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_weekly'] + \
                                 '?'
 ### 沪深股票--行情数据--月线行情
 GET_TUSHARE_MONTHLY = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_monthly'] + \
                                 '?'
 ### 沪深股票--行情数据--每日指标
 GET_TUSHARE_DAILY_BASIC = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_daily_basic'] + \
                                 '?'
 ### 沪深股票--财务数据--利润表
 GET_TUSHARE_INCOME = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_income'] + \
                                 '?'
 ### 沪深股票--财务数据--资产负债表
 GET_TUSHARE_BALANCESHEET = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_balancesheet'] + \
                                 '?'
 ### 沪深股票--财务数据--现金流量表
 GET_TUSHARE_CASHFLOW = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_cashflow'] + \
                                 '?'
 ### 沪深股票--财务数据--业绩预告
 GET_TUSHARE_FORECAST = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_forecast'] + \
                                 '?'  
 ### 沪深股票--财务数据--业绩快报
 GET_TUSHARE_EXPRESS = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_express'] + \
                                 '?'     
 ### 沪深股票--财务数据--财务指标数据
 GET_TUSHARE_FINA_INDICATOR = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_fina_indicator'] + \
                                 '?'        
 ### 沪深股票--指数数据--指数日线行情
 GET_TUSHARE_INDEX_DAILY = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_index_daily'] + \
                                 '?'    
 ### 沪深股票--指数数据--指数周线行情
 GET_TUSHARE_INDEX_WEEKLY = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_index_weekly'] + \
                                 '?' 
 ### 沪深股票--指数数据--指数月线行情
 GET_TUSHARE_INDEX_MONTHLY = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_index_monthly'] + \
                                 '?'     
 ### 沪深股票--指数数据--大盘指数每日指标
 GET_TUSHARE_INDEX_DAILYBASIC = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_index_dailybasic'] + \
                                 '?'      
 ### 沪深股票--指数数据--申万行业分类
 GET_TUSHARE_INDEX_CLASSIFY = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_index_classify'] + \
                                 '?' 
 ### 另类数据--新闻快讯
 GET_TUSHARE_NEWS = REQUEST_PROTOCOL['http'] + \
-                                '://' + REQUEST_HOST['local'] + \
+                                '://' + REQUEST_HOST['aliyun'] + \
                                 ':' + REQUEST_PORT['default'] + \
                                 '/' + DATAAPI['tushare'] + \
                                 '/' + OPERATOR['get_tushare_news'] + \
                                 '?'
```

### Comparing `shihua-roshareclient-0.1.1/roshareclient/test/test_dataapi.py` & `shihua-roshareclient-0.1.2/roshareclient/test/test_dataapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,12 +194,12 @@
 # print(df)
 ### get_tushare_news
 tmp_dict = {}
 tmp_dict['src'] = 'eastmoney'
 tmp_dict['start_date'] = '2023-06-09+00:00:00' ### url中+号表示空格
 tmp_dict['end_date'] = '2023-06-10+00:00:00'
 roshareclient = DataAPI(token_key = 7890,
-                    token='eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2ODYzMjQ5NDUuODkxOTEzNywidXNlciI6InRlc3QifQ.XElnwVRsMrT9LLJCUNVuRu00WDoTNNm0_X5bTKmoy2A',
+                    token='eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2ODY0OTYzMDIuMTE5MjAyNiwidXNlciI6InRlc3QifQ.wZE19w5MLM6FNn78vLTg3PPc-M8Blm-M1mwTLR0xpuw',
                     tushare_token='cd77d46c73f80cb42c4c1cadd52cd81daa9c40f7a137c809de96b90a',
                     timeout=6000)
 df = roshareclient.get_tushare_news(params=tmp_dict)
 print(df)
```

### Comparing `shihua-roshareclient-0.1.1/setup.py` & `shihua-roshareclient-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ### 打开readme文件流，使用utf-8编码
 with open("README.md","r",encoding="utf-8") as fh:
         long_description = fh.read()
 
 setup(
         ### 包与作者信息
         name = 'shihua-roshareclient',
-        version = '0.1.1',
+        version = '0.1.2',
         author = 'shihua',
         author_email = "15021408795@163.com",
         python_requires = ">=3.9.13",
         license = "MIT",
 
         ### 源码与依赖
         packages = find_packages(),
@@ -31,8 +31,8 @@
         long_description_content_type = "text/markdown",
         url = "https://github.com/redblue0216/RoShare",
         classsifiers = [
                 "Programming Language :: Python :: 3.9",
                 "License :: OSI Approved :: MIT License",
                 "Topic :: Scientific/Engineering :: Artificial Intelligence"
         ] 
-)
+)
```

### Comparing `shihua-roshareclient-0.1.1/shihua_roshareclient.egg-info/PKG-INFO` & `shihua-roshareclient-0.1.2/shihua_roshareclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shihua-roshareclient
-Version: 0.1.1
+Version: 0.1.2
 Summary: RoShareClient is a python sdk with chinese stock data client
 Home-page: https://github.com/redblue0216/RoShare
 Author: shihua
 Author-email: 15021408795@163.com
 License: MIT
 Requires-Python: >=3.9.13
 Description-Content-Type: text/markdown
```

