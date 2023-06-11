# Comparing `tmp/aiokwikset-0.2.2a1.tar.gz` & `tmp/aiokwikset-0.2.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiokwikset-0.2.2a1.tar", last modified: Fri Jun  9 01:58:35 2023, max compression
+gzip compressed data, was "aiokwikset-0.2.2a2.tar", last modified: Sun Jun 11 01:21:45 2023, max compression
```

## Comparing `aiokwikset-0.2.2a1.tar` & `aiokwikset-0.2.2a2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:58:35.364709 aiokwikset-0.2.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-09 01:58:35.364709 aiokwikset-0.2.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:58:35.364709 aiokwikset-0.2.2a1/aiokwikset/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/aws_kwikset.py
--rw-r--r--   0 runner    (1001) docker     (123)    23662 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/aiokwikset/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:58:35.364709 aiokwikset-0.2.2a1/aiokwikset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-09 01:58:35.000000 aiokwikset-0.2.2a1/aiokwikset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-09 01:58:35.000000 aiokwikset-0.2.2a1/aiokwikset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:58:35.000000 aiokwikset-0.2.2a1/aiokwikset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 01:58:35.000000 aiokwikset-0.2.2a1/aiokwikset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 01:58:35.000000 aiokwikset-0.2.2a1/aiokwikset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:58:35.000000 aiokwikset-0.2.2a1/aiokwikset.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 01:58:35.364709 aiokwikset-0.2.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-09 01:58:23.000000 aiokwikset-0.2.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:21:45.481462 aiokwikset-0.2.2a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-11 01:21:45.481462 aiokwikset-0.2.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:21:45.477462 aiokwikset-0.2.2a2/aiokwikset/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/aws_kwikset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23662 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/aiokwikset/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:21:45.477462 aiokwikset-0.2.2a2/aiokwikset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-11 01:21:45.000000 aiokwikset-0.2.2a2/aiokwikset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-11 01:21:45.000000 aiokwikset-0.2.2a2/aiokwikset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 01:21:45.000000 aiokwikset-0.2.2a2/aiokwikset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-11 01:21:45.000000 aiokwikset-0.2.2a2/aiokwikset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 01:21:45.000000 aiokwikset-0.2.2a2/aiokwikset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 01:21:45.000000 aiokwikset-0.2.2a2/aiokwikset.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 01:21:45.481462 aiokwikset-0.2.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-11 01:21:33.000000 aiokwikset-0.2.2a2/setup.py
```

### Comparing `aiokwikset-0.2.2a1/LICENSE` & `aiokwikset-0.2.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.2a1/PKG-INFO` & `aiokwikset-0.2.2a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokwikset
-Version: 0.2.2a1
+Version: 0.2.2a2
 Summary: Python interface for Kwikset Smart Locks
 Home-page: https://github.com/explosivo22/aiokwikset
 Author: Brad Barbour
 Author-email: barbourbj@gmail.com
 License: Apache Software License
 Keywords: kwikset,home automation,kwikset halo,kwikset smart lock
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aiokwikset-0.2.2a1/README.md` & `aiokwikset-0.2.2a2/README.md`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.2a1/aiokwikset/api.py` & `aiokwikset-0.2.2a2/aiokwikset/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,25 +163,28 @@
     async def check_token(self, renew=True):
         """
         Checks the exp attribute of the access_token and either refreshes
         the tokens by calling the renew_access_tokens method or does nothing
         :param renew: bool indicating whether to refresh on expiration
         :return: bool indicating whether access_token has expired
         """
-        if not self.access_token:
+        if not self.id_token:
             raise AttributeError('Access Token Required to Check Token')
         now = datetime.datetime.now()
         dec_access_token = jwt.get_unverified_claims(self.id_token)
 
         if now > datetime.datetime.fromtimestamp(dec_access_token['exp']):
             expired = True
+            LOGGER.debug("Access token has expired.")
             if renew:
+                LOGGER.debug("Attempting to renew access token.")
                 await self.renew_access_token()
         else:
             expired = False
+            LOGGER.debug("Access token not expired")
         return expired
 
     async def renew_access_token(self):
         """
         Sets a new access token on the User using the refresh token.
         """
         auth_params = {'SECRET_HASH': '', 'REFRESH_TOKEN': self.refresh_token}
@@ -244,15 +247,15 @@
                      client_secret=self.client_secret)
 
         self.code_type = code_type
 
         pre_verification = await self.aws.authenticate_user()
 
         if pre_verification.get('AuthenticationResult'):
-            print("2-step verification disabled")
+            LOGGER.debug("2-step verification disabled")
             await self.verify_token(pre_verification['AuthenticationResult']['IdToken'],
                                     'id_token', 'id')
             self.refresh_token = pre_verification['AuthenticationResult']['RefreshToken']
             await self.verify_token(pre_verification['AuthenticationResult']['AccessToken'],
                                     'access_token', 'access')
             self.token_type = pre_verification['AuthenticationResult']['TokenType']
 
@@ -260,15 +263,15 @@
                 self.device = Device(self._request)
 
             if not self.user:
                 self.user = User(self._request)
             
             return
         
-        print("2-step verification enabled")
+        LOGGER.debug("2-step verification enabled")
 
         return pre_verification
 
     async def verify_user(self, pre_verification, code):
         challenge_responses = {'ANSWER': 'answerType:verifyCode,medium:{},codeType:login,code:{}'.format(self.code_type, code),"USERNAME": self.username}
 
         async with self.get_client() as client:
```

### Comparing `aiokwikset-0.2.2a1/aiokwikset/aws_kwikset.py` & `aiokwikset-0.2.2a2/aiokwikset/aws_kwikset.py`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.2a1/aiokwikset/client.py` & `aiokwikset-0.2.2a2/aiokwikset/client.py`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.2a1/aiokwikset/const.py` & `aiokwikset-0.2.2a2/aiokwikset/const.py`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.2a1/aiokwikset/device.py` & `aiokwikset-0.2.2a2/aiokwikset/device.py`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.2a1/aiokwikset/user.py` & `aiokwikset-0.2.2a2/aiokwikset/user.py`

 * *Files identical despite different names*

### Comparing `aiokwikset-0.2.2a1/aiokwikset.egg-info/PKG-INFO` & `aiokwikset-0.2.2a2/aiokwikset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokwikset
-Version: 0.2.2a1
+Version: 0.2.2a2
 Summary: Python interface for Kwikset Smart Locks
 Home-page: https://github.com/explosivo22/aiokwikset
 Author: Brad Barbour
 Author-email: barbourbj@gmail.com
 License: Apache Software License
 Keywords: kwikset,home automation,kwikset halo,kwikset smart lock
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aiokwikset-0.2.2a1/setup.py` & `aiokwikset-0.2.2a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 setup(
     name="aiokwikset",
-    version="0.2.2a1",
+    version="0.2.2a2",
     description="Python interface for Kwikset Smart Locks",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/explosivo22/aiokwikset",
     author="Brad Barbour",
     author_email="barbourbj@gmail.com",
     license='Apache Software License',
```

