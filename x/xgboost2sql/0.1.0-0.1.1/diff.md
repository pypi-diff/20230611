# Comparing `tmp/xgboost2sql-0.1.0.tar.gz` & `tmp/xgboost2sql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xgboost2sql-0.1.0.tar", last modified: Sun Jun 11 01:40:18 2023, max compression
+gzip compressed data, was "dist/xgboost2sql-0.1.1.tar", last modified: Sun Jun 11 08:01:42 2023, max compression
```

## Comparing `xgboost2sql-0.1.0.tar` & `xgboost2sql-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-06-11 01:40:18.000000 xgboost2sql-0.1.0/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      158 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/AUTHORS.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)     3559 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)       89 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/HISTORY.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1068 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/LICENSE
--rw-r--r--   0 ryanzheng   (501) staff       (20)      262 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/MANIFEST.in
--rw-r--r--   0 ryanzheng   (501) staff       (20)    12636 2023-06-11 01:40:18.000000 xgboost2sql-0.1.0/PKG-INFO
--rw-r--r--   0 ryanzheng   (501) staff       (20)    11887 2023-06-10 11:52:02.000000 xgboost2sql-0.1.0/README.md
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-06-11 01:40:18.000000 xgboost2sql-0.1.0/docs/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      612 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/docs/Makefile
--rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/docs/authors.rst
--rwxr-xr-x   0 ryanzheng   (501) staff       (20)     4821 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/docs/conf.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)       33 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/docs/contributing.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/docs/history.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)      308 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/docs/index.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1150 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/docs/installation.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)      809 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/docs/make.bat
--rw-r--r--   0 ryanzheng   (501) staff       (20)       27 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/docs/readme.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)       77 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/docs/usage.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)      428 2023-06-11 01:40:18.000000 xgboost2sql-0.1.0/setup.cfg
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1711 2023-06-11 01:39:38.000000 xgboost2sql-0.1.0/setup.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-06-11 01:40:18.000000 xgboost2sql-0.1.0/tests/
--rw-r--r--   0 ryanzheng   (501) staff       (20)     6148 2023-06-10 11:52:51.000000 xgboost2sql-0.1.0/tests/.DS_Store
--rw-r--r--   0 ryanzheng   (501) staff       (20)       41 2023-06-04 09:08:13.000000 xgboost2sql-0.1.0/tests/__init__.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)      942 2023-06-10 08:46:50.000000 xgboost2sql-0.1.0/tests/test_xgboost2sql.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-06-11 01:40:18.000000 xgboost2sql-0.1.0/xgboost2sql/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      169 2023-06-10 08:20:23.000000 xgboost2sql-0.1.0/xgboost2sql/__init__.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     7656 2023-06-10 12:41:11.000000 xgboost2sql-0.1.0/xgboost2sql/xgboost2sql.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-06-11 01:40:18.000000 xgboost2sql-0.1.0/xgboost2sql.egg-info/
--rw-r--r--   0 ryanzheng   (501) staff       (20)    12636 2023-06-11 01:40:18.000000 xgboost2sql-0.1.0/xgboost2sql.egg-info/PKG-INFO
--rw-r--r--   0 ryanzheng   (501) staff       (20)      611 2023-06-11 01:40:18.000000 xgboost2sql-0.1.0/xgboost2sql.egg-info/SOURCES.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-06-11 01:40:18.000000 xgboost2sql-0.1.0/xgboost2sql.egg-info/dependency_links.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)       53 2023-06-11 01:40:18.000000 xgboost2sql-0.1.0/xgboost2sql.egg-info/entry_points.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-06-10 13:57:22.000000 xgboost2sql-0.1.0/xgboost2sql.egg-info/not-zip-safe
--rw-r--r--   0 ryanzheng   (501) staff       (20)       16 2023-06-11 01:40:18.000000 xgboost2sql-0.1.0/xgboost2sql.egg-info/requires.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)       12 2023-06-11 01:40:18.000000 xgboost2sql-0.1.0/xgboost2sql.egg-info/top_level.txt
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-06-11 08:01:42.000000 xgboost2sql-0.1.1/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      158 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/AUTHORS.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     3559 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       89 2023-06-11 08:01:29.000000 xgboost2sql-0.1.1/HISTORY.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1068 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/LICENSE
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      262 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/MANIFEST.in
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    12703 2023-06-11 08:01:42.000000 xgboost2sql-0.1.1/PKG-INFO
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    11954 2023-06-11 07:57:00.000000 xgboost2sql-0.1.1/README.md
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-06-11 08:01:42.000000 xgboost2sql-0.1.1/docs/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      612 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/docs/Makefile
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/docs/authors.rst
+-rwxr-xr-x   0 ryanzheng   (501) staff       (20)     4821 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/docs/conf.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       33 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/docs/contributing.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/docs/history.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      308 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/docs/index.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1150 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/docs/installation.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      809 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/docs/make.bat
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       27 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/docs/readme.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       77 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/docs/usage.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      428 2023-06-11 08:01:42.000000 xgboost2sql-0.1.1/setup.cfg
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1711 2023-06-11 02:56:37.000000 xgboost2sql-0.1.1/setup.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-06-11 08:01:42.000000 xgboost2sql-0.1.1/tests/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     6148 2023-06-10 11:52:51.000000 xgboost2sql-0.1.1/tests/.DS_Store
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       41 2023-06-04 09:08:13.000000 xgboost2sql-0.1.1/tests/__init__.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      942 2023-06-10 08:46:50.000000 xgboost2sql-0.1.1/tests/test_xgboost2sql.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-06-11 08:01:42.000000 xgboost2sql-0.1.1/xgboost2sql/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      169 2023-06-10 08:20:23.000000 xgboost2sql-0.1.1/xgboost2sql/__init__.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     7583 2023-06-11 02:53:26.000000 xgboost2sql-0.1.1/xgboost2sql/xgboost2sql.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-06-11 08:01:42.000000 xgboost2sql-0.1.1/xgboost2sql.egg-info/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    12703 2023-06-11 08:01:42.000000 xgboost2sql-0.1.1/xgboost2sql.egg-info/PKG-INFO
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      611 2023-06-11 08:01:42.000000 xgboost2sql-0.1.1/xgboost2sql.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-06-11 08:01:42.000000 xgboost2sql-0.1.1/xgboost2sql.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       53 2023-06-11 08:01:42.000000 xgboost2sql-0.1.1/xgboost2sql.egg-info/entry_points.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-06-10 13:57:22.000000 xgboost2sql-0.1.1/xgboost2sql.egg-info/not-zip-safe
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       16 2023-06-11 08:01:42.000000 xgboost2sql-0.1.1/xgboost2sql.egg-info/requires.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       12 2023-06-11 08:01:42.000000 xgboost2sql-0.1.1/xgboost2sql.egg-info/top_level.txt
```

### Comparing `xgboost2sql-0.1.0/CONTRIBUTING.rst` & `xgboost2sql-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xgboost2sql-0.1.0/LICENSE` & `xgboost2sql-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xgboost2sql-0.1.0/PKG-INFO` & `xgboost2sql-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,22 @@
-Metadata-Version: 2.1
-Name: xgboost2sql
-Version: 0.1.0
-Summary: Convert the trained xgboost model to sql
-Home-page: https://github.com/ZhengRyan/xgboost2sql
-Author: RyanZheng
-Author-email: zhengruiping000@163.com
-License: MIT license
-Keywords: xgboost2sql
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 # XGBoost模型转sql语句工具包
 现在是大数据量的时代，我们开发的模型要应用在特别大的待预测集上，使用单机的python，需要预测2、3天，甚至更久，中途很有可能中断。因此需要通过分布式的方式来预测。这个工具包就是实现了将训练好的python模型，转换成sql语句。将生成的sql语句可以放到大数据环境中进行分布式执行预测，能比单机的python预测快好几个量级
 
 
 ## 思想碰撞
 
 |  微信 |  微信公众号 |
 | :---: | :----: |
-| <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/RyanZheng.png" alt="RyanZheng.png" width="50%" border=0/> | <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E9%AD%94%E9%83%BD%E6%95%B0%E6%8D%AE%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="魔都数据干饭人.png" width="50%" border=0/> |
-|  RyanZheng  | 魔都数据干饭人 |
+| <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="RyanZheng.png" width="50%" border=0/> | <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E9%AD%94%E9%83%BD%E6%95%B0%E6%8D%AE%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="魔都数据干饭人.png" width="50%" border=0/> |
+|  干饭人  | 魔都数据干饭人 |
 
 
 > 仓库地址：https://github.com/ZhengRyan/xgboost2sql
 > 
-> 微信公众号文章：
+> 微信公众号文章：https://mp.weixin.qq.com/s/z3IjzMFKP7iEoag5KP6nAA
 > 
 > pipy包：https://pypi.org/project/xgboost2sql/
 
 
 
 ## 环境准备
 可以不用单独创建虚拟环境，因为对包的依赖没有版本要求
@@ -53,20 +31,20 @@
 
 Source code install（源码安装）
 
 ```bash
 python setup.py install
 ```
 
-### 运行样例
-####【注意：：：核验对比python模型预测出来的结果和sql语句预测出来的结果是否一致请查看"https://github.com/ZhengRyan/xgboost2sql/examples/tutorial_code.ipynb"教程代码】
+## 运行样例
+###【注意：：：核验对比python模型预测出来的结果和sql语句预测出来的结果是否一致请查看教程代码】"https://github.com/ZhengRyan/xgboost2sql/examples/tutorial_code.ipynb"
 
 + 导入相关依赖
 ```python
-import xgboost as xgb
+import xgboost as xgb 
 from sklearn.datasets import make_classification
 from sklearn.model_selection import train_test_split
 from xgboost2sql import XGBoost2Sql
 ```
 
 + 训练1个xgboost二分类模型
 ```python
@@ -81,15 +59,15 @@
                            random_state=1024)
 
 X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=1024)
 
 ###训练模型
 model = xgb.XGBClassifier(n_estimators=3)
 model.fit(X_train, y_train)
-xgb.to_graphviz(model)
+#xgb.to_graphviz(model)
 ```
 + 使用xgboost2sql工具包将模型转换成的sql语句
 ```python
 xgb2sql = XGBoost2Sql()
 sql_str = xgb2sql.transform(model)
 ```
```

### Comparing `xgboost2sql-0.1.0/README.md` & `xgboost2sql-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,44 @@
+Metadata-Version: 2.1
+Name: xgboost2sql
+Version: 0.1.1
+Summary: Convert the trained xgboost model to sql
+Home-page: https://github.com/ZhengRyan/xgboost2sql
+Author: RyanZheng
+Author-email: zhengruiping000@163.com
+License: MIT license
+Keywords: xgboost2sql
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+
 # XGBoost模型转sql语句工具包
 现在是大数据量的时代，我们开发的模型要应用在特别大的待预测集上，使用单机的python，需要预测2、3天，甚至更久，中途很有可能中断。因此需要通过分布式的方式来预测。这个工具包就是实现了将训练好的python模型，转换成sql语句。将生成的sql语句可以放到大数据环境中进行分布式执行预测，能比单机的python预测快好几个量级
 
 
 ## 思想碰撞
 
 |  微信 |  微信公众号 |
 | :---: | :----: |
-| <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/RyanZheng.png" alt="RyanZheng.png" width="50%" border=0/> | <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E9%AD%94%E9%83%BD%E6%95%B0%E6%8D%AE%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="魔都数据干饭人.png" width="50%" border=0/> |
-|  RyanZheng  | 魔都数据干饭人 |
+| <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="RyanZheng.png" width="50%" border=0/> | <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E9%AD%94%E9%83%BD%E6%95%B0%E6%8D%AE%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="魔都数据干饭人.png" width="50%" border=0/> |
+|  干饭人  | 魔都数据干饭人 |
 
 
 > 仓库地址：https://github.com/ZhengRyan/xgboost2sql
 > 
-> 微信公众号文章：
+> 微信公众号文章：https://mp.weixin.qq.com/s/z3IjzMFKP7iEoag5KP6nAA
 > 
 > pipy包：https://pypi.org/project/xgboost2sql/
 
 
 
 ## 环境准备
 可以不用单独创建虚拟环境，因为对包的依赖没有版本要求
@@ -31,20 +53,20 @@
 
 Source code install（源码安装）
 
 ```bash
 python setup.py install
 ```
 
-### 运行样例
-####【注意：：：核验对比python模型预测出来的结果和sql语句预测出来的结果是否一致请查看"https://github.com/ZhengRyan/xgboost2sql/examples/tutorial_code.ipynb"教程代码】
+## 运行样例
+###【注意：：：核验对比python模型预测出来的结果和sql语句预测出来的结果是否一致请查看教程代码】"https://github.com/ZhengRyan/xgboost2sql/examples/tutorial_code.ipynb"
 
 + 导入相关依赖
 ```python
-import xgboost as xgb
+import xgboost as xgb 
 from sklearn.datasets import make_classification
 from sklearn.model_selection import train_test_split
 from xgboost2sql import XGBoost2Sql
 ```
 
 + 训练1个xgboost二分类模型
 ```python
@@ -59,15 +81,15 @@
                            random_state=1024)
 
 X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=1024)
 
 ###训练模型
 model = xgb.XGBClassifier(n_estimators=3)
 model.fit(X_train, y_train)
-xgb.to_graphviz(model)
+#xgb.to_graphviz(model)
 ```
 + 使用xgboost2sql工具包将模型转换成的sql语句
 ```python
 xgb2sql = XGBoost2Sql()
 sql_str = xgb2sql.transform(model)
 ```
```

### Comparing `xgboost2sql-0.1.0/docs/Makefile` & `xgboost2sql-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xgboost2sql-0.1.0/docs/conf.py` & `xgboost2sql-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xgboost2sql-0.1.0/docs/installation.rst` & `xgboost2sql-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `xgboost2sql-0.1.0/docs/make.bat` & `xgboost2sql-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xgboost2sql-0.1.0/setup.py` & `xgboost2sql-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,10 +54,10 @@
     include_package_data=True,
     keywords='xgboost2sql',
     name=NAME,
     packages=find_packages(include=['xgboost2sql', 'xgboost2sql.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ZhengRyan/xgboost2sql',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `xgboost2sql-0.1.0/tests/.DS_Store` & `xgboost2sql-0.1.1/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `xgboost2sql-0.1.0/tests/test_xgboost2sql.py` & `xgboost2sql-0.1.1/tests/test_xgboost2sql.py`

 * *Files identical despite different names*

### Comparing `xgboost2sql-0.1.0/xgboost2sql/xgboost2sql.py` & `xgboost2sql-0.1.1/xgboost2sql/xgboost2sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,22 +101,18 @@
 
         try:
             ###-math.log((1 / x) - 1)
             x = float(json.loads(xgb_model.save_config())['learner']['learner_model_param']['base_score'])
             return -math.log((1 - x) / x)
         except:
             warnings.warn(
-                'xgboost model version less than :: 1.0.0, '
-                'If the base_score parameter is not 0.5 when developing the model, '
-                'Insert the base_score value into the formula "-math.log((1-x)/x)" '
-                'and replace the -0.0 value at +(-0.0) in the first sentence of the generated sql statement with the calculated value')
+                'xgboost model version less than :: 1.0.0, If the base_score parameter is not 0.5 when developing the model, Insert the base_score value into the formula "-math.log((1-x)/x)" and replace the -0.0 value at +(-0.0) in the first sentence of the generated sql statement with the calculated value')
             warnings.warn(
-                'xgboost 模型的版本低于1.0.0，如果开发模型时， base_score 参数不是0.5，'
-                '请将base_score的参数取值带入"-math.log((1 - x) / x)"公式，计算出的值，替换掉生成的sql语句第1句中的+(-0.0)处的-0.0取值')
-            return 0
+                'xgboost 模型的版本低于1.0.0，如果开发模型时， base_score 参数不是0.5，请将base_score的参数取值带入"-math.log((1 - x) / x)"公式，计算出的值，替换掉生成的sql语句第1句中的+(-0.0)处的-0.0取值')
+            return -0.0
 
     def pre_tree(self, lines, is_right, n):
         """
 
         Args:
             lines:二叉树行
             is_right:是否右边
```

### Comparing `xgboost2sql-0.1.0/xgboost2sql.egg-info/PKG-INFO` & `xgboost2sql-0.1.1/xgboost2sql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgboost2sql
-Version: 0.1.0
+Version: 0.1.1
 Summary: Convert the trained xgboost model to sql
 Home-page: https://github.com/ZhengRyan/xgboost2sql
 Author: RyanZheng
 Author-email: zhengruiping000@163.com
 License: MIT license
 Keywords: xgboost2sql
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -24,21 +24,21 @@
 现在是大数据量的时代，我们开发的模型要应用在特别大的待预测集上，使用单机的python，需要预测2、3天，甚至更久，中途很有可能中断。因此需要通过分布式的方式来预测。这个工具包就是实现了将训练好的python模型，转换成sql语句。将生成的sql语句可以放到大数据环境中进行分布式执行预测，能比单机的python预测快好几个量级
 
 
 ## 思想碰撞
 
 |  微信 |  微信公众号 |
 | :---: | :----: |
-| <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/RyanZheng.png" alt="RyanZheng.png" width="50%" border=0/> | <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E9%AD%94%E9%83%BD%E6%95%B0%E6%8D%AE%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="魔都数据干饭人.png" width="50%" border=0/> |
-|  RyanZheng  | 魔都数据干饭人 |
+| <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="RyanZheng.png" width="50%" border=0/> | <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E9%AD%94%E9%83%BD%E6%95%B0%E6%8D%AE%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="魔都数据干饭人.png" width="50%" border=0/> |
+|  干饭人  | 魔都数据干饭人 |
 
 
 > 仓库地址：https://github.com/ZhengRyan/xgboost2sql
 > 
-> 微信公众号文章：
+> 微信公众号文章：https://mp.weixin.qq.com/s/z3IjzMFKP7iEoag5KP6nAA
 > 
 > pipy包：https://pypi.org/project/xgboost2sql/
 
 
 
 ## 环境准备
 可以不用单独创建虚拟环境，因为对包的依赖没有版本要求
@@ -53,20 +53,20 @@
 
 Source code install（源码安装）
 
 ```bash
 python setup.py install
 ```
 
-### 运行样例
-####【注意：：：核验对比python模型预测出来的结果和sql语句预测出来的结果是否一致请查看"https://github.com/ZhengRyan/xgboost2sql/examples/tutorial_code.ipynb"教程代码】
+## 运行样例
+###【注意：：：核验对比python模型预测出来的结果和sql语句预测出来的结果是否一致请查看教程代码】"https://github.com/ZhengRyan/xgboost2sql/examples/tutorial_code.ipynb"
 
 + 导入相关依赖
 ```python
-import xgboost as xgb
+import xgboost as xgb 
 from sklearn.datasets import make_classification
 from sklearn.model_selection import train_test_split
 from xgboost2sql import XGBoost2Sql
 ```
 
 + 训练1个xgboost二分类模型
 ```python
@@ -81,15 +81,15 @@
                            random_state=1024)
 
 X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=1024)
 
 ###训练模型
 model = xgb.XGBClassifier(n_estimators=3)
 model.fit(X_train, y_train)
-xgb.to_graphviz(model)
+#xgb.to_graphviz(model)
 ```
 + 使用xgboost2sql工具包将模型转换成的sql语句
 ```python
 xgb2sql = XGBoost2Sql()
 sql_str = xgb2sql.transform(model)
 ```
```

### Comparing `xgboost2sql-0.1.0/xgboost2sql.egg-info/SOURCES.txt` & `xgboost2sql-0.1.1/xgboost2sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

