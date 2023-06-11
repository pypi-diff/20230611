# Comparing `tmp/readpy_P-Y-R-O-B-O-T-1.0.0.tar.gz` & `tmp/readpy_P-Y-R-O-B-O-T-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readpy_P-Y-R-O-B-O-T-1.0.0.tar", last modified: Sun Jun 11 17:06:38 2023, max compression
+gzip compressed data, was "readpy_P-Y-R-O-B-O-T-1.0.1.tar", last modified: Sun Jun 11 17:15:25 2023, max compression
```

## Comparing `readpy_P-Y-R-O-B-O-T-1.0.0.tar` & `readpy_P-Y-R-O-B-O-T-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-06-11 17:06:38.409483 readpy_P-Y-R-O-B-O-T-1.0.0/
--rw-rw-r--   0 kushal    (1000) kushal    (1000)    35142 2023-06-11 16:18:42.000000 readpy_P-Y-R-O-B-O-T-1.0.0/LICENSE
--rw-rw-r--   0 kushal    (1000) kushal    (1000)    43790 2023-06-11 17:06:38.409483 readpy_P-Y-R-O-B-O-T-1.0.0/PKG-INFO
--rw-rw-r--   0 kushal    (1000) kushal    (1000)     2778 2023-06-11 17:00:18.000000 readpy_P-Y-R-O-B-O-T-1.0.0/README.md
-drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-06-11 17:06:38.405481 readpy_P-Y-R-O-B-O-T-1.0.0/READPY/
-drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-06-11 17:06:38.405481 readpy_P-Y-R-O-B-O-T-1.0.0/READPY/CLIENT/
--rw-rw-r--   0 kushal    (1000) kushal    (1000)        0 2023-06-11 15:25:25.000000 readpy_P-Y-R-O-B-O-T-1.0.0/READPY/CLIENT/__init__.py
--rw-rw-r--   0 kushal    (1000) kushal    (1000)     3899 2023-06-11 16:02:03.000000 readpy_P-Y-R-O-B-O-T-1.0.0/READPY/CLIENT/client.py
-drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-06-11 17:06:38.405481 readpy_P-Y-R-O-B-O-T-1.0.0/READPY/SERVER/
--rw-rw-r--   0 kushal    (1000) kushal    (1000)        0 2023-06-11 15:45:19.000000 readpy_P-Y-R-O-B-O-T-1.0.0/READPY/SERVER/__init__.py
--rw-rw-r--   0 kushal    (1000) kushal    (1000)     4175 2023-06-11 16:02:08.000000 readpy_P-Y-R-O-B-O-T-1.0.0/READPY/SERVER/server.py
--rw-rw-r--   0 kushal    (1000) kushal    (1000)        0 2023-06-11 15:30:16.000000 readpy_P-Y-R-O-B-O-T-1.0.0/READPY/__init__.py
--rw-rw-r--   0 kushal    (1000) kushal    (1000)      692 2023-06-11 17:05:34.000000 readpy_P-Y-R-O-B-O-T-1.0.0/pyproject.toml
-drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-06-11 17:06:38.405481 readpy_P-Y-R-O-B-O-T-1.0.0/readpy_P_Y_R_O_B_O_T.egg-info/
--rw-rw-r--   0 kushal    (1000) kushal    (1000)    43790 2023-06-11 17:06:38.000000 readpy_P-Y-R-O-B-O-T-1.0.0/readpy_P_Y_R_O_B_O_T.egg-info/PKG-INFO
--rw-rw-r--   0 kushal    (1000) kushal    (1000)      370 2023-06-11 17:06:38.000000 readpy_P-Y-R-O-B-O-T-1.0.0/readpy_P_Y_R_O_B_O_T.egg-info/SOURCES.txt
--rw-rw-r--   0 kushal    (1000) kushal    (1000)        1 2023-06-11 17:06:38.000000 readpy_P-Y-R-O-B-O-T-1.0.0/readpy_P_Y_R_O_B_O_T.egg-info/dependency_links.txt
--rw-rw-r--   0 kushal    (1000) kushal    (1000)       30 2023-06-11 17:06:38.000000 readpy_P-Y-R-O-B-O-T-1.0.0/readpy_P_Y_R_O_B_O_T.egg-info/requires.txt
--rw-rw-r--   0 kushal    (1000) kushal    (1000)        7 2023-06-11 17:06:38.000000 readpy_P-Y-R-O-B-O-T-1.0.0/readpy_P_Y_R_O_B_O_T.egg-info/top_level.txt
--rw-rw-r--   0 kushal    (1000) kushal    (1000)       38 2023-06-11 17:06:38.409483 readpy_P-Y-R-O-B-O-T-1.0.0/setup.cfg
+drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-06-11 17:15:25.102351 readpy_P-Y-R-O-B-O-T-1.0.1/
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)    35142 2023-06-11 16:18:42.000000 readpy_P-Y-R-O-B-O-T-1.0.1/LICENSE
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)    43798 2023-06-11 17:15:25.102351 readpy_P-Y-R-O-B-O-T-1.0.1/PKG-INFO
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)     2786 2023-06-11 17:13:27.000000 readpy_P-Y-R-O-B-O-T-1.0.1/README.md
+drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-06-11 17:15:25.098350 readpy_P-Y-R-O-B-O-T-1.0.1/READPY/
+drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-06-11 17:15:25.098350 readpy_P-Y-R-O-B-O-T-1.0.1/READPY/CLIENT/
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)        0 2023-06-11 15:25:25.000000 readpy_P-Y-R-O-B-O-T-1.0.1/READPY/CLIENT/__init__.py
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)     3899 2023-06-11 16:02:03.000000 readpy_P-Y-R-O-B-O-T-1.0.1/READPY/CLIENT/client.py
+drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-06-11 17:15:25.098350 readpy_P-Y-R-O-B-O-T-1.0.1/READPY/SERVER/
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)        0 2023-06-11 15:45:19.000000 readpy_P-Y-R-O-B-O-T-1.0.1/READPY/SERVER/__init__.py
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)     4175 2023-06-11 16:02:08.000000 readpy_P-Y-R-O-B-O-T-1.0.1/READPY/SERVER/server.py
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)        0 2023-06-11 15:30:16.000000 readpy_P-Y-R-O-B-O-T-1.0.1/READPY/__init__.py
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)      692 2023-06-11 17:13:58.000000 readpy_P-Y-R-O-B-O-T-1.0.1/pyproject.toml
+drwxrwxr-x   0 kushal    (1000) kushal    (1000)        0 2023-06-11 17:15:25.098350 readpy_P-Y-R-O-B-O-T-1.0.1/readpy_P_Y_R_O_B_O_T.egg-info/
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)    43798 2023-06-11 17:15:25.000000 readpy_P-Y-R-O-B-O-T-1.0.1/readpy_P_Y_R_O_B_O_T.egg-info/PKG-INFO
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)      370 2023-06-11 17:15:25.000000 readpy_P-Y-R-O-B-O-T-1.0.1/readpy_P_Y_R_O_B_O_T.egg-info/SOURCES.txt
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)        1 2023-06-11 17:15:25.000000 readpy_P-Y-R-O-B-O-T-1.0.1/readpy_P_Y_R_O_B_O_T.egg-info/dependency_links.txt
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)       30 2023-06-11 17:15:25.000000 readpy_P-Y-R-O-B-O-T-1.0.1/readpy_P_Y_R_O_B_O_T.egg-info/requires.txt
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)        7 2023-06-11 17:15:25.000000 readpy_P-Y-R-O-B-O-T-1.0.1/readpy_P_Y_R_O_B_O_T.egg-info/top_level.txt
+-rw-rw-r--   0 kushal    (1000) kushal    (1000)       38 2023-06-11 17:15:25.102351 readpy_P-Y-R-O-B-O-T-1.0.1/setup.cfg
```

### Comparing `readpy_P-Y-R-O-B-O-T-1.0.0/LICENSE` & `readpy_P-Y-R-O-B-O-T-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `readpy_P-Y-R-O-B-O-T-1.0.0/PKG-INFO` & `readpy_P-Y-R-O-B-O-T-1.0.1/readpy_P_Y_R_O_B_O_T.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: readpy_P-Y-R-O-B-O-T
-Version: 1.0.0
+Name: readpy-P-Y-R-O-B-O-T
+Version: 1.0.1
 Summary: A MINI AND EASY TO USE REDIS SERVER
 Author-email: KUSHAL <NONE@NONE.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -704,28 +704,34 @@
 > Install it using pip.
 
 * Goto [PYPI](https://pypi.org/project/readpy-P-Y-R-O-B-O-T/)
 
 # USAGE
 
 ## CONFIGURATION
-> For configuration of server and client need a configuration file naed readpy_conf.json
+* For configuration of server and client need a configuration file naed readpy_conf.json
 
 ### CONFIG PARAMETERS
-> RECV_BUFFER and TRANSMISSION_BUFFER are parameters both should have same corresponding value for both server and client configuration.
-> ENCRYPTION_KEY and DECRYPTION_KEY are parameters which ensure encryption of data sent over connection, see CYPHER-PROTOCOL documentation for more information.
-> TIMEOUT is the time after which a connection is closed or reset from client side or server side.
-> READPY_NODE defines the interface address at which the server will be running (IP).
-> READPY_PORT defines port number on which server runs.
+* RECV_BUFFER and TRANSMISSION_BUFFER are parameters both should have same corresponding value for both server and client configuration.
 
-> Example readpy_conf is given in CONF_FILES folder, consider that for more details.
+* ENCRYPTION_KEY and DECRYPTION_KEY are parameters which ensure encryption of data sent over connection, see CYPHER-PROTOCOL documentation for more information.
+
+* TIMEOUT is the time after which a connection is closed or reset from client side or server side.
+
+* READPY_NODE defines the interface address at which the server will be running (IP).
+
+* READPY_PORT defines port number on which server runs.
+
+* Example readpy_conf is given in CONF_FILES folder, consider that for more details.
 
 ## CLIENT USAGE
-> Put the readpy_conf.json and TEST_SCRIPT/client.py in same folder and run in same directory space.
-> Consider the following code :
+* Put the readpy_conf.json and TEST_SCRIPT/client.py in same folder and run in same directory space.
+
+* Consider the following code :
+
 ```python3
 from READPY.CLIENT.client import READPY_CLIENT
 
 if __name__ == "__main__" :
 	# INITIALISING THE READPY_CLIENT
     CLIENT = READPY_CLIENT()
 
@@ -741,16 +747,18 @@
 	# READING FROM THE LOCATION ["CONSTANTS"] FROM THE SERVER
     print(CLIENT.read(["CONSTANTS"]))
 	# READING FROM THE LOCATION ["CONSTANTS", "MATH"] FROM THE SERVER
     print(CLIENT.read(["CONSTANTS", "MATH"]))
 ```
 
 ## SERVER USAGE
-> Put the readpy_conf.json and TEST_SCRIPT/server.py in same folder and run in same directory space.
-> Consider the following code :
+* Put the readpy_conf.json and TEST_SCRIPT/server.py in same folder and run in same directory space.
+
+* Consider the following code :
+
 ```python3
 from READPY.SERVER.server import READPY_SERVER
 
 if __name__ == "__main__" :
 	# INITIALISING THE READPY_SERVER
     SERVER = READPY_SERVER()
 	# STARTING THE SERVER
```

### Comparing `readpy_P-Y-R-O-B-O-T-1.0.0/README.md` & `readpy_P-Y-R-O-B-O-T-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,28 +18,34 @@
 > Install it using pip.
 
 * Goto [PYPI](https://pypi.org/project/readpy-P-Y-R-O-B-O-T/)
 
 # USAGE
 
 ## CONFIGURATION
-> For configuration of server and client need a configuration file naed readpy_conf.json
+* For configuration of server and client need a configuration file naed readpy_conf.json
 
 ### CONFIG PARAMETERS
-> RECV_BUFFER and TRANSMISSION_BUFFER are parameters both should have same corresponding value for both server and client configuration.
-> ENCRYPTION_KEY and DECRYPTION_KEY are parameters which ensure encryption of data sent over connection, see CYPHER-PROTOCOL documentation for more information.
-> TIMEOUT is the time after which a connection is closed or reset from client side or server side.
-> READPY_NODE defines the interface address at which the server will be running (IP).
-> READPY_PORT defines port number on which server runs.
+* RECV_BUFFER and TRANSMISSION_BUFFER are parameters both should have same corresponding value for both server and client configuration.
 
-> Example readpy_conf is given in CONF_FILES folder, consider that for more details.
+* ENCRYPTION_KEY and DECRYPTION_KEY are parameters which ensure encryption of data sent over connection, see CYPHER-PROTOCOL documentation for more information.
+
+* TIMEOUT is the time after which a connection is closed or reset from client side or server side.
+
+* READPY_NODE defines the interface address at which the server will be running (IP).
+
+* READPY_PORT defines port number on which server runs.
+
+* Example readpy_conf is given in CONF_FILES folder, consider that for more details.
 
 ## CLIENT USAGE
-> Put the readpy_conf.json and TEST_SCRIPT/client.py in same folder and run in same directory space.
-> Consider the following code :
+* Put the readpy_conf.json and TEST_SCRIPT/client.py in same folder and run in same directory space.
+
+* Consider the following code :
+
 ```python3
 from READPY.CLIENT.client import READPY_CLIENT
 
 if __name__ == "__main__" :
 	# INITIALISING THE READPY_CLIENT
     CLIENT = READPY_CLIENT()
 
@@ -55,16 +61,18 @@
 	# READING FROM THE LOCATION ["CONSTANTS"] FROM THE SERVER
     print(CLIENT.read(["CONSTANTS"]))
 	# READING FROM THE LOCATION ["CONSTANTS", "MATH"] FROM THE SERVER
     print(CLIENT.read(["CONSTANTS", "MATH"]))
 ```
 
 ## SERVER USAGE
-> Put the readpy_conf.json and TEST_SCRIPT/server.py in same folder and run in same directory space.
-> Consider the following code :
+* Put the readpy_conf.json and TEST_SCRIPT/server.py in same folder and run in same directory space.
+
+* Consider the following code :
+
 ```python3
 from READPY.SERVER.server import READPY_SERVER
 
 if __name__ == "__main__" :
 	# INITIALISING THE READPY_SERVER
     SERVER = READPY_SERVER()
 	# STARTING THE SERVER
```

### Comparing `readpy_P-Y-R-O-B-O-T-1.0.0/READPY/CLIENT/client.py` & `readpy_P-Y-R-O-B-O-T-1.0.1/READPY/CLIENT/client.py`

 * *Files identical despite different names*

### Comparing `readpy_P-Y-R-O-B-O-T-1.0.0/READPY/SERVER/server.py` & `readpy_P-Y-R-O-B-O-T-1.0.1/READPY/SERVER/server.py`

 * *Files identical despite different names*

### Comparing `readpy_P-Y-R-O-B-O-T-1.0.0/pyproject.toml` & `readpy_P-Y-R-O-B-O-T-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<=64.0.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "readpy_P-Y-R-O-B-O-T"
-version = "1.0.0"
+version = "1.0.1"
 description = "A MINI AND EASY TO USE REDIS SERVER"
 readme = "README.md"
 authors = [{name =  "KUSHAL", email = "NONE@NONE.com"}]
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
 keywords = ["redis", "memory", "communication",
 			"RAM", "RAM server", "memory server",
```

### Comparing `readpy_P-Y-R-O-B-O-T-1.0.0/readpy_P_Y_R_O_B_O_T.egg-info/PKG-INFO` & `readpy_P-Y-R-O-B-O-T-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: readpy-P-Y-R-O-B-O-T
-Version: 1.0.0
+Name: readpy_P-Y-R-O-B-O-T
+Version: 1.0.1
 Summary: A MINI AND EASY TO USE REDIS SERVER
 Author-email: KUSHAL <NONE@NONE.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -704,28 +704,34 @@
 > Install it using pip.
 
 * Goto [PYPI](https://pypi.org/project/readpy-P-Y-R-O-B-O-T/)
 
 # USAGE
 
 ## CONFIGURATION
-> For configuration of server and client need a configuration file naed readpy_conf.json
+* For configuration of server and client need a configuration file naed readpy_conf.json
 
 ### CONFIG PARAMETERS
-> RECV_BUFFER and TRANSMISSION_BUFFER are parameters both should have same corresponding value for both server and client configuration.
-> ENCRYPTION_KEY and DECRYPTION_KEY are parameters which ensure encryption of data sent over connection, see CYPHER-PROTOCOL documentation for more information.
-> TIMEOUT is the time after which a connection is closed or reset from client side or server side.
-> READPY_NODE defines the interface address at which the server will be running (IP).
-> READPY_PORT defines port number on which server runs.
+* RECV_BUFFER and TRANSMISSION_BUFFER are parameters both should have same corresponding value for both server and client configuration.
 
-> Example readpy_conf is given in CONF_FILES folder, consider that for more details.
+* ENCRYPTION_KEY and DECRYPTION_KEY are parameters which ensure encryption of data sent over connection, see CYPHER-PROTOCOL documentation for more information.
+
+* TIMEOUT is the time after which a connection is closed or reset from client side or server side.
+
+* READPY_NODE defines the interface address at which the server will be running (IP).
+
+* READPY_PORT defines port number on which server runs.
+
+* Example readpy_conf is given in CONF_FILES folder, consider that for more details.
 
 ## CLIENT USAGE
-> Put the readpy_conf.json and TEST_SCRIPT/client.py in same folder and run in same directory space.
-> Consider the following code :
+* Put the readpy_conf.json and TEST_SCRIPT/client.py in same folder and run in same directory space.
+
+* Consider the following code :
+
 ```python3
 from READPY.CLIENT.client import READPY_CLIENT
 
 if __name__ == "__main__" :
 	# INITIALISING THE READPY_CLIENT
     CLIENT = READPY_CLIENT()
 
@@ -741,16 +747,18 @@
 	# READING FROM THE LOCATION ["CONSTANTS"] FROM THE SERVER
     print(CLIENT.read(["CONSTANTS"]))
 	# READING FROM THE LOCATION ["CONSTANTS", "MATH"] FROM THE SERVER
     print(CLIENT.read(["CONSTANTS", "MATH"]))
 ```
 
 ## SERVER USAGE
-> Put the readpy_conf.json and TEST_SCRIPT/server.py in same folder and run in same directory space.
-> Consider the following code :
+* Put the readpy_conf.json and TEST_SCRIPT/server.py in same folder and run in same directory space.
+
+* Consider the following code :
+
 ```python3
 from READPY.SERVER.server import READPY_SERVER
 
 if __name__ == "__main__" :
 	# INITIALISING THE READPY_SERVER
     SERVER = READPY_SERVER()
 	# STARTING THE SERVER
```

