# Comparing `tmp/coinbase-commerce-API-1.0.1.tar.gz` & `tmp/coinbase-commerce-API-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinbase-commerce-API-1.0.1.tar", last modified: Mon Jun  5 15:50:45 2023, max compression
+gzip compressed data, was "coinbase-commerce-API-1.0.2.tar", last modified: Sun Jun 11 07:59:23 2023, max compression
```

## Comparing `coinbase-commerce-API-1.0.1.tar` & `coinbase-commerce-API-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-06-05 15:50:45.870901 coinbase-commerce-API-1.0.1/
--rw-r--r--   0 macbookair   (501) staff       (20)      723 2023-06-05 15:50:45.870779 coinbase-commerce-API-1.0.1/PKG-INFO
-drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-06-05 15:50:45.869826 coinbase-commerce-API-1.0.1/cbc_api/
--rw-r--r--   0 macbookair   (501) staff       (20)       43 2023-06-03 12:28:35.000000 coinbase-commerce-API-1.0.1/cbc_api/ __init__.py
--rw-r--r--   0 macbookair   (501) staff       (20)     5233 2023-06-05 15:46:52.000000 coinbase-commerce-API-1.0.1/cbc_api/cbc_api.py
-drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-06-05 15:50:45.870581 coinbase-commerce-API-1.0.1/coinbase_commerce_API.egg-info/
--rw-r--r--   0 macbookair   (501) staff       (20)      723 2023-06-05 15:50:45.000000 coinbase-commerce-API-1.0.1/coinbase_commerce_API.egg-info/PKG-INFO
--rw-r--r--   0 macbookair   (501) staff       (20)      272 2023-06-05 15:50:45.000000 coinbase-commerce-API-1.0.1/coinbase_commerce_API.egg-info/SOURCES.txt
--rw-r--r--   0 macbookair   (501) staff       (20)        1 2023-06-05 15:50:45.000000 coinbase-commerce-API-1.0.1/coinbase_commerce_API.egg-info/dependency_links.txt
--rw-r--r--   0 macbookair   (501) staff       (20)        9 2023-06-05 15:50:45.000000 coinbase-commerce-API-1.0.1/coinbase_commerce_API.egg-info/requires.txt
--rw-r--r--   0 macbookair   (501) staff       (20)        8 2023-06-05 15:50:45.000000 coinbase-commerce-API-1.0.1/coinbase_commerce_API.egg-info/top_level.txt
--rw-r--r--   0 macbookair   (501) staff       (20)       38 2023-06-05 15:50:45.870943 coinbase-commerce-API-1.0.1/setup.cfg
--rw-r--r--   0 macbookair   (501) staff       (20)      865 2023-06-05 15:47:39.000000 coinbase-commerce-API-1.0.1/setup.py
+drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-06-11 07:59:23.204372 coinbase-commerce-API-1.0.2/
+-rw-r--r--   0 macbookair   (501) staff       (20)      825 2023-06-11 07:59:23.204187 coinbase-commerce-API-1.0.2/PKG-INFO
+drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-06-11 07:59:23.203308 coinbase-commerce-API-1.0.2/cbc_api/
+-rw-r--r--   0 macbookair   (501) staff       (20)       43 2023-06-03 12:28:35.000000 coinbase-commerce-API-1.0.2/cbc_api/ __init__.py
+-rw-r--r--   0 macbookair   (501) staff       (20)     5469 2023-06-11 07:49:23.000000 coinbase-commerce-API-1.0.2/cbc_api/cbc_api.py
+drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-06-11 07:59:23.203976 coinbase-commerce-API-1.0.2/coinbase_commerce_API.egg-info/
+-rw-r--r--   0 macbookair   (501) staff       (20)      825 2023-06-11 07:59:23.000000 coinbase-commerce-API-1.0.2/coinbase_commerce_API.egg-info/PKG-INFO
+-rw-r--r--   0 macbookair   (501) staff       (20)      272 2023-06-11 07:59:23.000000 coinbase-commerce-API-1.0.2/coinbase_commerce_API.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookair   (501) staff       (20)        1 2023-06-11 07:59:23.000000 coinbase-commerce-API-1.0.2/coinbase_commerce_API.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookair   (501) staff       (20)        9 2023-06-11 07:59:23.000000 coinbase-commerce-API-1.0.2/coinbase_commerce_API.egg-info/requires.txt
+-rw-r--r--   0 macbookair   (501) staff       (20)        8 2023-06-11 07:59:23.000000 coinbase-commerce-API-1.0.2/coinbase_commerce_API.egg-info/top_level.txt
+-rw-r--r--   0 macbookair   (501) staff       (20)       38 2023-06-11 07:59:23.204427 coinbase-commerce-API-1.0.2/setup.cfg
+-rw-r--r--   0 macbookair   (501) staff       (20)      967 2023-06-11 07:54:09.000000 coinbase-commerce-API-1.0.2/setup.py
```

### Comparing `coinbase-commerce-API-1.0.1/cbc_api/cbc_api.py` & `coinbase-commerce-API-1.0.2/cbc_api/cbc_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,25 +10,29 @@
             'X-CC-Api-Key': token
         }
 
     def charge_list(self):
         response = requests.get('https://api.commerce.coinbase.com/charges', headers=self.headers).json()
         return response
 
-    def create_charge(self, name, description=None, pricing_type='no_price', amount=None, currency='USD'):
+    def create_charge(self, name, description=None, pricing_type='no_price', amount=None, currency='USD', customer_id=None, customer_name=None):
         data = {'name': name, 'pricing_type': pricing_type}
         if description is not None:
             data['description'] = {'description': description}
         if pricing_type == 'fixed_price':
             if amount is None:
                 raise ValueError("Amount is required for fixed pricing")
             data['local_price'] = {
                 'amount': str(amount),
                 'currency': currency
             }
+        if customer_id is not None:
+            data['metadata'] = {'customer_id': customer_id}
+        if customer_name is not None:
+            data['metadata'] = {'customer_name': customer_name}
         response = requests.post('https://api.commerce.coinbase.com/charges', headers=self.headers, json=data).json()
         return response
 
     def charge_show(self, charge_code):
         response = requests.get(f'https://api.commerce.coinbase.com/charges/{charge_code}', headers=self.headers).json()
         return response
```

### Comparing `coinbase-commerce-API-1.0.1/setup.py` & `coinbase-commerce-API-1.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name='coinbase-commerce-API',
-    version='1.0.1',
+    version='1.0.2',
     author='Rushifakami',
-    description='Coinbase Commerce API library. See github.',
+    description='Unofficial Coinbase Commerce API library. See github for explanations and examples: https://github.com/Rushifakami/API-Coinbase-Commerce-cbc_api',
     packages=['cbc_api'],
     install_requires=[
         'requests',
     ],
     url='https://github.com/Rushifakami/API-Coinbase-Commerce-cbc_api',
     license='MIT',
     classifiers=[
```

