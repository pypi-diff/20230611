# Comparing `tmp/haccrypto-0.1.2.tar.gz` & `tmp/haccrypto-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haccrypto-0.1.2.tar", last modified: Mon Jan 24 00:12:06 2022, max compression
+gzip compressed data, was "haccrypto-0.1.3.tar", last modified: Sun Jun 11 11:17:33 2023, max compression
```

## Comparing `haccrypto-0.1.2.tar` & `haccrypto-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-01-24 00:12:06.840468 haccrypto-0.1.2/
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1105 2022-01-20 06:01:23.000000 haccrypto-0.1.2/LICENSE.md
--rw-r--r--   0 ianburgwin   (501) staff       (20)      138 2022-01-20 06:01:23.000000 haccrypto-0.1.2/MANIFEST.in
--rw-r--r--   0 ianburgwin   (501) staff       (20)     2483 2022-01-24 00:12:06.840326 haccrypto-0.1.2/PKG-INFO
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1885 2022-01-20 06:01:23.000000 haccrypto-0.1.2/README.md
-drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-01-24 00:12:06.839597 haccrypto-0.1.2/haccrypto/
--rw-r--r--   0 ianburgwin   (501) staff       (20)        0 2022-01-22 03:54:55.000000 haccrypto-0.1.2/haccrypto/__init__.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)    20420 2022-01-22 03:54:55.000000 haccrypto-0.1.2/haccrypto/_crypto.cpp
--rw-r--r--   0 ianburgwin   (501) staff       (20)    10668 2022-01-22 03:54:55.000000 haccrypto-0.1.2/haccrypto/aes.cpp
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1522 2022-01-22 03:54:55.000000 haccrypto-0.1.2/haccrypto/aes.h
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1578 2022-01-22 03:54:55.000000 haccrypto-0.1.2/haccrypto/crypto.py
--rwxr-xr-x   0 ianburgwin   (501) staff       (20)  3406016 2022-01-22 03:54:55.000000 haccrypto-0.1.2/haccrypto/libcrypto-1_1-x64.dll
--rwxr-xr-x   0 ianburgwin   (501) staff       (20)  2235072 2022-01-22 03:54:55.000000 haccrypto-0.1.2/haccrypto/libcrypto-1_1.dll
--rwxr-xr-x   0 ianburgwin   (501) staff       (20)  5197376 2022-01-22 03:54:55.000000 haccrypto-0.1.2/haccrypto/libcrypto.1.1.dylib
--rw-r--r--   0 ianburgwin   (501) staff       (20)     6121 2022-01-22 03:54:55.000000 haccrypto-0.1.2/haccrypto/openssl-license.txt
-drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-01-24 00:12:06.840162 haccrypto-0.1.2/haccrypto.egg-info/
--rw-r--r--   0 ianburgwin   (501) staff       (20)     2483 2022-01-24 00:12:06.000000 haccrypto-0.1.2/haccrypto.egg-info/PKG-INFO
--rw-r--r--   0 ianburgwin   (501) staff       (20)      391 2022-01-24 00:12:06.000000 haccrypto-0.1.2/haccrypto.egg-info/SOURCES.txt
--rw-r--r--   0 ianburgwin   (501) staff       (20)        1 2022-01-24 00:12:06.000000 haccrypto-0.1.2/haccrypto.egg-info/dependency_links.txt
--rw-r--r--   0 ianburgwin   (501) staff       (20)       10 2022-01-24 00:12:06.000000 haccrypto-0.1.2/haccrypto.egg-info/top_level.txt
--rw-r--r--   0 ianburgwin   (501) staff       (20)       38 2022-01-24 00:12:06.840520 haccrypto-0.1.2/setup.cfg
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1451 2022-01-23 21:14:24.000000 haccrypto-0.1.2/setup.py
+drwxr-xr-x   0 luigoalma  (1000) luigoalma  (1000)        0 2023-06-11 11:17:33.037484 haccrypto-0.1.3/
+-rw-------   0 luigoalma  (1000) luigoalma  (1000)     1105 2022-04-11 21:43:32.000000 haccrypto-0.1.3/LICENSE.md
+-rw-------   0 luigoalma  (1000) luigoalma  (1000)      138 2022-04-11 21:43:32.000000 haccrypto-0.1.3/MANIFEST.in
+-rw-r--r--   0 luigoalma  (1000) luigoalma  (1000)     2565 2023-06-11 11:17:33.037484 haccrypto-0.1.3/PKG-INFO
+-rw-------   0 luigoalma  (1000) luigoalma  (1000)     1885 2022-04-11 21:43:32.000000 haccrypto-0.1.3/README.md
+drwxr-xr-x   0 luigoalma  (1000) luigoalma  (1000)        0 2023-06-11 11:17:33.036483 haccrypto-0.1.3/haccrypto/
+-rw-------   0 luigoalma  (1000) luigoalma  (1000)        0 2022-04-11 21:43:32.000000 haccrypto-0.1.3/haccrypto/__init__.py
+-rw-r--r--   0 luigoalma  (1000) luigoalma  (1000)    20618 2023-06-11 10:50:00.000000 haccrypto-0.1.3/haccrypto/_crypto.cpp
+-rw-------   0 luigoalma  (1000) luigoalma  (1000)    10668 2022-04-11 21:43:32.000000 haccrypto-0.1.3/haccrypto/aes.cpp
+-rw-------   0 luigoalma  (1000) luigoalma  (1000)     1522 2022-04-11 21:43:32.000000 haccrypto-0.1.3/haccrypto/aes.h
+-rw-------   0 luigoalma  (1000) luigoalma  (1000)     1578 2022-04-11 21:43:32.000000 haccrypto-0.1.3/haccrypto/crypto.py
+-rwx------   0 luigoalma  (1000) luigoalma  (1000)  3406016 2022-04-11 21:43:32.000000 haccrypto-0.1.3/haccrypto/libcrypto-1_1-x64.dll
+-rwx------   0 luigoalma  (1000) luigoalma  (1000)  2235072 2022-04-11 21:43:32.000000 haccrypto-0.1.3/haccrypto/libcrypto-1_1.dll
+-rwx------   0 luigoalma  (1000) luigoalma  (1000)  5197376 2022-04-11 21:43:32.000000 haccrypto-0.1.3/haccrypto/libcrypto.1.1.dylib
+-rw-------   0 luigoalma  (1000) luigoalma  (1000)     6121 2022-04-11 21:43:32.000000 haccrypto-0.1.3/haccrypto/openssl-license.txt
+drwxr-xr-x   0 luigoalma  (1000) luigoalma  (1000)        0 2023-06-11 11:17:33.036483 haccrypto-0.1.3/haccrypto.egg-info/
+-rw-r--r--   0 luigoalma  (1000) luigoalma  (1000)     2565 2023-06-11 11:17:32.000000 haccrypto-0.1.3/haccrypto.egg-info/PKG-INFO
+-rw-r--r--   0 luigoalma  (1000) luigoalma  (1000)      391 2023-06-11 11:17:32.000000 haccrypto-0.1.3/haccrypto.egg-info/SOURCES.txt
+-rw-r--r--   0 luigoalma  (1000) luigoalma  (1000)        1 2023-06-11 11:17:32.000000 haccrypto-0.1.3/haccrypto.egg-info/dependency_links.txt
+-rw-r--r--   0 luigoalma  (1000) luigoalma  (1000)       10 2023-06-11 11:17:32.000000 haccrypto-0.1.3/haccrypto.egg-info/top_level.txt
+-rw-r--r--   0 luigoalma  (1000) luigoalma  (1000)       38 2023-06-11 11:17:33.037484 haccrypto-0.1.3/setup.cfg
+-rw-------   0 luigoalma  (1000) luigoalma  (1000)     1551 2023-06-11 10:53:29.000000 haccrypto-0.1.3/setup.py
```

### Comparing `haccrypto-0.1.2/LICENSE.md` & `haccrypto-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `haccrypto-0.1.2/PKG-INFO` & `haccrypto-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: haccrypto
-Version: 0.1.2
+Version: 0.1.3
 Summary: Nintendo Switch XTSN crypto for Python
 Home-page: https://github.com/luigoalma/haccrypto
 Author: luigoalma
 License: MIT
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # haccrypto
 
 haccrypto is the Nintendo Switch XTSN crypto for Python, originally from ninfs and now standalone.
 
@@ -61,9 +62,7 @@
 
 # Licenses
 
 * `haccrypto` is under the MIT license.
   * `hac/aes.cpp` and `hac/aes.hpp` are from @openluopworld's [aes_128](https://github.com/openluopworld/aes_128) commit `b5b7f55`, and uses the MIT License.
   * `hac/_crypto.cpp` AES-XTS part by me(@luigoalma), based on @plutooo's [crypto module](https://gist.github.com/plutooo/fd4b22e7f533e780c1759057095d7896).
   * `hac/crypto.py` written by @ihaveamac, falls under MIT license as well.
-
-
```

### Comparing `haccrypto-0.1.2/README.md` & `haccrypto-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `haccrypto-0.1.2/haccrypto/_crypto.cpp` & `haccrypto-0.1.3/haccrypto/_crypto.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 #include <Python.h>
 
 #include <cstdio>
 #include <cstdlib>
 #include <cstring>
 #include <mutex>
+#include <string>
 #include <inttypes.h>
 
 extern "C" {
 #include "aes.h"
 }
 
 #if defined _WIN16 || defined _WIN32 || defined _WIN64
@@ -348,14 +349,15 @@
             sectoroffset.Step();
         }
     }
 public:
     inline PyObject *PythonRun(XTSNObject *self, PyObject *args, PyObject *kwds) {
         Py_buffer orig_buf;
         PyObject *local_buf = NULL;
+        bool error = false;
 
         static const char* keywords[] = {
             "buf",
             "sector_off",
             "sector_size",
             "skipped_bytes",
             NULL,
@@ -366,60 +368,69 @@
             return NULL;
 
         if (orig_buf.len == 0) { //nothing to crypt i guess
             local_buf = PyBytes_FromStringAndSize((char * ) NULL, 0);
             if (!local_buf) {
                 PyErr_SetString(PyExc_MemoryError, "Python doesn't have memory for the buffer.");
             }
-            goto end;
+            goto end_func;
         }
 
         if (orig_buf.len % 16) {
             PyErr_SetString(PyExc_ValueError, "length not divisable by 16");
-            goto end;
+            goto end_func;
         }
 
         if (skipped_bytes % 16) {
             PyErr_SetString(PyExc_ValueError, "skipped bytes not divisable by 16");
-            goto end;
+            goto end_func;
         }
 
         if (sector_size % 16 || sector_size == 0) {
             PyErr_SetString(PyExc_ValueError, sector_size == 0 ? "sector size must not be 0" : "sector size not divisable by 16");
-            goto end;
+            goto end_func;
         }
 
         local_buf = PyBytes_FromStringAndSize((char * ) orig_buf.buf, orig_buf.len);
 
         if (!local_buf) {
             PyErr_SetString(PyExc_MemoryError, "Python doesn't have memory for the buffer.");
-            goto end;
+            goto end_func;
         }
 
         roundkeys_key = self->roundkeys_x2;
         roundkeys_tweak = self->roundkeys_x2 + 0xB0;
         buf.ptr = (bigint128 *) PyBytes_AsString(local_buf);
         buf.len = (u64) orig_buf.len;
 
         #ifdef DEBUGON
         Debug();
         #endif
+
+        Py_BEGIN_ALLOW_THREADS;
+
         try {
             if(ossl) ctx = EVP_CIPHER_CTX_new();
             else ctx = NULL;
             Run();
         } catch(...) {
+            error = true;
+        }
+
+        Py_END_ALLOW_THREADS;
+
+        if(error) {
             Py_XDECREF(local_buf);
             local_buf = NULL;
             PyErr_SetString(PyExc_RuntimeError, "Unexpected error from openssl.");
         }
 
         if(ossl) EVP_CIPHER_CTX_free(ctx);
 
-    end:
+    end_func:
         PyBuffer_Release(&orig_buf);
         return local_buf;
     }
     inline XTSN() : sector_size(0x200), skipped_bytes(0) {}
 };
 
 typedef XTSN<&aes_decrypt_128_wrap, aes_encrypt_128_wrap, false> XTSNDecrypt;
```

### Comparing `haccrypto-0.1.2/haccrypto/aes.cpp` & `haccrypto-0.1.3/haccrypto/aes.cpp`

 * *Files identical despite different names*

### Comparing `haccrypto-0.1.2/haccrypto/aes.h` & `haccrypto-0.1.3/haccrypto/aes.h`

 * *Files identical despite different names*

### Comparing `haccrypto-0.1.2/haccrypto/crypto.py` & `haccrypto-0.1.3/haccrypto/crypto.py`

 * *Files identical despite different names*

### Comparing `haccrypto-0.1.2/haccrypto/libcrypto-1_1-x64.dll` & `haccrypto-0.1.3/haccrypto/libcrypto-1_1-x64.dll`

 * *Files identical despite different names*

### Comparing `haccrypto-0.1.2/haccrypto/libcrypto-1_1.dll` & `haccrypto-0.1.3/haccrypto/libcrypto-1_1.dll`

 * *Files identical despite different names*

### Comparing `haccrypto-0.1.2/haccrypto/libcrypto.1.1.dylib` & `haccrypto-0.1.3/haccrypto/libcrypto.1.1.dylib`

 * *Files identical despite different names*

### Comparing `haccrypto-0.1.2/haccrypto/openssl-license.txt` & `haccrypto-0.1.3/haccrypto/openssl-license.txt`

 * *Files identical despite different names*

### Comparing `haccrypto-0.1.2/haccrypto.egg-info/PKG-INFO` & `haccrypto-0.1.3/haccrypto.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: haccrypto
-Version: 0.1.2
+Version: 0.1.3
 Summary: Nintendo Switch XTSN crypto for Python
 Home-page: https://github.com/luigoalma/haccrypto
 Author: luigoalma
 License: MIT
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # haccrypto
 
 haccrypto is the Nintendo Switch XTSN crypto for Python, originally from ninfs and now standalone.
 
@@ -61,9 +62,7 @@
 
 # Licenses
 
 * `haccrypto` is under the MIT license.
   * `hac/aes.cpp` and `hac/aes.hpp` are from @openluopworld's [aes_128](https://github.com/openluopworld/aes_128) commit `b5b7f55`, and uses the MIT License.
   * `hac/_crypto.cpp` AES-XTS part by me(@luigoalma), based on @plutooo's [crypto module](https://gist.github.com/plutooo/fd4b22e7f533e780c1759057095d7896).
   * `hac/crypto.py` written by @ihaveamac, falls under MIT license as well.
-
-
```

### Comparing `haccrypto-0.1.2/setup.py` & `haccrypto-0.1.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     libcrypto = []
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='haccrypto',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     url='https://github.com/luigoalma/haccrypto',
     license='MIT',
     author='luigoalma',
     description='Nintendo Switch XTSN crypto for Python',
     long_description=readme,
     long_description_content_type='text/markdown',
@@ -30,12 +30,14 @@
         'Topic :: Utilities',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     ext_modules=[Extension('haccrypto._crypto', sources=['haccrypto/_crypto.cpp', 'haccrypto/aes.cpp'],
                            extra_compile_args=['/Ox' if sys.platform == 'win32' else '-O3',
                                                '' if sys.platform == 'win32' else '-std=c++11'])]
 )
```

