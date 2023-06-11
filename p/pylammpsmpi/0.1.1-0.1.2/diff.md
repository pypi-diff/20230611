# Comparing `tmp/pylammpsmpi-0.1.1.tar.gz` & `tmp/pylammpsmpi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylammpsmpi-0.1.1.tar", last modified: Wed Jun  7 15:18:09 2023, max compression
+gzip compressed data, was "pylammpsmpi-0.1.2.tar", last modified: Sun Jun 11 16:16:10 2023, max compression
```

## Comparing `pylammpsmpi-0.1.1.tar` & `pylammpsmpi-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/pylammpsmpi/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/pylammpsmpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/pylammpsmpi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/pylammpsmpi/lammps_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/pylammpsmpi/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/pylammpsmpi/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/pylammpsmpi/mpi/lmpmpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/pylammpsmpi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/pylammpsmpi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/pylammpsmpi/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    19103 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/pylammpsmpi/utils/lammps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:09.116839 pylammpsmpi-0.1.1/pylammpsmpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 15:18:09.000000 pylammpsmpi-0.1.1/pylammpsmpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-07 15:18:09.000000 pylammpsmpi-0.1.1/pylammpsmpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:18:09.000000 pylammpsmpi-0.1.1/pylammpsmpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-07 15:18:09.000000 pylammpsmpi-0.1.1/pylammpsmpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 15:18:09.000000 pylammpsmpi-0.1.1/pylammpsmpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-07 15:18:08.000000 pylammpsmpi-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:18:09.120839 pylammpsmpi-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/tests/test_pylammpsmpi_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/tests/test_pylammpsmpi_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-07 15:18:03.000000 pylammpsmpi-0.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/pylammpsmpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/pylammpsmpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/pylammpsmpi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/pylammpsmpi/lammps_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/pylammpsmpi/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/pylammpsmpi/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/pylammpsmpi/mpi/lmpmpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/pylammpsmpi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/pylammpsmpi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/pylammpsmpi/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19121 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/pylammpsmpi/utils/lammps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/pylammpsmpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-11 16:16:10.000000 pylammpsmpi-0.1.2/pylammpsmpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-11 16:16:10.000000 pylammpsmpi-0.1.2/pylammpsmpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 16:16:10.000000 pylammpsmpi-0.1.2/pylammpsmpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-11 16:16:10.000000 pylammpsmpi-0.1.2/pylammpsmpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 16:16:10.000000 pylammpsmpi-0.1.2/pylammpsmpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-11 16:16:10.000000 pylammpsmpi-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:16:10.906684 pylammpsmpi-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/tests/test_pylammpsmpi_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/tests/test_pylammpsmpi_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-11 16:16:07.000000 pylammpsmpi-0.1.2/versioneer.py
```

### Comparing `pylammpsmpi-0.1.1/LICENSE` & `pylammpsmpi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.1/PKG-INFO` & `pylammpsmpi-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylammpsmpi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Parallel Lammps Python interface
 Home-page: https://github.com/pyiron/pylammpsmpi
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: lammps,mpi4py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pylammpsmpi-0.1.1/README.md` & `pylammpsmpi-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.1/pylammpsmpi/lammps_wrapper.py` & `pylammpsmpi-0.1.2/pylammpsmpi/lammps_wrapper.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.1/pylammpsmpi/mpi/lmpmpi.py` & `pylammpsmpi-0.1.2/pylammpsmpi/mpi/lmpmpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -475,22 +475,24 @@
         if MPI.COMM_WORLD.rank == 0:
             input_dict = cloudpickle.loads(socket.recv())
             # with open('process.txt', 'a') as file:
             #     print('Input:', input_dict, file=file)
         else:
             input_dict = None
         input_dict = MPI.COMM_WORLD.bcast(input_dict, root=0)
-        if input_dict["c"] == "close":
+        if "shutdown" in input_dict.keys() and input_dict["shutdown"]:
             if MPI.COMM_WORLD.rank == 0:
                 socket.close()
                 context.term()
             job.close()
             break
-        output = select_cmd(input_dict["c"])(job=job, funct_args=input_dict["d"])
+        output = select_cmd(input_dict["command"])(
+            job=job, funct_args=input_dict["args"]
+        )
         if MPI.COMM_WORLD.rank == 0 and output is not None:
             # with open('process.txt', 'a') as file:
             #     print('Output:', output, file=file)
-            socket.send(cloudpickle.dumps({"r": output}))
+            socket.send(cloudpickle.dumps({"result": output}))
 
 
 if __name__ == "__main__":
     _run_lammps_mpi(argument_lst=sys.argv)
```

### Comparing `pylammpsmpi-0.1.1/pylammpsmpi/utils/commands.py` & `pylammpsmpi-0.1.2/pylammpsmpi/utils/commands.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.1/pylammpsmpi/utils/lammps.py` & `pylammpsmpi-0.1.2/pylammpsmpi/utils/lammps.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         ]
         if self._cmdargs is not None:
             cmds.extend(self._cmdargs)
         self._interface.bootup(command_lst=cmds, cwd=self.working_directory)
 
     def _send_and_receive_dict(self, command, data=None):
         return self._interface.send_and_receive_dict(
-            input_dict={"c": command, "d": data}
+            input_dict={"command": command, "args": data}
         )
 
     def _send(self, command, data=None):
         """
         Send a command to the Lammps Library executable
 
         Parameters
@@ -66,15 +66,15 @@
         data: optional, default None
             data to be sent to the command
 
         Returns
         -------
         None
         """
-        self._interface.send_dict({"c": command, "d": data})
+        self._interface.send_dict({"command": command, "args": data})
 
     def _receive(self):
         """
         Receive data from the Lammps library
 
         Parameters
         ----------
```

### Comparing `pylammpsmpi-0.1.1/pylammpsmpi.egg-info/PKG-INFO` & `pylammpsmpi-0.1.2/pylammpsmpi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylammpsmpi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Parallel Lammps Python interface
 Home-page: https://github.com/pyiron/pylammpsmpi
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: lammps,mpi4py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pylammpsmpi-0.1.1/pylammpsmpi.egg-info/SOURCES.txt` & `pylammpsmpi-0.1.2/pylammpsmpi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.1/setup.py` & `pylammpsmpi-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,11 +22,11 @@
                  'Programming Language :: Python :: 3.10',
                  'Programming Language :: Python :: 3.11'
                 ],
 
     keywords='lammps, mpi4py',
     packages=find_packages(exclude=["*tests*"]),
     install_requires=[
-        "cloudpickle>=2.2.1", "mpi4py>=3.1.4", "pympipool>=0.4.2", "pyzmq>=25.1.0",
+        "cloudpickle>=2.2.1", "mpi4py>=3.1.4", "pympipool>=0.5.0", "pyzmq>=25.1.0",
     ],
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `pylammpsmpi-0.1.1/tests/test_pylammpsmpi_cluster.py` & `pylammpsmpi-0.1.2/tests/test_pylammpsmpi_cluster.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.1/tests/test_pylammpsmpi_local.py` & `pylammpsmpi-0.1.2/tests/test_pylammpsmpi_local.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.1.1/versioneer.py` & `pylammpsmpi-0.1.2/versioneer.py`

 * *Files identical despite different names*

