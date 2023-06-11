# Comparing `tmp/airflow-data-validation-4.0.1.tar.gz` & `tmp/airflow-data-validation-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-data-validation-4.0.1.tar", max compression
+gzip compressed data, was "airflow-data-validation-4.0.2.tar", max compression
```

## Comparing `airflow-data-validation-4.0.1.tar` & `airflow-data-validation-4.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-06 08:59:19.718494 airflow-data-validation-4.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-08 08:24:12.682050 airflow-data-validation-4.0.1/airflow_data_validation/__init__.py
--rw-r--r--   0        0        0     8498 2023-06-11 08:57:06.879333 airflow-data-validation-4.0.1/airflow_data_validation/data_validation.py
--rw-r--r--   0        0        0      279 2023-06-08 08:49:06.605887 airflow-data-validation-4.0.1/airflow_data_validation/setup.py
--rw-r--r--   0        0        0      583 2023-06-11 09:02:06.446643 airflow-data-validation-4.0.1/pyproject.toml
--rw-r--r--   0        0        0      684 2023-06-11 09:02:13.072480 airflow-data-validation-4.0.1/setup.py
--rw-r--r--   0        0        0      653 2023-06-11 09:02:13.072675 airflow-data-validation-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 08:59:19.718494 airflow-data-validation-4.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 08:24:12.682050 airflow-data-validation-4.0.2/airflow_data_validation/__init__.py
+-rw-r--r--   0        0        0     8428 2023-06-11 11:12:24.582890 airflow-data-validation-4.0.2/airflow_data_validation/data_validation.py
+-rw-r--r--   0        0        0      279 2023-06-08 08:49:06.605887 airflow-data-validation-4.0.2/airflow_data_validation/setup.py
+-rw-r--r--   0        0        0      583 2023-06-11 11:12:24.596352 airflow-data-validation-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0      684 2023-06-11 11:13:21.270217 airflow-data-validation-4.0.2/setup.py
+-rw-r--r--   0        0        0      653 2023-06-11 11:13:21.270421 airflow-data-validation-4.0.2/PKG-INFO
```

### Comparing `airflow-data-validation-4.0.1/airflow_data_validation/data_validation.py` & `airflow-data-validation-4.0.2/airflow_data_validation/data_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 
 class Data_validation():
     # template_fields = ['run_date','run_id']
 
     def __init__(
             self,
             bigquery_conn_id='bigquery_default',
-            exit_on_failure=False,
             gcp_project='guesty-data',
             *args, **kwargs):
         super(Data_validation, self).__init__(*args, **kwargs)
         self.bigquery_conn_id = bigquery_conn_id
-        self.exit_on_failure = exit_on_failure
         self.gcp_project = gcp_project
 
     ui_color = '#A6E6A6'
 
     def get_dup_query(self, destination_table, column_ids_list, is_partitioned, partition_field):
         column_id = ','.join(column_ids_list)
         sql = f'''
@@ -141,15 +139,15 @@
                 integer_value = int(float_value)
                 return integer_value
             else:
                 raise Exception("Error: Unable to convert the value to an integer.")
 
     def test_data(self, destination_table, test_name, column_ids_list, min_value=None, max_value=None,
                   is_partitioned=False,
-                  set_of_values=None, partition_field='partition_date'):
+                  set_of_values=None, partition_field='partition_date',exit_on_failure=False):
         ## duplication QA ##
         if destination_table:
             self.table_name = destination_table.split('.')[2]
 
         if test_name == 'expect_columns_distinct_values':
             sql = self.get_dup_query(destination_table=destination_table, column_ids_list=column_ids_list,
                                      is_partitioned=is_partitioned, partition_field=partition_field)
@@ -180,16 +178,16 @@
         if qa_result:  # True means that the quality test failed
             logging.info(f'#### {test_name} Quality Test failed ####')
             msg_text = f"You test failed {test_name}"
             logging.info(msg_text)
             logging.info(f'{msg_text}')
             logging.info(f'#################')
 
-            if self.exit_on_failure:
-                if self.exit_on_failure == True:
+            if exit_on_failure:
+                if exit_on_failure == True:
                     exit(1)
                     raise Exception(f'{test_name} Quality Test failed')
 
         else:
             logging.info(f'{test_name} - TEST passed')
 
         logging.info(f'{test_name} - Validation test End')
```

### Comparing `airflow-data-validation-4.0.1/pyproject.toml` & `airflow-data-validation-4.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-data-validation"
-version = "4.0.1"
+version = "4.0.2"
 description = ""
 authors = ["sapir.krespil <sapir.krespil@guesty.com>"]
 readme = "README.md"
 homepage = "https://github.com/guestyorg/airflow_data_validation"
 repository = "https://github.com/guestyorg/airflow_data_validation"
 packages = [{include = "airflow_data_validation"}]
```

### Comparing `airflow-data-validation-4.0.1/setup.py` & `airflow-data-validation-4.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['google-cloud-bigquery>=2.4.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'airflow-data-validation',
-    'version': '4.0.1',
+    'version': '4.0.2',
     'description': '',
     'long_description': '',
     'author': 'sapir.krespil',
     'author_email': 'sapir.krespil@guesty.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/guestyorg/airflow_data_validation',
```

### Comparing `airflow-data-validation-4.0.1/PKG-INFO` & `airflow-data-validation-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-data-validation
-Version: 4.0.1
+Version: 4.0.2
 Summary: 
 Home-page: https://github.com/guestyorg/airflow_data_validation
 Author: sapir.krespil
 Author-email: sapir.krespil@guesty.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

