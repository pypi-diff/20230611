# Comparing `tmp/basicqiwip2p-0.0.2.tar.gz` & `tmp/basicqiwip2p-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicqiwip2p-0.0.2.tar", last modified: Wed Jun  7 20:44:35 2023, max compression
+gzip compressed data, was "basicqiwip2p-0.0.3.tar", last modified: Sun Jun 11 14:11:39 2023, max compression
```

## Comparing `basicqiwip2p-0.0.2.tar` & `basicqiwip2p-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 20:44:35.234386 basicqiwip2p-0.0.2/
--rw-rw-rw-   0        0        0      194 2023-06-07 20:44:35.235782 basicqiwip2p-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-07 20:00:29.000000 basicqiwip2p-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 20:44:35.191832 basicqiwip2p-0.0.2/basicqiwip2p/
--rw-rw-rw-   0        0        0      159 2023-06-07 20:43:26.000000 basicqiwip2p-0.0.2/basicqiwip2p/__init__.py
--rw-rw-rw-   0        0        0     1880 2023-06-07 20:31:15.000000 basicqiwip2p-0.0.2/basicqiwip2p/aiobasicqiwip2p.py
--rw-rw-rw-   0        0        0     1814 2023-06-07 20:21:24.000000 basicqiwip2p-0.0.2/basicqiwip2p/basicqiwip2p.py
-drwxrwxrwx   0        0        0        0 2023-06-07 20:44:35.232164 basicqiwip2p-0.0.2/basicqiwip2p.egg-info/
--rw-rw-rw-   0        0        0      194 2023-06-07 20:44:34.000000 basicqiwip2p-0.0.2/basicqiwip2p.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-06-07 20:44:34.000000 basicqiwip2p-0.0.2/basicqiwip2p.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 20:44:34.000000 basicqiwip2p-0.0.2/basicqiwip2p.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-07 20:39:38.000000 basicqiwip2p-0.0.2/basicqiwip2p.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-07 20:44:34.000000 basicqiwip2p-0.0.2/basicqiwip2p.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 20:44:35.250935 basicqiwip2p-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      339 2023-06-07 20:44:15.000000 basicqiwip2p-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:11:39.901426 basicqiwip2p-0.0.3/
+-rw-rw-rw-   0        0        0      194 2023-06-11 14:11:39.901426 basicqiwip2p-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1018 2023-06-08 09:08:20.000000 basicqiwip2p-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 14:11:39.869790 basicqiwip2p-0.0.3/basicqiwip2p/
+-rw-rw-rw-   0        0        0      159 2023-06-07 20:51:49.000000 basicqiwip2p-0.0.3/basicqiwip2p/__init__.py
+-rw-rw-rw-   0        0        0     2058 2023-06-11 14:05:39.000000 basicqiwip2p-0.0.3/basicqiwip2p/aiobasicqiwip2p.py
+-rw-rw-rw-   0        0        0     1991 2023-06-11 13:45:26.000000 basicqiwip2p-0.0.3/basicqiwip2p/basicqiwip2p.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:11:39.897541 basicqiwip2p-0.0.3/basicqiwip2p.egg-info/
+-rw-rw-rw-   0        0        0      194 2023-06-11 14:11:39.000000 basicqiwip2p-0.0.3/basicqiwip2p.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-11 14:11:39.000000 basicqiwip2p-0.0.3/basicqiwip2p.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 14:11:39.000000 basicqiwip2p-0.0.3/basicqiwip2p.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-11 14:11:39.000000 basicqiwip2p-0.0.3/basicqiwip2p.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-11 14:11:39.000000 basicqiwip2p-0.0.3/basicqiwip2p.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 14:11:39.905172 basicqiwip2p-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      351 2023-06-11 13:17:35.000000 basicqiwip2p-0.0.3/setup.py
```

### Comparing `basicqiwip2p-0.0.2/basicqiwip2p/basicqiwip2p.py` & `basicqiwip2p-0.0.3/basicqiwip2p/basicqiwip2p.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from httpx import Client
+from basicqiwip2p.models import Response
 
 import datetime
 import json
 
 
 class BasicQiwiP2P:
 	"""
@@ -37,21 +38,24 @@
 					'value': str(amount),
 					'currency': 'RUB'
 				},
 			'comment': comment,
 			'expirationDateTime': self._lifetime(minutes=lifetime)
 		}
 
-		return self.client.put(url, json=data).json()
+		response = self.client.put(url, json=data).json()
+		return Response.parse_obj(response)
 
 
 	def check(self, bill_id: str) -> dict:
 		""" Gets invoice information """
 		url = f'https://api.qiwi.com/partner/bill/v1/bills/{bill_id}'
-		return self.client.get(url).json()
+
+		response = self.client.get(url).json()
+		return Response.parse_obj(response)
 
 
 	def is_paid(self, bill_id: str) -> bool:
 		""" Checks whether the user has paid the invoice """
 		check_data = self.check(bill_id)
 		
 		if 'errorCode' in check_data:
@@ -60,10 +64,12 @@
 		status = check_data['status']['value']
 		return status == 'PAID'
 
 
 	def reject(self, bill_id: str) -> dict:
 		""" Closes the invoice """
 		url = f'https://api.qiwi.com/partner/bill/v1/bills/{bill_id}/reject'
-		return self.client.post(url).json()
+		
+		response = self.client.post(url).json()
+		return Response.parse_obj(response)
```

