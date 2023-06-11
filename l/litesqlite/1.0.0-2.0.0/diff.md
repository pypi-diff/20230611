# Comparing `tmp/litesqlite-1.0.0.tar.gz` & `tmp/litesqlite-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesqlite-1.0.0.tar", last modified: Sat Jun 10 21:23:09 2023, max compression
+gzip compressed data, was "litesqlite-2.0.0.tar", last modified: Sun Jun 11 15:27:49 2023, max compression
```

## Comparing `litesqlite-1.0.0.tar` & `litesqlite-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 21:23:09.128800 litesqlite-1.0.0/
--rw-rw-rw-   0        0        0    35149 2023-06-10 20:40:52.000000 litesqlite-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      593 2023-06-10 21:23:09.126799 litesqlite-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3028 2023-06-10 20:40:52.000000 litesqlite-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 21:23:09.004801 litesqlite-1.0.0/litesqlite/
--rw-rw-rw-   0        0        0      100 2023-06-10 21:17:16.000000 litesqlite-1.0.0/litesqlite/__init__.py
--rw-rw-rw-   0        0        0     4248 2023-06-10 19:18:49.000000 litesqlite-1.0.0/litesqlite/datatypes.py
--rw-rw-rw-   0        0        0     7944 2023-06-10 19:24:44.000000 litesqlite-1.0.0/litesqlite/lite_sqlite.py
-drwxrwxrwx   0        0        0        0 2023-06-10 21:23:09.124804 litesqlite-1.0.0/litesqlite.egg-info/
--rw-rw-rw-   0        0        0      593 2023-06-10 21:23:08.000000 litesqlite-1.0.0/litesqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-06-10 21:23:08.000000 litesqlite-1.0.0/litesqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 21:23:08.000000 litesqlite-1.0.0/litesqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-10 21:23:08.000000 litesqlite-1.0.0/litesqlite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-10 21:23:08.000000 litesqlite-1.0.0/litesqlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 21:23:09.129799 litesqlite-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      729 2023-06-10 21:22:52.000000 litesqlite-1.0.0/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 15:27:49.868689 litesqlite-2.0.0/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.0.0/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-11 15:27:49.868689 litesqlite-2.0.0/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.0.0/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 15:27:49.864689 litesqlite-2.0.0/litesqlite/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.0.0/litesqlite/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4363 2023-06-11 15:26:19.000000 litesqlite-2.0.0/litesqlite/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8624 2023-06-11 15:26:19.000000 litesqlite-2.0.0/litesqlite/lite_sqlite.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 15:27:49.868689 litesqlite-2.0.0/litesqlite.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-11 15:27:49.000000 litesqlite-2.0.0/litesqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-11 15:27:49.000000 litesqlite-2.0.0/litesqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-11 15:27:49.000000 litesqlite-2.0.0/litesqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-11 15:27:49.000000 litesqlite-2.0.0/litesqlite.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-11 15:27:49.000000 litesqlite-2.0.0/litesqlite.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-11 15:27:49.868689 litesqlite-2.0.0/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-11 15:26:19.000000 litesqlite-2.0.0/setup.py
```

### Comparing `litesqlite-1.0.0/LICENSE` & `litesqlite-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litesqlite-1.0.0/README.md` & `litesqlite-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `litesqlite-1.0.0/litesqlite/datatypes.py` & `litesqlite-2.0.0/litesqlite/datatypes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from typing import Union
 
 
 class DataTypes:
 
+    class Fetch:
+        FETCHONE = 'fetchone'
+        FETCHALL = 'fetchall'
+        FETCHMANY = 'fetchmany'
+
     class Collation:
         BINARY = 'BINARY'
         NOCASE = 'NOCASE'
         RTRIM = 'RTRIM'
         UTF16 = 'UTF16'
         UTF16CI = 'UTF16CI'
```

### Comparing `litesqlite-1.0.0/litesqlite/lite_sqlite.py` & `litesqlite-2.0.0/litesqlite/lite_sqlite.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,203 +1,209 @@
 import aiosqlite
 import sqlite3
 from typing import Dict, Union, Tuple, List
-from .datatypes import DataTypes
+from datatypes import DataTypes
 
 
 class Sqlite:
 
     def __init__(self,
                  db_name: str) -> None:
         self.__db_name = db_name
         self.__conn = None
         self.__cursor = None
 
-    def __init2(self) -> None:
+    def open_conn(self) -> None:
         self.__conn = sqlite3.connect(self.__db_name)
         self.__cursor = self.__conn.cursor()
 
+    def __enter__(self) -> 'Sqlite':
+        self.open_conn()
+        return self
+
     def create_table(self,
                      table_name: str,
                      columns: Dict[str, Union[DataTypes, str]]) -> None:
-        self.__init2()
-        columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
-        self.__cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})")
-        self.__conn.commit()
-        self.__close_conn()
+        with self:
+            columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
+            self.__cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})")
+            self.__conn.commit()
 
     def insert_data(self,
                     table_name: str,
                     data: Dict[str, Union[str, int, float]]) -> None:
-        self.__init2()
-        columns = ', '.join(data.keys())
-        placeholders = ', '.join(['?' for _ in range(len(data))])
-        values = tuple(data.values())
-        self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
-        self.__conn.commit()
-        self.__close_conn()
+        with self:
+            columns = ', '.join(data.keys())
+            placeholders = ', '.join(['?' for _ in range(len(data))])
+            values = tuple(data.values())
+            self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
+            self.__conn.commit()
 
     def select_data(self,
                     table_name: str,
                     columns: Union[List[str], None] = None,
                     where: Union[Dict[str, Union[str, int, float]], None] = None,
                     limit: Union[int, None] = None,
                     offset: Union[int, None] = None,
-                    fetchall: bool = False) -> Union[Tuple, List[Tuple]]:
-        self.__init2()
-        if columns:
-            columns = ', '.join(columns)
-        else:
-            columns = '*'
-        if where:
-            where_clause = 'WHERE ' + ' AND '.join([f'{col}=?' for col in where.keys()])
-            values = tuple(where.values())
-        else:
-            where_clause = ''
-            values = ()
-        if limit:
-            limit_clause = f"LIMIT {limit}"
-        else:
-            limit_clause = ""
-        if offset:
-            offset_clause = f'OFFSET {offset}'
-        else:
-            offset_clause = ""
-        self.__cursor.execute(f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}",
-                            values)
-
-        if fetchall:
-            result = self.__cursor.fetchall()
-        else:
-            result = self.__cursor.fetchone()
-        self.__close_conn()
-        return result
+                    fetch: DataTypes.Fetch = DataTypes.Fetch.FETCHONE) -> Union[Tuple, List[Tuple]]:
+        with self:
+            if columns:
+                columns = ', '.join(columns)
+            else:
+                columns = '*'
+            if where:
+                where_clause = 'WHERE ' + ' AND '.join([f'{col}=?' for col in where.keys()])
+                values = tuple(where.values())
+            else:
+                where_clause = ''
+                values = ()
+            if limit:
+                limit_clause = f"LIMIT {limit}"
+            else:
+                limit_clause = ""
+            if offset:
+                offset_clause = f'OFFSET {offset}'
+            else:
+                offset_clause = ""
+            self.__cursor.execute(f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}",
+                                  values)
+
+            if fetch == DataTypes.Fetch.FETCHONE:
+                result = self.__cursor.fetchone()
+            elif fetch == DataTypes.Fetch.FETCHALL:
+                result = self.__cursor.fetchall()
+            elif fetch == DataTypes.Fetch.FETCHMANY:
+                result = self.__cursor.fetchmany()
+            return result
 
     def update_data(self,
                     table_name: str,
                     set_data: Dict[str, Union[str, int, float]],
                     where: Dict[str, Union[str, int, float]],
                     sign: Union[str, None] = None) -> None:
-        self.__init2()
-        if sign:
-            set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
-        else:
-            set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
-        where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
-        values = tuple(set_data.values()) + tuple(where.values())
-        self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
-        self.__conn.commit()
-        self.__close_conn()
+        with self:
+            if sign:
+                set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
+            else:
+                set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
+            where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
+            values = tuple(set_data.values()) + tuple(where.values())
+            self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
+            self.__conn.commit()
 
     def delete_data(self,
                     table_name: str,
                     where: Dict[str, Union[str, int, float]]) -> None:
-        self.__init2()
-        where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
-        values = tuple(where.values())
-        self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
-        self.__conn.commit()
-        self.__close_conn()
+        with self:
+            where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
+            values = tuple(where.values())
+            self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
+            self.__conn.commit()
 
-    def __close_conn(self) -> None:
-        self.__init2()
+    def close_conn(self) -> None:
         self.__conn.close()
 
+    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+        self.close_conn()
+
 
 class AioSqlite:
 
     def __init__(self,
                  db_name: str) -> None:
         self.__db_name = db_name
         self.__conn = None
         self.__cursor = None
 
-    async def __init2(self) -> None:
+    async def open_conn(self) -> None:
         self.__conn = await aiosqlite.connect(self.__db_name)
         self.__cursor = await self.__conn.cursor()
 
+    async def __aenter__(self) -> 'AioSqlite':
+        await self.open_conn()
+        return self
+
     async def create_table(self,
                            table_name: str,
                            columns: Dict[str, Union[DataTypes, str]]) -> None:
-        await self.__init2()
-        columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
-        await self.__cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})")
-        await self.__conn.commit()
-        await self.__close_conn()
+        async with self:
+            columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
+            await self.__cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})")
+            await self.__conn.commit()
 
     async def insert_data(self,
                           table_name: str,
                           data: Dict[str, Union[str, int, float]]) -> None:
-        await self.__init2()
-        columns = ', '.join(data.keys())
-        placeholders = ', '.join(['?' for _ in range(len(data))])
-        values = tuple(data.values())
-        await self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
-        await self.__conn.commit()
-        await self.__close_conn()
+        async with self:
+            columns = ', '.join(data.keys())
+            placeholders = ', '.join(['?' for _ in range(len(data))])
+            values = tuple(data.values())
+            await self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
+            await self.__conn.commit()
 
     async def select_data(self,
                           table_name: str,
                           columns: Union[List[str], None] = None,
                           where: Union[Dict[str, Union[str, int, float]], None] = None,
                           limit: Union[int, None] = None,
                           offset: Union[int, None] = None,
-                          fetchall: bool = False) -> Union[Tuple, List[Tuple]]:
-        await self.__init2()
-        if columns:
-            columns = ', '.join(columns)
-        else:
-            columns = '*'
-        if where:
-            where_clause = 'WHERE ' + ' AND '.join([f'{col}=?' for col in where.keys()])
-            values = tuple(where.values())
-        else:
-            where_clause = ''
-            values = ()
-        if limit:
-            limit_clause = f"LIMIT {limit}"
-        else:
-            limit_clause = ""
-        if offset:
-            offset_clause = f'OFFSET {offset}'
-        else:
-            offset_clause = ""
-        await self.__cursor.execute(f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}",
-                                  values)
-
-        if fetchall:
-            result = await self.__cursor.fetchall()
-        else:
-            result = await self.__cursor.fetchone()
-        await self.__close_conn()
-        return result
+                          fetch: DataTypes.Fetch = DataTypes.Fetch.FETCHONE) -> Union[Tuple, List[Tuple]]:
+        async with self:
+            if columns:
+                columns = ', '.join(columns)
+            else:
+                columns = '*'
+            if where:
+                where_clause = 'WHERE ' + ' AND '.join([f'{col}=?' for col in where.keys()])
+                values = tuple(where.values())
+            else:
+                where_clause = ''
+                values = ()
+            if limit:
+                limit_clause = f"LIMIT {limit}"
+            else:
+                limit_clause = ""
+            if offset:
+                offset_clause = f'OFFSET {offset}'
+            else:
+                offset_clause = ""
+            await self.__cursor.execute(f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}",
+                                        values)
+
+            if fetch == DataTypes.Fetch.FETCHONE:
+                result = self.__cursor.fetchone()
+            elif fetch == DataTypes.Fetch.FETCHALL:
+                result = self.__cursor.fetchall()
+            elif fetch == DataTypes.Fetch.FETCHMANY:
+                result = self.__cursor.fetchmany()
+            return result
 
     async def update_data(self,
                           table_name: str,
                           set_data: Dict[str, Union[str, int, float]],
                           where: Dict[str, Union[str, int, float]],
                           sign: Union[str, None] = None) -> None:
-        await self.__init2()
-        if sign:
-            set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
-        else:
-            set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
-        where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
-        values = tuple(set_data.values()) + tuple(where.values())
-        await self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
-        await self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
-        await self.__conn.commit()
-        await self.__close_conn()
+        with self:
+            if sign:
+                set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
+            else:
+                set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
+            where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
+            values = tuple(set_data.values()) + tuple(where.values())
+            await self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
+            await self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
+            await self.__conn.commit()
 
     async def delete_data(self,
                           table_name: str,
                           where: Dict[str, Union[str, int, float]]) -> None:
-        await self.__init2()
-        where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
-        values = tuple(where.values())
-        await self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
-        await self.__conn.commit()
-        await self.__close_conn()
+        with self:
+            where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
+            values = tuple(where.values())
+            await self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
+            await self.__conn.commit()
 
-    async def __close_conn(self) -> None:
-        await self.__init2()
+    async def close_conn(self) -> None:
         await self.__conn.close()
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self.close_conn()
```

### Comparing `litesqlite-1.0.0/setup.py` & `litesqlite-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='litesqlite',
-    version='1.0.0',
+    version='2.0.0',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/FREVOD/litesqlite',
     author='FREVOD',
     author_email='frevod_dev@mail.ru',
     license='GPLv3',
     packages=['litesqlite'],
     install_requires=[
@@ -15,10 +15,11 @@
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ]
 )
```

