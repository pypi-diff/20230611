# Comparing `tmp/pympipool-0.4.2.tar.gz` & `tmp/pympipool-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.4.2.tar", last modified: Wed Jun  7 05:16:59 2023, max compression
+gzip compressed data, was "pympipool-0.5.0.tar", last modified: Sun Jun 11 14:13:06 2023, max compression
```

## Comparing `pympipool-0.4.2.tar` & `pympipool-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:59.527638 pympipool-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-07 05:16:56.000000 pympipool-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-07 05:16:56.000000 pympipool-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-07 05:16:59.527638 pympipool-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-07 05:16:56.000000 pympipool-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:59.527638 pympipool-0.4.2/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-07 05:16:59.527638 pympipool-0.4.2/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:59.523638 pympipool-0.4.2/pympipool/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/executor/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/executor/mpipool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:59.523638 pympipool-0.4.2/pympipool/share/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/share/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/share/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-07 05:16:56.000000 pympipool-0.4.2/pympipool/share/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:59.523638 pympipool-0.4.2/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-07 05:16:59.000000 pympipool-0.4.2/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-07 05:16:59.000000 pympipool-0.4.2/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 05:16:59.000000 pympipool-0.4.2/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 05:16:59.000000 pympipool-0.4.2/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 05:16:59.000000 pympipool-0.4.2/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-07 05:16:59.527638 pympipool-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-07 05:16:59.000000 pympipool-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:16:59.527638 pympipool-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-07 05:16:56.000000 pympipool-0.4.2/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-07 05:16:56.000000 pympipool-0.4.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:06.544708 pympipool-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-11 14:13:03.000000 pympipool-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-11 14:13:03.000000 pympipool-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-06-11 14:13:06.544708 pympipool-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-06-11 14:13:03.000000 pympipool-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:06.544708 pympipool-0.5.0/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-11 14:13:06.544708 pympipool-0.5.0/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:06.540708 pympipool-0.5.0/pympipool/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/executor/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/executor/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:06.540708 pympipool-0.5.0/pympipool/share/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/share/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/share/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/share/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/share/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/share/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:06.540708 pympipool-0.5.0/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-06-11 14:13:06.000000 pympipool-0.5.0/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-11 14:13:06.000000 pympipool-0.5.0/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 14:13:06.000000 pympipool-0.5.0/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-11 14:13:06.000000 pympipool-0.5.0/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 14:13:06.000000 pympipool-0.5.0/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-11 14:13:06.544708 pympipool-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-11 14:13:06.000000 pympipool-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:06.544708 pympipool-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-11 14:13:03.000000 pympipool-0.5.0/versioneer.py
```

### Comparing `pympipool-0.4.2/LICENSE` & `pympipool-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.2/pympipool/executor/mpiexec.py` & `pympipool-0.5.0/pympipool/executor/mpiexec.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
     MPI.pickle.__init__(
         cloudpickle.dumps,
         cloudpickle.loads,
         pickle.HIGHEST_PROTOCOL,
     )
     mpi_rank_zero = MPI.COMM_WORLD.Get_rank() == 0
+    mpi_size_larger_one = MPI.COMM_WORLD.Get_size() > 1
 
     argument_dict = parse_arguments(argument_lst=sys.argv)
     if mpi_rank_zero:
         context, socket = initialize_zmq(
             host=argument_dict["host"], port=argument_dict["zmqport"]
         )
     else:
@@ -31,35 +32,47 @@
         if mpi_rank_zero:
             input_dict = cloudpickle.loads(socket.recv())
         else:
             input_dict = None
         input_dict = MPI.COMM_WORLD.bcast(input_dict, root=0)
 
         # Parse input
-        if "c" in input_dict.keys() and input_dict["c"] == "close":
+        if "shutdown" in input_dict.keys() and input_dict["shutdown"]:
             if mpi_rank_zero:
                 socket.close()
                 context.term()
             break
         elif (
-            "f" in input_dict.keys()
-            and "i" not in input_dict.keys()
-            and "a" in input_dict.keys()
-            and "k" in input_dict.keys()
+            "fn" in input_dict.keys()
+            and "init" not in input_dict.keys()
+            and "args" in input_dict.keys()
+            and "kwargs" in input_dict.keys()
         ):
             # Execute function
-            output = call_funct(input_dict=input_dict, funct=None, memory=memory)
-            output_reply = MPI.COMM_WORLD.gather(output, root=0)
-
-            # Send output
-            if mpi_rank_zero:
-                socket.send(cloudpickle.dumps({"r": output_reply}))
+            try:
+                output = call_funct(input_dict=input_dict, funct=None, memory=memory)
+                if mpi_size_larger_one:
+                    output_reply = MPI.COMM_WORLD.gather(output, root=0)
+                else:
+                    output_reply = output
+            except Exception as error:
+                if mpi_rank_zero:
+                    socket.send(
+                        cloudpickle.dumps(
+                            {"error": error, "error_type": str(type(error))}
+                        )
+                    )
+            else:
+                # Send output
+                if mpi_rank_zero:
+                    socket.send(cloudpickle.dumps({"result": output_reply}))
         elif (
-            "i" in input_dict.keys()
-            and input_dict["i"]
-            and ("a" in input_dict.keys() or "k" in input_dict.keys())
+            "init" in input_dict.keys()
+            and input_dict["init"]
+            and "args" in input_dict.keys()
+            and "kwargs" in input_dict.keys()
         ):
             memory = call_funct(input_dict=input_dict, funct=None)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pympipool-0.4.2/pympipool/executor/mpipool.py` & `pympipool-0.5.0/pympipool/executor/mpipool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.2/pympipool/share/communication.py` & `pympipool-0.5.0/pympipool/share/communication.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,19 @@
         self._process = None
 
     def send_dict(self, input_dict):
         self._socket.send(cloudpickle.dumps(input_dict))
 
     def receive_dict(self):
         output = cloudpickle.loads(self._socket.recv())
-        if "r" in output.keys():
-            return output["r"]
+        if "result" in output.keys():
+            return output["result"]
         else:
-            error_type = output["et"].split("'")[1]
-            raise eval(error_type)(output["e"])
+            error_type = output["error_type"].split("'")[1]
+            raise eval(error_type)(output["error"])
 
     def send_and_receive_dict(self, input_dict):
         self.send_dict(input_dict=input_dict)
         return self.receive_dict()
 
     def bind_to_random_port(self):
         return self._socket.bind_to_random_port("tcp://*")
@@ -35,15 +35,15 @@
             stderr=subprocess.PIPE,
             stdin=subprocess.PIPE,
             cwd=cwd,
         )
 
     def shutdown(self, wait=True):
         if self._process is not None and self._process.poll() is None:
-            self.send_dict(input_dict={"c": "close"})
+            self.send_dict(input_dict={"shutdown": True})
             self._process_close(wait=wait)
         if self._socket is not None:
             self._socket.close()
         if self._context is not None:
             self._context.term()
         self._process = None
         self._socket = None
```

### Comparing `pympipool-0.4.2/pympipool/share/parallel.py` & `pympipool-0.5.0/pympipool/share/executor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,118 +1,131 @@
-import inspect
-import zmq
-from tqdm import tqdm
-
-
-def parse_arguments(argument_lst):
-    argument_dict = {
-        "total_cores": "--cores-total",
-        "zmqport": "--zmqport",
-        "cores_per_task": "--cores-per-task",
-        "host": "--host",
-    }
-    parse_dict = {"host": "localhost"}
-    parse_dict.update(
-        {
-            k: argument_lst[argument_lst.index(v) + 1]
-            for k, v in argument_dict.items()
-            if v in argument_lst
-        }
-    )
-    return parse_dict
-
-
-def initialize_zmq(host, port):
-    context = zmq.Context()
-    socket = context.socket(zmq.PAIR)
-    socket.connect("tcp://" + host + ":" + port)
-    return context, socket
-
-
-def wrap(funct, number_of_cores_per_communicator):
-    def functwrapped(*args, **kwargs):
-        from mpi4py import MPI
-
-        MPI.COMM_WORLD.Barrier()
-        rank = MPI.COMM_WORLD.Get_rank()
-        comm_new = MPI.COMM_WORLD.Split(
-            rank // number_of_cores_per_communicator,
-            rank % number_of_cores_per_communicator,
+from concurrent.futures import Executor as FutureExecutor, Future
+from queue import Queue
+from threading import Thread
+
+from pympipool.share.serial import (
+    execute_parallel_tasks,
+    execute_serial_tasks,
+    cloudpickle_register,
+    cancel_items_in_queue,
+)
+
+
+class ExecutorBase(FutureExecutor):
+    def __init__(self):
+        self._future_queue = Queue()
+        self._process = None
+        cloudpickle_register(ind=3)
+
+    def submit(self, fn, *args, **kwargs):
+        """Submits a callable to be executed with the given arguments.
+
+        Schedules the callable to be executed as fn(*args, **kwargs) and returns
+        a Future instance representing the execution of the callable.
+
+        Returns:
+            A Future representing the given call.
+        """
+        f = Future()
+        self._future_queue.put({"fn": fn, "args": args, "kwargs": kwargs, "future": f})
+        return f
+
+    def shutdown(self, wait=True, *, cancel_futures=False):
+        """Clean-up the resources associated with the Executor.
+
+        It is safe to call this method several times. Otherwise, no other
+        methods can be called after this one.
+
+        Args:
+            wait: If True then shutdown will not return until all running
+                futures have finished executing and the resources used by the
+                executor have been reclaimed.
+            cancel_futures: If True then shutdown will cancel all pending
+                futures. Futures that are completed or running will not be
+                cancelled.
+        """
+        if cancel_futures:
+            cancel_items_in_queue(que=self._future_queue)
+        self._future_queue.put({"shutdown": True})
+        self._process.join()
+
+    def __len__(self):
+        return self._future_queue.qsize()
+
+
+class Executor(ExecutorBase):
+    """
+    The pympipool.Executor behaves like the concurrent.futures.Executor but it uses mpi4py to execute parallel tasks.
+    In contrast to the mpi4py.futures.MPIPoolExecutor the pympipool.Executor can be executed in a serial python process
+    and does not require the python script to be executed with MPI. Still internally the pympipool.Executor uses the
+    mpi4py.futures.MPIPoolExecutor, consequently it is primarily an abstraction of its functionality to improve the
+    usability in particular when used in combination with Jupyter notebooks.
+
+    Args:
+        cores (int): defines the number of MPI ranks to use for each function call
+        oversubscribe (bool): adds the `--oversubscribe` command line flag (OpenMPI only) - default False
+        enable_flux_backend (bool): use the flux-framework as backend rather than just calling mpiexec
+        init_function (None): optional function to preset arguments for functions which are submitted later
+        cwd (str/None): current working directory where the parallel python task is executed
+
+    Simple example:
+        ```
+        import numpy as np
+        from pympipool import Executor
+
+        def calc(i, j, k):
+            from mpi4py import MPI
+            size = MPI.COMM_WORLD.Get_size()
+            rank = MPI.COMM_WORLD.Get_rank()
+            return np.array([i, j, k]), size, rank
+
+        def init_k():
+            return {"k": 3}
+
+        with Executor(cores=2, init_function=init_k) as p:
+            fs = p.submit(calc, 2, j=4)
+            print(fs.result())
+
+        >>> [(array([2, 4, 3]), 2, 0), (array([2, 4, 3]), 2, 1)]
+        ```
+    """
+
+    def __init__(
+        self,
+        cores,
+        oversubscribe=False,
+        enable_flux_backend=False,
+        init_function=None,
+        cwd=None,
+    ):
+        super().__init__()
+        self._process = Thread(
+            target=execute_parallel_tasks,
+            args=(self._future_queue, cores, oversubscribe, enable_flux_backend, cwd),
         )
-        comm_new.Barrier()
-        return funct(*args, comm=comm_new, **kwargs)
-
-    return functwrapped
+        self._process.start()
+        if init_function is not None:
+            self._future_queue.put(
+                {"init": True, "fn": init_function, "args": (), "kwargs": {}}
+            )
 
 
-def map_funct(executor, funct, lst, cores_per_task):
-    if cores_per_task == 1:
-        results = executor.map(funct, lst)
-        return list(tqdm(results, desc="Tasks", total=len(lst)))
-    else:
-        lst_parallel = []
-        for input_parameter in lst:
-            for _ in range(cores_per_task):
-                lst_parallel.append(input_parameter)
-        results = executor.map(
-            wrap(funct=funct, number_of_cores_per_communicator=cores_per_task),
-            lst_parallel,
-        )
-        return list(tqdm(results, desc="Tasks", total=len(lst_parallel)))[
-            ::cores_per_task
-        ]
-
-
-def call_funct(input_dict, funct=None, memory=None):
-    if funct is None:
-
-        def funct(*args, **kwargs):
-            return args[0].__call__(*args[1:], **kwargs)
-
-    funct_args = inspect.getfullargspec(input_dict["f"]).args
-    if memory is not None:
-        input_dict["k"].update({k: v for k, v in memory.items() if k in funct_args})
-
-    return funct(input_dict["f"], *input_dict["a"], **input_dict["k"])
-
-
-def parse_socket_communication(executor, input_dict, future_dict, cores_per_task):
-    if "c" in input_dict.keys() and input_dict["c"] == "close":
-        # If close "c" is communicated the process is shutdown.
-        return "exit"
-    elif "f" in input_dict.keys() and "l" in input_dict.keys():
-        # If a function "f" and a list or arguments "l" are communicated,
-        # pympipool uses the map() function to apply the function on the list.
-        try:
-            output = map_funct(
-                executor=executor,
-                funct=input_dict["f"],
-                lst=input_dict["l"],
-                cores_per_task=cores_per_task,
-            )
-        except Exception as error:
-            return {"e": error, "et": str(type(error))}
-        else:
-            return {"r": output}
-    elif (
-        "f" in input_dict.keys()
-        and "a" in input_dict.keys()
-        and "k" in input_dict.keys()
+class PoolExecutor(ExecutorBase):
+    def __init__(
+        self,
+        max_workers=1,
+        oversubscribe=False,
+        enable_flux_backend=False,
+        cwd=None,
     ):
-        # If a function "f" and either arguments "a" or keyword arguments "k" are
-        # communicated pympipool uses submit() to asynchronously apply the function
-        # on the arguments and or keyword arguments.
-        future = call_funct(input_dict=input_dict, funct=executor.submit)
-        future_hash = hash(future)
-        future_dict[future_hash] = future
-        return {"r": future_hash}
-    elif "u" in input_dict.keys():
-        # If update "u" is communicated pympipool checks for asynchronously submitted
-        # functions which have completed in the meantime and communicates their results.
-        done_dict = {
-            k: f.result()
-            for k, f in {k: future_dict[k] for k in input_dict["u"]}.items()
-            if f.done()
-        }
-        for k in done_dict.keys():
-            del future_dict[k]
-        return {"r": done_dict}
+        super().__init__()
+        self._process = Thread(
+            target=execute_serial_tasks,
+            args=(
+                self._future_queue,
+                max_workers,
+                oversubscribe,
+                enable_flux_backend,
+                cwd,
+            ),
+        )
+        self._process.start()
```

### Comparing `pympipool-0.4.2/pympipool.egg-info/SOURCES.txt` & `pympipool-0.5.0/pympipool.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -12,19 +12,23 @@
 pympipool.egg-info/requires.txt
 pympipool.egg-info/top_level.txt
 pympipool/executor/__init__.py
 pympipool/executor/mpiexec.py
 pympipool/executor/mpipool.py
 pympipool/share/__init__.py
 pympipool/share/communication.py
+pympipool/share/executor.py
 pympipool/share/parallel.py
+pympipool/share/pool.py
 pympipool/share/serial.py
 tests/test_communicator_split.py
 tests/test_executor.py
 tests/test_future.py
 tests/test_interface.py
+tests/test_multitask.py
 tests/test_parse.py
 tests/test_pool.py
+tests/test_queue.py
 tests/test_task.py
 tests/test_worker.py
 tests/test_worker_memory.py
 tests/test_zmq.py
```

### Comparing `pympipool-0.4.2/setup.py` & `pympipool-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 import versioneer
 
 
 setup(
     name='pympipool',
     version=versioneer.get_version(),
-    description='pympipool - scale functions over multiple compute nodes using mpi4py',
+    description='pympipool - scale python functions over multiple compute nodes',
     long_description=Path("README.md").read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/jan-janssen/pympipool',
     author_email='jan.janssen@outlook.com',
     license='BSD',
 
     classifiers=[
```

### Comparing `pympipool-0.4.2/tests/test_future.py` & `pympipool-0.5.0/tests/test_future.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import numpy as np
 import unittest
 from time import sleep
-from pympipool import Pool
+from pympipool import Executor
 from concurrent.futures import Future
 
 
 def calc(i):
     return np.array(i ** 2)
 
 
 class TestFuture(unittest.TestCase):
     def test_pool_serial(self):
-        with Pool(cores=1) as p:
+        with Executor(cores=1) as p:
             output = p.submit(calc, i=2)
             self.assertTrue(isinstance(output, Future))
             self.assertFalse(output.done())
             sleep(1)
-            p.update()
         self.assertTrue(output.done())
-        self.assertEqual(output.result(), 4)
+        self.assertEqual(output.result(), np.array(4))
 
     def test_pool_serial_multi_core(self):
-        with Pool(cores=2) as p:
+        with Executor(cores=2) as p:
             output = p.submit(calc, i=2)
             self.assertTrue(isinstance(output, Future))
             self.assertFalse(output.done())
             sleep(1)
-            p.update()
         self.assertTrue(output.done())
-        self.assertEqual(output.result(), 4)
+        self.assertEqual(output.result(), [np.array(4), np.array(4)])
```

### Comparing `pympipool-0.4.2/tests/test_interface.py` & `pympipool-0.5.0/tests/test_interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import numpy as np
 import unittest
-from pympipool import _cloudpickle_update
 from pympipool.share.communication import SocketInterface
-from pympipool.share.serial import get_parallel_subprocess_command
+from pympipool.share.serial import get_parallel_subprocess_command, cloudpickle_register
 
 
 def calc(i):
     return np.array(i ** 2)
 
 
 class TestInterface(unittest.TestCase):
     def test_interface(self):
-        _cloudpickle_update(ind=1)
-        task_dict = {"f": calc, 'a': (), "k": {"i": 2}}
+        cloudpickle_register(ind=1)
+        task_dict = {"fn": calc, 'args': (), "kwargs": {"i": 2}}
         interface = SocketInterface()
         interface.bootup(
             command_lst=get_parallel_subprocess_command(
                 port_selected=interface.bind_to_random_port(),
                 cores=1,
                 cores_per_task=1,
                 oversubscribe=False,
```

### Comparing `pympipool-0.4.2/tests/test_parse.py` & `pympipool-0.5.0/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.2/tests/test_pool.py` & `pympipool-0.5.0/tests/test_pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,58 +3,74 @@
 from pympipool import Pool
 
 
 def calc(i):
     return np.array(i ** 2)
 
 
+def calc_add(i, j):
+    return i + j
+
+
 def calc_none(i):
     return None
 
 
 def calc_error_value_error(i):
     raise ValueError("calc_error value error")
 
 
 def calc_error_type_error(i):
     raise TypeError("calc_error value error")
 
 
 class TestPool(unittest.TestCase):
-    def test_pool_serial(self):
-        with Pool(cores=1) as p:
-            output = p.map(fn=calc, iterables=[1, 2, 3, 4])
+    def test_map_serial(self):
+        with Pool(max_workers=1) as p:
+            output = p.map(func=calc, iterable=[1, 2, 3, 4])
         self.assertEqual(output[0], 1)
         self.assertEqual(output[1], 4)
         self.assertEqual(output[2], 9)
         self.assertEqual(output[3], 16)
 
-    def test_pool_parallel(self):
-        with Pool(cores=2) as p:
-            output = p.map(fn=calc, iterables=[1, 2, 3, 4])
+    def test_starmap_serial(self):
+        with Pool(max_workers=1) as p:
+            output = p.starmap(func=calc_add, iterable=[[1, 2], [3, 4]])
+        self.assertEqual(output[0], 3)
+        self.assertEqual(output[1], 7)
+
+    def test_map_parallel(self):
+        with Pool(max_workers=2) as p:
+            output = p.map(func=calc, iterable=[1, 2, 3, 4])
         self.assertEqual(output[0], 1)
         self.assertEqual(output[1], 4)
         self.assertEqual(output[2], 9)
         self.assertEqual(output[3], 16)
 
+    def test_starmap_parallel(self):
+        with Pool(max_workers=2) as p:
+            output = p.starmap(func=calc_add, iterable=[[1, 2], [3, 4]])
+        self.assertEqual(output[0], 3)
+        self.assertEqual(output[1], 7)
+
     def test_pool_none(self):
-        with Pool(cores=2) as p:
-            output = p.map(fn=calc_none, iterables=[1, 2, 3, 4])
+        with Pool(max_workers=2) as p:
+            output = p.map(func=calc_none, iterable=[1, 2, 3, 4])
         self.assertEqual(output, [None, None, None, None])
 
     def test_pool_error(self):
         with self.assertRaises(ValueError):
-            with Pool(cores=2) as p:
-                p.map(fn=calc_error_value_error, iterables=[1, 2, 3, 4])
+            with Pool(max_workers=2) as p:
+                p.map(func=calc_error_value_error, iterable=[1, 2, 3, 4])
         with self.assertRaises(TypeError):
-            with Pool(cores=2) as p:
-                p.map(fn=calc_error_type_error, iterables=[1, 2, 3, 4])
+            with Pool(max_workers=2) as p:
+                p.map(func=calc_error_type_error, iterable=[1, 2, 3, 4])
 
     def test_shutdown(self):
-        p = Pool(cores=1)
-        output = p.map(fn=calc, iterables=[1, 2, 3, 4])
+        p = Pool(max_workers=1)
+        output = p.map(func=calc, iterable=[1, 2, 3, 4])
         p.shutdown(wait=True)
         p.shutdown(wait=False)
         self.assertEqual(output[0], 1)
         self.assertEqual(output[1], 4)
         self.assertEqual(output[2], 9)
         self.assertEqual(output[3], 16)
```

### Comparing `pympipool-0.4.2/tests/test_worker.py` & `pympipool-0.5.0/tests/test_multitask.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,75 @@
 import numpy as np
 import unittest
 from queue import Queue
 from time import sleep
-from pympipool import Worker, _cloudpickle_update
-from pympipool.share.serial import execute_tasks
+from pympipool import PoolExecutor
+from pympipool.share.serial import execute_serial_tasks, cloudpickle_register
 from concurrent.futures import Future
 
 
 def calc(i):
     return np.array(i ** 2)
 
 
-def mpi_funct(i):
-    from mpi4py import MPI
-    size = MPI.COMM_WORLD.Get_size()
-    rank = MPI.COMM_WORLD.Get_rank()
-    return i, size, rank
+def sleep_one(i):
+    sleep(1)
+    return i
 
 
 class TestFuturePool(unittest.TestCase):
     def test_pool_serial(self):
-        with Worker(cores=1) as p:
+        with PoolExecutor(max_workers=1) as p:
             output = p.submit(calc, i=2)
             self.assertEqual(len(p), 1)
             self.assertTrue(isinstance(output, Future))
             self.assertFalse(output.done())
             sleep(1)
             self.assertTrue(output.done())
             self.assertEqual(len(p), 0)
         self.assertEqual(output.result(), np.array(4))
 
-    def test_pool_serial_multi_core(self):
-        with Worker(cores=2) as p:
-            output = p.submit(mpi_funct, i=2)
-            self.assertEqual(len(p), 1)
-            self.assertTrue(isinstance(output, Future))
-            self.assertFalse(output.done())
-            sleep(1)
-            self.assertTrue(output.done())
-            self.assertEqual(len(p), 0)
-        self.assertEqual(output.result(), [(2, 2, 0), (2, 2, 1)])
-
     def test_execute_task(self):
         f = Future()
         q = Queue()
-        q.put({"f": calc, 'a': (), "k": {"i": 2}, "l": f})
-        q.put({"c": "close"})
-        _cloudpickle_update(ind=1)
-        execute_tasks(
+        q.put({"fn": calc, 'args': (), "kwargs": {"i": 2}, "future": f})
+        q.put({"shutdown": True})
+        cloudpickle_register(ind=1)
+        execute_serial_tasks(
             future_queue=q,
             cores=1,
             oversubscribe=False,
             enable_flux_backend=False
         )
         self.assertEqual(f.result(), np.array(4))
 
-    def test_execute_task_parallel(self):
-        f = Future()
+    def test_pool_cancel(self):
+        with PoolExecutor(max_workers=2) as p:
+            fs1 = p.submit(sleep_one, i=2)
+            fs2 = p.submit(sleep_one, i=2)
+            fs3 = p.submit(sleep_one, i=2)
+            fs4 = p.submit(sleep_one, i=2)
+            sleep(1)
+            fs1.cancel()
+            fs2.cancel()
+            fs3.cancel()
+            fs4.cancel()
+        self.assertTrue(fs1.done())
+        self.assertTrue(fs2.done())
+        self.assertTrue(fs3.done())
+        self.assertTrue(fs4.done())
+
+    def test_cancel_task(self):
+        fs1 = Future()
+        fs1.cancel()
         q = Queue()
-        q.put({"f": calc, 'a': (), "k": {"i": 2}, "l": f})
-        q.put({"c": "close"})
-        _cloudpickle_update(ind=1)
-        execute_tasks(
+        q.put({"fn": sleep_one, 'args': (), "kwargs": {"i": 1}, "future": fs1})
+        q.put({"shutdown": True})
+        cloudpickle_register(ind=1)
+        execute_serial_tasks(
             future_queue=q,
-            cores=2,
+            cores=1,
             oversubscribe=False,
             enable_flux_backend=False
         )
-        self.assertEqual(f.result(), [np.array(4), np.array(4)])
+        self.assertTrue(fs1.done())
+        self.assertTrue(fs1.cancelled())
```

### Comparing `pympipool-0.4.2/tests/test_worker_memory.py` & `pympipool-0.5.0/tests/test_worker_memory.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import unittest
 import numpy as np
 from queue import Queue
-from pympipool import Worker, _cloudpickle_update
+from pympipool import Executor
 from pympipool.share.parallel import call_funct
-from pympipool.share.serial import execute_tasks
+from pympipool.share.serial import execute_parallel_tasks, cloudpickle_register
 from concurrent.futures import Future
 
 
 def get_global(memory=None):
     return memory
 
 
 def set_global():
     return {"memory": np.array([5])}
 
 
 class TestWorkerMemory(unittest.TestCase):
     def test_internal_memory(self):
-        with Worker(cores=1, init_function=set_global) as p:
+        with Executor(cores=1, init_function=set_global) as p:
             f = p.submit(get_global)
             self.assertFalse(f.done())
             self.assertEqual(f.result(), np.array([5]))
             self.assertTrue(f.done())
 
     def test_call_funct(self):
         self.assertEqual(call_funct(
-            input_dict={"f": get_global, "a": (), "k": {}},
+            input_dict={"fn": get_global, "args": (), "kwargs": {}},
             memory={"memory": 4}
         ), 4)
 
     def test_execute_task(self):
         f = Future()
         q = Queue()
-        q.put({"i": True, "f": set_global, "a": (), "k": {}})
-        q.put({"f": get_global, 'a': (), "k": {}, "l": f})
-        q.put({"c": "close"})
-        _cloudpickle_update(ind=1)
-        execute_tasks(
+        q.put({"init": True, "fn": set_global, "args": (), "kwargs": {}})
+        q.put({"fn": get_global, 'args': (), "kwargs": {}, "future": f})
+        q.put({"shutdown": True})
+        cloudpickle_register(ind=1)
+        execute_parallel_tasks(
             future_queue=q,
             cores=1,
             oversubscribe=False,
             enable_flux_backend=False
         )
         self.assertEqual(f.result(), np.array([5]))
```

### Comparing `pympipool-0.4.2/tests/test_zmq.py` & `pympipool-0.5.0/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.4.2/versioneer.py` & `pympipool-0.5.0/versioneer.py`

 * *Files identical despite different names*

