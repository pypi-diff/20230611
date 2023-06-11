# Comparing `tmp/litesqlite-2.4.0.tar.gz` & `tmp/litesqlite-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesqlite-2.4.0.tar", last modified: Sun Jun 11 18:07:11 2023, max compression
+gzip compressed data, was "litesqlite-2.5.0.tar", last modified: Sun Jun 11 18:14:14 2023, max compression
```

## Comparing `litesqlite-2.4.0.tar` & `litesqlite-2.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 18:07:11.067786 litesqlite-2.4.0/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.4.0/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-11 18:07:11.067786 litesqlite-2.4.0/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.4.0/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 18:07:11.063785 litesqlite-2.4.0/litesqlite/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.4.0/litesqlite/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.4.0/litesqlite/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8628 2023-06-11 18:06:33.000000 litesqlite-2.4.0/litesqlite/lite_sqlite.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 18:07:11.067786 litesqlite-2.4.0/litesqlite.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-11 18:07:10.000000 litesqlite-2.4.0/litesqlite.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-11 18:07:10.000000 litesqlite-2.4.0/litesqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-11 18:07:10.000000 litesqlite-2.4.0/litesqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-11 18:07:10.000000 litesqlite-2.4.0/litesqlite.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-11 18:07:10.000000 litesqlite-2.4.0/litesqlite.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-11 18:07:11.067786 litesqlite-2.4.0/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-11 18:07:03.000000 litesqlite-2.4.0/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 18:14:14.649854 litesqlite-2.5.0/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.5.0/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-11 18:14:14.649854 litesqlite-2.5.0/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.5.0/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 18:14:14.649854 litesqlite-2.5.0/litesqlite/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.5.0/litesqlite/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.5.0/litesqlite/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8652 2023-06-11 18:11:02.000000 litesqlite-2.5.0/litesqlite/lite_sqlite.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 18:14:14.649854 litesqlite-2.5.0/litesqlite.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-11 18:14:14.000000 litesqlite-2.5.0/litesqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-11 18:14:14.000000 litesqlite-2.5.0/litesqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-11 18:14:14.000000 litesqlite-2.5.0/litesqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-11 18:14:14.000000 litesqlite-2.5.0/litesqlite.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-11 18:14:14.000000 litesqlite-2.5.0/litesqlite.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-11 18:14:14.649854 litesqlite-2.5.0/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-11 18:12:38.000000 litesqlite-2.5.0/setup.py
```

### Comparing `litesqlite-2.4.0/LICENSE` & `litesqlite-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litesqlite-2.4.0/PKG-INFO` & `litesqlite-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.4.0
+Version: 2.5.0
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.4.0/README.md` & `litesqlite-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `litesqlite-2.4.0/litesqlite/datatypes.py` & `litesqlite-2.5.0/litesqlite/datatypes.py`

 * *Files identical despite different names*

### Comparing `litesqlite-2.4.0/litesqlite/lite_sqlite.py` & `litesqlite-2.5.0/litesqlite/lite_sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             values = tuple(data.values())
             self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
             self.__conn.commit()
 
     def select_data(self,
                     table_name: str,
                     columns: Union[List[str], str, None] = None,
-                    where: Dict[str, Union[str, int, float], None] = None,
+                    where: Union[str, Dict[str, Union[str, int, float]], None] = None,
                     limit: Union[int, None] = None,
                     offset: Union[int, None] = None,
                     fetch: DataTypes.Fetch = DataTypes.Fetch.FETCHONE) -> Union[Tuple, List[Tuple]]:
         with self:
             if columns:
                 columns = ', '.join(columns)
             else:
@@ -146,15 +146,15 @@
             values = tuple(data.values())
             await self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
             await self.__conn.commit()
 
     async def select_data(self,
                           table_name: str,
                           columns: Union[List[str], None] = None,
-                          where: Dict[str, Union[str, int, float], None] = None,
+                          where: Union[str, Dict[str, Union[str, int, float]], None] = None,
                           limit: Union[int, None] = None,
                           offset: Union[int, None] = None,
                           fetch: DataTypes.Fetch = DataTypes.Fetch.FETCHONE) -> Union[Tuple, List[Tuple]]:
         async with self:
             if columns:
                 columns = ', '.join(columns)
             else:
```

### Comparing `litesqlite-2.4.0/litesqlite.egg-info/PKG-INFO` & `litesqlite-2.5.0/litesqlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.4.0
+Version: 2.5.0
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.4.0/setup.py` & `litesqlite-2.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='litesqlite',
-    version='2.4.0',
+    version='2.5.0',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/FREVOD/litesqlite',
     author='FREVOD',
     author_email='frevod_dev@mail.ru',
     license='GPLv3',
     packages=['litesqlite'],
     install_requires=[
```

