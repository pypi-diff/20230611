# Comparing `tmp/bhv-0.5.6.tar.gz` & `tmp/bhv-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.5.6.tar", last modified: Sat Jun 10 23:28:24 2023, max compression
+gzip compressed data, was "bhv-0.5.7.tar", last modified: Sun Jun 11 00:58:32 2023, max compression
```

## Comparing `bhv-0.5.6.tar` & `bhv-0.5.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-10 23:28:24.702582 bhv-0.5.6/
--rw-r--r--   0 adam      (1000) adam      (1000)    35149 2023-05-25 19:11:00.000000 bhv-0.5.6/LICENSE
--rw-r--r--   0 adam      (1000) adam      (1000)     1091 2023-06-10 23:28:24.701583 bhv-0.5.6/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)     3989 2023-06-08 12:48:26.000000 bhv-0.5.6/README.md
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-10 23:28:24.701583 bhv-0.5.6/bhv/
--rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.5.6/bhv/__init__.py
--rw-r--r--   0 adam      (1000) adam      (1000)    14829 2023-06-06 19:12:06.000000 bhv-0.5.6/bhv/abstract.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-10 23:28:24.701583 bhv-0.5.6/bhv/cnative/
--rw-r--r--   0 adam      (1000) adam      (1000)     8830 2023-06-10 21:53:26.000000 bhv-0.5.6/bhv/cnative/bindings.cpp
--rw-r--r--   0 adam      (1000) adam      (1000)     2120 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/embedding.py
--rw-r--r--   0 adam      (1000) adam      (1000)     4220 2023-06-06 19:12:06.000000 bhv-0.5.6/bhv/lookup.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1115 2023-06-10 22:42:14.000000 bhv-0.5.6/bhv/native.py
--rw-r--r--   0 adam      (1000) adam      (1000)    11951 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/np.py
--rw-r--r--   0 adam      (1000) adam      (1000)    11425 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/poibin.py
--rw-r--r--   0 adam      (1000) adam      (1000)     8293 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/pytorch.py
--rw-r--r--   0 adam      (1000) adam      (1000)     3360 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/shared.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1195 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/slice.py
--rw-r--r--   0 adam      (1000) adam      (1000)    26226 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/symbolic.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1747 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/unification.py
--rw-r--r--   0 adam      (1000) adam      (1000)     3456 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/vanilla.py
--rw-r--r--   0 adam      (1000) adam      (1000)      782 2023-05-25 19:11:00.000000 bhv-0.5.6/bhv/visualization.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-10 23:28:24.701583 bhv-0.5.6/bhv.egg-info/
--rw-r--r--   0 adam      (1000) adam      (1000)     1091 2023-06-10 23:28:24.000000 bhv-0.5.6/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)      399 2023-06-10 23:28:24.000000 bhv-0.5.6/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-06-10 23:28:24.000000 bhv-0.5.6/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       45 2023-06-10 23:28:24.000000 bhv-0.5.6/bhv.egg-info/requires.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-06-10 23:28:24.000000 bhv-0.5.6/bhv.egg-info/top_level.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-06-10 23:28:24.702582 bhv-0.5.6/setup.cfg
--rw-r--r--   0 adam      (1000) adam      (1000)     1565 2023-06-10 21:52:04.000000 bhv-0.5.6/setup.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 00:58:32.537017 bhv-0.5.7/
+-rw-r--r--   0 adam      (1000) adam      (1000)    35149 2023-05-25 19:11:00.000000 bhv-0.5.7/LICENSE
+-rw-r--r--   0 adam      (1000) adam      (1000)     1091 2023-06-11 00:58:32.536017 bhv-0.5.7/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)     3989 2023-06-08 12:48:26.000000 bhv-0.5.7/README.md
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 00:58:32.536017 bhv-0.5.7/bhv/
+-rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.5.7/bhv/__init__.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    14829 2023-06-06 19:12:06.000000 bhv-0.5.7/bhv/abstract.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 00:58:32.536017 bhv-0.5.7/bhv/cnative/
+-rw-r--r--   0 adam      (1000) adam      (1000)     9757 2023-06-11 00:54:32.000000 bhv-0.5.7/bhv/cnative/bindings.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)     2120 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/embedding.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     4220 2023-06-06 19:12:06.000000 bhv-0.5.7/bhv/lookup.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1476 2023-06-11 00:46:52.000000 bhv-0.5.7/bhv/native.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    11951 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/np.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    11425 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/poibin.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     8293 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/pytorch.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     3360 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/shared.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1195 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/slice.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    26226 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/symbolic.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1747 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/unification.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     3456 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/vanilla.py
+-rw-r--r--   0 adam      (1000) adam      (1000)      782 2023-05-25 19:11:00.000000 bhv-0.5.7/bhv/visualization.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 00:58:32.536017 bhv-0.5.7/bhv.egg-info/
+-rw-r--r--   0 adam      (1000) adam      (1000)     1091 2023-06-11 00:58:32.000000 bhv-0.5.7/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)      399 2023-06-11 00:58:32.000000 bhv-0.5.7/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-06-11 00:58:32.000000 bhv-0.5.7/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       45 2023-06-11 00:58:32.000000 bhv-0.5.7/bhv.egg-info/requires.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-06-11 00:58:32.000000 bhv-0.5.7/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-06-11 00:58:32.537017 bhv-0.5.7/setup.cfg
+-rw-r--r--   0 adam      (1000) adam      (1000)     1565 2023-06-11 00:55:47.000000 bhv-0.5.7/setup.py
```

### Comparing `bhv-0.5.6/LICENSE` & `bhv-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.5.6/PKG-INFO` & `bhv-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.5.6
+Version: 0.5.7
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
 Platform: UNKNOWN
```

### Comparing `bhv-0.5.6/README.md` & `bhv-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `bhv-0.5.6/bhv/abstract.py` & `bhv-0.5.7/bhv/abstract.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.6/bhv/cnative/bindings.cpp` & `bhv-0.5.7/bhv/cnative/bindings.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 static PyObject *BHV_rand(PyTypeObject *type, PyObject *Py_UNUSED(ignored));
 static PyObject *BHV_random(PyTypeObject *type, PyObject *args);
 
 static PyObject *BHV_majority(PyTypeObject *type, PyObject *args);
 
 static PyObject *BHV_representative(PyTypeObject *type, PyObject *args);
 
-static PyObject *BHV_select(BHV *v1, PyObject *args);
+static PyObject *BHV_select(BHV *cond, PyObject *args);
+static PyObject *BHV_permute(BHV *v1, PyObject *args);
 
 static PyObject *BHV_eq(BHV *v1, PyObject *args);
 static PyObject *BHV_richcompare(PyObject *self, PyObject *other, int op) {
     switch (op) {
         case Py_EQ: if (bhv::eq(((BHV*)self)->data, ((BHV*)other)->data)) Py_RETURN_TRUE; else Py_RETURN_FALSE;
         case Py_NE: if (bhv::eq(((BHV*)self)->data, ((BHV*)other)->data)) Py_RETURN_FALSE; else Py_RETURN_TRUE;
         default:
@@ -68,14 +69,16 @@
                 "Bernoulli p distributed bit vector"},
         {"majority", (PyCFunction) BHV_majority,  METH_CLASS | METH_VARARGS,
                 "The majority of a list of BHVs"},
         {"representative", (PyCFunction) BHV_representative, METH_CLASS | METH_VARARGS,
                 "Random representative of a list of BHVs"},
         {"select",         (PyCFunction) BHV_select,         METH_VARARGS,
                 "MUX or IF-THEN-ELSE"},
+        {"permute",         (PyCFunction) BHV_permute,         METH_VARARGS,
+                "Word-level permutation"},
         {"eq",         (PyCFunction) BHV_eq,         METH_VARARGS,
                 "Check equality"},
         {"hamming",         (PyCFunction) BHV_hamming,         METH_VARARGS,
                 "Hamming distance between two BHVs"},
         {"active",         (PyCFunction) BHV_active,     METH_NOARGS,
                 "Count the number of active bits"},
         {nullptr}
@@ -96,14 +99,15 @@
         .tp_dealloc = (destructor) BHV_dealloc,
         .tp_as_number = &BHV_nb_methods,
         .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE,
         .tp_doc = "Packed, native implementation of Boolean Hypervectors",
         .tp_richcompare = BHV_richcompare,
         .tp_methods = BHV_methods,
         .tp_members = BHV_members,
+        .tp_dict = PyDict_New(),
         .tp_init = (initproc) BHV_init,
         .tp_new = BHV_new,
 };
 
 
 static PyObject *BHV_rand(PyTypeObject *type, PyObject *Py_UNUSED(ignored)) {
     PyObject * v = BHV_new(type, nullptr, nullptr);
@@ -238,14 +242,25 @@
         return nullptr;
 
     PyObject * ret = BHV_new(&BHVType, nullptr, nullptr);
     bhv::select_into(cond->data, when1->data, when0->data, ((BHV *) ret)->data);
     return ret;
 }
 
+static PyObject *BHV_permute(BHV *cond, PyObject *args) {
+    int32_t perm;
+
+    if (!PyArg_ParseTuple(args, "i", &perm))
+        return nullptr;
+
+    PyObject * ret = BHV_new(&BHVType, nullptr, nullptr);
+    bhv::permute_into(cond->data, perm, ((BHV *) ret)->data);
+    return ret;
+}
+
 static PyObject *dimension(PyObject * self, PyObject * args, PyObject * kwds) {
     return PyLong_FromLong(BITS);
 }
 
 
 static PyMethodDef module_methods[] = {
         {"_DIMENSION", (PyCFunction) dimension, METH_NOARGS,
@@ -272,14 +287,24 @@
     if (PyType_Ready(&BHVType) < 0)
         return nullptr;
 
     m = PyModule_Create(&cModPyDem);
     if (m == nullptr)
         return nullptr;
 
+    BHV *z = (BHV*) BHVType.tp_alloc(&BHVType, 0);
+    z->data = bhv::zero();
+    PyDict_SetItemString(BHVType.tp_dict, "ZERO", (PyObject *)z);
+    BHV *o = (BHV*) BHVType.tp_alloc(&BHVType, 0);
+    o->data = bhv::one();
+    PyDict_SetItemString(BHVType.tp_dict, "ONE", (PyObject *)o);
+    BHV *h = (BHV*) BHVType.tp_alloc(&BHVType, 0);
+    h->data = bhv::half();
+    PyDict_SetItemString(BHVType.tp_dict, "HALF", (PyObject *)h);
+
     Py_INCREF(&BHVType);
     PyModule_AddObject(m, "CNativePackedBHV", (PyObject *) &BHVType);
 
     return m;
 };
```

### Comparing `bhv-0.5.6/bhv/embedding.py` & `bhv-0.5.7/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.6/bhv/lookup.py` & `bhv-0.5.7/bhv/lookup.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.6/bhv/native.py` & `bhv-0.5.7/bhv/native.py`

 * *Files 24% similar despite different names*

```diff
@@ -37,7 +37,16 @@
 
     def active(self):
         return self.ins.active()
 
     def hamming(self, other):
         return self.ins.hamming(other.ins)
 
+    def permute(self, permutation_id: int):
+        return NativePackedBHV(self.ins.permute(permutation_id))
+
+    def __eq__(self, other):
+        return self.ins == other.ins
+
+NativePackedBHV.ZERO = NativePackedBHV(CNativePackedBHV.ZERO)
+NativePackedBHV.ONE = NativePackedBHV(CNativePackedBHV.ONE)
+NativePackedBHV.HALF = NativePackedBHV(CNativePackedBHV.HALF)
```

### Comparing `bhv-0.5.6/bhv/np.py` & `bhv-0.5.7/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.6/bhv/poibin.py` & `bhv-0.5.7/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.6/bhv/pytorch.py` & `bhv-0.5.7/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.6/bhv/shared.py` & `bhv-0.5.7/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.6/bhv/slice.py` & `bhv-0.5.7/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.6/bhv/symbolic.py` & `bhv-0.5.7/bhv/symbolic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.6/bhv/unification.py` & `bhv-0.5.7/bhv/unification.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.6/bhv/vanilla.py` & `bhv-0.5.7/bhv/vanilla.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.6/bhv/visualization.py` & `bhv-0.5.7/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.6/bhv.egg-info/PKG-INFO` & `bhv-0.5.7/bhv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.5.6
+Version: 0.5.7
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
 Platform: UNKNOWN
```

### Comparing `bhv-0.5.6/setup.py` & `bhv-0.5.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages, Extension
 
-VERSION = '0.5.6'
+VERSION = '0.5.7'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 native = Extension("bhv.cnative", sources=['bhv/cnative/bindings.cpp'],
                    extra_compile_args=['-std=c++20', '-O3', '-march=native'],
                    language='c++')
 setup(
```

