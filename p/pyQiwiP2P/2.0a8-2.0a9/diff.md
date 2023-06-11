# Comparing `tmp/pyQiwiP2P-2.0a8.tar.gz` & `tmp/pyQiwiP2P-2.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyQiwiP2P-2.0a8.tar", last modified: Wed Jul 21 22:58:29 2021, max compression
+gzip compressed data, was "pyQiwiP2P-2.0a9.tar", last modified: Wed Jul 21 23:44:22 2021, max compression
```

## Comparing `pyQiwiP2P-2.0a8.tar` & `pyQiwiP2P-2.0a9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-07-21 22:58:29.567554 pyQiwiP2P-2.0a8/
--rw-r--r--   0 white     (1000) white     (1000)    16725 2020-07-18 06:46:07.000000 pyQiwiP2P-2.0a8/LICENSE
--rw-r--r--   0 white     (1000) white     (1000)    11544 2021-07-21 22:58:29.564221 pyQiwiP2P-2.0a8/PKG-INFO
--rw-r--r--   0 white     (1000) white     (1000)    10895 2021-07-17 18:38:00.000000 pyQiwiP2P-2.0a8/README.md
-drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-07-21 22:58:29.564221 pyQiwiP2P-2.0a8/pyQiwiP2P.egg-info/
--rw-r--r--   0 white     (1000) white     (1000)    11544 2021-07-21 22:58:29.000000 pyQiwiP2P-2.0a8/pyQiwiP2P.egg-info/PKG-INFO
--rw-r--r--   0 white     (1000) white     (1000)      482 2021-07-21 22:58:29.000000 pyQiwiP2P-2.0a8/pyQiwiP2P.egg-info/SOURCES.txt
--rw-r--r--   0 white     (1000) white     (1000)        1 2021-07-21 22:58:29.000000 pyQiwiP2P-2.0a8/pyQiwiP2P.egg-info/dependency_links.txt
--rw-r--r--   0 white     (1000) white     (1000)      228 2021-07-21 22:58:29.000000 pyQiwiP2P-2.0a8/pyQiwiP2P.egg-info/requires.txt
--rw-r--r--   0 white     (1000) white     (1000)       10 2021-07-21 22:58:29.000000 pyQiwiP2P-2.0a8/pyQiwiP2P.egg-info/top_level.txt
-drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-07-21 22:58:29.564221 pyQiwiP2P-2.0a8/pyqiwip2p/
--rw-r--r--   0 white     (1000) white     (1000)    10065 2021-07-21 22:57:55.000000 pyQiwiP2P-2.0a8/pyqiwip2p/AioQiwip2p.py
--rw-r--r--   0 white     (1000) white     (1000)     9462 2021-07-21 22:57:55.000000 pyQiwiP2P-2.0a8/pyqiwip2p/Qiwip2p.py
--rw-r--r--   0 white     (1000) white     (1000)       82 2021-07-17 18:38:00.000000 pyQiwiP2P-2.0a8/pyqiwip2p/__init__.py
-drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-07-21 22:58:29.564221 pyQiwiP2P-2.0a8/pyqiwip2p/notify/
--rw-r--r--   0 white     (1000) white     (1000)     3006 2021-07-17 18:38:00.000000 pyQiwiP2P-2.0a8/pyqiwip2p/notify/__init__.py
--rw-r--r--   0 white     (1000) white     (1000)     2531 2021-07-17 18:38:00.000000 pyQiwiP2P-2.0a8/pyqiwip2p/notify/async_client.py
-drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-07-21 22:58:29.564221 pyQiwiP2P-2.0a8/pyqiwip2p/p2p_types/
--rw-r--r--   0 white     (1000) white     (1000)     2721 2020-07-21 11:06:01.000000 pyQiwiP2P-2.0a8/pyqiwip2p/p2p_types/Customer.py
--rw-r--r--   0 white     (1000) white     (1000)     1512 2021-07-17 18:38:00.000000 pyQiwiP2P-2.0a8/pyqiwip2p/p2p_types/Errors.py
--rw-r--r--   0 white     (1000) white     (1000)     3709 2021-05-02 18:05:48.000000 pyQiwiP2P-2.0a8/pyqiwip2p/p2p_types/QiwiDatetime.py
--rw-r--r--   0 white     (1000) white     (1000)     3414 2021-07-17 18:38:00.000000 pyQiwiP2P-2.0a8/pyqiwip2p/p2p_types/Responses.py
--rw-r--r--   0 white     (1000) white     (1000)      175 2021-06-12 18:30:29.000000 pyQiwiP2P-2.0a8/pyqiwip2p/p2p_types/__init__.py
--rw-r--r--   0 white     (1000) white     (1000)       38 2021-07-21 22:58:29.567554 pyQiwiP2P-2.0a8/setup.cfg
--rw-r--r--   0 white     (1000) white     (1000)     1014 2021-07-21 22:58:06.000000 pyQiwiP2P-2.0a8/setup.py
+drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-07-21 23:44:22.982445 pyQiwiP2P-2.0a9/
+-rw-r--r--   0 white     (1000) white     (1000)    16725 2020-07-18 06:46:07.000000 pyQiwiP2P-2.0a9/LICENSE
+-rw-r--r--   0 white     (1000) white     (1000)    11544 2021-07-21 23:44:22.979112 pyQiwiP2P-2.0a9/PKG-INFO
+-rw-r--r--   0 white     (1000) white     (1000)    10895 2021-07-17 18:38:00.000000 pyQiwiP2P-2.0a9/README.md
+drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-07-21 23:44:22.975778 pyQiwiP2P-2.0a9/pyQiwiP2P.egg-info/
+-rw-r--r--   0 white     (1000) white     (1000)    11544 2021-07-21 23:44:22.000000 pyQiwiP2P-2.0a9/pyQiwiP2P.egg-info/PKG-INFO
+-rw-r--r--   0 white     (1000) white     (1000)      482 2021-07-21 23:44:22.000000 pyQiwiP2P-2.0a9/pyQiwiP2P.egg-info/SOURCES.txt
+-rw-r--r--   0 white     (1000) white     (1000)        1 2021-07-21 23:44:22.000000 pyQiwiP2P-2.0a9/pyQiwiP2P.egg-info/dependency_links.txt
+-rw-r--r--   0 white     (1000) white     (1000)      259 2021-07-21 23:44:22.000000 pyQiwiP2P-2.0a9/pyQiwiP2P.egg-info/requires.txt
+-rw-r--r--   0 white     (1000) white     (1000)       10 2021-07-21 23:44:22.000000 pyQiwiP2P-2.0a9/pyQiwiP2P.egg-info/top_level.txt
+drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-07-21 23:44:22.975778 pyQiwiP2P-2.0a9/pyqiwip2p/
+-rw-r--r--   0 white     (1000) white     (1000)    10023 2021-07-21 23:44:12.000000 pyQiwiP2P-2.0a9/pyqiwip2p/AioQiwip2p.py
+-rw-r--r--   0 white     (1000) white     (1000)     9462 2021-07-21 22:57:55.000000 pyQiwiP2P-2.0a9/pyqiwip2p/Qiwip2p.py
+-rw-r--r--   0 white     (1000) white     (1000)       82 2021-07-17 18:38:00.000000 pyQiwiP2P-2.0a9/pyqiwip2p/__init__.py
+drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-07-21 23:44:22.979112 pyQiwiP2P-2.0a9/pyqiwip2p/notify/
+-rw-r--r--   0 white     (1000) white     (1000)     3006 2021-07-17 18:38:00.000000 pyQiwiP2P-2.0a9/pyqiwip2p/notify/__init__.py
+-rw-r--r--   0 white     (1000) white     (1000)     2531 2021-07-17 18:38:00.000000 pyQiwiP2P-2.0a9/pyqiwip2p/notify/async_client.py
+drwxr-xr-x   0 white     (1000) white     (1000)        0 2021-07-21 23:44:22.979112 pyQiwiP2P-2.0a9/pyqiwip2p/p2p_types/
+-rw-r--r--   0 white     (1000) white     (1000)     2721 2020-07-21 11:06:01.000000 pyQiwiP2P-2.0a9/pyqiwip2p/p2p_types/Customer.py
+-rw-r--r--   0 white     (1000) white     (1000)     1512 2021-07-17 18:38:00.000000 pyQiwiP2P-2.0a9/pyqiwip2p/p2p_types/Errors.py
+-rw-r--r--   0 white     (1000) white     (1000)     3626 2021-07-21 23:28:50.000000 pyQiwiP2P-2.0a9/pyqiwip2p/p2p_types/QiwiDatetime.py
+-rw-r--r--   0 white     (1000) white     (1000)     3414 2021-07-17 18:38:00.000000 pyQiwiP2P-2.0a9/pyqiwip2p/p2p_types/Responses.py
+-rw-r--r--   0 white     (1000) white     (1000)      175 2021-06-12 18:30:29.000000 pyQiwiP2P-2.0a9/pyqiwip2p/p2p_types/__init__.py
+-rw-r--r--   0 white     (1000) white     (1000)       38 2021-07-21 23:44:22.982445 pyQiwiP2P-2.0a9/setup.cfg
+-rw-r--r--   0 white     (1000) white     (1000)     1014 2021-07-21 23:44:12.000000 pyQiwiP2P-2.0a9/setup.py
```

### Comparing `pyQiwiP2P-2.0a8/LICENSE` & `pyQiwiP2P-2.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyQiwiP2P-2.0a8/PKG-INFO` & `pyQiwiP2P-2.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyQiwiP2P
-Version: 2.0a8
+Version: 2.0a9
 Summary: pyQiwiP2P
 Home-page: https://github.com/WhiteApfel/pyQiwiP2P
 Author: WhiteApfel
 Author-email: white@pfel.ru
 License: Mozilla Public License 2.0
 Project-URL: Документальное чтиво, https://pyqiwip2p.readthedocs.io/ru/latest/
 Project-URL: Донатик, https://pfel.cc/donate
```

### Comparing `pyQiwiP2P-2.0a8/README.md` & `pyQiwiP2P-2.0a9/README.md`

 * *Files identical despite different names*

### Comparing `pyQiwiP2P-2.0a8/pyQiwiP2P.egg-info/PKG-INFO` & `pyQiwiP2P-2.0a9/pyQiwiP2P.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyQiwiP2P
-Version: 2.0a8
+Version: 2.0a9
 Summary: pyQiwiP2P
 Home-page: https://github.com/WhiteApfel/pyQiwiP2P
 Author: WhiteApfel
 Author-email: white@pfel.ru
 License: Mozilla Public License 2.0
 Project-URL: Документальное чтиво, https://pyqiwip2p.readthedocs.io/ru/latest/
 Project-URL: Донатик, https://pfel.cc/donate
```

### Comparing `pyQiwiP2P-2.0a8/pyqiwip2p/AioQiwip2p.py` & `pyQiwiP2P-2.0a9/pyqiwip2p/AioQiwip2p.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import random
 from loguru import logger
 import httpx
 import asyncio
 from ipaddress import IPv4Network, IPv4Address
 
 from pyqiwip2p.p2p_types import Bill
-from pyqiwip2p.p2p_types import QiwiError
 from pyqiwip2p.p2p_types import QiwiCustomer
 from pyqiwip2p.p2p_types import QiwiDatetime
 
 logger.disable("pyqiwip2p")
 requests = httpx.AsyncClient()
```

### Comparing `pyQiwiP2P-2.0a8/pyqiwip2p/Qiwip2p.py` & `pyQiwiP2P-2.0a9/pyqiwip2p/Qiwip2p.py`

 * *Files identical despite different names*

### Comparing `pyQiwiP2P-2.0a8/pyqiwip2p/notify/__init__.py` & `pyQiwiP2P-2.0a9/pyqiwip2p/notify/__init__.py`

 * *Files identical despite different names*

### Comparing `pyQiwiP2P-2.0a8/pyqiwip2p/notify/async_client.py` & `pyQiwiP2P-2.0a9/pyqiwip2p/notify/async_client.py`

 * *Files identical despite different names*

### Comparing `pyQiwiP2P-2.0a8/pyqiwip2p/p2p_types/Customer.py` & `pyQiwiP2P-2.0a9/pyqiwip2p/p2p_types/Customer.py`

 * *Files identical despite different names*

### Comparing `pyQiwiP2P-2.0a8/pyqiwip2p/p2p_types/Errors.py` & `pyQiwiP2P-2.0a9/pyqiwip2p/p2p_types/Errors.py`

 * *Files identical despite different names*

### Comparing `pyQiwiP2P-2.0a8/pyqiwip2p/p2p_types/QiwiDatetime.py` & `pyQiwiP2P-2.0a9/pyqiwip2p/p2p_types/QiwiDatetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,17 @@
 			self.qiwi = self.datetime.isoformat()
 			self.timestamp = self.datetime.timestamp()
 			if moment:
 				if type(moment) is str:
 					if re.match(self._exp_regex, moment):
 						self.set_from_qiwi(moment)
 					else:
-						raise TypeError("The string does not match the format 'ГГГГ-ММ-ДДTчч:мм:сс.мсс+\-чч:мм'")
+						raise TypeError(r"The string does not match the format 'ГГГГ-ММ-ДДTчч:мм:сс.мсс+\-чч:мм'")
 				if type(moment) is int or type(moment) is float:
-					if moment < time.time():
-						raise ValueError("Time has passed")
-					else:
-						self.set_from_timestamp(moment)
+					self.set_from_timestamp(moment)
 				if type(moment) is datetime:
 					self.set_from_datetime(moment)
 			else:
 				self.set_from_datetime(self.now_datetime())
 
 	def now_datetime(self):
 		return datetime.now(timezone(timedelta(hours=3))).replace(microsecond=0)
```

### Comparing `pyQiwiP2P-2.0a8/pyqiwip2p/p2p_types/Responses.py` & `pyQiwiP2P-2.0a9/pyqiwip2p/p2p_types/Responses.py`

 * *Files identical despite different names*

### Comparing `pyQiwiP2P-2.0a8/setup.py` & `pyQiwiP2P-2.0a9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def requirements():
 	with open('requirements.txt', 'r') as req:
 		return [r for r in req.read().split("\n") if r]
 
 
 setup(
 	name='pyQiwiP2P',
-	version='2.0a8',
+	version='2.0a9',
 	packages=['pyqiwip2p', 'pyqiwip2p.p2p_types', 'pyqiwip2p.notify'],
 	url='https://github.com/WhiteApfel/pyQiwiP2P',
 	license='Mozilla Public License 2.0',
 	author='WhiteApfel',
 	author_email='white@pfel.ru',
 	description='pyQiwiP2P',
 	install_requires=requirements(),
```

