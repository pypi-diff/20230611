# Comparing `tmp/postnormalism-0.0.3.tar.gz` & `tmp/postnormalism-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postnormalism-0.0.3.tar", last modified: Sat May 27 03:02:00 2023, max compression
+gzip compressed data, was "postnormalism-0.0.4.tar", last modified: Sun Jun 11 16:01:32 2023, max compression
```

## Comparing `postnormalism-0.0.3.tar` & `postnormalism-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 03:02:00.157980 postnormalism-0.0.3/
--rw-rw-rw-   0        0        0     1119 2023-05-06 02:54:20.000000 postnormalism-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     7408 2023-05-27 03:02:00.156979 postnormalism-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6247 2023-05-27 02:52:47.000000 postnormalism-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 03:02:00.090039 postnormalism-0.0.3/postnormalism/
--rw-rw-rw-   0        0        0        5 2023-05-27 02:52:47.000000 postnormalism-0.0.3/postnormalism/VERSION
--rw-rw-rw-   0        0        0        0 2023-05-06 02:40:21.000000 postnormalism-0.0.3/postnormalism/__init__.py
--rw-rw-rw-   0        0        0     2143 2023-05-22 03:33:00.000000 postnormalism-0.0.3/postnormalism/core.py
-drwxrwxrwx   0        0        0        0 2023-05-27 03:02:00.139981 postnormalism-0.0.3/postnormalism/schema/
--rw-rw-rw-   0        0        0      182 2023-05-20 21:39:27.000000 postnormalism-0.0.3/postnormalism/schema/__init__.py
--rw-rw-rw-   0        0        0     4713 2023-05-20 22:09:21.000000 postnormalism-0.0.3/postnormalism/schema/database.py
--rw-rw-rw-   0        0        0     1082 2023-05-17 02:15:23.000000 postnormalism-0.0.3/postnormalism/schema/database_item.py
--rw-rw-rw-   0        0        0      408 2023-05-08 03:58:46.000000 postnormalism-0.0.3/postnormalism/schema/function.py
--rw-rw-rw-   0        0        0      406 2023-05-20 21:52:37.000000 postnormalism-0.0.3/postnormalism/schema/migrations.py
--rw-rw-rw-   0        0        0      774 2023-05-17 02:19:15.000000 postnormalism-0.0.3/postnormalism/schema/table.py
--rw-rw-rw-   0        0        0      711 2023-05-06 03:40:39.000000 postnormalism-0.0.3/postnormalism/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-27 03:02:00.106038 postnormalism-0.0.3/postnormalism.egg-info/
--rw-rw-rw-   0        0        0     7408 2023-05-27 03:02:00.000000 postnormalism-0.0.3/postnormalism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-05-27 03:02:00.000000 postnormalism-0.0.3/postnormalism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 03:02:00.000000 postnormalism-0.0.3/postnormalism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-27 03:02:00.000000 postnormalism-0.0.3/postnormalism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1342 2023-05-20 00:26:25.000000 postnormalism-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 03:02:00.157980 postnormalism-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 03:02:00.155982 postnormalism-0.0.3/tests/
--rw-rw-rw-   0        0        0     1778 2023-05-06 17:12:44.000000 postnormalism-0.0.3/tests/test_core.py
--rw-rw-rw-   0        0        0     2288 2023-05-06 17:12:44.000000 postnormalism-0.0.3/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:01:32.918480 postnormalism-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-11 16:01:23.000000 postnormalism-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-11 16:01:32.918480 postnormalism-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-11 16:01:23.000000 postnormalism-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:01:32.918480 postnormalism-0.0.4/postnormalism/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:01:32.918480 postnormalism-0.0.4/postnormalism/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/schema/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/schema/database_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/schema/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/schema/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/schema/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:01:32.918480 postnormalism-0.0.4/postnormalism.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-11 16:01:32.000000 postnormalism-0.0.4/postnormalism.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-11 16:01:32.000000 postnormalism-0.0.4/postnormalism.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 16:01:32.000000 postnormalism-0.0.4/postnormalism.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-11 16:01:32.000000 postnormalism-0.0.4/postnormalism.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-11 16:01:23.000000 postnormalism-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 16:01:32.918480 postnormalism-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:01:32.918480 postnormalism-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-11 16:01:23.000000 postnormalism-0.0.4/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-11 16:01:23.000000 postnormalism-0.0.4/tests/test_schema.py
```

### Comparing `postnormalism-0.0.3/LICENSE` & `postnormalism-0.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2023 Zac Miller and other contributors
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+The MIT License (MIT)
+
+Copyright (c) 2023 Zac Miller and other contributors
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `postnormalism-0.0.3/PKG-INFO` & `postnormalism-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,175 +1,192 @@
-Metadata-Version: 2.1
-Name: postnormalism
-Version: 0.0.3
-Summary: Postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.
-Author-email: Zac Miller <zac@informatical.info>
-Maintainer-email: Zac Miller <zac@informatical.info>
-License: MIT License
-Project-URL: Homepage, https://github.com/jzmiller1/postnormalism
-Project-URL: Bug Tracker, https://github.com/jzmiller1/postnormalism/issues
-Project-URL: Repository, https://github.com/jzmiller1/postnormalism.git
-Project-URL: History, https://github.com/jzmiller1/postnormalism/blob/master/HISTORY.md
-Keywords: python,postgresql,schema
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# postnormalism: PostgreSQL Schema Management  
-  
-postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.  
-  
-## Features  
-  
-- Define tables and functions using Python dataclasses  
-- Create database items (Tables, Functions) with comments
-- Group related database items and create them within a single transaction  
-- Create a Database object that allows loading database items in a specified load order and managing database extensions
-- IF NOT EXISTS mode for loading
-- SQL Migration Loader
-
-  
-## NORM vs. ORM: Features Comparison  
-  
-postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
-  
-Here is a comparison of postnormalism's features with typical ORM characteristics:  
-  
-1. **Object-oriented representation**: postnormalism does not map database tables to classes or table rows to instances. Instead, it uses dataclasses to represent schema items, like tables and functions, for organizing and generating schema items.  
-  
-2. **Abstraction**: postnormalism provides a smidgen of abstraction for creating schema items, but doesn't bother with things like query generation.    
-  
-3. **Query generation**: postnormalism does not include a query builder or DSL for constructing database queries. It focuses on schema management, not query generation.  You are the query generator.
-  
-4. **Transactions and concurrency**: postnormalism kindly allows you to group related schema items and create them within a single transaction. However, it knows when to draw the line and leaves transaction management and concurrency handling for other database operations to more heavyweight solutions.  
-  
-5. **Schema management**: postnormalism excels at schema management by allowing you to excel at schema management. Create schema items and load them in a specified order.  
-  
-6. **Relationships and associations**: postnormalism doesn't get entangled in relationships or associations between tables or objects. After all, it's just a simple library with simple needs.  You have to understand your schema.
-  
-7. **Data validation and constraints**: postnormalism doesn't have time for built-in data validation or constraint enforcement. But fear not, you can still define constraints in your schema items.
-  
-8. **Caching**: postnormalism believes in living in the moment, so caching mechanisms to improve performance are left to others.  
-  
-Should you require a complete ORM solution for your project, consider using a full-fledged ORM like SQLAlchemy or Django's ORM for Python. postnormalism is for those brave souls who seek a lightweight way to manage PostgreSQL schemas without all the bells and whistles.  
-  
-## Installation  
-  
-You can install postnormalism using pip:  
-  
-```sh  
-pip install postnormalism  
-```  
-  
-## Usage  
-  
-### Defining Database Items  
-  
-To define a table or a function, use the `Table` and `Function` dataclasses from the `postnormalism` module:  
-  
-```python  
-from postnormalism.schema import Table, Function  
-```
-  
-### Define a Table
-```python
-from postnormalism.schema import Table
-
-create_table_sql = """  
-CREATE TABLE material (  
-id uuid PRIMARY KEY DEFAULT uuid_generate_v4(),  
-name varchar(120) NOT NULL,  
-description varchar(240)  
-);  
-"""  
-  
-Material = Table(create=create_table_sql)  
-```
-  
-### Define a Postgresql Function  
-```python
-from postnormalism.schema import Function
-
-create_function_sql = """  
-CREATE FUNCTION get_material_for_variant(variant uuid)  
-RETURNS uuid  
-AS $$  
-material_plan = plpy.prepare("SELECT material FROM material_variant WHERE id = $1",  
-["uuid"])  
-material = plpy.execute(material_plan, [variant])[0]["material"]  
-return material  
-$$ LANGUAGE plpython3u;  
-"""  
-  
-comment_function_sql = """  
-COMMENT ON FUNCTION get_material_for_variant IS  
-$$ An example function $$;  
-"""  
-  
-get_material_for_variant = Function(create=create_function_sql, comment=comment_function_sql)  
-```  
-  
-### Creating Database Items in a Database  
-  
-To create database items in a PostgreSQL database, use the `Database` class:  
-  
-```python  
-import psycopg  
-from postnormalism.schema import Database
-from your_example_file import Material, get_material_for_variant
-
-universe = Database(
-    load_order=[
-        Material, get_material_for_variant,
-        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
-    ],
-    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto']
-)
-
-db_connection_string = "dbname=test user=postgres password=secret host=localhost port=port"  
-
-connection = psycopg.connect(db_connection_string)  
-cursor = connection.cursor()  
-
-universe.create(cursor)  
-
-connection.commit()  
-connection.close()  
-```  
-
-### Using exists Mode
-Calling Database.create with exists=True inserts a IF NOT EXISTS into all of your CREATE statements allowing you to easily add new items.
-
-```python
-universe.create(cursor, exists=True)
-```
-
-### Doing migrations
-Update your `DatabaseItem`s and write your SQL migration transaction.  If you create your Database instance with 
-a `migrations_folder` they will run during the create call.  Migration files should ideally be prefixed with a 
-load order (ex: 0001) and must end with `.sql`.
-
-```python
-universe = Database(
-    load_order=[
-        Material, get_material_for_variant,
-        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
-    ],
-    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto'],
-    migrations_folder='/example/folder/path'
-)
-
-```
-
-
-## Contributing  
-  
-Please submit a pull request or create an issue if you have any suggestions or improvements.  
-  
-## License  
-  
-postnormalism is released under the MIT License. See the `LICENSE` file for more information.
+Metadata-Version: 2.1
+Name: postnormalism
+Version: 0.0.4
+Summary: Postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.
+Author-email: Zac Miller <zac@informatical.info>
+Maintainer-email: Zac Miller <zac@informatical.info>
+License: MIT License
+Project-URL: Homepage, https://github.com/jzmiller1/postnormalism
+Project-URL: Bug Tracker, https://github.com/jzmiller1/postnormalism/issues
+Project-URL: Repository, https://github.com/jzmiller1/postnormalism.git
+Project-URL: History, https://github.com/jzmiller1/postnormalism/blob/master/HISTORY.md
+Keywords: python,postgresql,schema
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# postnormalism: PostgreSQL Schema Management  
+  
+postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.  
+  
+## Features  
+  
+- Define schemas, tables and functions using Python dataclasses  
+- Create database items (Schemas, Tables, Functions) with comments
+- Group related database items and create them within a single transaction  
+- Create a Database object that allows loading database items in a specified load order and managing database extensions
+- IF NOT EXISTS mode for loading
+- SQL Migration Loader
+
+  
+## NORM vs. ORM: Features Comparison  
+  
+postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
+  
+Here is a comparison of postnormalism's features with typical ORM characteristics:  
+  
+1. **Object-oriented representation**: postnormalism does not map database tables to classes or table rows to instances. Instead, it uses dataclasses to represent schema items, like tables and functions, for organizing and generating schema items.  
+  
+2. **Abstraction**: postnormalism provides a smidgen of abstraction for creating schema items, but doesn't bother with things like query generation.    
+  
+3. **Query generation**: postnormalism does not include a query builder or DSL for constructing database queries. It focuses on schema management, not query generation.  You are the query generator.
+  
+4. **Transactions and concurrency**: postnormalism kindly allows you to group related schema items and create them within a single transaction. However, it knows when to draw the line and leaves transaction management and concurrency handling for other database operations to more heavyweight solutions.  
+  
+5. **Schema management**: postnormalism excels at schema management by allowing you to excel at schema management. Create schema items and load them in a specified order.  
+  
+6. **Relationships and associations**: postnormalism doesn't get entangled in relationships or associations between tables or objects. After all, it's just a simple library with simple needs.  You have to understand your schema.
+  
+7. **Data validation and constraints**: postnormalism doesn't have time for built-in data validation or constraint enforcement. But fear not, you can still define constraints in your schema items.
+  
+8. **Caching**: postnormalism believes in living in the moment, so caching mechanisms to improve performance are left to others.  
+  
+Should you require a complete ORM solution for your project, consider using a full-fledged ORM like SQLAlchemy or Django's ORM for Python. postnormalism is for those brave souls who seek a lightweight way to manage PostgreSQL schemas without all the bells and whistles.  
+  
+## Installation  
+  
+You can install postnormalism using pip:  
+  
+```sh  
+pip install postnormalism  
+```  
+  
+## Usage  
+  
+### Defining Database Items  
+  
+To define a table or a function, use the `Table` and `Function` dataclasses from the `postnormalism` module:  
+  
+```python  
+from postnormalism.schema import Schema, Table, Function  
+```
+
+### Define a Schema
+```python
+from postnormalism import schema
+
+create = """
+CREATE SCHEMA basic_auth;
+"""
+
+comment = """
+COMMENT ON SCHEMA basic_auth IS
+  $$ The basic auth schema $$;
+"""
+
+basic_auth = schema.Schema(create=create, comment=comment)
+```
+  
+### Define a Table
+```python
+from postnormalism.schema import Table
+
+create_table_sql = """  
+CREATE TABLE material (  
+id uuid PRIMARY KEY DEFAULT uuid_generate_v4(),  
+name varchar(120) NOT NULL,  
+description varchar(240)  
+);  
+"""  
+  
+Material = Table(create=create_table_sql)  
+```
+  
+### Define a Postgresql Function  
+```python
+from postnormalism.schema import Function
+
+create_function_sql = """  
+CREATE FUNCTION get_material_for_variant(variant uuid)  
+RETURNS uuid  
+AS $$  
+material_plan = plpy.prepare("SELECT material FROM material_variant WHERE id = $1",  
+["uuid"])  
+material = plpy.execute(material_plan, [variant])[0]["material"]  
+return material  
+$$ LANGUAGE plpython3u;  
+"""  
+  
+comment_function_sql = """  
+COMMENT ON FUNCTION get_material_for_variant IS  
+$$ An example function $$;  
+"""  
+  
+get_material_for_variant = Function(create=create_function_sql, comment=comment_function_sql)  
+```  
+  
+### Creating Database Items in a Database  
+  
+To create database items in a PostgreSQL database, use the `Database` class:  
+  
+```python  
+import psycopg  
+from postnormalism.schema import Database
+from your_example_file import Material, get_material_for_variant, Player, Inventory, basic_auth
+
+universe = Database(
+    load_order=[
+        basic_auth,
+        Material, get_material_for_variant,
+        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
+    ],
+    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto']
+)
+
+db_connection_string = "dbname=test user=postgres password=secret host=localhost port=port"  
+
+connection = psycopg.connect(db_connection_string)  
+cursor = connection.cursor()  
+
+universe.create(cursor)  
+
+connection.commit()  
+connection.close()  
+```  
+
+### Using exists Mode
+Calling Database.create with exists=True inserts a IF NOT EXISTS into all of your CREATE statements allowing you to easily add new items.
+
+```python
+universe.create(cursor, exists=True)
+```
+
+### Doing migrations
+Update your `DatabaseItem`s and write your SQL migration transaction.  If you create your Database instance with 
+a `migrations_folder` they will run during the create call.  Migration files should ideally be prefixed with a 
+load order (ex: 0001) and must end with `.sql`.
+
+```python
+universe = Database(
+    load_order=[
+        Material, get_material_for_variant,
+        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
+    ],
+    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto'],
+    migrations_folder='/example/folder/path'
+)
+
+```
+
+
+## Contributing  
+  
+Please submit a pull request or create an issue if you have any suggestions or improvements.  
+  
+## License  
+  
+postnormalism is released under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `postnormalism-0.0.3/README.md` & `postnormalism-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,154 +1,171 @@
-# postnormalism: PostgreSQL Schema Management  
-  
-postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.  
-  
-## Features  
-  
-- Define tables and functions using Python dataclasses  
-- Create database items (Tables, Functions) with comments
-- Group related database items and create them within a single transaction  
-- Create a Database object that allows loading database items in a specified load order and managing database extensions
-- IF NOT EXISTS mode for loading
-- SQL Migration Loader
-
-  
-## NORM vs. ORM: Features Comparison  
-  
-postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
-  
-Here is a comparison of postnormalism's features with typical ORM characteristics:  
-  
-1. **Object-oriented representation**: postnormalism does not map database tables to classes or table rows to instances. Instead, it uses dataclasses to represent schema items, like tables and functions, for organizing and generating schema items.  
-  
-2. **Abstraction**: postnormalism provides a smidgen of abstraction for creating schema items, but doesn't bother with things like query generation.    
-  
-3. **Query generation**: postnormalism does not include a query builder or DSL for constructing database queries. It focuses on schema management, not query generation.  You are the query generator.
-  
-4. **Transactions and concurrency**: postnormalism kindly allows you to group related schema items and create them within a single transaction. However, it knows when to draw the line and leaves transaction management and concurrency handling for other database operations to more heavyweight solutions.  
-  
-5. **Schema management**: postnormalism excels at schema management by allowing you to excel at schema management. Create schema items and load them in a specified order.  
-  
-6. **Relationships and associations**: postnormalism doesn't get entangled in relationships or associations between tables or objects. After all, it's just a simple library with simple needs.  You have to understand your schema.
-  
-7. **Data validation and constraints**: postnormalism doesn't have time for built-in data validation or constraint enforcement. But fear not, you can still define constraints in your schema items.
-  
-8. **Caching**: postnormalism believes in living in the moment, so caching mechanisms to improve performance are left to others.  
-  
-Should you require a complete ORM solution for your project, consider using a full-fledged ORM like SQLAlchemy or Django's ORM for Python. postnormalism is for those brave souls who seek a lightweight way to manage PostgreSQL schemas without all the bells and whistles.  
-  
-## Installation  
-  
-You can install postnormalism using pip:  
-  
-```sh  
-pip install postnormalism  
-```  
-  
-## Usage  
-  
-### Defining Database Items  
-  
-To define a table or a function, use the `Table` and `Function` dataclasses from the `postnormalism` module:  
-  
-```python  
-from postnormalism.schema import Table, Function  
-```
-  
-### Define a Table
-```python
-from postnormalism.schema import Table
-
-create_table_sql = """  
-CREATE TABLE material (  
-id uuid PRIMARY KEY DEFAULT uuid_generate_v4(),  
-name varchar(120) NOT NULL,  
-description varchar(240)  
-);  
-"""  
-  
-Material = Table(create=create_table_sql)  
-```
-  
-### Define a Postgresql Function  
-```python
-from postnormalism.schema import Function
-
-create_function_sql = """  
-CREATE FUNCTION get_material_for_variant(variant uuid)  
-RETURNS uuid  
-AS $$  
-material_plan = plpy.prepare("SELECT material FROM material_variant WHERE id = $1",  
-["uuid"])  
-material = plpy.execute(material_plan, [variant])[0]["material"]  
-return material  
-$$ LANGUAGE plpython3u;  
-"""  
-  
-comment_function_sql = """  
-COMMENT ON FUNCTION get_material_for_variant IS  
-$$ An example function $$;  
-"""  
-  
-get_material_for_variant = Function(create=create_function_sql, comment=comment_function_sql)  
-```  
-  
-### Creating Database Items in a Database  
-  
-To create database items in a PostgreSQL database, use the `Database` class:  
-  
-```python  
-import psycopg  
-from postnormalism.schema import Database
-from your_example_file import Material, get_material_for_variant
-
-universe = Database(
-    load_order=[
-        Material, get_material_for_variant,
-        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
-    ],
-    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto']
-)
-
-db_connection_string = "dbname=test user=postgres password=secret host=localhost port=port"  
-
-connection = psycopg.connect(db_connection_string)  
-cursor = connection.cursor()  
-
-universe.create(cursor)  
-
-connection.commit()  
-connection.close()  
-```  
-
-### Using exists Mode
-Calling Database.create with exists=True inserts a IF NOT EXISTS into all of your CREATE statements allowing you to easily add new items.
-
-```python
-universe.create(cursor, exists=True)
-```
-
-### Doing migrations
-Update your `DatabaseItem`s and write your SQL migration transaction.  If you create your Database instance with 
-a `migrations_folder` they will run during the create call.  Migration files should ideally be prefixed with a 
-load order (ex: 0001) and must end with `.sql`.
-
-```python
-universe = Database(
-    load_order=[
-        Material, get_material_for_variant,
-        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
-    ],
-    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto'],
-    migrations_folder='/example/folder/path'
-)
-
-```
-
-
-## Contributing  
-  
-Please submit a pull request or create an issue if you have any suggestions or improvements.  
-  
-## License  
-  
-postnormalism is released under the MIT License. See the `LICENSE` file for more information.
+# postnormalism: PostgreSQL Schema Management  
+  
+postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.  
+  
+## Features  
+  
+- Define schemas, tables and functions using Python dataclasses  
+- Create database items (Schemas, Tables, Functions) with comments
+- Group related database items and create them within a single transaction  
+- Create a Database object that allows loading database items in a specified load order and managing database extensions
+- IF NOT EXISTS mode for loading
+- SQL Migration Loader
+
+  
+## NORM vs. ORM: Features Comparison  
+  
+postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
+  
+Here is a comparison of postnormalism's features with typical ORM characteristics:  
+  
+1. **Object-oriented representation**: postnormalism does not map database tables to classes or table rows to instances. Instead, it uses dataclasses to represent schema items, like tables and functions, for organizing and generating schema items.  
+  
+2. **Abstraction**: postnormalism provides a smidgen of abstraction for creating schema items, but doesn't bother with things like query generation.    
+  
+3. **Query generation**: postnormalism does not include a query builder or DSL for constructing database queries. It focuses on schema management, not query generation.  You are the query generator.
+  
+4. **Transactions and concurrency**: postnormalism kindly allows you to group related schema items and create them within a single transaction. However, it knows when to draw the line and leaves transaction management and concurrency handling for other database operations to more heavyweight solutions.  
+  
+5. **Schema management**: postnormalism excels at schema management by allowing you to excel at schema management. Create schema items and load them in a specified order.  
+  
+6. **Relationships and associations**: postnormalism doesn't get entangled in relationships or associations between tables or objects. After all, it's just a simple library with simple needs.  You have to understand your schema.
+  
+7. **Data validation and constraints**: postnormalism doesn't have time for built-in data validation or constraint enforcement. But fear not, you can still define constraints in your schema items.
+  
+8. **Caching**: postnormalism believes in living in the moment, so caching mechanisms to improve performance are left to others.  
+  
+Should you require a complete ORM solution for your project, consider using a full-fledged ORM like SQLAlchemy or Django's ORM for Python. postnormalism is for those brave souls who seek a lightweight way to manage PostgreSQL schemas without all the bells and whistles.  
+  
+## Installation  
+  
+You can install postnormalism using pip:  
+  
+```sh  
+pip install postnormalism  
+```  
+  
+## Usage  
+  
+### Defining Database Items  
+  
+To define a table or a function, use the `Table` and `Function` dataclasses from the `postnormalism` module:  
+  
+```python  
+from postnormalism.schema import Schema, Table, Function  
+```
+
+### Define a Schema
+```python
+from postnormalism import schema
+
+create = """
+CREATE SCHEMA basic_auth;
+"""
+
+comment = """
+COMMENT ON SCHEMA basic_auth IS
+  $$ The basic auth schema $$;
+"""
+
+basic_auth = schema.Schema(create=create, comment=comment)
+```
+  
+### Define a Table
+```python
+from postnormalism.schema import Table
+
+create_table_sql = """  
+CREATE TABLE material (  
+id uuid PRIMARY KEY DEFAULT uuid_generate_v4(),  
+name varchar(120) NOT NULL,  
+description varchar(240)  
+);  
+"""  
+  
+Material = Table(create=create_table_sql)  
+```
+  
+### Define a Postgresql Function  
+```python
+from postnormalism.schema import Function
+
+create_function_sql = """  
+CREATE FUNCTION get_material_for_variant(variant uuid)  
+RETURNS uuid  
+AS $$  
+material_plan = plpy.prepare("SELECT material FROM material_variant WHERE id = $1",  
+["uuid"])  
+material = plpy.execute(material_plan, [variant])[0]["material"]  
+return material  
+$$ LANGUAGE plpython3u;  
+"""  
+  
+comment_function_sql = """  
+COMMENT ON FUNCTION get_material_for_variant IS  
+$$ An example function $$;  
+"""  
+  
+get_material_for_variant = Function(create=create_function_sql, comment=comment_function_sql)  
+```  
+  
+### Creating Database Items in a Database  
+  
+To create database items in a PostgreSQL database, use the `Database` class:  
+  
+```python  
+import psycopg  
+from postnormalism.schema import Database
+from your_example_file import Material, get_material_for_variant, Player, Inventory, basic_auth
+
+universe = Database(
+    load_order=[
+        basic_auth,
+        Material, get_material_for_variant,
+        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
+    ],
+    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto']
+)
+
+db_connection_string = "dbname=test user=postgres password=secret host=localhost port=port"  
+
+connection = psycopg.connect(db_connection_string)  
+cursor = connection.cursor()  
+
+universe.create(cursor)  
+
+connection.commit()  
+connection.close()  
+```  
+
+### Using exists Mode
+Calling Database.create with exists=True inserts a IF NOT EXISTS into all of your CREATE statements allowing you to easily add new items.
+
+```python
+universe.create(cursor, exists=True)
+```
+
+### Doing migrations
+Update your `DatabaseItem`s and write your SQL migration transaction.  If you create your Database instance with 
+a `migrations_folder` they will run during the create call.  Migration files should ideally be prefixed with a 
+load order (ex: 0001) and must end with `.sql`.
+
+```python
+universe = Database(
+    load_order=[
+        Material, get_material_for_variant,
+        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
+    ],
+    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto'],
+    migrations_folder='/example/folder/path'
+)
+
+```
+
+
+## Contributing  
+  
+Please submit a pull request or create an issue if you have any suggestions or improvements.  
+  
+## License  
+  
+postnormalism is released under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `postnormalism-0.0.3/postnormalism/core.py` & `postnormalism-0.0.4/postnormalism/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from . import schema
-
-
-def create_schema_items_in_transaction(schema_items: list[schema.DatabaseItem], exists=False) -> str:
-    """
-    Create schema items within a single transaction.
-    """
-    sql_parts = ["BEGIN;"]
-
-    # First, create all schema items and add comments
-    for item in schema_items:
-        # Get the SQL parts of each item
-        full_sql_parts = item.full_sql(exists=exists).split("\n\n")
-        # Append only the CREATE TABLE statements (and comments if any)
-        sql_parts.append(full_sql_parts[0])
-        if item.comment:
-            sql_parts.append(full_sql_parts[1])
-
-    # Then, add the ALTER TABLE statements for tables
-    for item in schema_items:
-        if isinstance(item, schema.Table) and item.alter:
-            # Get the SQL parts of each item
-            full_sql_parts = item.full_sql(exists=exists).split("\n\n")
-            # Append only the ALTER TABLE statements
-            if len(full_sql_parts) > 2:
-                sql_parts.append(full_sql_parts[2])
-
-    sql_parts.append("COMMIT;")
-
-    return "\n\n".join(sql_parts)
-
-
-def create_schema(load_order: list[schema.DatabaseItem | list[schema.DatabaseItem]], cursor, exists=False):
-    """
-    Create schema items in a specified load order.
-    """
-    for item_or_group in load_order:
-        if isinstance(item_or_group, list):
-            # For related tables or functions, create them within a single transaction
-            transaction_sql = create_schema_items_in_transaction(item_or_group, exists=exists)
-            cursor.execute(transaction_sql)
-        elif isinstance(item_or_group, (schema.Table, schema.Function)):
-            # For tables and functions, execute the full_sql
-            cursor.execute(item_or_group.full_sql(exists=exists))
-        else:
-            raise ValueError(f"Unsupported type in load_order: {type(item_or_group)}")
-
-
-def create_extensions(extensions: list[str], cursor):
-    """
-    Create extensions in a specified load order.
-    """
-    for extension in extensions:
-        cursor.execute(f'CREATE EXTENSION IF NOT EXISTS "{extension}";')
+from . import schema
+
+
+def create_schema_items_in_transaction(schema_items: list[schema.DatabaseItem], exists=False) -> str:
+    """
+    Create schema items within a single transaction.
+    """
+    sql_parts = ["BEGIN;"]
+
+    # First, create all schema items and add comments
+    for item in schema_items:
+        # Get the SQL parts of each item
+        full_sql_parts = item.full_sql(exists=exists).split("\n\n")
+        # Append only the CREATE TABLE statements (and comments if any)
+        sql_parts.append(full_sql_parts[0])
+        if item.comment:
+            sql_parts.append(full_sql_parts[1])
+
+    # Then, add the ALTER TABLE statements for tables
+    for item in schema_items:
+        if isinstance(item, schema.Table) and item.alter:
+            # Get the SQL parts of each item
+            full_sql_parts = item.full_sql(exists=exists).split("\n\n")
+            # Append only the ALTER TABLE statements
+            if len(full_sql_parts) > 2:
+                sql_parts.append(full_sql_parts[2])
+
+    sql_parts.append("COMMIT;")
+
+    return "\n\n".join(sql_parts)
+
+
+def create_items(load_order: list[schema.DatabaseItem | list[schema.DatabaseItem]], cursor, exists=False):
+    """
+    Create database items in a specified load order.
+    """
+    for item_or_group in load_order:
+        if isinstance(item_or_group, list):
+            # For related tables or functions, create them within a single transaction
+            transaction_sql = create_schema_items_in_transaction(item_or_group, exists=exists)
+            cursor.execute(transaction_sql)
+        elif isinstance(item_or_group, (schema.Schema, schema.Table, schema.Function)):
+            # For tables and functions, execute the full_sql
+            cursor.execute(item_or_group.full_sql(exists=exists))
+        else:
+            raise ValueError(f"Unsupported type in load_order: {type(item_or_group)}")
+
+
+def create_extensions(extensions: list[str], cursor):
+    """
+    Create extensions in a specified load order.
+    """
+    for extension in extensions:
+        cursor.execute(f'CREATE EXTENSION IF NOT EXISTS "{extension}";')
```

### Comparing `postnormalism-0.0.3/postnormalism.egg-info/PKG-INFO` & `postnormalism-0.0.4/postnormalism.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,175 +1,192 @@
-Metadata-Version: 2.1
-Name: postnormalism
-Version: 0.0.3
-Summary: Postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.
-Author-email: Zac Miller <zac@informatical.info>
-Maintainer-email: Zac Miller <zac@informatical.info>
-License: MIT License
-Project-URL: Homepage, https://github.com/jzmiller1/postnormalism
-Project-URL: Bug Tracker, https://github.com/jzmiller1/postnormalism/issues
-Project-URL: Repository, https://github.com/jzmiller1/postnormalism.git
-Project-URL: History, https://github.com/jzmiller1/postnormalism/blob/master/HISTORY.md
-Keywords: python,postgresql,schema
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# postnormalism: PostgreSQL Schema Management  
-  
-postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.  
-  
-## Features  
-  
-- Define tables and functions using Python dataclasses  
-- Create database items (Tables, Functions) with comments
-- Group related database items and create them within a single transaction  
-- Create a Database object that allows loading database items in a specified load order and managing database extensions
-- IF NOT EXISTS mode for loading
-- SQL Migration Loader
-
-  
-## NORM vs. ORM: Features Comparison  
-  
-postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
-  
-Here is a comparison of postnormalism's features with typical ORM characteristics:  
-  
-1. **Object-oriented representation**: postnormalism does not map database tables to classes or table rows to instances. Instead, it uses dataclasses to represent schema items, like tables and functions, for organizing and generating schema items.  
-  
-2. **Abstraction**: postnormalism provides a smidgen of abstraction for creating schema items, but doesn't bother with things like query generation.    
-  
-3. **Query generation**: postnormalism does not include a query builder or DSL for constructing database queries. It focuses on schema management, not query generation.  You are the query generator.
-  
-4. **Transactions and concurrency**: postnormalism kindly allows you to group related schema items and create them within a single transaction. However, it knows when to draw the line and leaves transaction management and concurrency handling for other database operations to more heavyweight solutions.  
-  
-5. **Schema management**: postnormalism excels at schema management by allowing you to excel at schema management. Create schema items and load them in a specified order.  
-  
-6. **Relationships and associations**: postnormalism doesn't get entangled in relationships or associations between tables or objects. After all, it's just a simple library with simple needs.  You have to understand your schema.
-  
-7. **Data validation and constraints**: postnormalism doesn't have time for built-in data validation or constraint enforcement. But fear not, you can still define constraints in your schema items.
-  
-8. **Caching**: postnormalism believes in living in the moment, so caching mechanisms to improve performance are left to others.  
-  
-Should you require a complete ORM solution for your project, consider using a full-fledged ORM like SQLAlchemy or Django's ORM for Python. postnormalism is for those brave souls who seek a lightweight way to manage PostgreSQL schemas without all the bells and whistles.  
-  
-## Installation  
-  
-You can install postnormalism using pip:  
-  
-```sh  
-pip install postnormalism  
-```  
-  
-## Usage  
-  
-### Defining Database Items  
-  
-To define a table or a function, use the `Table` and `Function` dataclasses from the `postnormalism` module:  
-  
-```python  
-from postnormalism.schema import Table, Function  
-```
-  
-### Define a Table
-```python
-from postnormalism.schema import Table
-
-create_table_sql = """  
-CREATE TABLE material (  
-id uuid PRIMARY KEY DEFAULT uuid_generate_v4(),  
-name varchar(120) NOT NULL,  
-description varchar(240)  
-);  
-"""  
-  
-Material = Table(create=create_table_sql)  
-```
-  
-### Define a Postgresql Function  
-```python
-from postnormalism.schema import Function
-
-create_function_sql = """  
-CREATE FUNCTION get_material_for_variant(variant uuid)  
-RETURNS uuid  
-AS $$  
-material_plan = plpy.prepare("SELECT material FROM material_variant WHERE id = $1",  
-["uuid"])  
-material = plpy.execute(material_plan, [variant])[0]["material"]  
-return material  
-$$ LANGUAGE plpython3u;  
-"""  
-  
-comment_function_sql = """  
-COMMENT ON FUNCTION get_material_for_variant IS  
-$$ An example function $$;  
-"""  
-  
-get_material_for_variant = Function(create=create_function_sql, comment=comment_function_sql)  
-```  
-  
-### Creating Database Items in a Database  
-  
-To create database items in a PostgreSQL database, use the `Database` class:  
-  
-```python  
-import psycopg  
-from postnormalism.schema import Database
-from your_example_file import Material, get_material_for_variant
-
-universe = Database(
-    load_order=[
-        Material, get_material_for_variant,
-        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
-    ],
-    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto']
-)
-
-db_connection_string = "dbname=test user=postgres password=secret host=localhost port=port"  
-
-connection = psycopg.connect(db_connection_string)  
-cursor = connection.cursor()  
-
-universe.create(cursor)  
-
-connection.commit()  
-connection.close()  
-```  
-
-### Using exists Mode
-Calling Database.create with exists=True inserts a IF NOT EXISTS into all of your CREATE statements allowing you to easily add new items.
-
-```python
-universe.create(cursor, exists=True)
-```
-
-### Doing migrations
-Update your `DatabaseItem`s and write your SQL migration transaction.  If you create your Database instance with 
-a `migrations_folder` they will run during the create call.  Migration files should ideally be prefixed with a 
-load order (ex: 0001) and must end with `.sql`.
-
-```python
-universe = Database(
-    load_order=[
-        Material, get_material_for_variant,
-        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
-    ],
-    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto'],
-    migrations_folder='/example/folder/path'
-)
-
-```
-
-
-## Contributing  
-  
-Please submit a pull request or create an issue if you have any suggestions or improvements.  
-  
-## License  
-  
-postnormalism is released under the MIT License. See the `LICENSE` file for more information.
+Metadata-Version: 2.1
+Name: postnormalism
+Version: 0.0.4
+Summary: Postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.
+Author-email: Zac Miller <zac@informatical.info>
+Maintainer-email: Zac Miller <zac@informatical.info>
+License: MIT License
+Project-URL: Homepage, https://github.com/jzmiller1/postnormalism
+Project-URL: Bug Tracker, https://github.com/jzmiller1/postnormalism/issues
+Project-URL: Repository, https://github.com/jzmiller1/postnormalism.git
+Project-URL: History, https://github.com/jzmiller1/postnormalism/blob/master/HISTORY.md
+Keywords: python,postgresql,schema
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# postnormalism: PostgreSQL Schema Management  
+  
+postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.  
+  
+## Features  
+  
+- Define schemas, tables and functions using Python dataclasses  
+- Create database items (Schemas, Tables, Functions) with comments
+- Group related database items and create them within a single transaction  
+- Create a Database object that allows loading database items in a specified load order and managing database extensions
+- IF NOT EXISTS mode for loading
+- SQL Migration Loader
+
+  
+## NORM vs. ORM: Features Comparison  
+  
+postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
+  
+Here is a comparison of postnormalism's features with typical ORM characteristics:  
+  
+1. **Object-oriented representation**: postnormalism does not map database tables to classes or table rows to instances. Instead, it uses dataclasses to represent schema items, like tables and functions, for organizing and generating schema items.  
+  
+2. **Abstraction**: postnormalism provides a smidgen of abstraction for creating schema items, but doesn't bother with things like query generation.    
+  
+3. **Query generation**: postnormalism does not include a query builder or DSL for constructing database queries. It focuses on schema management, not query generation.  You are the query generator.
+  
+4. **Transactions and concurrency**: postnormalism kindly allows you to group related schema items and create them within a single transaction. However, it knows when to draw the line and leaves transaction management and concurrency handling for other database operations to more heavyweight solutions.  
+  
+5. **Schema management**: postnormalism excels at schema management by allowing you to excel at schema management. Create schema items and load them in a specified order.  
+  
+6. **Relationships and associations**: postnormalism doesn't get entangled in relationships or associations between tables or objects. After all, it's just a simple library with simple needs.  You have to understand your schema.
+  
+7. **Data validation and constraints**: postnormalism doesn't have time for built-in data validation or constraint enforcement. But fear not, you can still define constraints in your schema items.
+  
+8. **Caching**: postnormalism believes in living in the moment, so caching mechanisms to improve performance are left to others.  
+  
+Should you require a complete ORM solution for your project, consider using a full-fledged ORM like SQLAlchemy or Django's ORM for Python. postnormalism is for those brave souls who seek a lightweight way to manage PostgreSQL schemas without all the bells and whistles.  
+  
+## Installation  
+  
+You can install postnormalism using pip:  
+  
+```sh  
+pip install postnormalism  
+```  
+  
+## Usage  
+  
+### Defining Database Items  
+  
+To define a table or a function, use the `Table` and `Function` dataclasses from the `postnormalism` module:  
+  
+```python  
+from postnormalism.schema import Schema, Table, Function  
+```
+
+### Define a Schema
+```python
+from postnormalism import schema
+
+create = """
+CREATE SCHEMA basic_auth;
+"""
+
+comment = """
+COMMENT ON SCHEMA basic_auth IS
+  $$ The basic auth schema $$;
+"""
+
+basic_auth = schema.Schema(create=create, comment=comment)
+```
+  
+### Define a Table
+```python
+from postnormalism.schema import Table
+
+create_table_sql = """  
+CREATE TABLE material (  
+id uuid PRIMARY KEY DEFAULT uuid_generate_v4(),  
+name varchar(120) NOT NULL,  
+description varchar(240)  
+);  
+"""  
+  
+Material = Table(create=create_table_sql)  
+```
+  
+### Define a Postgresql Function  
+```python
+from postnormalism.schema import Function
+
+create_function_sql = """  
+CREATE FUNCTION get_material_for_variant(variant uuid)  
+RETURNS uuid  
+AS $$  
+material_plan = plpy.prepare("SELECT material FROM material_variant WHERE id = $1",  
+["uuid"])  
+material = plpy.execute(material_plan, [variant])[0]["material"]  
+return material  
+$$ LANGUAGE plpython3u;  
+"""  
+  
+comment_function_sql = """  
+COMMENT ON FUNCTION get_material_for_variant IS  
+$$ An example function $$;  
+"""  
+  
+get_material_for_variant = Function(create=create_function_sql, comment=comment_function_sql)  
+```  
+  
+### Creating Database Items in a Database  
+  
+To create database items in a PostgreSQL database, use the `Database` class:  
+  
+```python  
+import psycopg  
+from postnormalism.schema import Database
+from your_example_file import Material, get_material_for_variant, Player, Inventory, basic_auth
+
+universe = Database(
+    load_order=[
+        basic_auth,
+        Material, get_material_for_variant,
+        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
+    ],
+    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto']
+)
+
+db_connection_string = "dbname=test user=postgres password=secret host=localhost port=port"  
+
+connection = psycopg.connect(db_connection_string)  
+cursor = connection.cursor()  
+
+universe.create(cursor)  
+
+connection.commit()  
+connection.close()  
+```  
+
+### Using exists Mode
+Calling Database.create with exists=True inserts a IF NOT EXISTS into all of your CREATE statements allowing you to easily add new items.
+
+```python
+universe.create(cursor, exists=True)
+```
+
+### Doing migrations
+Update your `DatabaseItem`s and write your SQL migration transaction.  If you create your Database instance with 
+a `migrations_folder` they will run during the create call.  Migration files should ideally be prefixed with a 
+load order (ex: 0001) and must end with `.sql`.
+
+```python
+universe = Database(
+    load_order=[
+        Material, get_material_for_variant,
+        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
+    ],
+    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto'],
+    migrations_folder='/example/folder/path'
+)
+
+```
+
+
+## Contributing  
+  
+Please submit a pull request or create an issue if you have any suggestions or improvements.  
+  
+## License  
+  
+postnormalism is released under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `postnormalism-0.0.3/postnormalism.egg-info/SOURCES.txt` & `postnormalism-0.0.4/postnormalism.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,10 +10,11 @@
 postnormalism.egg-info/dependency_links.txt
 postnormalism.egg-info/top_level.txt
 postnormalism/schema/__init__.py
 postnormalism/schema/database.py
 postnormalism/schema/database_item.py
 postnormalism/schema/function.py
 postnormalism/schema/migrations.py
+postnormalism/schema/schema.py
 postnormalism/schema/table.py
 tests/test_core.py
 tests/test_schema.py
```

### Comparing `postnormalism-0.0.3/pyproject.toml` & `postnormalism-0.0.4/pyproject.toml`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "postnormalism"
-authors = [
-  { name="Zac Miller", email="zac@informatical.info" },
-]
-maintainers = [
-  { name="Zac Miller", email="zac@informatical.info" },
-]
-description = "Postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order."
-readme = "README.md"
-requires-python = ">=3.11"
-license = {text = "MIT License"}
-keywords = ["python", "postgresql", "schema"]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Development Status :: 2 - Pre-Alpha",
-    "Intended Audience :: Developers",
-]
-dynamic = ["version"]
-
-[project.urls]
-"Homepage" = "https://github.com/jzmiller1/postnormalism"
-"Bug Tracker" = "https://github.com/jzmiller1/postnormalism/issues"
-"Repository" = "https://github.com/jzmiller1/postnormalism.git"
-"History" = "https://github.com/jzmiller1/postnormalism/blob/master/HISTORY.md"
-
-
-[tool.setuptools.dynamic]
-version = {file = "postnormalism/VERSION"}
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "postnormalism"
+authors = [
+  { name="Zac Miller", email="zac@informatical.info" },
+]
+maintainers = [
+  { name="Zac Miller", email="zac@informatical.info" },
+]
+description = "Postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order."
+readme = "README.md"
+requires-python = ">=3.11"
+license = {text = "MIT License"}
+keywords = ["python", "postgresql", "schema"]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Development Status :: 2 - Pre-Alpha",
+    "Intended Audience :: Developers",
+]
+dynamic = ["version"]
+
+[project.urls]
+"Homepage" = "https://github.com/jzmiller1/postnormalism"
+"Bug Tracker" = "https://github.com/jzmiller1/postnormalism/issues"
+"Repository" = "https://github.com/jzmiller1/postnormalism.git"
+"History" = "https://github.com/jzmiller1/postnormalism/blob/master/HISTORY.md"
+
+
+[tool.setuptools.dynamic]
+version = {file = "postnormalism/VERSION"}
```

