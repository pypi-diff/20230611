# Comparing `tmp/stripe_api_client-0.1.1.tar.gz` & `tmp/stripe_api_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stripe_api_client-0.1.1.tar", max compression
+gzip compressed data, was "stripe_api_client-0.1.2.tar", max compression
```

## Comparing `stripe_api_client-0.1.1.tar` & `stripe_api_client-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0        0 2023-06-07 10:16:48.295067 stripe_api_client-0.1.1/README.md
--rw-r--r--   0        0        0      343 2023-06-07 12:03:49.532384 stripe_api_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       26 2023-06-07 10:30:36.351871 stripe_api_client-0.1.1/stripe_api_client/__init__.py
--rw-r--r--   0        0        0     1345 2023-06-07 10:57:31.456854 stripe_api_client-0.1.1/stripe_api_client/client.py
--rw-r--r--   0        0        0      117 2023-06-07 10:55:06.849167 stripe_api_client-0.1.1/stripe_api_client/resources/__init__.py
--rw-r--r--   0        0        0     1412 2023-06-07 10:39:02.667985 stripe_api_client-0.1.1/stripe_api_client/resources/base.py
--rw-r--r--   0        0        0      538 2023-06-07 10:43:23.129565 stripe_api_client-0.1.1/stripe_api_client/resources/charges.py
--rw-r--r--   0        0        0     1093 2023-06-07 10:52:35.422836 stripe_api_client-0.1.1/stripe_api_client/resources/customers.py
--rw-r--r--   0        0        0      589 2023-06-07 10:50:26.654229 stripe_api_client-0.1.1/stripe_api_client/resources/payment_methods.py
--rw-r--r--   0        0        0      255 2023-06-07 10:20:06.632274 stripe_api_client-0.1.1/stripe_api_client/utils.py
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 stripe_api_client-0.1.1/setup.py
--rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 stripe_api_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-07 10:16:48.295067 stripe_api_client-0.1.2/README.md
+-rw-r--r--   0        0        0      343 2023-06-11 12:25:38.121181 stripe_api_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-06-07 10:30:36.351871 stripe_api_client-0.1.2/stripe_api_client/__init__.py
+-rw-r--r--   0        0        0     2054 2023-06-09 12:54:09.952976 stripe_api_client-0.1.2/stripe_api_client/client.py
+-rw-r--r--   0        0        0      266 2023-06-09 12:12:59.578367 stripe_api_client-0.1.2/stripe_api_client/resources/__init__.py
+-rw-r--r--   0        0        0     1412 2023-06-07 10:39:02.667985 stripe_api_client-0.1.2/stripe_api_client/resources/base.py
+-rw-r--r--   0        0        0      538 2023-06-07 10:43:23.129565 stripe_api_client-0.1.2/stripe_api_client/resources/charges.py
+-rw-r--r--   0        0        0     1093 2023-06-07 10:52:35.422836 stripe_api_client-0.1.2/stripe_api_client/resources/customers.py
+-rw-r--r--   0        0        0     1728 2023-06-09 12:10:34.150731 stripe_api_client-0.1.2/stripe_api_client/resources/invoices.py
+-rw-r--r--   0        0        0     1158 2023-06-09 11:55:29.570309 stripe_api_client-0.1.2/stripe_api_client/resources/payment_intents.py
+-rw-r--r--   0        0        0      589 2023-06-07 10:50:26.654229 stripe_api_client-0.1.2/stripe_api_client/resources/payment_methods.py
+-rw-r--r--   0        0        0      570 2023-06-09 12:12:50.834821 stripe_api_client-0.1.2/stripe_api_client/resources/subscriptions.py
+-rw-r--r--   0        0        0      255 2023-06-07 10:20:06.632274 stripe_api_client-0.1.2/stripe_api_client/utils.py
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 stripe_api_client-0.1.2/setup.py
+-rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 stripe_api_client-0.1.2/PKG-INFO
```

### Comparing `stripe_api_client-0.1.1/stripe_api_client/client.py` & `stripe_api_client-0.1.2/stripe_api_client/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,14 +26,23 @@
             ),
             'charges': resources.ChargesPool(
                 urljoin(self._base_url, 'charges'), self._session
             ),
             'payment_methods': resources.PaymentMethodsPool(
                 urljoin(self._base_url, 'payment_methods'), self._session
             ),
+            'payment_intents': resources.PaymentIntentsPool(
+                urljoin(self._base_url, 'payment_intents'), self._session
+            ),
+            'invoices': resources.InvoicesPool(
+                urljoin(self._base_url, 'invoices'), self._session
+            ),
+            'subscriptions': resources.SubscriptionsPool(
+                urljoin(self._base_url, 'subscriptions'), self._session
+            )
         }
 
 
     @property
     def resources(self):
         return self._resources
     
@@ -44,8 +53,19 @@
     @property
     def charges(self):
         return self._resources['charges']
 
     @property
     def payment_methods(self):
         return self._resources['payment_methods']        
+
+    @property
+    def payment_intents(self):
+        return self._resources['payment_intents']   
     
+    @property
+    def invoices(self):
+        return self._resources['invoices']  
+
+    @property
+    def subscriptions(self):
+        return self._resources['subscriptions']
```

### Comparing `stripe_api_client-0.1.1/stripe_api_client/resources/base.py` & `stripe_api_client-0.1.2/stripe_api_client/resources/base.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.1/stripe_api_client/resources/charges.py` & `stripe_api_client-0.1.2/stripe_api_client/resources/charges.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.1/stripe_api_client/resources/customers.py` & `stripe_api_client-0.1.2/stripe_api_client/resources/customers.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.1/stripe_api_client/resources/payment_methods.py` & `stripe_api_client-0.1.2/stripe_api_client/resources/payment_methods.py`

 * *Files identical despite different names*

### Comparing `stripe_api_client-0.1.1/setup.py` & `stripe_api_client-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'stripe-api-client',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': '',
     'author': 'Steven Athouel',
     'author_email': 'sathouel@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

