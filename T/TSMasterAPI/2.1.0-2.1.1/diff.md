# Comparing `tmp/TSMasterAPI-2.1.0.tar.gz` & `tmp/TSMasterAPI-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSMasterAPI-2.1.0.tar", last modified: Wed May 17 07:00:06 2023, max compression
+gzip compressed data, was "TSMasterAPI-2.1.1.tar", last modified: Sun Jun 11 05:41:50 2023, max compression
```

## Comparing `TSMasterAPI-2.1.0.tar` & `TSMasterAPI-2.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 07:00:06.400349 TSMasterAPI-2.1.0/
--rw-rw-rw-   0        0        0     1024 2023-05-17 07:00:06.398846 TSMasterAPI-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 07:00:06.390008 TSMasterAPI-2.1.0/TSMasterAPI/
--rw-rw-rw-   0        0        0    42782 2023-05-17 06:16:11.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSBUSDriver.py
--rw-rw-rw-   0        0        0    70944 2023-05-17 06:59:34.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSCommon.py
--rw-rw-rw-   0        0        0     1027 2023-05-05 03:08:12.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSDirver.py
--rw-rw-rw-   0        0        0     4152 2023-05-05 03:08:28.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSEnumdefine.py
--rw-rw-rw-   0        0        0    22804 2023-05-17 05:00:47.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSFibex_parse.py
--rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSFlexRayDriver.py
--rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSLINDriver.py
--rw-rw-rw-   0        0        0   155849 2023-05-17 06:27:29.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSMasterAPI.py
--rw-rw-rw-   0        0        0    27697 2023-05-17 06:26:49.000000 TSMasterAPI-2.1.0/TSMasterAPI/TSStructure.py
--rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.1.0/TSMasterAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 07:00:06.398846 TSMasterAPI-2.1.0/TSMasterAPI.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-05-17 07:00:06.000000 TSMasterAPI-2.1.0/TSMasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-17 07:00:06.000000 TSMasterAPI-2.1.0/TSMasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 07:00:06.000000 TSMasterAPI-2.1.0/TSMasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-17 07:00:06.000000 TSMasterAPI-2.1.0/TSMasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.1.0/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 07:00:06.400349 TSMasterAPI-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1585 2023-05-17 06:59:52.000000 TSMasterAPI-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:41:50.483279 TSMasterAPI-2.1.1/
+-rw-rw-rw-   0        0        0     1024 2023-06-11 05:41:50.481859 TSMasterAPI-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-11 05:41:50.471732 TSMasterAPI-2.1.1/TSMasterAPI/
+-rw-rw-rw-   0        0        0    42782 2023-05-17 06:16:11.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSBUSDriver.py
+-rw-rw-rw-   0        0        0    70928 2023-06-11 05:41:15.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSCommon.py
+-rw-rw-rw-   0        0        0     1027 2023-05-05 03:08:12.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSDirver.py
+-rw-rw-rw-   0        0        0     4152 2023-05-05 03:08:28.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSEnumdefine.py
+-rw-rw-rw-   0        0        0    22804 2023-05-17 05:00:47.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSFibex_parse.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSFlexRayDriver.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSLINDriver.py
+-rw-rw-rw-   0        0        0   155849 2023-05-17 06:27:29.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSMasterAPI.py
+-rw-rw-rw-   0        0        0    27697 2023-05-17 06:26:49.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSStructure.py
+-rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.1.1/TSMasterAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-11 05:41:50.480836 TSMasterAPI-2.1.1/TSMasterAPI.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-06-11 05:41:50.000000 TSMasterAPI-2.1.1/TSMasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-06-11 05:41:50.000000 TSMasterAPI-2.1.1/TSMasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 05:41:50.000000 TSMasterAPI-2.1.1/TSMasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-11 05:41:50.000000 TSMasterAPI-2.1.1/TSMasterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.1.1/license.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 05:41:50.483279 TSMasterAPI-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1585 2023-06-11 05:41:40.000000 TSMasterAPI-2.1.1/setup.py
```

### Comparing `TSMasterAPI-2.1.0/PKG-INFO` & `TSMasterAPI-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.1.0
+Version: 2.1.1
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-2.1.0/TSMasterAPI/TSBUSDriver.py` & `TSMasterAPI-2.1.1/TSMasterAPI/TSBUSDriver.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.0/TSMasterAPI/TSCommon.py` & `TSMasterAPI-2.1.1/TSMasterAPI/TSCommon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-04-21 11:59:15
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-05-17 14:59:34
+LastEditTime: 2023-06-11 13:37:22
 '''
 from .TSDirver import *
 from .TSStructure import *  
 from .TSEnumdefine import *  
 from .TSFibex_parse import * 
 
 # Common Functions
@@ -21,15 +21,15 @@
 
 
 def check_status_operation(result, function, arguments):
     """Check the status and raise """
     if result != 0:
         ret = c_char_p()
         tsapp_get_error_description(result, ret)
-        raise Exception("TSDriverOperationError: " + str(function.__name__) + "(" + str(arguments) + ") returned " + str(result) + ": " + str(ret.value))
+        print("TSDriverOperationError: " + str(function.__name__) + "(" + str(arguments) + ") returned " + str(result) + ": " + str(ret.value))
     return result
 
 # 初始化函数 API函数使用之前 必须调用该函数 否则无法正常使用 在工程起始时 调用
 initialize_lib_tsmaster = dll.initialize_lib_tsmaster
 # APPName = b'TSMaster'
 initialize_lib_tsmaster.argtypes = [c_char_p]
 initialize_lib_tsmaster.restype = TS_ReturnType  
@@ -1315,20 +1315,20 @@
 tslog_blf_write_end.errcheck = check_status_operation
 
 # UDS诊断
 
 # CAN
 # 创建诊断服务
 tsdiag_can_create = dll.tsdiag_can_create
-tslog_blf_write_end.argtypes = [pu8,s32,u8,u8,s32,c_bool,s32,c_bool,s32,c_bool]
-tslog_blf_write_end.restype = TS_ReturnType
-tslog_blf_write_end.errcheck = check_status_operation
+tsdiag_can_create.argtypes = [pu8,s32,u8,u8,s32,c_bool,s32,c_bool,s32,c_bool]
+tsdiag_can_create.restype = TS_ReturnType
+tsdiag_can_create.errcheck = check_status_operation
 
 # 删除指定诊断服务
-tsdiag_can_delete = dll.tsdiag_can_create
+tsdiag_can_delete = dll.tsdiag_can_delete
 tsdiag_can_delete.argtypes = [u8]
 tsdiag_can_delete.restype = TS_ReturnType
 tsdiag_can_delete.errcheck = check_status_operation
 
 # 删除所有诊断服务
 tsdiag_can_delete_all = dll.tsdiag_can_delete_all
 tsdiag_can_delete_all.argtypes = []
@@ -1406,39 +1406,39 @@
 tsdiag_can_security_access_send_key = dll.tsdiag_can_security_access_send_key
 tsdiag_can_security_access_send_key.argtypes = [u8,s32,pu8,ps32]
 tsdiag_can_security_access_send_key.restype = TS_ReturnType
 tsdiag_can_security_access_send_key.errcheck = check_status_operation
 
 # 34
 tsdiag_can_request_download = dll.tsdiag_can_request_download
-tsdiag_can_request_download.argtypes = [u8,s32,s32]
+tsdiag_can_request_download.argtypes = [u8,u32,u32]
 tsdiag_can_request_download.restype = TS_ReturnType
 tsdiag_can_request_download.errcheck = check_status_operation
 
 # 35
 tsdiag_can_request_upload = dll.tsdiag_can_request_upload
-tsdiag_can_request_upload.argtypes = [u8,s32,s32]
+tsdiag_can_request_upload.argtypes = [u8,u32,u32]
 tsdiag_can_request_upload.restype = TS_ReturnType
 tsdiag_can_request_upload.errcheck = check_status_operation
 
 # 36
 tsdiag_can_transfer_data = dll.tsdiag_can_transfer_data
-tsdiag_can_transfer_data.argtypes = [u8,pu8,s32,s32]
+tsdiag_can_transfer_data.argtypes = [u8,pu8,u32,u32]
 tsdiag_can_transfer_data.restype = TS_ReturnType
 tsdiag_can_transfer_data.errcheck = check_status_operation
 
 # 37
 tsdiag_can_request_transfer_exit = dll.tsdiag_can_request_transfer_exit
 tsdiag_can_request_transfer_exit.argtypes = [u8]
 tsdiag_can_request_transfer_exit.restype = TS_ReturnType
 tsdiag_can_request_transfer_exit.errcheck = check_status_operation
 
 # 2E
 tsdiag_can_write_data_by_identifier = dll.tsdiag_can_write_data_by_identifier
-tsdiag_can_write_data_by_identifier.argtypes = [u8,u16,pu8,s32]
+tsdiag_can_write_data_by_identifier.argtypes = [u8,u16,pu8,u32]
 tsdiag_can_write_data_by_identifier.restype = TS_ReturnType
 tsdiag_can_write_data_by_identifier.errcheck = check_status_operation
 
 # 22
 tsdiag_can_read_data_by_identifier = dll.tsdiag_can_read_data_by_identifier
 tsdiag_can_read_data_by_identifier.argtypes = [u8,u16,pu8,ps32]
 tsdiag_can_read_data_by_identifier.restype = TS_ReturnType
```

### Comparing `TSMasterAPI-2.1.0/TSMasterAPI/TSDirver.py` & `TSMasterAPI-2.1.1/TSMasterAPI/TSDirver.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.0/TSMasterAPI/TSEnumdefine.py` & `TSMasterAPI-2.1.1/TSMasterAPI/TSEnumdefine.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.0/TSMasterAPI/TSFibex_parse.py` & `TSMasterAPI-2.1.1/TSMasterAPI/TSFibex_parse.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.0/TSMasterAPI/TSMasterAPI.py` & `TSMasterAPI-2.1.1/TSMasterAPI/TSMasterAPI.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.0/TSMasterAPI/TSStructure.py` & `TSMasterAPI-2.1.1/TSMasterAPI/TSStructure.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.0/TSMasterAPI.egg-info/PKG-INFO` & `TSMasterAPI-2.1.1/TSMasterAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.1.0
+Version: 2.1.1
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-2.1.0/license.txt` & `TSMasterAPI-2.1.1/license.txt`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.0/setup.py` & `TSMasterAPI-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-24 09:26:29
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-05-17 14:27:55
+LastEditTime: 2023-06-11 13:41:40
 FilePath: \VSCode_Pro\Python_Pro\TSMasterApi\setup.py
 Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r",encoding="utf-8") as f:
   long_description = f.read()
 
 # 
 setup(name='TSMasterAPI',  # 包名
-      version='2.1.0',  # 版本号
+      version='2.1.1',  # 版本号
       description='Use TSMaster hardware',
       long_description=long_description,
       author='seven',
       author_email='865762826@qq.com',
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
```

