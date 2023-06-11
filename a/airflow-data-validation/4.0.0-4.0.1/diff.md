# Comparing `tmp/airflow-data-validation-4.0.0.tar.gz` & `tmp/airflow-data-validation-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-data-validation-4.0.0.tar", max compression
+gzip compressed data, was "airflow-data-validation-4.0.1.tar", max compression
```

## Comparing `airflow-data-validation-4.0.0.tar` & `airflow-data-validation-4.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-06 08:59:19.718494 airflow-data-validation-4.0.0/README.md
--rw-r--r--   0        0        0        0 2023-06-08 08:24:12.682050 airflow-data-validation-4.0.0/airflow_data_validation/__init__.py
--rw-r--r--   0        0        0     7682 2023-06-08 09:56:46.659080 airflow-data-validation-4.0.0/airflow_data_validation/data_validation.py
--rw-r--r--   0        0        0      279 2023-06-08 08:49:06.605887 airflow-data-validation-4.0.0/airflow_data_validation/setup.py
--rw-r--r--   0        0        0      583 2023-06-08 08:49:06.623019 airflow-data-validation-4.0.0/pyproject.toml
--rw-r--r--   0        0        0      684 2023-06-08 10:11:43.694449 airflow-data-validation-4.0.0/setup.py
--rw-r--r--   0        0        0      653 2023-06-08 10:11:43.694664 airflow-data-validation-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 08:59:19.718494 airflow-data-validation-4.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 08:24:12.682050 airflow-data-validation-4.0.1/airflow_data_validation/__init__.py
+-rw-r--r--   0        0        0     8498 2023-06-11 08:57:06.879333 airflow-data-validation-4.0.1/airflow_data_validation/data_validation.py
+-rw-r--r--   0        0        0      279 2023-06-08 08:49:06.605887 airflow-data-validation-4.0.1/airflow_data_validation/setup.py
+-rw-r--r--   0        0        0      583 2023-06-11 09:02:06.446643 airflow-data-validation-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0      684 2023-06-11 09:02:13.072480 airflow-data-validation-4.0.1/setup.py
+-rw-r--r--   0        0        0      653 2023-06-11 09:02:13.072675 airflow-data-validation-4.0.1/PKG-INFO
```

### Comparing `airflow-data-validation-4.0.0/airflow_data_validation/data_validation.py` & `airflow-data-validation-4.0.1/airflow_data_validation/data_validation.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,103 +17,106 @@
             bigquery_conn_id='bigquery_default',
             exit_on_failure=False,
             gcp_project='guesty-data',
             *args, **kwargs):
         super(Data_validation, self).__init__(*args, **kwargs)
         self.bigquery_conn_id = bigquery_conn_id
         self.exit_on_failure = exit_on_failure
-        self.gcp_project =gcp_project
-
+        self.gcp_project = gcp_project
 
     ui_color = '#A6E6A6'
 
-    def get_dup_query(self, destination_table, column_ids_list, is_partitioned):
+    def get_dup_query(self, destination_table, column_ids_list, is_partitioned, partition_field):
         column_id = ','.join(column_ids_list)
         sql = f'''
             SELECT EXISTS (
             SELECT {column_id}
             FROM `{destination_table}`
         '''
         if is_partitioned:
-            sql += f'''    WHERE partition_date = (SELECT MAX(partition_date) FROM `{destination_table}` WHERE partition_date >= DATE_SUB(current_date, INTERVAL 1 DAY))'''
+            sql += f'''    WHERE {partition_field} >= DATE_SUB(current_date, INTERVAL 1 DAY)  
+                             AND {partition_field} = (SELECT MAX({partition_field}) FROM `{destination_table}` WHERE {partition_field} >= DATE_SUB(current_date, INTERVAL 1 DAY))'''
         sql += f'''
             GROUP BY {column_id}
             HAVING COUNT(*) > 1
             )
             '''
         return sql
 
-    def test_set_of_values(self, destination_table, column_ids_list, set_of_values, is_partitioned):
+    def test_set_of_values(self, destination_table, column_ids_list, set_of_values, is_partitioned, partition_field):
         values = ','.join("'" + col + "'" for col in set_of_values)
         column_id = ','.join(column_ids_list)
         sql = f'''
             SELECT EXISTS (
             SELECT {column_id}
             FROM `{destination_table}`
         '''
         if is_partitioned:
             sql += f'''    WHERE {column_id} not in ({values})
-                             AND partition_date >= DATE_SUB(current_date, INTERVAL 1 DAY) 
-                             AND partition_date = (SELECT MAX(partition_date) FROM `{destination_table}` 
-                                                    WHERE partition_date >= DATE_SUB(current_date, INTERVAL 1 DAY)))'''
+                             AND {partition_field} >= DATE_SUB(current_date, INTERVAL 1 DAY) 
+                             AND {partition_field} = (SELECT MAX({partition_field}) FROM `{destination_table}` 
+                                                    WHERE {partition_field} >= DATE_SUB(current_date, INTERVAL 1 DAY)))'''
         else:
             sql += f"WHERE {column_id} not in ({values}) )"
 
         return sql
 
-    def test_range_of_values(self, destination_table, column_ids_list, min_value, max_value, is_partitioned):
+    def test_range_of_values(self, destination_table, column_ids_list, min_value, max_value, is_partitioned,
+                             partition_field):
         column_id = ','.join(column_ids_list)
         sql = f'''
             SELECT EXISTS (
             SELECT {column_id}
             FROM `{destination_table}`
         '''
         if is_partitioned:
             sql += f'''    WHERE {column_id} not between {min_value} and {max_value} 
-                             AND partition_date >= DATE_SUB(current_date, INTERVAL 1 DAY) 
-                             AND partition_date = (SELECT MAX(partition_date) FROM `{destination_table}` 
-                                                    WHERE partition_date >= DATE_SUB(current_date, INTERVAL 1 DAY)))'''
+                             AND {partition_field} >= DATE_SUB(current_date, INTERVAL 1 DAY) 
+                             AND {partition_field} = (SELECT MAX({partition_field}) FROM `{destination_table}` 
+                                                    WHERE {partition_field} >= DATE_SUB(current_date, INTERVAL 1 DAY)))'''
         else:
             sql += f"WHERE {column_id} not between {min_value} and {max_value} )"
 
         return sql
 
-    def test_table_rows_count(self, destination_table, min_value, max_value, is_partitioned):
+    def test_table_rows_count(self, destination_table, min_value, max_value, is_partitioned, partition_field):
         sql = f'''
             SELECT EXISTS (
             SELECT COUNT(*) 
             FROM `{destination_table}`
         '''
         if is_partitioned:
-            sql += f'''    WHERE  partition_date >= DATE_SUB(current_date, INTERVAL 1 DAY) 
-                             AND partition_date = (SELECT MAX(partition_date) FROM `{destination_table}` WHERE partition_date >= DATE_SUB(current_date, INTERVAL 1 DAY))'''
+            sql += f'''    WHERE  {partition_field} >= DATE_SUB(current_date, INTERVAL 1 DAY) 
+                             AND {partition_field} = (SELECT MAX({partition_field})
+                                                        FROM `{destination_table}` 
+                                                        WHERE {partition_field} >= DATE_SUB(current_date, INTERVAL 1 DAY))'''
         sql += f'''
             HAVING COUNT(*) between {min_value} and {max_value} 
             )
             '''
 
         return sql
 
-    def get_values_not_null_query(self, destination_table, column_ids_list, is_partitioned):
+    def get_values_not_null_query(self, destination_table, column_ids_list, is_partitioned, partition_field):
         new_c = []
         column_id = ','.join(column_ids_list)
         for v in column_ids_list:
             new_c.append(v + ' is null')
 
         condition_not_null = ' or '.join(new_c)
 
         sql = f'''
             SELECT EXISTS (
             SELECT {column_id}
             FROM `{destination_table}`
         '''
         if is_partitioned:
             sql += f'''  WHERE ({condition_not_null})
-                           AND partition_date >= DATE_SUB(current_date, INTERVAL 1 DAY) 
-                           AND partition_date = (SELECT MAX(partition_date) FROM `{destination_table}` WHERE partition_date >= DATE_SUB(current_date, INTERVAL 1 DAY))'''
+                           AND {partition_field} >= DATE_SUB(current_date, INTERVAL 1 DAY) 
+                           AND {partition_field} = (SELECT MAX({partition_field}) FROM `{destination_table}` WHERE {partition_field} >= DATE_SUB(current_date, INTERVAL 1 DAY))'''
         else:
             sql += f"WHERE {condition_not_null}"
         sql += f'''
             GROUP BY {column_id}
             HAVING COUNT(*) > 1
             )
             '''
@@ -136,39 +139,45 @@
             elif isinstance(value, float):
                 float_value = float(value)
                 integer_value = int(float_value)
                 return integer_value
             else:
                 raise Exception("Error: Unable to convert the value to an integer.")
 
-    def test_data(self, destination_table, test_name, column_ids_list, min_value=None, max_value=None, is_partitioned=False,
-                  set_of_values=None):
+    def test_data(self, destination_table, test_name, column_ids_list, min_value=None, max_value=None,
+                  is_partitioned=False,
+                  set_of_values=None, partition_field='partition_date'):
         ## duplication QA ##
         if destination_table:
             self.table_name = destination_table.split('.')[2]
 
         if test_name == 'expect_columns_distinct_values':
-            sql = self.get_dup_query(destination_table=destination_table,column_ids_list=column_ids_list, is_partitioned=is_partitioned)
+            sql = self.get_dup_query(destination_table=destination_table, column_ids_list=column_ids_list,
+                                     is_partitioned=is_partitioned, partition_field=partition_field)
         elif test_name == 'expect_columns_values_not_null':
-            sql = self.get_values_not_null_query(destination_table=destination_table,column_ids_list=column_ids_list, is_partitioned=is_partitioned)
+            sql = self.get_values_not_null_query(destination_table=destination_table, column_ids_list=column_ids_list,
+                                                 is_partitioned=is_partitioned,partition_field=partition_field)
         elif test_name == 'expect_column_set_of_values':
 
             if len(column_ids_list) > 1:
                 raise ValueError("this test is only available on one column")
             else:
-                sql = self.test_set_of_values(destination_table=destination_table,column_ids_list=column_ids_list, is_partitioned=is_partitioned,
-                                              set_of_values=set_of_values)
+                sql = self.test_set_of_values(destination_table=destination_table, column_ids_list=column_ids_list,
+                                              is_partitioned=is_partitioned,
+                                              set_of_values=set_of_values,partition_field=partition_field)
         elif test_name == 'expect_table_rows_count_to_be_between':
 
-            sql = self.test_table_rows_count(destination_table=destination_table,is_partitioned=is_partitioned, min_value=min_value, max_value=max_value)
+            sql = self.test_table_rows_count(destination_table=destination_table, is_partitioned=is_partitioned,
+                                             min_value=min_value, max_value=max_value,partition_field=partition_field)
         elif test_name == 'expect_column_values_range_to_be_between':
             if len(column_ids_list) > 1:
                 raise ValueError("this test is only available on one column")
-            sql = self.test_range_of_values(destination_table=destination_table,column_ids_list=column_ids_list, min_value=min_value, max_value=max_value,
-                                            is_partitioned=is_partitioned)
+            sql = self.test_range_of_values(destination_table=destination_table, column_ids_list=column_ids_list,
+                                            min_value=min_value, max_value=max_value,
+                                            is_partitioned=is_partitioned,partition_field=partition_field)
 
         qa_result = self.run_query(sql)
 
         if qa_result:  # True means that the quality test failed
             logging.info(f'#### {test_name} Quality Test failed ####')
             msg_text = f"You test failed {test_name}"
             logging.info(msg_text)
@@ -180,9 +189,7 @@
                     exit(1)
                     raise Exception(f'{test_name} Quality Test failed')
 
         else:
             logging.info(f'{test_name} - TEST passed')
 
         logging.info(f'{test_name} - Validation test End')
-
-
```

### Comparing `airflow-data-validation-4.0.0/pyproject.toml` & `airflow-data-validation-4.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-data-validation"
-version = "4.0.0"
+version = "4.0.1"
 description = ""
 authors = ["sapir.krespil <sapir.krespil@guesty.com>"]
 readme = "README.md"
 homepage = "https://github.com/guestyorg/airflow_data_validation"
 repository = "https://github.com/guestyorg/airflow_data_validation"
 packages = [{include = "airflow_data_validation"}]
```

### Comparing `airflow-data-validation-4.0.0/setup.py` & `airflow-data-validation-4.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['google-cloud-bigquery>=2.4.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'airflow-data-validation',
-    'version': '4.0.0',
+    'version': '4.0.1',
     'description': '',
     'long_description': '',
     'author': 'sapir.krespil',
     'author_email': 'sapir.krespil@guesty.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/guestyorg/airflow_data_validation',
```

### Comparing `airflow-data-validation-4.0.0/PKG-INFO` & `airflow-data-validation-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-data-validation
-Version: 4.0.0
+Version: 4.0.1
 Summary: 
 Home-page: https://github.com/guestyorg/airflow_data_validation
 Author: sapir.krespil
 Author-email: sapir.krespil@guesty.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

