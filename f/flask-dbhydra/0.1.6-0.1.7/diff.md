# Comparing `tmp/flask_dbhydra-0.1.6.tar.gz` & `tmp/flask_dbhydra-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_dbhydra-0.1.6.tar", last modified: Mon Jan  9 03:20:43 2023, max compression
+gzip compressed data, was "flask_dbhydra-0.1.7.tar", last modified: Sat Jun 10 23:25:38 2023, max compression
```

## Comparing `flask_dbhydra-0.1.6.tar` & `flask_dbhydra-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-01-09 03:20:43.460702 flask_dbhydra-0.1.6/
--rw-rw-rw-   0        0        0     1090 2021-09-30 15:20:39.000000 flask_dbhydra-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     2131 2023-01-09 03:20:43.459704 flask_dbhydra-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1629 2021-10-01 01:50:41.000000 flask_dbhydra-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-01-09 03:20:43.444746 flask_dbhydra-0.1.6/flask_dbhydra/
--rw-rw-rw-   0        0        0        0 2021-09-30 15:19:40.000000 flask_dbhydra-0.1.6/flask_dbhydra/__init__.py
--rw-rw-rw-   0        0        0     6368 2023-01-09 03:19:49.000000 flask_dbhydra-0.1.6/flask_dbhydra/flask_dbhydra_core.py
-drwxrwxrwx   0        0        0        0 2023-01-09 03:20:43.459704 flask_dbhydra-0.1.6/flask_dbhydra.egg-info/
--rw-rw-rw-   0        0        0     2131 2023-01-09 03:20:42.000000 flask_dbhydra-0.1.6/flask_dbhydra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-01-09 03:20:43.000000 flask_dbhydra-0.1.6/flask_dbhydra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-09 03:20:42.000000 flask_dbhydra-0.1.6/flask_dbhydra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-01-09 03:20:43.000000 flask_dbhydra-0.1.6/flask_dbhydra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-01-09 03:20:43.000000 flask_dbhydra-0.1.6/flask_dbhydra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-09 03:20:43.460702 flask_dbhydra-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      759 2023-01-09 03:20:40.000000 flask_dbhydra-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:25:38.148793 flask_dbhydra-0.1.7/
+-rw-rw-rw-   0        0        0     1090 2021-09-30 15:20:39.000000 flask_dbhydra-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     2131 2023-06-10 23:25:38.147796 flask_dbhydra-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1629 2021-10-01 01:50:41.000000 flask_dbhydra-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 23:25:38.124858 flask_dbhydra-0.1.7/flask_dbhydra/
+-rw-rw-rw-   0        0        0        0 2021-09-30 15:19:40.000000 flask_dbhydra-0.1.7/flask_dbhydra/__init__.py
+-rw-rw-rw-   0        0        0     6328 2023-06-10 23:24:40.000000 flask_dbhydra-0.1.7/flask_dbhydra/flask_dbhydra_core.py
+drwxrwxrwx   0        0        0        0 2023-06-10 23:25:38.146799 flask_dbhydra-0.1.7/flask_dbhydra.egg-info/
+-rw-rw-rw-   0        0        0     2131 2023-06-10 23:25:37.000000 flask_dbhydra-0.1.7/flask_dbhydra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-10 23:25:38.000000 flask_dbhydra-0.1.7/flask_dbhydra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 23:25:37.000000 flask_dbhydra-0.1.7/flask_dbhydra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-10 23:25:37.000000 flask_dbhydra-0.1.7/flask_dbhydra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-10 23:25:37.000000 flask_dbhydra-0.1.7/flask_dbhydra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 23:25:38.148793 flask_dbhydra-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      759 2023-06-10 23:25:34.000000 flask_dbhydra-0.1.7/setup.py
```

### Comparing `flask_dbhydra-0.1.6/LICENSE` & `flask_dbhydra-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_dbhydra-0.1.6/PKG-INFO` & `flask_dbhydra-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_dbhydra
-Version: 0.1.6
+Version: 0.1.7
 Summary: Autogenerate Flask API for dbhydra ORM DB structure
 Home-page: https://github.com/DovaX/flask_dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flask_dbhydra-0.1.6/README.md` & `flask_dbhydra-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `flask_dbhydra-0.1.6/flask_dbhydra/flask_dbhydra_core.py` & `flask_dbhydra-0.1.7/flask_dbhydra/flask_dbhydra_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             item=k[:-1]    
             @app.route('/api/'+item+'/register', methods=['POST'])
             @rename_function('register_'+item)
             def register(k=k): #k=k because of late binding - otherwise, it would assign all endpoints with the same k
                 cur = mysql.connection.cursor()
                 email = request.get_json(force=True)['email']
                 #req_pass=request.get_json(force=True)['password']
-                password = bcrypt.generate_password_hash(request.get_json()['password']).decode('utf-8')
+                password = bcrypt.generate_password_hash(request.get_json(force=True)['password']).decode('utf-8')
                 creation_utc_time = datetime.utcnow()
             	
                 cur.execute("INSERT INTO "+k+" (email, password, creation_utc_time) VALUES ('" + 
             		str(email) + "', '" + 
             		str(password) + "', '" + 
             		str(creation_utc_time) + "')")
                 mysql.connection.commit()
@@ -104,15 +104,14 @@
       
         if 'login' in v:
             item=k[:-1]    
             @app.route('/api/'+item+'/login', methods=['POST'])
             @rename_function('login_'+item)
             def login(k=k): #k=k because of late binding - otherwise, it would assign all endpoints with the same k
                 cur = mysql.connection.cursor()
-                print("TEST",request.get_json())
                 email = request.get_json(force=True)['email']
                 password = request.get_json(force=True)['password']
                 result = ""
             	
                 cur.execute("SELECT * FROM "+k+" where email = '" + str(email) + "'")
                 rv = cur.fetchone()
                 print("RV",rv)
```

### Comparing `flask_dbhydra-0.1.6/flask_dbhydra.egg-info/PKG-INFO` & `flask_dbhydra-0.1.7/flask_dbhydra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-dbhydra
-Version: 0.1.6
+Version: 0.1.7
 Summary: Autogenerate Flask API for dbhydra ORM DB structure
 Home-page: https://github.com/DovaX/flask_dbhydra
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flask_dbhydra-0.1.6/setup.py` & `flask_dbhydra-0.1.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='flask_dbhydra',
-    version='0.1.6',
+    version='0.1.7',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Autogenerate Flask API for dbhydra ORM DB structure',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/flask_dbhydra',
     packages=setuptools.find_packages(),
```

