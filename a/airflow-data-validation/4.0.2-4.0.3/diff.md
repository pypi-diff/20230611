# Comparing `tmp/airflow-data-validation-4.0.2.tar.gz` & `tmp/airflow-data-validation-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-data-validation-4.0.2.tar", max compression
+gzip compressed data, was "airflow-data-validation-4.0.3.tar", max compression
```

## Comparing `airflow-data-validation-4.0.2.tar` & `airflow-data-validation-4.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-06 08:59:19.718494 airflow-data-validation-4.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-08 08:24:12.682050 airflow-data-validation-4.0.2/airflow_data_validation/__init__.py
--rw-r--r--   0        0        0     8428 2023-06-11 11:12:24.582890 airflow-data-validation-4.0.2/airflow_data_validation/data_validation.py
--rw-r--r--   0        0        0      279 2023-06-08 08:49:06.605887 airflow-data-validation-4.0.2/airflow_data_validation/setup.py
--rw-r--r--   0        0        0      583 2023-06-11 11:12:24.596352 airflow-data-validation-4.0.2/pyproject.toml
--rw-r--r--   0        0        0      684 2023-06-11 11:13:21.270217 airflow-data-validation-4.0.2/setup.py
--rw-r--r--   0        0        0      653 2023-06-11 11:13:21.270421 airflow-data-validation-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 08:59:19.718494 airflow-data-validation-4.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 08:24:12.682050 airflow-data-validation-4.0.3/airflow_data_validation/__init__.py
+-rw-r--r--   0        0        0     9467 2023-06-11 13:32:57.418396 airflow-data-validation-4.0.3/airflow_data_validation/data_validation.py
+-rw-r--r--   0        0        0      279 2023-06-08 08:49:06.605887 airflow-data-validation-4.0.3/airflow_data_validation/setup.py
+-rw-r--r--   0        0        0      604 2023-06-11 13:31:39.159595 airflow-data-validation-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0      711 2023-06-11 13:34:05.196623 airflow-data-validation-4.0.3/setup.py
+-rw-r--r--   0        0        0      695 2023-06-11 13:34:05.196824 airflow-data-validation-4.0.3/PKG-INFO
```

### Comparing `airflow-data-validation-4.0.2/airflow_data_validation/data_validation.py` & `airflow-data-validation-4.0.3/airflow_data_validation/data_validation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,55 @@
+import datetime
 import logging
 import sys
-
+import requests
+import json
 # airflow_data_validation
 
 # google
 from google.cloud import bigquery
 
 PY3 = sys.version_info[0] == 3
 
 
 class Data_validation():
     # template_fields = ['run_date','run_id']
 
     def __init__(
             self,
+            slack_token,
             bigquery_conn_id='bigquery_default',
             gcp_project='guesty-data',
+            on_call=None,
             *args, **kwargs):
         super(Data_validation, self).__init__(*args, **kwargs)
         self.bigquery_conn_id = bigquery_conn_id
         self.gcp_project = gcp_project
+        self.slack_token = slack_token
+        self.on_call = on_call
 
     ui_color = '#A6E6A6'
 
+    def send_slack_alert(self, test_name, table_name, slack_token, on_call):
+        today = datetime.datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S')
+        text = f'FYI: <!channel>\n' \
+               'BI On Call: <{0}>\n' \
+               '*Test Name*: {1}\n' \
+               '-----------------------------\n' \
+               ':large_blue_circle: *DQA Notification*\n' \
+               '-----------------------------\n' \
+               '*Table*:               {2}\n' \
+               '*Execution Time*:    {3}'.format(on_call, test_name, table_name, today)
+
+        alert = {
+            "text": text
+        }
+
+        requests.post(slack_token, json.dumps(alert))
+
     def get_dup_query(self, destination_table, column_ids_list, is_partitioned, partition_field):
         column_id = ','.join(column_ids_list)
         sql = f'''
             SELECT EXISTS (
             SELECT {column_id}
             FROM `{destination_table}`
         '''
@@ -137,57 +160,60 @@
             elif isinstance(value, float):
                 float_value = float(value)
                 integer_value = int(float_value)
                 return integer_value
             else:
                 raise Exception("Error: Unable to convert the value to an integer.")
 
-    def test_data(self, destination_table, test_name, column_ids_list, min_value=None, max_value=None,
-                  is_partitioned=False,
-                  set_of_values=None, partition_field='partition_date',exit_on_failure=False):
+    def test_data(self, destination_table, test_name, column_ids_list,
+                  is_partitioned=False, min_value=None, max_value=None,
+                  set_of_values=None, partition_field='partition_date', exit_on_failure=False):
         ## duplication QA ##
         if destination_table:
             self.table_name = destination_table.split('.')[2]
 
         if test_name == 'expect_columns_distinct_values':
             sql = self.get_dup_query(destination_table=destination_table, column_ids_list=column_ids_list,
                                      is_partitioned=is_partitioned, partition_field=partition_field)
         elif test_name == 'expect_columns_values_not_null':
             sql = self.get_values_not_null_query(destination_table=destination_table, column_ids_list=column_ids_list,
-                                                 is_partitioned=is_partitioned,partition_field=partition_field)
+                                                 is_partitioned=is_partitioned, partition_field=partition_field)
         elif test_name == 'expect_column_set_of_values':
 
             if len(column_ids_list) > 1:
                 raise ValueError("this test is only available on one column")
             else:
                 sql = self.test_set_of_values(destination_table=destination_table, column_ids_list=column_ids_list,
                                               is_partitioned=is_partitioned,
-                                              set_of_values=set_of_values,partition_field=partition_field)
+                                              set_of_values=set_of_values, partition_field=partition_field)
         elif test_name == 'expect_table_rows_count_to_be_between':
 
             sql = self.test_table_rows_count(destination_table=destination_table, is_partitioned=is_partitioned,
-                                             min_value=min_value, max_value=max_value,partition_field=partition_field)
+                                             min_value=min_value, max_value=max_value, partition_field=partition_field)
         elif test_name == 'expect_column_values_range_to_be_between':
             if len(column_ids_list) > 1:
                 raise ValueError("this test is only available on one column")
             sql = self.test_range_of_values(destination_table=destination_table, column_ids_list=column_ids_list,
                                             min_value=min_value, max_value=max_value,
-                                            is_partitioned=is_partitioned,partition_field=partition_field)
+                                            is_partitioned=is_partitioned, partition_field=partition_field)
 
         qa_result = self.run_query(sql)
 
         if qa_result:  # True means that the quality test failed
             logging.info(f'#### {test_name} Quality Test failed ####')
             msg_text = f"You test failed {test_name}"
             logging.info(msg_text)
             logging.info(f'{msg_text}')
             logging.info(f'#################')
 
             if exit_on_failure:
                 if exit_on_failure == True:
                     exit(1)
                     raise Exception(f'{test_name} Quality Test failed')
+            else:
+                self.send_slack_alert(test_name=test_name, table_name=destination_table, slack_token=self.slack_token,
+                                      on_call=self.on_call)
 
         else:
             logging.info(f'{test_name} - TEST passed')
 
         logging.info(f'{test_name} - Validation test End')
```

### Comparing `airflow-data-validation-4.0.2/pyproject.toml` & `airflow-data-validation-4.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "airflow-data-validation"
-version = "4.0.2"
+version = "4.0.3"
 description = ""
 authors = ["sapir.krespil <sapir.krespil@guesty.com>"]
 readme = "README.md"
 homepage = "https://github.com/guestyorg/airflow_data_validation"
 repository = "https://github.com/guestyorg/airflow_data_validation"
 packages = [{include = "airflow_data_validation"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 google-cloud-bigquery = "^2.4.0"
+requests = "^2.31.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools>=61.1.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
```

### Comparing `airflow-data-validation-4.0.2/setup.py` & `airflow-data-validation-4.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['airflow_data_validation']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['google-cloud-bigquery>=2.4.0,<3.0.0']
+['google-cloud-bigquery>=2.4.0,<3.0.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'airflow-data-validation',
-    'version': '4.0.2',
+    'version': '4.0.3',
     'description': '',
     'long_description': '',
     'author': 'sapir.krespil',
     'author_email': 'sapir.krespil@guesty.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/guestyorg/airflow_data_validation',
```

### Comparing `airflow-data-validation-4.0.2/PKG-INFO` & `airflow-data-validation-4.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: airflow-data-validation
-Version: 4.0.2
+Version: 4.0.3
 Summary: 
 Home-page: https://github.com/guestyorg/airflow_data_validation
 Author: sapir.krespil
 Author-email: sapir.krespil@guesty.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: google-cloud-bigquery (>=2.4.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/guestyorg/airflow_data_validation
 Description-Content-Type: text/markdown
```

