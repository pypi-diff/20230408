# Comparing `tmp/gencodegenes-1.0.7.tar.gz` & `tmp/gencodegenes-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gencodegenes-1.0.7.tar", last modified: Fri Apr  7 22:27:56 2023, max compression
+gzip compressed data, was "gencodegenes-1.0.8.tar", last modified: Fri Apr  7 22:53:05 2023, max compression
```

## Comparing `gencodegenes-1.0.7.tar` & `gencodegenes-1.0.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:27:56.125340 gencodegenes-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-07 22:27:56.125340 gencodegenes-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 22:27:56.125340 gencodegenes-1.0.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4444 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:27:56.121340 gencodegenes-1.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/src/gencode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/src/gencode.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:27:56.125340 gencodegenes-1.0.7/src/gencodegenes/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/src/gencodegenes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   726558 2023-04-07 22:27:55.000000 gencodegenes-1.0.7/src/gencodegenes/gencode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/src/gencodegenes/gencode.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   650679 2023-04-07 22:27:56.000000 gencodegenes-1.0.7/src/gencodegenes/transcript.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/src/gencodegenes/transcript.pxd
--rwxr-xr-x   0 runner    (1001) docker     (123)    17447 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/src/gencodegenes/transcript.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    28901 2023-04-07 22:27:56.000000 gencodegenes-1.0.7/src/gencodegenes/tx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-07 22:27:56.000000 gencodegenes-1.0.7/src/gencodegenes/tx.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:27:56.125340 gencodegenes-1.0.7/src/gencodegenes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-07 22:27:56.000000 gencodegenes-1.0.7/src/gencodegenes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-07 22:27:56.000000 gencodegenes-1.0.7/src/gencodegenes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 22:27:56.000000 gencodegenes-1.0.7/src/gencodegenes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-07 22:27:56.000000 gencodegenes-1.0.7/src/gencodegenes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-07 22:27:56.000000 gencodegenes-1.0.7/src/gencodegenes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/src/gtf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/src/gtf.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:27:56.125340 gencodegenes-1.0.7/src/gzstream/
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-04-07 22:27:55.000000 gencodegenes-1.0.7/src/gzstream/gzstream.C
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-07 22:27:19.000000 gencodegenes-1.0.7/src/gzstream/gzstream.h
--rw-r--r--   0 runner    (1001) docker     (123)    28901 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/src/tx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/src/tx.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:27:56.125340 gencodegenes-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:27:56.125340 gencodegenes-1.0.7/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    71865 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/tests/data/example.grch38.fa
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/tests/data/example.grch38.gtf
--rw-r--r--   0 runner    (1001) docker     (123)    25199 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/tests/test_gencode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/tests/test_sequence_methods.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16312 2023-04-07 22:27:18.000000 gencodegenes-1.0.7/tests/test_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:53:05.894858 gencodegenes-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-07 22:53:05.894858 gencodegenes-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 22:53:05.894858 gencodegenes-1.0.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4444 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:53:05.890858 gencodegenes-1.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/src/gencode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/src/gencode.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:53:05.890858 gencodegenes-1.0.8/src/gencodegenes/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/src/gencodegenes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   726558 2023-04-07 22:53:05.000000 gencodegenes-1.0.8/src/gencodegenes/gencode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/src/gencodegenes/gencode.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   648422 2023-04-07 22:53:05.000000 gencodegenes-1.0.8/src/gencodegenes/transcript.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/src/gencodegenes/transcript.pxd
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17355 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/src/gencodegenes/transcript.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    28901 2023-04-07 22:53:05.000000 gencodegenes-1.0.8/src/gencodegenes/tx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-07 22:53:05.000000 gencodegenes-1.0.8/src/gencodegenes/tx.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:53:05.894858 gencodegenes-1.0.8/src/gencodegenes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-07 22:53:05.000000 gencodegenes-1.0.8/src/gencodegenes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-07 22:53:05.000000 gencodegenes-1.0.8/src/gencodegenes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 22:53:05.000000 gencodegenes-1.0.8/src/gencodegenes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-07 22:53:05.000000 gencodegenes-1.0.8/src/gencodegenes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-07 22:53:05.000000 gencodegenes-1.0.8/src/gencodegenes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/src/gtf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/src/gtf.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:53:05.894858 gencodegenes-1.0.8/src/gzstream/
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-04-07 22:53:04.000000 gencodegenes-1.0.8/src/gzstream/gzstream.C
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-07 22:52:21.000000 gencodegenes-1.0.8/src/gzstream/gzstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28901 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/src/tx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/src/tx.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:53:05.894858 gencodegenes-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:53:05.894858 gencodegenes-1.0.8/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    71865 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/tests/data/example.grch38.fa
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/tests/data/example.grch38.gtf
+-rw-r--r--   0 runner    (1001) docker     (123)    25199 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/tests/test_gencode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/tests/test_sequence_methods.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16314 2023-04-07 22:52:19.000000 gencodegenes-1.0.8/tests/test_transcript.py
```

### Comparing `gencodegenes-1.0.7/LICENSE.txt` & `gencodegenes-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/PKG-INFO` & `gencodegenes-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gencodegenes
-Version: 1.0.7
+Version: 1.0.8
 Summary: Package to load genes from GENCODE GTF files
 Home-page: https://github.com/jeremymcrae/gencodegenes
 Author: Jeremy McRae
 Author-email: jeremy.mcrae@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `gencodegenes-1.0.7/README.md` & `gencodegenes-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/setup.py` & `gencodegenes-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,22 +108,22 @@
 shutil.copy("src/tx.h", "src/gencodegenes/tx.h")
 shutil.copy("src/tx.cpp", "src/gencodegenes/tx.cpp")
 
 setup(name="gencodegenes",
     description='Package to load genes from GENCODE GTF files',
     long_description=io.open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
-    version="1.0.7",
+    version="1.0.8",
     author="Jeremy McRae",
     author_email="jeremy.mcrae@gmail.com",
     license="MIT",
     url='https://github.com/jeremymcrae/gencodegenes',
     packages=["gencodegenes"],
     install_requires=[
-        'cython >= 0.19.0',
+        'cython >= 0.27.0',
         'pyfaidx >= 0.5.8',
     ],
     package_dir={'': 'src'},
     package_data={'gencodegenes': ['transcript.pxd', 'tx.h', 'tx.cpp']},
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `gencodegenes-1.0.7/src/gencode.cpp` & `gencodegenes-1.0.8/src/gencode.cpp`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/src/gencode.h` & `gencodegenes-1.0.8/src/gencode.h`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/src/gencodegenes/gencode.cpp` & `gencodegenes-1.0.8/src/gencodegenes/gencode.cpp`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/src/gencodegenes/gencode.pyx` & `gencodegenes-1.0.8/src/gencodegenes/gencode.pyx`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/src/gencodegenes/transcript.cpp` & `gencodegenes-1.0.8/src/gencodegenes/transcript.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1015,29 +1015,29 @@
  */
 struct __pyx_obj_12gencodegenes_10transcript_Transcript {
   PyObject_HEAD
   Tx *thisptr;
 };
 
 
-/* "gencodegenes/transcript.pyx":102
+/* "gencodegenes/transcript.pyx":98
  *             exon['start'] <= x['end'] and exon['end'] >= x['start'] ]
  * 
  *     def _insert_region(self, coords, region):             # <<<<<<<<<<<<<<
  *         ''' include a region into a list of regions
  * 
  */
 struct __pyx_obj_12gencodegenes_10transcript___pyx_scope_struct___insert_region {
   PyObject_HEAD
   PyObject *__pyx_v_overlaps;
   PyObject *__pyx_v_region;
 };
 
 
-/* "gencodegenes/transcript.pyx":114
+/* "gencodegenes/transcript.pyx":110
  *         indices = self._get_overlaps(region, coords)
  *         overlaps = [ coords[i] for i in indices ]
  *         start = min( x['start'] for x in overlaps + [region] )             # <<<<<<<<<<<<<<
  *         end = max( x['end'] for x in overlaps + [region] )
  * 
  */
 struct __pyx_obj_12gencodegenes_10transcript___pyx_scope_struct_1_genexpr {
@@ -1045,15 +1045,15 @@
   struct __pyx_obj_12gencodegenes_10transcript___pyx_scope_struct___insert_region *__pyx_outer_scope;
   PyObject *__pyx_v_x;
   PyObject *__pyx_t_0;
   Py_ssize_t __pyx_t_1;
 };
 
 
-/* "gencodegenes/transcript.pyx":115
+/* "gencodegenes/transcript.pyx":111
  *         overlaps = [ coords[i] for i in indices ]
  *         start = min( x['start'] for x in overlaps + [region] )
  *         end = max( x['end'] for x in overlaps + [region] )             # <<<<<<<<<<<<<<
  * 
  *         for i in sorted(indices, reverse=True):
  */
 struct __pyx_obj_12gencodegenes_10transcript___pyx_scope_struct_2_genexpr {
@@ -1300,56 +1300,14 @@
 /* PyObjectCallNoArg.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 #else
 #define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
 #endif
 
-/* PyIntCompare.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
-
-/* PyThreadStateGet.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
-#else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
-#endif
-
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
-#else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#endif
-#else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
-#endif
-
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
 /* PyIntBinop.proto */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
 #else
 #define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
 #endif
@@ -1542,14 +1500,56 @@
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
+/* PyIntCompare.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
+
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#endif
+
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
@@ -1651,21 +1651,21 @@
     PyErr_SetString(PyExc_RuntimeError, "Unknown exception");
   }
 }
 #endif
 
 static PyObject* __pyx_convert__to_py_struct__Region(struct Region s);
 static PyObject* __pyx_convert__to_py_struct__Codon(struct Codon s);
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
+/* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
@@ -1822,15 +1822,14 @@
 static std::vector<int>  __pyx_convert_vector_from_py_int(PyObject *); /*proto*/
 static std::vector<std::vector<int> >  __pyx_convert_vector_from_py_std_3a__3a_vector_3c_int_3e___(PyObject *); /*proto*/
 #define __Pyx_MODULE_NAME "gencodegenes.transcript"
 extern int __pyx_module_is_main_gencodegenes__transcript;
 int __pyx_module_is_main_gencodegenes__transcript = 0;
 
 /* Implementation of 'gencodegenes.transcript' */
-static PyObject *__pyx_builtin_NotImplementedError;
 static PyObject *__pyx_builtin_enumerate;
 static PyObject *__pyx_builtin_min;
 static PyObject *__pyx_builtin_max;
 static PyObject *__pyx_builtin_sorted;
 static PyObject *__pyx_builtin_chr;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_range;
@@ -1909,27 +1908,24 @@
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_genomic_offset[] = "genomic_offset";
 static const char __pyx_k_protein_coding[] = "protein_coding";
 static const char __pyx_k_Transcript_name[] = "Transcript(name=\"";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_transcript_type[] = "transcript_type";
 static const char __pyx_k_genomic_sequence[] = "genomic_sequence";
-static const char __pyx_k_merge_coordinates[] = "merge_coordinates";
-static const char __pyx_k_merge_genomic_seq[] = "merge_genomic_seq";
+static const char __pyx_k_merge_coordinates[] = "_merge_coordinates";
+static const char __pyx_k_merge_genomic_seq[] = "_merge_genomic_seq";
 static const char __pyx_k_transcript_type_2[] = "\", transcript_type=\"";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_NotImplementedError[] = "NotImplementedError";
 static const char __pyx_k_gencodegenes_transcript[] = "gencodegenes.transcript";
-static const char __pyx_k_op_0_isn_t_implemented_yet[] = "op {0} isn't implemented yet";
 static const char __pyx_k_insert_region_locals_genexpr[] = "_insert_region.<locals>.genexpr";
 static const char __pyx_k_Copyright_c_2015_Genome_Researc[] = "\nCopyright (c) 2015 Genome Research Ltd.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of\nthis software and associated documentation files (the \"Software\"), to deal in\nthe Software without restriction, including without limitation the rights to\nuse, copy, modify, merge, publish, distribute, sublicense, and/or sell copies\nof the Software, and to permit persons to whom the Software is furnished to do\nso, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS\nFOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR\nCOPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER\nIN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN\nCONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n";
-static const char __pyx_k_merge_coordinates_locals_lambda[] = "merge_coordinates.<locals>.<lambda>";
+static const char __pyx_k_merge_coordinates_locals_lambda[] = "_merge_coordinates.<locals>.<lambda>";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static PyObject *__pyx_n_u_N;
-static PyObject *__pyx_n_s_NotImplementedError;
 static PyObject *__pyx_n_s_Transcript;
 static PyObject *__pyx_kp_u_Transcript_name;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_u__3;
 static PyObject *__pyx_kp_u__4;
 static PyObject *__pyx_kp_u__5;
 static PyObject *__pyx_kp_u__6;
@@ -1986,15 +1982,14 @@
 static PyObject *__pyx_n_s_min;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_offset;
 static PyObject *__pyx_n_u_offset;
 static PyObject *__pyx_kp_u_offset_2;
-static PyObject *__pyx_kp_u_op_0_isn_t_implemented_yet;
 static PyObject *__pyx_n_s_pos;
 static PyObject *__pyx_n_u_pos;
 static PyObject *__pyx_n_u_protein_coding;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
@@ -2022,22 +2017,22 @@
 static PyObject *__pyx_n_s_type;
 static PyObject *__pyx_n_u_utf8;
 static int __pyx_pf_12gencodegenes_10transcript_10Transcript___cinit__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_name, PyObject *__pyx_v_chrom, PyObject *__pyx_v_start, PyObject *__pyx_v_end, PyObject *__pyx_v_strand, PyObject *__pyx_v_transcript_type, PyObject *__pyx_v_exons, PyObject *__pyx_v_cds, PyObject *__pyx_v_sequence, PyObject *__pyx_v_offset); /* proto */
 static void __pyx_pf_12gencodegenes_10transcript_10Transcript_2__dealloc__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_4__repr__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_6__str__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self); /* proto */
 static Py_hash_t __pyx_pf_12gencodegenes_10transcript_10Transcript_8__hash__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_10__richcmp__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_other, PyObject *__pyx_v_op); /* proto */
+static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_10__eq__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
 static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_12_get_overlaps(CYTHON_UNUSED struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_exon, PyObject *__pyx_v_regions); /* proto */
 static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_14_insert_region_genexpr(PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_14_insert_region_3genexpr(PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_14_insert_region(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_coords, PyObject *__pyx_v_region); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda2(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_x); /* proto */
-static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_16merge_coordinates(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_first, PyObject *__pyx_v_second); /* proto */
-static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_18merge_genomic_seq(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_16_merge_coordinates(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_first, PyObject *__pyx_v_second); /* proto */
+static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_18_merge_genomic_seq(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
 static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_20__add__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
 static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_4name___get__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_5chrom___get__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_4type___get__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_5start___get__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_3end___get__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_6strand___get__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self); /* proto */
@@ -3280,15 +3275,15 @@
   __Pyx_RefNannySetupContext("__hash__", 0);
 
   /* "gencodegenes/transcript.pyx":86
  * 
  *     def __hash__(self):
  *         return hash((self.chrom, self.start, self.end))             # <<<<<<<<<<<<<<
  * 
- *     def __richcmp__(self, other, op):
+ *     def __eq__(self, other):
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_chrom); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
@@ -3329,197 +3324,121 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "gencodegenes/transcript.pyx":88
  *         return hash((self.chrom, self.start, self.end))
  * 
- *     def __richcmp__(self, other, op):             # <<<<<<<<<<<<<<
- * 
- *         if op == 2:
+ *     def __eq__(self, other):             # <<<<<<<<<<<<<<
+ *         ''' check if transcripts occupy exact same genomic region '''
+ *         return self.__hash__() == other.__hash__()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_11__richcmp__(PyObject *__pyx_v_self, PyObject *__pyx_v_other, int __pyx_arg_op); /*proto*/
-static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_11__richcmp__(PyObject *__pyx_v_self, PyObject *__pyx_v_other, int __pyx_arg_op) {
-  PyObject *__pyx_v_op = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_11__eq__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
+static char __pyx_doc_12gencodegenes_10transcript_10Transcript_10__eq__[] = " check if transcripts occupy exact same genomic region ";
+#if CYTHON_UPDATE_DESCRIPTOR_DOC
+struct wrapperbase __pyx_wrapperbase_12gencodegenes_10transcript_10Transcript_10__eq__;
+#endif
+static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_11__eq__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__richcmp__ (wrapper)", 0);
-  __pyx_v_op = __Pyx_PyInt_From_int(__pyx_arg_op); if (unlikely(!__pyx_v_op)) __PYX_ERR(0, 88, __pyx_L3_error)
-  __Pyx_GOTREF(__pyx_v_op);
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("gencodegenes.transcript.Transcript.__richcmp__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_12gencodegenes_10transcript_10Transcript_10__richcmp__(((struct __pyx_obj_12gencodegenes_10transcript_Transcript *)__pyx_v_self), ((PyObject *)__pyx_v_other), ((PyObject *)__pyx_v_op));
+  __Pyx_RefNannySetupContext("__eq__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_12gencodegenes_10transcript_10Transcript_10__eq__(((struct __pyx_obj_12gencodegenes_10transcript_Transcript *)__pyx_v_self), ((PyObject *)__pyx_v_other));
 
   /* function exit code */
-  __Pyx_XDECREF(__pyx_v_op);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_10__richcmp__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_other, PyObject *__pyx_v_op) {
-  PyObject *__pyx_v_err_msg = NULL;
+static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_10__eq__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
+  PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__richcmp__", 0);
+  __Pyx_RefNannySetupContext("__eq__", 0);
 
   /* "gencodegenes/transcript.pyx":90
- *     def __richcmp__(self, other, op):
- * 
- *         if op == 2:             # <<<<<<<<<<<<<<
- *             return self.__hash__() == other.__hash__()
- *         else:
- */
-  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_op, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (likely(__pyx_t_2)) {
-
-    /* "gencodegenes/transcript.pyx":91
+ *     def __eq__(self, other):
+ *         ''' check if transcripts occupy exact same genomic region '''
+ *         return self.__hash__() == other.__hash__()             # <<<<<<<<<<<<<<
  * 
- *         if op == 2:
- *             return self.__hash__() == other.__hash__()             # <<<<<<<<<<<<<<
- *         else:
- *             err_msg = "op {0} isn't implemented yet".format(op)
+ *     def _get_overlaps(self, exon, regions):
  */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_hash); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_4);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
-      }
-    }
-    __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_hash); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_5);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
-      }
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_hash); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_r = __pyx_t_4;
-    __pyx_t_4 = 0;
-    goto __pyx_L0;
-
-    /* "gencodegenes/transcript.pyx":90
- *     def __richcmp__(self, other, op):
- * 
- *         if op == 2:             # <<<<<<<<<<<<<<
- *             return self.__hash__() == other.__hash__()
- *         else:
- */
   }
-
-  /* "gencodegenes/transcript.pyx":93
- *             return self.__hash__() == other.__hash__()
- *         else:
- *             err_msg = "op {0} isn't implemented yet".format(op)             # <<<<<<<<<<<<<<
- *             raise NotImplementedError(err_msg)
- * 
- */
-  /*else*/ {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_op_0_isn_t_implemented_yet, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_1)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_1);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
-      }
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_hash); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
-    __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_op) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_op);
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_v_err_msg = __pyx_t_4;
-    __pyx_t_4 = 0;
-
-    /* "gencodegenes/transcript.pyx":94
- *         else:
- *             err_msg = "op {0} isn't implemented yet".format(op)
- *             raise NotImplementedError(err_msg)             # <<<<<<<<<<<<<<
- * 
- *     def _get_overlaps(self, exon, regions):
- */
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_v_err_msg); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 94, __pyx_L1_error)
   }
+  __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
 
   /* "gencodegenes/transcript.pyx":88
  *         return hash((self.chrom, self.start, self.end))
  * 
- *     def __richcmp__(self, other, op):             # <<<<<<<<<<<<<<
- * 
- *         if op == 2:
+ *     def __eq__(self, other):             # <<<<<<<<<<<<<<
+ *         ''' check if transcripts occupy exact same genomic region '''
+ *         return self.__hash__() == other.__hash__()
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("gencodegenes.transcript.Transcript.__richcmp__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("gencodegenes.transcript.Transcript.__eq__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_err_msg);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":96
- *             raise NotImplementedError(err_msg)
+/* "gencodegenes/transcript.pyx":92
+ *         return self.__hash__() == other.__hash__()
  * 
  *     def _get_overlaps(self, exon, regions):             # <<<<<<<<<<<<<<
  *         ''' find all regions which overlap a given region
  *         '''
  */
 
 /* Python wrapper */
@@ -3553,32 +3472,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exon)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_regions)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_get_overlaps", 1, 2, 2, 1); __PYX_ERR(0, 96, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_get_overlaps", 1, 2, 2, 1); __PYX_ERR(0, 92, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_get_overlaps") < 0)) __PYX_ERR(0, 96, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_get_overlaps") < 0)) __PYX_ERR(0, 92, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_exon = values[0];
     __pyx_v_regions = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_get_overlaps", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 96, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_get_overlaps", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 92, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gencodegenes.transcript.Transcript._get_overlaps", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_12gencodegenes_10transcript_10Transcript_12_get_overlaps(((struct __pyx_obj_12gencodegenes_10transcript_Transcript *)__pyx_v_self), __pyx_v_exon, __pyx_v_regions);
 
@@ -3603,118 +3522,118 @@
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_overlaps", 0);
 
-  /* "gencodegenes/transcript.pyx":99
+  /* "gencodegenes/transcript.pyx":95
  *         ''' find all regions which overlap a given region
  *         '''
  *         return [ i for i, x in enumerate(regions) if             # <<<<<<<<<<<<<<
  *             exon['start'] <= x['end'] and exon['end'] >= x['start'] ]
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
     if (likely(PyList_CheckExact(__pyx_v_regions)) || PyTuple_CheckExact(__pyx_v_regions)) {
       __pyx_t_3 = __pyx_v_regions; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
       __pyx_t_5 = NULL;
     } else {
-      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_regions); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L5_error)
+      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_regions); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L5_error)
+      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L5_error)
     }
     for (;;) {
       if (likely(!__pyx_t_5)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_6 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_6); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 99, __pyx_L5_error)
+          __pyx_t_6 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_6); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 95, __pyx_L5_error)
           #else
-          __pyx_t_6 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 99, __pyx_L5_error)
+          __pyx_t_6 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 95, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_6);
           #endif
         } else {
           if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_6); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 99, __pyx_L5_error)
+          __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_6); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 95, __pyx_L5_error)
           #else
-          __pyx_t_6 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 99, __pyx_L5_error)
+          __pyx_t_6 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 95, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_6);
           #endif
         }
       } else {
         __pyx_t_6 = __pyx_t_5(__pyx_t_3);
         if (unlikely(!__pyx_t_6)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 99, __pyx_L5_error)
+            else __PYX_ERR(0, 95, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_6);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_x, __pyx_t_6);
       __pyx_t_6 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_i, __pyx_t_2);
-      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 99, __pyx_L5_error)
+      __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 95, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_6;
       __pyx_t_6 = 0;
 
-      /* "gencodegenes/transcript.pyx":100
+      /* "gencodegenes/transcript.pyx":96
  *         '''
  *         return [ i for i, x in enumerate(regions) if
  *             exon['start'] <= x['end'] and exon['end'] >= x['start'] ]             # <<<<<<<<<<<<<<
  * 
  *     def _insert_region(self, coords, region):
  */
-      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_exon, __pyx_n_u_start); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 100, __pyx_L5_error)
+      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_exon, __pyx_n_u_start); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_8genexpr2__pyx_v_x, __pyx_n_u_end); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 100, __pyx_L5_error)
+      __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_8genexpr2__pyx_v_x, __pyx_n_u_end); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 96, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_9 = PyObject_RichCompare(__pyx_t_6, __pyx_t_8, Py_LE); __Pyx_XGOTREF(__pyx_t_9); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 100, __pyx_L5_error)
+      __pyx_t_9 = PyObject_RichCompare(__pyx_t_6, __pyx_t_8, Py_LE); __Pyx_XGOTREF(__pyx_t_9); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 96, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 100, __pyx_L5_error)
+      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 96, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       if (__pyx_t_10) {
       } else {
         __pyx_t_7 = __pyx_t_10;
         goto __pyx_L9_bool_binop_done;
       }
-      __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_exon, __pyx_n_u_end); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 100, __pyx_L5_error)
+      __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_exon, __pyx_n_u_end); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 96, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_8genexpr2__pyx_v_x, __pyx_n_u_start); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 100, __pyx_L5_error)
+      __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_8genexpr2__pyx_v_x, __pyx_n_u_start); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 96, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_6 = PyObject_RichCompare(__pyx_t_9, __pyx_t_8, Py_GE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 100, __pyx_L5_error)
+      __pyx_t_6 = PyObject_RichCompare(__pyx_t_9, __pyx_t_8, Py_GE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 100, __pyx_L5_error)
+      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 96, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_7 = __pyx_t_10;
       __pyx_L9_bool_binop_done:;
 
-      /* "gencodegenes/transcript.pyx":99
+      /* "gencodegenes/transcript.pyx":95
  *         ''' find all regions which overlap a given region
  *         '''
  *         return [ i for i, x in enumerate(regions) if             # <<<<<<<<<<<<<<
  *             exon['start'] <= x['end'] and exon['end'] >= x['start'] ]
  * 
  */
       if (__pyx_t_7) {
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_8genexpr2__pyx_v_i))) __PYX_ERR(0, 99, __pyx_L5_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_8genexpr2__pyx_v_i))) __PYX_ERR(0, 95, __pyx_L5_error)
       }
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_i); __pyx_8genexpr2__pyx_v_i = 0;
     __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_x); __pyx_8genexpr2__pyx_v_x = 0;
     goto __pyx_L11_exit_scope;
@@ -3724,16 +3643,16 @@
     goto __pyx_L1_error;
     __pyx_L11_exit_scope:;
   } /* exit inner scope */
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":96
- *             raise NotImplementedError(err_msg)
+  /* "gencodegenes/transcript.pyx":92
+ *         return self.__hash__() == other.__hash__()
  * 
  *     def _get_overlaps(self, exon, regions):             # <<<<<<<<<<<<<<
  *         ''' find all regions which overlap a given region
  *         '''
  */
 
   /* function exit code */
@@ -3750,15 +3669,15 @@
   __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_i);
   __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_x);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":102
+/* "gencodegenes/transcript.pyx":98
  *             exon['start'] <= x['end'] and exon['end'] >= x['start'] ]
  * 
  *     def _insert_region(self, coords, region):             # <<<<<<<<<<<<<<
  *         ''' include a region into a list of regions
  * 
  */
 
@@ -3793,46 +3712,46 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_coords)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_region)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_insert_region", 1, 2, 2, 1); __PYX_ERR(0, 102, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_insert_region", 1, 2, 2, 1); __PYX_ERR(0, 98, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_insert_region") < 0)) __PYX_ERR(0, 102, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_insert_region") < 0)) __PYX_ERR(0, 98, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_coords = values[0];
     __pyx_v_region = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_insert_region", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 102, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_insert_region", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 98, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gencodegenes.transcript.Transcript._insert_region", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_12gencodegenes_10transcript_10Transcript_14_insert_region(((struct __pyx_obj_12gencodegenes_10transcript_Transcript *)__pyx_v_self), __pyx_v_coords, __pyx_v_region);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_12gencodegenes_10transcript_10Transcript_14_insert_region_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "gencodegenes/transcript.pyx":114
+/* "gencodegenes/transcript.pyx":110
  *         indices = self._get_overlaps(region, coords)
  *         overlaps = [ coords[i] for i in indices ]
  *         start = min( x['start'] for x in overlaps + [region] )             # <<<<<<<<<<<<<<
  *         end = max( x['end'] for x in overlaps + [region] )
  * 
  */
 
@@ -3844,23 +3763,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_12gencodegenes_10transcript___pyx_scope_struct_1_genexpr *)__pyx_tp_new_12gencodegenes_10transcript___pyx_scope_struct_1_genexpr(__pyx_ptype_12gencodegenes_10transcript___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_12gencodegenes_10transcript___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 114, __pyx_L1_error)
+    __PYX_ERR(0, 110, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_12gencodegenes_10transcript___pyx_scope_struct___insert_region *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_12gencodegenes_10transcript_10Transcript_14_insert_region_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_insert_region_locals_genexpr, __pyx_n_s_gencodegenes_transcript); if (unlikely(!gen)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_12gencodegenes_10transcript_10Transcript_14_insert_region_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_insert_region_locals_genexpr, __pyx_n_s_gencodegenes_transcript); if (unlikely(!gen)) __PYX_ERR(0, 110, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3888,40 +3807,40 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 114, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_overlaps)) { __Pyx_RaiseClosureNameError("overlaps"); __PYX_ERR(0, 114, __pyx_L1_error) }
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_region)) { __Pyx_RaiseClosureNameError("region"); __PYX_ERR(0, 114, __pyx_L1_error) }
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 110, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_overlaps)) { __Pyx_RaiseClosureNameError("overlaps"); __PYX_ERR(0, 110, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_region)) { __Pyx_RaiseClosureNameError("region"); __PYX_ERR(0, 110, __pyx_L1_error) }
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_region);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_region);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_cur_scope->__pyx_outer_scope->__pyx_v_region);
-  __pyx_t_2 = PyNumber_Add(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_overlaps, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_overlaps, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __pyx_t_2; __Pyx_INCREF(__pyx_t_1); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   for (;;) {
     if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_1)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 110, __pyx_L1_error)
     #else
-    __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     #endif
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_x);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_x, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_cur_scope->__pyx_v_x, __pyx_n_u_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_cur_scope->__pyx_v_x, __pyx_n_u_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     __Pyx_XGIVEREF(__pyx_t_1);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_3;
     __Pyx_XGIVEREF(__pyx_r);
@@ -3931,15 +3850,15 @@
     __pyx_generator->resume_label = 1;
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_1);
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_1;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 114, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 110, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -3955,15 +3874,15 @@
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_12gencodegenes_10transcript_10Transcript_14_insert_region_5generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "gencodegenes/transcript.pyx":115
+/* "gencodegenes/transcript.pyx":111
  *         overlaps = [ coords[i] for i in indices ]
  *         start = min( x['start'] for x in overlaps + [region] )
  *         end = max( x['end'] for x in overlaps + [region] )             # <<<<<<<<<<<<<<
  * 
  *         for i in sorted(indices, reverse=True):
  */
 
@@ -3975,23 +3894,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_12gencodegenes_10transcript___pyx_scope_struct_2_genexpr *)__pyx_tp_new_12gencodegenes_10transcript___pyx_scope_struct_2_genexpr(__pyx_ptype_12gencodegenes_10transcript___pyx_scope_struct_2_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_12gencodegenes_10transcript___pyx_scope_struct_2_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 115, __pyx_L1_error)
+    __PYX_ERR(0, 111, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_12gencodegenes_10transcript___pyx_scope_struct___insert_region *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_12gencodegenes_10transcript_10Transcript_14_insert_region_5generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_insert_region_locals_genexpr, __pyx_n_s_gencodegenes_transcript); if (unlikely(!gen)) __PYX_ERR(0, 115, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_12gencodegenes_10transcript_10Transcript_14_insert_region_5generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_insert_region_locals_genexpr, __pyx_n_s_gencodegenes_transcript); if (unlikely(!gen)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4019,40 +3938,40 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 115, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_overlaps)) { __Pyx_RaiseClosureNameError("overlaps"); __PYX_ERR(0, 115, __pyx_L1_error) }
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_region)) { __Pyx_RaiseClosureNameError("region"); __PYX_ERR(0, 115, __pyx_L1_error) }
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 111, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_overlaps)) { __Pyx_RaiseClosureNameError("overlaps"); __PYX_ERR(0, 111, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_region)) { __Pyx_RaiseClosureNameError("region"); __PYX_ERR(0, 111, __pyx_L1_error) }
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_region);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_region);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_cur_scope->__pyx_outer_scope->__pyx_v_region);
-  __pyx_t_2 = PyNumber_Add(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_overlaps, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_overlaps, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __pyx_t_2; __Pyx_INCREF(__pyx_t_1); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   for (;;) {
     if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_1)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 115, __pyx_L1_error)
+    __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
     #else
-    __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     #endif
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_x);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_x, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_cur_scope->__pyx_v_x, __pyx_n_u_end); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_cur_scope->__pyx_v_x, __pyx_n_u_end); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     __Pyx_XGIVEREF(__pyx_t_1);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_3;
     __Pyx_XGIVEREF(__pyx_r);
@@ -4062,15 +3981,15 @@
     __pyx_generator->resume_label = 1;
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_1);
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_1;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 115, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 111, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -4085,15 +4004,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":102
+/* "gencodegenes/transcript.pyx":98
  *             exon['start'] <= x['end'] and exon['end'] >= x['start'] ]
  * 
  *     def _insert_region(self, coords, region):             # <<<<<<<<<<<<<<
  *         ''' include a region into a list of regions
  * 
  */
 
@@ -4119,30 +4038,30 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_insert_region", 0);
   __pyx_cur_scope = (struct __pyx_obj_12gencodegenes_10transcript___pyx_scope_struct___insert_region *)__pyx_tp_new_12gencodegenes_10transcript___pyx_scope_struct___insert_region(__pyx_ptype_12gencodegenes_10transcript___pyx_scope_struct___insert_region, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_12gencodegenes_10transcript___pyx_scope_struct___insert_region *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 102, __pyx_L1_error)
+    __PYX_ERR(0, 98, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_region = __pyx_v_region;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_region);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_region);
 
-  /* "gencodegenes/transcript.pyx":112
+  /* "gencodegenes/transcript.pyx":108
  *             region: dict of {'start': X, 'end': Y} positions
  *         '''
  *         indices = self._get_overlaps(region, coords)             # <<<<<<<<<<<<<<
  *         overlaps = [ coords[i] for i in indices ]
  *         start = min( x['start'] for x in overlaps + [region] )
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_overlaps); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_overlaps); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -4151,251 +4070,251 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_cur_scope->__pyx_v_region, __pyx_v_coords};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_cur_scope->__pyx_v_region, __pyx_v_coords};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 108, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_region);
     __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_region);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_cur_scope->__pyx_v_region);
     __Pyx_INCREF(__pyx_v_coords);
     __Pyx_GIVEREF(__pyx_v_coords);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_coords);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_indices = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "gencodegenes/transcript.pyx":113
+  /* "gencodegenes/transcript.pyx":109
  *         '''
  *         indices = self._get_overlaps(region, coords)
  *         overlaps = [ coords[i] for i in indices ]             # <<<<<<<<<<<<<<
  *         start = min( x['start'] for x in overlaps + [region] )
  *         end = max( x['end'] for x in overlaps + [region] )
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (likely(PyList_CheckExact(__pyx_v_indices)) || PyTuple_CheckExact(__pyx_v_indices)) {
       __pyx_t_2 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_2); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
     } else {
-      __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L5_error)
+      __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_7 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 113, __pyx_L5_error)
+      __pyx_t_7 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L5_error)
     }
     for (;;) {
       if (likely(!__pyx_t_7)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_5); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 113, __pyx_L5_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_5); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 109, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_5); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 113, __pyx_L5_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_5); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 109, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_7(__pyx_t_2);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 113, __pyx_L5_error)
+            else __PYX_ERR(0, 109, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr3__pyx_v_i, __pyx_t_5);
       __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_coords, __pyx_8genexpr3__pyx_v_i); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L5_error)
+      __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_coords, __pyx_8genexpr3__pyx_v_i); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 109, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 113, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 109, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_i); __pyx_8genexpr3__pyx_v_i = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_i); __pyx_8genexpr3__pyx_v_i = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_overlaps = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "gencodegenes/transcript.pyx":114
+  /* "gencodegenes/transcript.pyx":110
  *         indices = self._get_overlaps(region, coords)
  *         overlaps = [ coords[i] for i in indices ]
  *         start = min( x['start'] for x in overlaps + [region] )             # <<<<<<<<<<<<<<
  *         end = max( x['end'] for x in overlaps + [region] )
  * 
  */
-  __pyx_t_1 = __pyx_pf_12gencodegenes_10transcript_10Transcript_14_insert_region_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_1 = __pyx_pf_12gencodegenes_10transcript_10Transcript_14_insert_region_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_min, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_min, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_start = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "gencodegenes/transcript.pyx":115
+  /* "gencodegenes/transcript.pyx":111
  *         overlaps = [ coords[i] for i in indices ]
  *         start = min( x['start'] for x in overlaps + [region] )
  *         end = max( x['end'] for x in overlaps + [region] )             # <<<<<<<<<<<<<<
  * 
  *         for i in sorted(indices, reverse=True):
  */
-  __pyx_t_2 = __pyx_pf_12gencodegenes_10transcript_10Transcript_14_insert_region_3genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_t_2 = __pyx_pf_12gencodegenes_10transcript_10Transcript_14_insert_region_3genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_max, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_max, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_end = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "gencodegenes/transcript.pyx":117
+  /* "gencodegenes/transcript.pyx":113
  *         end = max( x['end'] for x in overlaps + [region] )
  * 
  *         for i in sorted(indices, reverse=True):             # <<<<<<<<<<<<<<
  *             del coords[i]
  * 
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_indices);
   __Pyx_GIVEREF(__pyx_v_indices);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_indices);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_reverse, Py_True) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 117, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_reverse, Py_True) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (likely(PyList_CheckExact(__pyx_t_5)) || PyTuple_CheckExact(__pyx_t_5)) {
     __pyx_t_2 = __pyx_t_5; __Pyx_INCREF(__pyx_t_2); __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
   } else {
-    __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 117, __pyx_L1_error)
+    __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 117, __pyx_L1_error)
+    __pyx_t_7 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 113, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_5); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 117, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_5); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 117, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_5); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 117, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_5); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 117, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_7(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 117, __pyx_L1_error)
+          else __PYX_ERR(0, 113, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "gencodegenes/transcript.pyx":118
+    /* "gencodegenes/transcript.pyx":114
  * 
  *         for i in sorted(indices, reverse=True):
  *             del coords[i]             # <<<<<<<<<<<<<<
  * 
  *         return coords + [{'start': start, 'end': end}]
  */
-    if (unlikely(PyObject_DelItem(__pyx_v_coords, __pyx_v_i) < 0)) __PYX_ERR(0, 118, __pyx_L1_error)
+    if (unlikely(PyObject_DelItem(__pyx_v_coords, __pyx_v_i) < 0)) __PYX_ERR(0, 114, __pyx_L1_error)
 
-    /* "gencodegenes/transcript.pyx":117
+    /* "gencodegenes/transcript.pyx":113
  *         end = max( x['end'] for x in overlaps + [region] )
  * 
  *         for i in sorted(indices, reverse=True):             # <<<<<<<<<<<<<<
  *             del coords[i]
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gencodegenes/transcript.pyx":120
+  /* "gencodegenes/transcript.pyx":116
  *             del coords[i]
  * 
  *         return coords + [{'start': start, 'end': end}]             # <<<<<<<<<<<<<<
  * 
- *     def merge_coordinates(self, first, second):
+ *     def _merge_coordinates(self, first, second):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_start, __pyx_v_start) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_end, __pyx_v_end) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
-  __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 120, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_start, __pyx_v_start) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_end, __pyx_v_end) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_v_coords, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_v_coords, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":102
+  /* "gencodegenes/transcript.pyx":98
  *             exon['start'] <= x['end'] and exon['end'] >= x['start'] ]
  * 
  *     def _insert_region(self, coords, region):             # <<<<<<<<<<<<<<
  *         ''' include a region into a list of regions
  * 
  */
 
@@ -4417,34 +4336,34 @@
   __Pyx_XDECREF(__pyx_gb_12gencodegenes_10transcript_10Transcript_14_insert_region_5generator1);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":122
+/* "gencodegenes/transcript.pyx":118
  *         return coords + [{'start': start, 'end': end}]
  * 
- *     def merge_coordinates(self, first, second):             # <<<<<<<<<<<<<<
+ *     def _merge_coordinates(self, first, second):             # <<<<<<<<<<<<<<
  *         ''' merge two sets of coordinates, to get the union of regions
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_17merge_coordinates(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_12gencodegenes_10transcript_10Transcript_16merge_coordinates[] = " merge two sets of coordinates, to get the union of regions\n        \n        This uses an inefficient approach, looping over and over, but we won't\n        need to perform this often.\n        \n        Args:\n            first: list of {'start': x, 'end': y} dictionaries for first transcript\n            second: list of {'start': x, 'end': y} dictionaries for second transcript\n        \n        Returns:\n            list of [start, end] lists, sorted by position.\n        ";
-static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_17merge_coordinates(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_17_merge_coordinates(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_12gencodegenes_10transcript_10Transcript_16_merge_coordinates[] = " merge two sets of coordinates, to get the union of regions\n        \n        This uses an inefficient approach, looping over and over, but we won't\n        need to perform this often.\n        \n        Args:\n            first: list of {'start': x, 'end': y} dictionaries for first transcript\n            second: list of {'start': x, 'end': y} dictionaries for second transcript\n        \n        Returns:\n            list of [start, end] lists, sorted by position.\n        ";
+static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_17_merge_coordinates(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_first = 0;
   PyObject *__pyx_v_second = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("merge_coordinates (wrapper)", 0);
+  __Pyx_RefNannySetupContext("_merge_coordinates (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_first,&__pyx_n_s_second,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
@@ -4460,56 +4379,56 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_first)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_second)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("merge_coordinates", 1, 2, 2, 1); __PYX_ERR(0, 122, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_merge_coordinates", 1, 2, 2, 1); __PYX_ERR(0, 118, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "merge_coordinates") < 0)) __PYX_ERR(0, 122, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_merge_coordinates") < 0)) __PYX_ERR(0, 118, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_first = values[0];
     __pyx_v_second = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("merge_coordinates", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 122, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_merge_coordinates", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 118, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("gencodegenes.transcript.Transcript.merge_coordinates", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("gencodegenes.transcript.Transcript._merge_coordinates", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_12gencodegenes_10transcript_10Transcript_16merge_coordinates(((struct __pyx_obj_12gencodegenes_10transcript_Transcript *)__pyx_v_self), __pyx_v_first, __pyx_v_second);
+  __pyx_r = __pyx_pf_12gencodegenes_10transcript_10Transcript_16_merge_coordinates(((struct __pyx_obj_12gencodegenes_10transcript_Transcript *)__pyx_v_self), __pyx_v_first, __pyx_v_second);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":145
+/* "gencodegenes/transcript.pyx":141
  *             coords = self._insert_region(coords, b)
  * 
  *         return [ (x['start'], x['end']) for x in sorted(coords, key=lambda x: x['start']) ]             # <<<<<<<<<<<<<<
  * 
- *     def merge_genomic_seq(self, other):
+ *     def _merge_genomic_seq(self, other):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_17merge_coordinates_8genexpr6_lambda2(PyObject *__pyx_self, PyObject *__pyx_v_x); /*proto*/
-static PyMethodDef __pyx_mdef_12gencodegenes_10transcript_10Transcript_17merge_coordinates_8genexpr6_lambda2 = {"lambda2", (PyCFunction)__pyx_pw_12gencodegenes_10transcript_10Transcript_17merge_coordinates_8genexpr6_lambda2, METH_O, 0};
-static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_17merge_coordinates_8genexpr6_lambda2(PyObject *__pyx_self, PyObject *__pyx_v_x) {
+static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_18_merge_coordinates_8genexpr6_lambda2(PyObject *__pyx_self, PyObject *__pyx_v_x); /*proto*/
+static PyMethodDef __pyx_mdef_12gencodegenes_10transcript_10Transcript_18_merge_coordinates_8genexpr6_lambda2 = {"lambda2", (PyCFunction)__pyx_pw_12gencodegenes_10transcript_10Transcript_18_merge_coordinates_8genexpr6_lambda2, METH_O, 0};
+static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_18_merge_coordinates_8genexpr6_lambda2(PyObject *__pyx_self, PyObject *__pyx_v_x) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("lambda2 (wrapper)", 0);
   __pyx_r = __pyx_lambda_funcdef_lambda2(__pyx_self, ((PyObject *)__pyx_v_x));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -4521,40 +4440,40 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda2", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_x, __pyx_n_u_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_x, __pyx_n_u_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("gencodegenes.transcript.Transcript.merge_coordinates.lambda2", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("gencodegenes.transcript.Transcript._merge_coordinates.lambda2", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":122
+/* "gencodegenes/transcript.pyx":118
  *         return coords + [{'start': start, 'end': end}]
  * 
- *     def merge_coordinates(self, first, second):             # <<<<<<<<<<<<<<
+ *     def _merge_coordinates(self, first, second):             # <<<<<<<<<<<<<<
  *         ''' merge two sets of coordinates, to get the union of regions
  * 
  */
 
-static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_16merge_coordinates(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_first, PyObject *__pyx_v_second) {
+static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_16_merge_coordinates(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_first, PyObject *__pyx_v_second) {
   PyObject *__pyx_v_coords = NULL;
   PyObject *__pyx_v_a = NULL;
   PyObject *__pyx_v_b = NULL;
   PyObject *__pyx_v_region = NULL;
   PyObject *__pyx_8genexpr6__pyx_v_x = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -4569,38 +4488,38 @@
   PyObject *(*__pyx_t_9)(PyObject *);
   int __pyx_t_10;
   int __pyx_t_11;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("merge_coordinates", 0);
+  __Pyx_RefNannySetupContext("_merge_coordinates", 0);
 
-  /* "gencodegenes/transcript.pyx":135
+  /* "gencodegenes/transcript.pyx":131
  *             list of [start, end] lists, sorted by position.
  *         '''
  *         coords = []             # <<<<<<<<<<<<<<
  *         for a, b in combinations(first + second, 2):
  *             if a['start'] <= b['end'] and a['end'] >= b['start']:
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_coords = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "gencodegenes/transcript.pyx":136
+  /* "gencodegenes/transcript.pyx":132
  *         '''
  *         coords = []
  *         for a, b in combinations(first + second, 2):             # <<<<<<<<<<<<<<
  *             if a['start'] <= b['end'] and a['end'] >= b['start']:
  *                 region = {'start': min(a['start'], b['start']),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_combinations); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_combinations); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Add(__pyx_v_first, __pyx_v_second); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_v_first, __pyx_v_second); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -4609,228 +4528,228 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_3, __pyx_int_2};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_3, __pyx_int_2};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 136, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_t_3);
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_GIVEREF(__pyx_int_2);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_int_2);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 136, __pyx_L1_error)
+    __pyx_t_8 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 132, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 136, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 132, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 136, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 132, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_8(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 136, __pyx_L1_error)
+          else __PYX_ERR(0, 132, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
       PyObject* sequence = __pyx_t_1;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 136, __pyx_L1_error)
+        __PYX_ERR(0, 132, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_6 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_3);
       #else
-      __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 136, __pyx_L1_error)
+      __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 132, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+      __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 132, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L1_error)
+      __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 132, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_9 = Py_TYPE(__pyx_t_4)->tp_iternext;
       index = 0; __pyx_t_6 = __pyx_t_9(__pyx_t_4); if (unlikely(!__pyx_t_6)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_6);
       index = 1; __pyx_t_3 = __pyx_t_9(__pyx_t_4); if (unlikely(!__pyx_t_3)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_3);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_4), 2) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_4), 2) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
       __pyx_t_9 = NULL;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       goto __pyx_L6_unpacking_done;
       __pyx_L5_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_9 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 136, __pyx_L1_error)
+      __PYX_ERR(0, 132, __pyx_L1_error)
       __pyx_L6_unpacking_done:;
     }
     __Pyx_XDECREF_SET(__pyx_v_a, __pyx_t_6);
     __pyx_t_6 = 0;
     __Pyx_XDECREF_SET(__pyx_v_b, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "gencodegenes/transcript.pyx":137
+    /* "gencodegenes/transcript.pyx":133
  *         coords = []
  *         for a, b in combinations(first + second, 2):
  *             if a['start'] <= b['end'] and a['end'] >= b['start']:             # <<<<<<<<<<<<<<
  *                 region = {'start': min(a['start'], b['start']),
  *                     'end': max(a['end'], b['end'])}
  */
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_a, __pyx_n_u_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_a, __pyx_n_u_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_b, __pyx_n_u_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_b, __pyx_n_u_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_LE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __pyx_t_6 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_LE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (__pyx_t_11) {
     } else {
       __pyx_t_10 = __pyx_t_11;
       goto __pyx_L8_bool_binop_done;
     }
-    __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_a, __pyx_n_u_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_a, __pyx_n_u_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_b, __pyx_n_u_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_b, __pyx_n_u_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = PyObject_RichCompare(__pyx_t_6, __pyx_t_3, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_t_6, __pyx_t_3, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_10 = __pyx_t_11;
     __pyx_L8_bool_binop_done:;
     if (__pyx_t_10) {
 
-      /* "gencodegenes/transcript.pyx":138
+      /* "gencodegenes/transcript.pyx":134
  *         for a, b in combinations(first + second, 2):
  *             if a['start'] <= b['end'] and a['end'] >= b['start']:
  *                 region = {'start': min(a['start'], b['start']),             # <<<<<<<<<<<<<<
  *                     'end': max(a['end'], b['end'])}
  *                 a, b = region, region
  */
-      __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_b, __pyx_n_u_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 138, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_b, __pyx_n_u_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_a, __pyx_n_u_start); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 138, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_a, __pyx_n_u_start); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_12 = PyObject_RichCompare(__pyx_t_3, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_12); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 138, __pyx_L1_error)
-      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_12); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 138, __pyx_L1_error)
+      __pyx_t_12 = PyObject_RichCompare(__pyx_t_3, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_12); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 134, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_12); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       if (__pyx_t_10) {
         __Pyx_INCREF(__pyx_t_3);
         __pyx_t_4 = __pyx_t_3;
       } else {
         __Pyx_INCREF(__pyx_t_6);
         __pyx_t_4 = __pyx_t_6;
       }
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_start, __pyx_t_4) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_start, __pyx_t_4) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "gencodegenes/transcript.pyx":139
+      /* "gencodegenes/transcript.pyx":135
  *             if a['start'] <= b['end'] and a['end'] >= b['start']:
  *                 region = {'start': min(a['start'], b['start']),
  *                     'end': max(a['end'], b['end'])}             # <<<<<<<<<<<<<<
  *                 a, b = region, region
  * 
  */
-      __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_b, __pyx_n_u_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 139, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_b, __pyx_n_u_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 135, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_a, __pyx_n_u_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_a, __pyx_n_u_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_12 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_GT); __Pyx_XGOTREF(__pyx_t_12); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 139, __pyx_L1_error)
-      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_12); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 139, __pyx_L1_error)
+      __pyx_t_12 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_GT); __Pyx_XGOTREF(__pyx_t_12); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 135, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_12); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 135, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       if (__pyx_t_10) {
         __Pyx_INCREF(__pyx_t_4);
         __pyx_t_6 = __pyx_t_4;
       } else {
         __Pyx_INCREF(__pyx_t_3);
         __pyx_t_6 = __pyx_t_3;
       }
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_end, __pyx_t_6) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_end, __pyx_t_6) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF_SET(__pyx_v_region, ((PyObject*)__pyx_t_1));
       __pyx_t_1 = 0;
 
-      /* "gencodegenes/transcript.pyx":140
+      /* "gencodegenes/transcript.pyx":136
  *                 region = {'start': min(a['start'], b['start']),
  *                     'end': max(a['end'], b['end'])}
  *                 a, b = region, region             # <<<<<<<<<<<<<<
  * 
  *             coords = self._insert_region(coords, a)
  */
       __pyx_t_1 = __pyx_v_region;
@@ -4838,31 +4757,31 @@
       __pyx_t_6 = __pyx_v_region;
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_DECREF_SET(__pyx_v_a, __pyx_t_1);
       __pyx_t_1 = 0;
       __Pyx_DECREF_SET(__pyx_v_b, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "gencodegenes/transcript.pyx":137
+      /* "gencodegenes/transcript.pyx":133
  *         coords = []
  *         for a, b in combinations(first + second, 2):
  *             if a['start'] <= b['end'] and a['end'] >= b['start']:             # <<<<<<<<<<<<<<
  *                 region = {'start': min(a['start'], b['start']),
  *                     'end': max(a['end'], b['end'])}
  */
     }
 
-    /* "gencodegenes/transcript.pyx":142
+    /* "gencodegenes/transcript.pyx":138
  *                 a, b = region, region
  * 
  *             coords = self._insert_region(coords, a)             # <<<<<<<<<<<<<<
  *             coords = self._insert_region(coords, b)
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_insert_region); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_insert_region); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -4871,55 +4790,55 @@
         __Pyx_DECREF_SET(__pyx_t_1, function);
         __pyx_t_5 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_1)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_coords, __pyx_v_a};
-      __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 142, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 138, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_6);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_coords, __pyx_v_a};
-      __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 142, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 138, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_6);
     } else
     #endif
     {
-      __pyx_t_3 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
+      __pyx_t_3 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 138, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       if (__pyx_t_4) {
         __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
       __Pyx_INCREF(__pyx_v_coords);
       __Pyx_GIVEREF(__pyx_v_coords);
       PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_5, __pyx_v_coords);
       __Pyx_INCREF(__pyx_v_a);
       __Pyx_GIVEREF(__pyx_v_a);
       PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_5, __pyx_v_a);
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 142, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 138, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_coords, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "gencodegenes/transcript.pyx":143
+    /* "gencodegenes/transcript.pyx":139
  * 
  *             coords = self._insert_region(coords, a)
  *             coords = self._insert_region(coords, b)             # <<<<<<<<<<<<<<
  * 
  *         return [ (x['start'], x['end']) for x in sorted(coords, key=lambda x: x['start']) ]
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_insert_region); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_insert_region); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -4928,204 +4847,204 @@
         __Pyx_DECREF_SET(__pyx_t_1, function);
         __pyx_t_5 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_1)) {
       PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_coords, __pyx_v_b};
-      __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 143, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_GOTREF(__pyx_t_6);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
       PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_coords, __pyx_v_b};
-      __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 143, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_GOTREF(__pyx_t_6);
     } else
     #endif
     {
-      __pyx_t_4 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
+      __pyx_t_4 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       if (__pyx_t_3) {
         __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3); __pyx_t_3 = NULL;
       }
       __Pyx_INCREF(__pyx_v_coords);
       __Pyx_GIVEREF(__pyx_v_coords);
       PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_5, __pyx_v_coords);
       __Pyx_INCREF(__pyx_v_b);
       __Pyx_GIVEREF(__pyx_v_b);
       PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_5, __pyx_v_b);
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 143, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_coords, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "gencodegenes/transcript.pyx":136
+    /* "gencodegenes/transcript.pyx":132
  *         '''
  *         coords = []
  *         for a, b in combinations(first + second, 2):             # <<<<<<<<<<<<<<
  *             if a['start'] <= b['end'] and a['end'] >= b['start']:
  *                 region = {'start': min(a['start'], b['start']),
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gencodegenes/transcript.pyx":145
+  /* "gencodegenes/transcript.pyx":141
  *             coords = self._insert_region(coords, b)
  * 
  *         return [ (x['start'], x['end']) for x in sorted(coords, key=lambda x: x['start']) ]             # <<<<<<<<<<<<<<
  * 
- *     def merge_genomic_seq(self, other):
+ *     def _merge_genomic_seq(self, other):
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 145, __pyx_L12_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 141, __pyx_L12_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 145, __pyx_L12_error)
+    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 141, __pyx_L12_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_v_coords);
     __Pyx_GIVEREF(__pyx_v_coords);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_coords);
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L12_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L12_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_12gencodegenes_10transcript_10Transcript_17merge_coordinates_8genexpr6_lambda2, 0, __pyx_n_s_merge_coordinates_locals_lambda, NULL, __pyx_n_s_gencodegenes_transcript, __pyx_d, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L12_error)
+    __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_12gencodegenes_10transcript_10Transcript_18_merge_coordinates_8genexpr6_lambda2, 0, __pyx_n_s_merge_coordinates_locals_lambda, NULL, __pyx_n_s_gencodegenes_transcript, __pyx_d, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L12_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_key, __pyx_t_4) < 0) __PYX_ERR(0, 145, __pyx_L12_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_key, __pyx_t_4) < 0) __PYX_ERR(0, 141, __pyx_L12_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L12_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L12_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
       __pyx_t_1 = __pyx_t_4; __Pyx_INCREF(__pyx_t_1); __pyx_t_7 = 0;
       __pyx_t_8 = NULL;
     } else {
-      __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L12_error)
+      __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_8 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 145, __pyx_L12_error)
+      __pyx_t_8 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 141, __pyx_L12_error)
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     for (;;) {
       if (likely(!__pyx_t_8)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 145, __pyx_L12_error)
+          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 141, __pyx_L12_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L12_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L12_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         } else {
           if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 145, __pyx_L12_error)
+          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 141, __pyx_L12_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L12_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L12_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         }
       } else {
         __pyx_t_4 = __pyx_t_8(__pyx_t_1);
         if (unlikely(!__pyx_t_4)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 145, __pyx_L12_error)
+            else __PYX_ERR(0, 141, __pyx_L12_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_4);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr6__pyx_v_x, __pyx_t_4);
       __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_8genexpr6__pyx_v_x, __pyx_n_u_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L12_error)
+      __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_8genexpr6__pyx_v_x, __pyx_n_u_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_8genexpr6__pyx_v_x, __pyx_n_u_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 145, __pyx_L12_error)
+      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_8genexpr6__pyx_v_x, __pyx_n_u_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 141, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L12_error)
+      __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 141, __pyx_L12_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_6 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 145, __pyx_L12_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 141, __pyx_L12_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_x); __pyx_8genexpr6__pyx_v_x = 0;
     goto __pyx_L15_exit_scope;
     __pyx_L12_error:;
     __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_x); __pyx_8genexpr6__pyx_v_x = 0;
     goto __pyx_L1_error;
     __pyx_L15_exit_scope:;
   } /* exit inner scope */
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":122
+  /* "gencodegenes/transcript.pyx":118
  *         return coords + [{'start': start, 'end': end}]
  * 
- *     def merge_coordinates(self, first, second):             # <<<<<<<<<<<<<<
+ *     def _merge_coordinates(self, first, second):             # <<<<<<<<<<<<<<
  *         ''' merge two sets of coordinates, to get the union of regions
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_12);
-  __Pyx_AddTraceback("gencodegenes.transcript.Transcript.merge_coordinates", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("gencodegenes.transcript.Transcript._merge_coordinates", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_coords);
   __Pyx_XDECREF(__pyx_v_a);
   __Pyx_XDECREF(__pyx_v_b);
   __Pyx_XDECREF(__pyx_v_region);
   __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_x);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":147
+/* "gencodegenes/transcript.pyx":143
  *         return [ (x['start'], x['end']) for x in sorted(coords, key=lambda x: x['start']) ]
  * 
- *     def merge_genomic_seq(self, other):             # <<<<<<<<<<<<<<
+ *     def _merge_genomic_seq(self, other):             # <<<<<<<<<<<<<<
  *         ''' merge the genomic sequence from two transcripts
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_19merge_genomic_seq(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
-static char __pyx_doc_12gencodegenes_10transcript_10Transcript_18merge_genomic_seq[] = " merge the genomic sequence from two transcripts\n        \n        We have two transcripts A, and B. We need to get the contiguous sequence\n        from the start of the first transcript on the chromosome to the end of\n        the second transcript. The transcripts may or may not overlap. There are\n        three scenarios we need to account for:\n        \n        \n        overlap without   A   =================\n        enveloping                           ================= B\n        \n        \n            overlap       A   ==============================\n        and envelop               ==================  B\n        \n        \n        no overlap        A  ===============\n                                               ===============  B\n        \n        I've called the transcript whose sequence is first along the chromosome\n        as 'lead', and the transcript whose sequence is last as 'lag', and the\n        converse as 'not_lead', and 'not_lag'. Note that in the envelope case,\n        the lead transcript can also be the lag transcript.\n        ";
-static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_19merge_genomic_seq(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_19_merge_genomic_seq(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
+static char __pyx_doc_12gencodegenes_10transcript_10Transcript_18_merge_genomic_seq[] = " merge the genomic sequence from two transcripts\n        \n        We have two transcripts A, and B. We need to get the contiguous sequence\n        from the start of the first transcript on the chromosome to the end of\n        the second transcript. The transcripts may or may not overlap. There are\n        three scenarios we need to account for:\n        \n        \n        overlap without   A   =================\n        enveloping                           ================= B\n        \n        \n            overlap       A   ==============================\n        and envelop               ==================  B\n        \n        \n        no overlap        A  ===============\n                                               ===============  B\n        \n        I've called the transcript whose sequence is first along the chromosome\n        as 'lead', and the transcript whose sequence is last as 'lag', and the\n        converse as 'not_lead', and 'not_lag'. Note that in the envelope case,\n        the lead transcript can also be the lag transcript.\n        ";
+static PyObject *__pyx_pw_12gencodegenes_10transcript_10Transcript_19_merge_genomic_seq(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("merge_genomic_seq (wrapper)", 0);
-  __pyx_r = __pyx_pf_12gencodegenes_10transcript_10Transcript_18merge_genomic_seq(((struct __pyx_obj_12gencodegenes_10transcript_Transcript *)__pyx_v_self), ((PyObject *)__pyx_v_other));
+  __Pyx_RefNannySetupContext("_merge_genomic_seq (wrapper)", 0);
+  __pyx_r = __pyx_pf_12gencodegenes_10transcript_10Transcript_18_merge_genomic_seq(((struct __pyx_obj_12gencodegenes_10transcript_Transcript *)__pyx_v_self), ((PyObject *)__pyx_v_other));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_18merge_genomic_seq(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pf_12gencodegenes_10transcript_10Transcript_18_merge_genomic_seq(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_v_lead = NULL;
   PyObject *__pyx_v_not_lead = NULL;
   PyObject *__pyx_v_lag = NULL;
   PyObject *__pyx_v_not_lag = NULL;
   PyObject *__pyx_v_lead_offset = NULL;
   PyObject *__pyx_v_lead_gdna = NULL;
   PyObject *__pyx_v_initial = NULL;
@@ -5143,42 +5062,42 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("merge_genomic_seq", 0);
+  __Pyx_RefNannySetupContext("_merge_genomic_seq", 0);
 
-  /* "gencodegenes/transcript.pyx":177
+  /* "gencodegenes/transcript.pyx":173
  *         # TODO: this could be worked around, by figuring the minimum offset length,
  *         # TODO: then trimming the respective DNA offset sequences to that length.
  *         assert self.genomic_offset == other.genomic_offset             # <<<<<<<<<<<<<<
  * 
  *         # figure out which transcripts hold the leading and lagging sections
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_genomic_offset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_genomic_offset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_genomic_offset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_genomic_offset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 173, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(!__pyx_t_4)) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 177, __pyx_L1_error)
+      __PYX_ERR(0, 173, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "gencodegenes/transcript.pyx":180
+  /* "gencodegenes/transcript.pyx":176
  * 
  *         # figure out which transcripts hold the leading and lagging sections
  *         lead, not_lead = self, other             # <<<<<<<<<<<<<<
  *         if self.start > other.start:
  *             lead, not_lead = other, self
  */
   __pyx_t_3 = ((PyObject *)__pyx_v_self);
@@ -5186,33 +5105,33 @@
   __pyx_t_2 = __pyx_v_other;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_lead = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_not_lead = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "gencodegenes/transcript.pyx":181
+  /* "gencodegenes/transcript.pyx":177
  *         # figure out which transcripts hold the leading and lagging sections
  *         lead, not_lead = self, other
  *         if self.start > other.start:             # <<<<<<<<<<<<<<
  *             lead, not_lead = other, self
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_4) {
 
-    /* "gencodegenes/transcript.pyx":182
+    /* "gencodegenes/transcript.pyx":178
  *         lead, not_lead = self, other
  *         if self.start > other.start:
  *             lead, not_lead = other, self             # <<<<<<<<<<<<<<
  * 
  *         lag, not_lag = self, other
  */
     __pyx_t_1 = __pyx_v_other;
@@ -5220,24 +5139,24 @@
     __pyx_t_3 = ((PyObject *)__pyx_v_self);
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_DECREF_SET(__pyx_v_lead, __pyx_t_1);
     __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_not_lead, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "gencodegenes/transcript.pyx":181
+    /* "gencodegenes/transcript.pyx":177
  *         # figure out which transcripts hold the leading and lagging sections
  *         lead, not_lead = self, other
  *         if self.start > other.start:             # <<<<<<<<<<<<<<
  *             lead, not_lead = other, self
  * 
  */
   }
 
-  /* "gencodegenes/transcript.pyx":184
+  /* "gencodegenes/transcript.pyx":180
  *             lead, not_lead = other, self
  * 
  *         lag, not_lag = self, other             # <<<<<<<<<<<<<<
  *         if self.end < other.end:
  *             lag, not_lag = other, self
  */
   __pyx_t_3 = ((PyObject *)__pyx_v_self);
@@ -5245,33 +5164,33 @@
   __pyx_t_1 = __pyx_v_other;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_lag = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_not_lag = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "gencodegenes/transcript.pyx":185
+  /* "gencodegenes/transcript.pyx":181
  * 
  *         lag, not_lag = self, other
  *         if self.end < other.end:             # <<<<<<<<<<<<<<
  *             lag, not_lag = other, self
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_4) {
 
-    /* "gencodegenes/transcript.pyx":186
+    /* "gencodegenes/transcript.pyx":182
  *         lag, not_lag = self, other
  *         if self.end < other.end:
  *             lag, not_lag = other, self             # <<<<<<<<<<<<<<
  * 
  *         lead_offset = lead.genomic_offset
  */
     __pyx_t_2 = __pyx_v_other;
@@ -5279,236 +5198,236 @@
     __pyx_t_3 = ((PyObject *)__pyx_v_self);
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_DECREF_SET(__pyx_v_lag, __pyx_t_2);
     __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_not_lag, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "gencodegenes/transcript.pyx":185
+    /* "gencodegenes/transcript.pyx":181
  * 
  *         lag, not_lag = self, other
  *         if self.end < other.end:             # <<<<<<<<<<<<<<
  *             lag, not_lag = other, self
  * 
  */
   }
 
-  /* "gencodegenes/transcript.pyx":188
+  /* "gencodegenes/transcript.pyx":184
  *             lag, not_lag = other, self
  * 
  *         lead_offset = lead.genomic_offset             # <<<<<<<<<<<<<<
  *         lead_gdna = lead.genomic_sequence
  *         initial = lead_gdna[:not_lead.start - lead.start + lead_offset]
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_lead, __pyx_n_s_genomic_offset); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_lead, __pyx_n_s_genomic_offset); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 184, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_lead_offset = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "gencodegenes/transcript.pyx":189
+  /* "gencodegenes/transcript.pyx":185
  * 
  *         lead_offset = lead.genomic_offset
  *         lead_gdna = lead.genomic_sequence             # <<<<<<<<<<<<<<
  *         initial = lead_gdna[:not_lead.start - lead.start + lead_offset]
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_lead, __pyx_n_s_genomic_sequence); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_lead, __pyx_n_s_genomic_sequence); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_lead_gdna = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "gencodegenes/transcript.pyx":190
+  /* "gencodegenes/transcript.pyx":186
  *         lead_offset = lead.genomic_offset
  *         lead_gdna = lead.genomic_sequence
  *         initial = lead_gdna[:not_lead.start - lead.start + lead_offset]             # <<<<<<<<<<<<<<
  * 
  *         if self.start <= other.end and self.end >= other.start:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_not_lead, __pyx_n_s_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_not_lead, __pyx_n_s_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_lead, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_lead, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyNumber_Subtract(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Subtract(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_lead_offset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_lead_offset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_lead_gdna, 0, 0, NULL, &__pyx_t_2, NULL, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_lead_gdna, 0, 0, NULL, &__pyx_t_2, NULL, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_initial = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "gencodegenes/transcript.pyx":192
+  /* "gencodegenes/transcript.pyx":188
  *         initial = lead_gdna[:not_lead.start - lead.start + lead_offset]
  * 
  *         if self.start <= other.end and self.end >= other.start:             # <<<<<<<<<<<<<<
  *             intersect_start = not_lead.start - lead.start + lead_offset
  *             intersect_end = not_lag.end - lead.start + lead_offset
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_end); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_end); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_5) {
   } else {
     __pyx_t_4 = __pyx_t_5;
     goto __pyx_L6_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_4 = __pyx_t_5;
   __pyx_L6_bool_binop_done:;
   if (__pyx_t_4) {
 
-    /* "gencodegenes/transcript.pyx":193
+    /* "gencodegenes/transcript.pyx":189
  * 
  *         if self.start <= other.end and self.end >= other.start:
  *             intersect_start = not_lead.start - lead.start + lead_offset             # <<<<<<<<<<<<<<
  *             intersect_end = not_lag.end - lead.start + lead_offset
  *             intersect = lead_gdna[intersect_start:intersect_end]
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_not_lead, __pyx_n_s_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_not_lead, __pyx_n_s_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_lead, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_lead, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Subtract(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Subtract(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyNumber_Add(__pyx_t_3, __pyx_v_lead_offset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_t_3, __pyx_v_lead_offset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_intersect_start = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "gencodegenes/transcript.pyx":194
+    /* "gencodegenes/transcript.pyx":190
  *         if self.start <= other.end and self.end >= other.start:
  *             intersect_start = not_lead.start - lead.start + lead_offset
  *             intersect_end = not_lag.end - lead.start + lead_offset             # <<<<<<<<<<<<<<
  *             intersect = lead_gdna[intersect_start:intersect_end]
  *         else:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_not_lag, __pyx_n_s_end); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_not_lag, __pyx_n_s_end); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_lead, __pyx_n_s_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 194, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_lead, __pyx_n_s_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_v_lead_offset); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 194, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_v_lead_offset); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_intersect_end = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "gencodegenes/transcript.pyx":195
+    /* "gencodegenes/transcript.pyx":191
  *             intersect_start = not_lead.start - lead.start + lead_offset
  *             intersect_end = not_lag.end - lead.start + lead_offset
  *             intersect = lead_gdna[intersect_start:intersect_end]             # <<<<<<<<<<<<<<
  *         else:
  *             intersect = 'N' * (lag.start - lead.end - lead_offset * 2)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_v_lead_gdna, 0, 0, &__pyx_v_intersect_start, &__pyx_v_intersect_end, NULL, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_v_lead_gdna, 0, 0, &__pyx_v_intersect_start, &__pyx_v_intersect_end, NULL, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_intersect = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "gencodegenes/transcript.pyx":192
+    /* "gencodegenes/transcript.pyx":188
  *         initial = lead_gdna[:not_lead.start - lead.start + lead_offset]
  * 
  *         if self.start <= other.end and self.end >= other.start:             # <<<<<<<<<<<<<<
  *             intersect_start = not_lead.start - lead.start + lead_offset
  *             intersect_end = not_lag.end - lead.start + lead_offset
  */
     goto __pyx_L5;
   }
 
-  /* "gencodegenes/transcript.pyx":197
+  /* "gencodegenes/transcript.pyx":193
  *             intersect = lead_gdna[intersect_start:intersect_end]
  *         else:
  *             intersect = 'N' * (lag.start - lead.end - lead_offset * 2)             # <<<<<<<<<<<<<<
  * 
  *         lag_offset = lag.genomic_offset
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_lag, __pyx_n_s_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_lag, __pyx_n_s_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_lead, __pyx_n_s_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_lead, __pyx_n_s_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyNumber_Subtract(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Subtract(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Multiply(__pyx_v_lead_offset, __pyx_int_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Multiply(__pyx_v_lead_offset, __pyx_int_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyNumber_Subtract(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Subtract(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Multiply(__pyx_n_u_N, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Multiply(__pyx_n_u_N, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_intersect = __pyx_t_1;
     __pyx_t_1 = 0;
   }
   __pyx_L5:;
 
-  /* "gencodegenes/transcript.pyx":199
+  /* "gencodegenes/transcript.pyx":195
  *             intersect = 'N' * (lag.start - lead.end - lead_offset * 2)
  * 
  *         lag_offset = lag.genomic_offset             # <<<<<<<<<<<<<<
  *         lag_gdna = lag.genomic_sequence
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_lag, __pyx_n_s_genomic_offset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_lag, __pyx_n_s_genomic_offset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_lag_offset = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "gencodegenes/transcript.pyx":200
+  /* "gencodegenes/transcript.pyx":196
  * 
  *         lag_offset = lag.genomic_offset
  *         lag_gdna = lag.genomic_sequence             # <<<<<<<<<<<<<<
  * 
  *         # some transcripts overlap, but some do not. We need to find the position
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_lag, __pyx_n_s_genomic_sequence); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_lag, __pyx_n_s_genomic_sequence); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_lag_gdna = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "gencodegenes/transcript.pyx":206
+  /* "gencodegenes/transcript.pyx":202
  *         # not lagging transcript, or the start of the lagging transcript,
  *         # whichever is higher
  *         pos = max(not_lag.end, lag.start)             # <<<<<<<<<<<<<<
  *         final = lag_gdna[pos - lag.start + lead_offset:]
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_lag, __pyx_n_s_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_lag, __pyx_n_s_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_not_lag, __pyx_n_s_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_not_lag, __pyx_n_s_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_GT); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 206, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_6 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_GT); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_4) {
     __Pyx_INCREF(__pyx_t_1);
     __pyx_t_2 = __pyx_t_1;
   } else {
     __Pyx_INCREF(__pyx_t_3);
     __pyx_t_2 = __pyx_t_3;
@@ -5517,67 +5436,67 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __pyx_t_2;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_pos = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "gencodegenes/transcript.pyx":207
+  /* "gencodegenes/transcript.pyx":203
  *         # whichever is higher
  *         pos = max(not_lag.end, lag.start)
  *         final = lag_gdna[pos - lag.start + lead_offset:]             # <<<<<<<<<<<<<<
  * 
  *         return initial + intersect + final
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_lag, __pyx_n_s_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_lag, __pyx_n_s_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Subtract(__pyx_v_pos, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Subtract(__pyx_v_pos, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_v_lead_offset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_v_lead_offset); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_v_lag_gdna, 0, 0, &__pyx_t_1, NULL, NULL, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_v_lag_gdna, 0, 0, &__pyx_t_1, NULL, NULL, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_final = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "gencodegenes/transcript.pyx":209
+  /* "gencodegenes/transcript.pyx":205
  *         final = lag_gdna[pos - lag.start + lead_offset:]
  * 
  *         return initial + intersect + final             # <<<<<<<<<<<<<<
  * 
  *     def __add__(self, other):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyNumber_Add(__pyx_v_initial, __pyx_v_intersect); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_v_initial, __pyx_v_intersect); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_v_final); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_v_final); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":147
+  /* "gencodegenes/transcript.pyx":143
  *         return [ (x['start'], x['end']) for x in sorted(coords, key=lambda x: x['start']) ]
  * 
- *     def merge_genomic_seq(self, other):             # <<<<<<<<<<<<<<
+ *     def _merge_genomic_seq(self, other):             # <<<<<<<<<<<<<<
  *         ''' merge the genomic sequence from two transcripts
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("gencodegenes.transcript.Transcript.merge_genomic_seq", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("gencodegenes.transcript.Transcript._merge_genomic_seq", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_lead);
   __Pyx_XDECREF(__pyx_v_not_lead);
   __Pyx_XDECREF(__pyx_v_lag);
   __Pyx_XDECREF(__pyx_v_not_lag);
   __Pyx_XDECREF(__pyx_v_lead_offset);
@@ -5591,15 +5510,15 @@
   __Pyx_XDECREF(__pyx_v_pos);
   __Pyx_XDECREF(__pyx_v_final);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":211
+/* "gencodegenes/transcript.pyx":207
  *         return initial + intersect + final
  * 
  *     def __add__(self, other):             # <<<<<<<<<<<<<<
  *         """ combine the coding sequences of two Transcript objects
  * 
  */
 
@@ -5637,90 +5556,90 @@
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__add__", 0);
 
-  /* "gencodegenes/transcript.pyx":237
+  /* "gencodegenes/transcript.pyx":233
  *         # if we try transcript + None or None + transcript, return the original
  *         # transcript, rather than raising an error.
  *         if other is None:             # <<<<<<<<<<<<<<
  *             return self
  *         if self is None:
  */
   __pyx_t_1 = (__pyx_v_other == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "gencodegenes/transcript.pyx":238
+    /* "gencodegenes/transcript.pyx":234
  *         # transcript, rather than raising an error.
  *         if other is None:
  *             return self             # <<<<<<<<<<<<<<
  *         if self is None:
  *             return other
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_self);
     __pyx_r = __pyx_v_self;
     goto __pyx_L0;
 
-    /* "gencodegenes/transcript.pyx":237
+    /* "gencodegenes/transcript.pyx":233
  *         # if we try transcript + None or None + transcript, return the original
  *         # transcript, rather than raising an error.
  *         if other is None:             # <<<<<<<<<<<<<<
  *             return self
  *         if self is None:
  */
   }
 
-  /* "gencodegenes/transcript.pyx":239
+  /* "gencodegenes/transcript.pyx":235
  *         if other is None:
  *             return self
  *         if self is None:             # <<<<<<<<<<<<<<
  *             return other
  * 
  */
   __pyx_t_2 = (__pyx_v_self == Py_None);
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "gencodegenes/transcript.pyx":240
+    /* "gencodegenes/transcript.pyx":236
  *             return self
  *         if self is None:
  *             return other             # <<<<<<<<<<<<<<
  * 
  *         altered = Transcript('{}:{}'.format(self.name, other.name),
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_other);
     __pyx_r = __pyx_v_other;
     goto __pyx_L0;
 
-    /* "gencodegenes/transcript.pyx":239
+    /* "gencodegenes/transcript.pyx":235
  *         if other is None:
  *             return self
  *         if self is None:             # <<<<<<<<<<<<<<
  *             return other
  * 
  */
   }
 
-  /* "gencodegenes/transcript.pyx":242
+  /* "gencodegenes/transcript.pyx":238
  *             return other
  * 
  *         altered = Transcript('{}:{}'.format(self.name, other.name),             # <<<<<<<<<<<<<<
  *             self.chrom, min(self.start, other.start),
  *             max(self.end, other.end), self.strand, self.type)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u__6, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u__6, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_name); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_name); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -5729,111 +5648,111 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_5, __pyx_t_6};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 242, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_5, __pyx_t_6};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 242, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 242, __pyx_L1_error)
+    __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_t_6);
     __pyx_t_5 = 0;
     __pyx_t_6 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 242, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "gencodegenes/transcript.pyx":243
+  /* "gencodegenes/transcript.pyx":239
  * 
  *         altered = Transcript('{}:{}'.format(self.name, other.name),
  *             self.chrom, min(self.start, other.start),             # <<<<<<<<<<<<<<
  *             max(self.end, other.end), self.strand, self.type)
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_chrom); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_chrom); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_start); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_start); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = PyObject_RichCompare(__pyx_t_9, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 243, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_7 = PyObject_RichCompare(__pyx_t_9, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (__pyx_t_1) {
     __Pyx_INCREF(__pyx_t_9);
     __pyx_t_5 = __pyx_t_9;
   } else {
     __Pyx_INCREF(__pyx_t_6);
     __pyx_t_5 = __pyx_t_6;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "gencodegenes/transcript.pyx":244
+  /* "gencodegenes/transcript.pyx":240
  *         altered = Transcript('{}:{}'.format(self.name, other.name),
  *             self.chrom, min(self.start, other.start),
  *             max(self.end, other.end), self.strand, self.type)             # <<<<<<<<<<<<<<
  * 
- *         exons = self.merge_coordinates(self.exons, other.exons)
+ *         exons = self._merge_coordinates(self.exons, other.exons)
  */
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_end); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_end); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 240, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 240, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_10 = PyObject_RichCompare(__pyx_t_9, __pyx_t_6, Py_GT); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 244, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_10 = PyObject_RichCompare(__pyx_t_9, __pyx_t_6, Py_GT); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 240, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   if (__pyx_t_1) {
     __Pyx_INCREF(__pyx_t_9);
     __pyx_t_7 = __pyx_t_9;
   } else {
     __Pyx_INCREF(__pyx_t_6);
     __pyx_t_7 = __pyx_t_6;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_strand); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_strand); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 240, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 240, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "gencodegenes/transcript.pyx":242
+  /* "gencodegenes/transcript.pyx":238
  *             return other
  * 
  *         altered = Transcript('{}:{}'.format(self.name, other.name),             # <<<<<<<<<<<<<<
  *             self.chrom, min(self.start, other.start),
  *             max(self.end, other.end), self.strand, self.type)
  */
-  __pyx_t_10 = PyTuple_New(6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_10 = PyTuple_New(6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_4);
   __Pyx_INCREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
@@ -5847,32 +5766,32 @@
   PyTuple_SET_ITEM(__pyx_t_10, 5, __pyx_t_6);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_9 = 0;
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_12gencodegenes_10transcript_Transcript), __pyx_t_10, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_12gencodegenes_10transcript_Transcript), __pyx_t_10, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_v_altered = ((struct __pyx_obj_12gencodegenes_10transcript_Transcript *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "gencodegenes/transcript.pyx":246
+  /* "gencodegenes/transcript.pyx":242
  *             max(self.end, other.end), self.strand, self.type)
  * 
- *         exons = self.merge_coordinates(self.exons, other.exons)             # <<<<<<<<<<<<<<
- *         cds = self.merge_coordinates(self.cds, other.cds)
+ *         exons = self._merge_coordinates(self.exons, other.exons)             # <<<<<<<<<<<<<<
+ *         cds = self._merge_coordinates(self.cds, other.cds)
  * 
  */
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_merge_coordinates); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_merge_coordinates); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_exons); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_exons); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_exons); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_exons); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_5 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_10);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
@@ -5881,63 +5800,63 @@
       __Pyx_DECREF_SET(__pyx_t_10, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_10)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_9, __pyx_t_7};
-    __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 246, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_9, __pyx_t_7};
-    __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 246, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   {
-    __pyx_t_4 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 246, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_8, __pyx_t_9);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_8, __pyx_t_7);
     __pyx_t_9 = 0;
     __pyx_t_7 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 246, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_v_exons = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "gencodegenes/transcript.pyx":247
+  /* "gencodegenes/transcript.pyx":243
  * 
- *         exons = self.merge_coordinates(self.exons, other.exons)
- *         cds = self.merge_coordinates(self.cds, other.cds)             # <<<<<<<<<<<<<<
+ *         exons = self._merge_coordinates(self.exons, other.exons)
+ *         cds = self._merge_coordinates(self.cds, other.cds)             # <<<<<<<<<<<<<<
  * 
  *         altered.exons = exons
  */
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_merge_coordinates); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_merge_coordinates); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_cds); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_cds); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_cds); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_cds); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_9 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_10);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
@@ -5946,143 +5865,143 @@
       __Pyx_DECREF_SET(__pyx_t_10, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_10)) {
     PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_4, __pyx_t_7};
-    __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 243, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
     PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_4, __pyx_t_7};
-    __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 243, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_9) {
       __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_9); __pyx_t_9 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_8, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_8, __pyx_t_7);
     __pyx_t_4 = 0;
     __pyx_t_7 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 243, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_v_cds = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "gencodegenes/transcript.pyx":249
- *         cds = self.merge_coordinates(self.cds, other.cds)
+  /* "gencodegenes/transcript.pyx":245
+ *         cds = self._merge_coordinates(self.cds, other.cds)
  * 
  *         altered.exons = exons             # <<<<<<<<<<<<<<
  *         altered.cds = cds
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_altered), __pyx_n_s_exons, __pyx_v_exons) < 0) __PYX_ERR(0, 249, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_altered), __pyx_n_s_exons, __pyx_v_exons) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
 
-  /* "gencodegenes/transcript.pyx":250
+  /* "gencodegenes/transcript.pyx":246
  * 
  *         altered.exons = exons
  *         altered.cds = cds             # <<<<<<<<<<<<<<
  * 
  *         if self.genomic_sequence != "":
  */
-  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_altered), __pyx_n_s_cds, __pyx_v_cds) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_altered), __pyx_n_s_cds, __pyx_v_cds) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
 
-  /* "gencodegenes/transcript.pyx":252
+  /* "gencodegenes/transcript.pyx":248
  *         altered.cds = cds
  * 
  *         if self.genomic_sequence != "":             # <<<<<<<<<<<<<<
  *             altered.genomic_offset = self.genomic_offset
- *             altered.genomic_sequence = self.merge_genomic_seq(other)
+ *             altered.genomic_sequence = self._merge_genomic_seq(other)
  */
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_genomic_sequence); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_genomic_sequence); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_6, __pyx_kp_u__3, Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_6, __pyx_kp_u__3, Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_1) {
 
-    /* "gencodegenes/transcript.pyx":253
+    /* "gencodegenes/transcript.pyx":249
  * 
  *         if self.genomic_sequence != "":
  *             altered.genomic_offset = self.genomic_offset             # <<<<<<<<<<<<<<
- *             altered.genomic_sequence = self.merge_genomic_seq(other)
+ *             altered.genomic_sequence = self._merge_genomic_seq(other)
  * 
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_genomic_offset); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_genomic_offset); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_altered), __pyx_n_s_genomic_offset, __pyx_t_6) < 0) __PYX_ERR(0, 253, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_altered), __pyx_n_s_genomic_offset, __pyx_t_6) < 0) __PYX_ERR(0, 249, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "gencodegenes/transcript.pyx":254
+    /* "gencodegenes/transcript.pyx":250
  *         if self.genomic_sequence != "":
  *             altered.genomic_offset = self.genomic_offset
- *             altered.genomic_sequence = self.merge_genomic_seq(other)             # <<<<<<<<<<<<<<
+ *             altered.genomic_sequence = self._merge_genomic_seq(other)             # <<<<<<<<<<<<<<
  * 
  *         return altered
  */
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_merge_genomic_seq); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 254, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_merge_genomic_seq); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_10);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_10, function);
       }
     }
     __pyx_t_6 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_5, __pyx_v_other) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_v_other);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 254, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_altered), __pyx_n_s_genomic_sequence, __pyx_t_6) < 0) __PYX_ERR(0, 254, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_altered), __pyx_n_s_genomic_sequence, __pyx_t_6) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "gencodegenes/transcript.pyx":252
+    /* "gencodegenes/transcript.pyx":248
  *         altered.cds = cds
  * 
  *         if self.genomic_sequence != "":             # <<<<<<<<<<<<<<
  *             altered.genomic_offset = self.genomic_offset
- *             altered.genomic_sequence = self.merge_genomic_seq(other)
+ *             altered.genomic_sequence = self._merge_genomic_seq(other)
  */
   }
 
-  /* "gencodegenes/transcript.pyx":256
- *             altered.genomic_sequence = self.merge_genomic_seq(other)
+  /* "gencodegenes/transcript.pyx":252
+ *             altered.genomic_sequence = self._merge_genomic_seq(other)
  * 
  *         return altered             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_altered));
   __pyx_r = ((PyObject *)__pyx_v_altered);
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":211
+  /* "gencodegenes/transcript.pyx":207
  *         return initial + intersect + final
  * 
  *     def __add__(self, other):             # <<<<<<<<<<<<<<
  *         """ combine the coding sequences of two Transcript objects
  * 
  */
 
@@ -6102,15 +6021,15 @@
   __Pyx_XDECREF(__pyx_v_exons);
   __Pyx_XDECREF(__pyx_v_cds);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":259
+/* "gencodegenes/transcript.pyx":255
  * 
  *     @property
  *     def name(self):             # <<<<<<<<<<<<<<
  *         '''transcript ID'''
  *         return self.thisptr.get_name().decode('utf8')
  */
 
@@ -6132,29 +6051,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gencodegenes/transcript.pyx":261
+  /* "gencodegenes/transcript.pyx":257
  *     def name(self):
  *         '''transcript ID'''
  *         return self.thisptr.get_name().decode('utf8')             # <<<<<<<<<<<<<<
  *     @property
  *     def chrom(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_self->thisptr->get_name(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 261, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_self->thisptr->get_name(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":259
+  /* "gencodegenes/transcript.pyx":255
  * 
  *     @property
  *     def name(self):             # <<<<<<<<<<<<<<
  *         '''transcript ID'''
  *         return self.thisptr.get_name().decode('utf8')
  */
 
@@ -6165,15 +6084,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":263
+/* "gencodegenes/transcript.pyx":259
  *         return self.thisptr.get_name().decode('utf8')
  *     @property
  *     def chrom(self):             # <<<<<<<<<<<<<<
  *         '''chromosome the gene is on'''
  *         return self.thisptr.get_chrom().decode('utf8')
  */
 
@@ -6195,29 +6114,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gencodegenes/transcript.pyx":265
+  /* "gencodegenes/transcript.pyx":261
  *     def chrom(self):
  *         '''chromosome the gene is on'''
  *         return self.thisptr.get_chrom().decode('utf8')             # <<<<<<<<<<<<<<
  *     @property
  *     def type(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_self->thisptr->get_chrom(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_self->thisptr->get_chrom(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 261, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":263
+  /* "gencodegenes/transcript.pyx":259
  *         return self.thisptr.get_name().decode('utf8')
  *     @property
  *     def chrom(self):             # <<<<<<<<<<<<<<
  *         '''chromosome the gene is on'''
  *         return self.thisptr.get_chrom().decode('utf8')
  */
 
@@ -6228,15 +6147,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":267
+/* "gencodegenes/transcript.pyx":263
  *         return self.thisptr.get_chrom().decode('utf8')
  *     @property
  *     def type(self):             # <<<<<<<<<<<<<<
  *         '''transcript functional type (protein_coding etc.)'''
  *         return self.thisptr.get_type().decode('utf8')
  */
 
@@ -6258,29 +6177,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gencodegenes/transcript.pyx":269
+  /* "gencodegenes/transcript.pyx":265
  *     def type(self):
  *         '''transcript functional type (protein_coding etc.)'''
  *         return self.thisptr.get_type().decode('utf8')             # <<<<<<<<<<<<<<
  *     @property
  *     def start(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_self->thisptr->get_type(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_self->thisptr->get_type(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":267
+  /* "gencodegenes/transcript.pyx":263
  *         return self.thisptr.get_chrom().decode('utf8')
  *     @property
  *     def type(self):             # <<<<<<<<<<<<<<
  *         '''transcript functional type (protein_coding etc.)'''
  *         return self.thisptr.get_type().decode('utf8')
  */
 
@@ -6291,15 +6210,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":271
+/* "gencodegenes/transcript.pyx":267
  *         return self.thisptr.get_type().decode('utf8')
  *     @property
  *     def start(self):             # <<<<<<<<<<<<<<
  *         '''transcript start position (TSS) on chromosome'''
  *         return self.thisptr.get_start()
  */
 
@@ -6321,29 +6240,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gencodegenes/transcript.pyx":273
+  /* "gencodegenes/transcript.pyx":269
  *     def start(self):
  *         '''transcript start position (TSS) on chromosome'''
  *         return self.thisptr.get_start()             # <<<<<<<<<<<<<<
  *     @property
  *     def end(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_start()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_start()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":271
+  /* "gencodegenes/transcript.pyx":267
  *         return self.thisptr.get_type().decode('utf8')
  *     @property
  *     def start(self):             # <<<<<<<<<<<<<<
  *         '''transcript start position (TSS) on chromosome'''
  *         return self.thisptr.get_start()
  */
 
@@ -6354,15 +6273,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":275
+/* "gencodegenes/transcript.pyx":271
  *         return self.thisptr.get_start()
  *     @property
  *     def end(self):             # <<<<<<<<<<<<<<
  *         '''transcript end position on chromosome'''
  *         return self.thisptr.get_end()
  */
 
@@ -6384,29 +6303,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gencodegenes/transcript.pyx":277
+  /* "gencodegenes/transcript.pyx":273
  *     def end(self):
  *         '''transcript end position on chromosome'''
  *         return self.thisptr.get_end()             # <<<<<<<<<<<<<<
  *     @property
  *     def strand(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_end()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_end()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":275
+  /* "gencodegenes/transcript.pyx":271
  *         return self.thisptr.get_start()
  *     @property
  *     def end(self):             # <<<<<<<<<<<<<<
  *         '''transcript end position on chromosome'''
  *         return self.thisptr.get_end()
  */
 
@@ -6417,15 +6336,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":279
+/* "gencodegenes/transcript.pyx":275
  *         return self.thisptr.get_end()
  *     @property
  *     def strand(self):             # <<<<<<<<<<<<<<
  *         '''strand the transcript is on (+ or -)'''
  *         return chr(self.thisptr.get_strand())
  */
 
@@ -6448,32 +6367,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gencodegenes/transcript.pyx":281
+  /* "gencodegenes/transcript.pyx":277
  *     def strand(self):
  *         '''strand the transcript is on (+ or -)'''
  *         return chr(self.thisptr.get_strand())             # <<<<<<<<<<<<<<
  *     @property
  *     def cds_start(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_char(__pyx_v_self->thisptr->get_strand()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_char(__pyx_v_self->thisptr->get_strand()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_chr, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_chr, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":279
+  /* "gencodegenes/transcript.pyx":275
  *         return self.thisptr.get_end()
  *     @property
  *     def strand(self):             # <<<<<<<<<<<<<<
  *         '''strand the transcript is on (+ or -)'''
  *         return chr(self.thisptr.get_strand())
  */
 
@@ -6485,15 +6404,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":283
+/* "gencodegenes/transcript.pyx":279
  *         return chr(self.thisptr.get_strand())
  *     @property
  *     def cds_start(self):             # <<<<<<<<<<<<<<
  *         '''CDS start position on chromosome'''
  *         return self.thisptr.get_cds_start()
  */
 
@@ -6515,29 +6434,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gencodegenes/transcript.pyx":285
+  /* "gencodegenes/transcript.pyx":281
  *     def cds_start(self):
  *         '''CDS start position on chromosome'''
  *         return self.thisptr.get_cds_start()             # <<<<<<<<<<<<<<
  *     @property
  *     def cds_end(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_cds_start()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_cds_start()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":283
+  /* "gencodegenes/transcript.pyx":279
  *         return chr(self.thisptr.get_strand())
  *     @property
  *     def cds_start(self):             # <<<<<<<<<<<<<<
  *         '''CDS start position on chromosome'''
  *         return self.thisptr.get_cds_start()
  */
 
@@ -6548,15 +6467,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":287
+/* "gencodegenes/transcript.pyx":283
  *         return self.thisptr.get_cds_start()
  *     @property
  *     def cds_end(self):             # <<<<<<<<<<<<<<
  *         '''CDS end position on chromosome'''
  *         return self.thisptr.get_cds_end()
  */
 
@@ -6578,29 +6497,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gencodegenes/transcript.pyx":289
+  /* "gencodegenes/transcript.pyx":285
  *     def cds_end(self):
  *         '''CDS end position on chromosome'''
  *         return self.thisptr.get_cds_end()             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_cds_end()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_cds_end()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":287
+  /* "gencodegenes/transcript.pyx":283
  *         return self.thisptr.get_cds_start()
  *     @property
  *     def cds_end(self):             # <<<<<<<<<<<<<<
  *         '''CDS end position on chromosome'''
  *         return self.thisptr.get_cds_end()
  */
 
@@ -6611,15 +6530,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":292
+/* "gencodegenes/transcript.pyx":288
  * 
  *     @property
  *     def exons(self):             # <<<<<<<<<<<<<<
  *         ''' list of exon coords as {'start': int, 'end': int} dicts '''
  *         return self.thisptr.get_exons()
  */
 
@@ -6641,29 +6560,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gencodegenes/transcript.pyx":294
+  /* "gencodegenes/transcript.pyx":290
  *     def exons(self):
  *         ''' list of exon coords as {'start': int, 'end': int} dicts '''
  *         return self.thisptr.get_exons()             # <<<<<<<<<<<<<<
  *     @exons.setter
  *     def exons(self, exon_ranges):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_vector_to_py_struct__Region(__pyx_v_self->thisptr->get_exons()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py_struct__Region(__pyx_v_self->thisptr->get_exons()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":292
+  /* "gencodegenes/transcript.pyx":288
  * 
  *     @property
  *     def exons(self):             # <<<<<<<<<<<<<<
  *         ''' list of exon coords as {'start': int, 'end': int} dicts '''
  *         return self.thisptr.get_exons()
  */
 
@@ -6674,15 +6593,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":296
+/* "gencodegenes/transcript.pyx":292
  *         return self.thisptr.get_exons()
  *     @exons.setter
  *     def exons(self, exon_ranges):             # <<<<<<<<<<<<<<
  *         self.thisptr.set_exons(exon_ranges)
  * 
  */
 
@@ -6704,30 +6623,30 @@
   __Pyx_RefNannyDeclarations
   std::vector<std::vector<int> >  __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "gencodegenes/transcript.pyx":297
+  /* "gencodegenes/transcript.pyx":293
  *     @exons.setter
  *     def exons(self, exon_ranges):
  *         self.thisptr.set_exons(exon_ranges)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __pyx_t_1 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_int_3e___(__pyx_v_exon_ranges); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_int_3e___(__pyx_v_exon_ranges); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 293, __pyx_L1_error)
   try {
     __pyx_v_self->thisptr->set_exons(__pyx_t_1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 297, __pyx_L1_error)
+    __PYX_ERR(0, 293, __pyx_L1_error)
   }
 
-  /* "gencodegenes/transcript.pyx":296
+  /* "gencodegenes/transcript.pyx":292
  *         return self.thisptr.get_exons()
  *     @exons.setter
  *     def exons(self, exon_ranges):             # <<<<<<<<<<<<<<
  *         self.thisptr.set_exons(exon_ranges)
  * 
  */
 
@@ -6738,15 +6657,15 @@
   __Pyx_AddTraceback("gencodegenes.transcript.Transcript.exons.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":300
+/* "gencodegenes/transcript.pyx":296
  * 
  *     @property
  *     def cds(self):             # <<<<<<<<<<<<<<
  *         '''list of CDS coords as {'start': int, 'end': int} dicts '''
  *         return self.thisptr.get_cds()
  */
 
@@ -6768,29 +6687,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gencodegenes/transcript.pyx":302
+  /* "gencodegenes/transcript.pyx":298
  *     def cds(self):
  *         '''list of CDS coords as {'start': int, 'end': int} dicts '''
  *         return self.thisptr.get_cds()             # <<<<<<<<<<<<<<
  *     @cds.setter
  *     def cds(self, cds_ranges):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_vector_to_py_struct__Region(__pyx_v_self->thisptr->get_cds()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py_struct__Region(__pyx_v_self->thisptr->get_cds()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":300
+  /* "gencodegenes/transcript.pyx":296
  * 
  *     @property
  *     def cds(self):             # <<<<<<<<<<<<<<
  *         '''list of CDS coords as {'start': int, 'end': int} dicts '''
  *         return self.thisptr.get_cds()
  */
 
@@ -6801,15 +6720,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":304
+/* "gencodegenes/transcript.pyx":300
  *         return self.thisptr.get_cds()
  *     @cds.setter
  *     def cds(self, cds_ranges):             # <<<<<<<<<<<<<<
  *         self.thisptr.set_cds(cds_ranges)
  * 
  */
 
@@ -6831,30 +6750,30 @@
   __Pyx_RefNannyDeclarations
   std::vector<std::vector<int> >  __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "gencodegenes/transcript.pyx":305
+  /* "gencodegenes/transcript.pyx":301
  *     @cds.setter
  *     def cds(self, cds_ranges):
  *         self.thisptr.set_cds(cds_ranges)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __pyx_t_1 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_int_3e___(__pyx_v_cds_ranges); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 305, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_int_3e___(__pyx_v_cds_ranges); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 301, __pyx_L1_error)
   try {
     __pyx_v_self->thisptr->set_cds(__pyx_t_1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 305, __pyx_L1_error)
+    __PYX_ERR(0, 301, __pyx_L1_error)
   }
 
-  /* "gencodegenes/transcript.pyx":304
+  /* "gencodegenes/transcript.pyx":300
  *         return self.thisptr.get_cds()
  *     @cds.setter
  *     def cds(self, cds_ranges):             # <<<<<<<<<<<<<<
  *         self.thisptr.set_cds(cds_ranges)
  * 
  */
 
@@ -6865,15 +6784,15 @@
   __Pyx_AddTraceback("gencodegenes.transcript.Transcript.cds.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":308
+/* "gencodegenes/transcript.pyx":304
  * 
  *     @property
  *     def cds_sequence(self):             # <<<<<<<<<<<<<<
  *         ''' CDS sequence for the transcript
  *         '''
  */
 
@@ -6895,29 +6814,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gencodegenes/transcript.pyx":311
+  /* "gencodegenes/transcript.pyx":307
  *         ''' CDS sequence for the transcript
  *         '''
  *         return self.thisptr.get_cds_sequence().decode('utf8')             # <<<<<<<<<<<<<<
  * 
  *     @cds_sequence.setter
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_self->thisptr->get_cds_sequence(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 311, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_self->thisptr->get_cds_sequence(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 307, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":308
+  /* "gencodegenes/transcript.pyx":304
  * 
  *     @property
  *     def cds_sequence(self):             # <<<<<<<<<<<<<<
  *         ''' CDS sequence for the transcript
  *         '''
  */
 
@@ -6928,15 +6847,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":314
+/* "gencodegenes/transcript.pyx":310
  * 
  *     @cds_sequence.setter
  *     def cds_sequence(self, text):             # <<<<<<<<<<<<<<
  *         self.thisptr.add_cds_sequence(text.encode('utf8'))
  * 
  */
 
@@ -6961,43 +6880,43 @@
   PyObject *__pyx_t_3 = NULL;
   std::string __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "gencodegenes/transcript.pyx":315
+  /* "gencodegenes/transcript.pyx":311
  *     @cds_sequence.setter
  *     def cds_sequence(self, text):
  *         self.thisptr.add_cds_sequence(text.encode('utf8'))             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_text, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 315, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_text, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 311, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_n_u_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_u_utf8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 315, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 311, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 315, __pyx_L1_error)
+  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 311, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->thisptr->add_cds_sequence(__pyx_t_4);
 
-  /* "gencodegenes/transcript.pyx":314
+  /* "gencodegenes/transcript.pyx":310
  * 
  *     @cds_sequence.setter
  *     def cds_sequence(self, text):             # <<<<<<<<<<<<<<
  *         self.thisptr.add_cds_sequence(text.encode('utf8'))
  * 
  */
 
@@ -7011,15 +6930,15 @@
   __Pyx_AddTraceback("gencodegenes.transcript.Transcript.cds_sequence.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":318
+/* "gencodegenes/transcript.pyx":314
  * 
  *     @property
  *     def genomic_offset(self):             # <<<<<<<<<<<<<<
  *         '''distance the DNA sequence extends symmetrically beyond gene boundaries'''
  *         return self.thisptr.get_genomic_offset()
  */
 
@@ -7041,29 +6960,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gencodegenes/transcript.pyx":320
+  /* "gencodegenes/transcript.pyx":316
  *     def genomic_offset(self):
  *         '''distance the DNA sequence extends symmetrically beyond gene boundaries'''
  *         return self.thisptr.get_genomic_offset()             # <<<<<<<<<<<<<<
  * 
  *     @genomic_offset.setter
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_genomic_offset()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 320, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_genomic_offset()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 316, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":318
+  /* "gencodegenes/transcript.pyx":314
  * 
  *     @property
  *     def genomic_offset(self):             # <<<<<<<<<<<<<<
  *         '''distance the DNA sequence extends symmetrically beyond gene boundaries'''
  *         return self.thisptr.get_genomic_offset()
  */
 
@@ -7074,15 +6993,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":323
+/* "gencodegenes/transcript.pyx":319
  * 
  *     @genomic_offset.setter
  *     def genomic_offset(self, int offset):             # <<<<<<<<<<<<<<
  *         self.thisptr.set_genomic_offset(offset)
  * 
  */
 
@@ -7093,15 +7012,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_offset); {
-    __pyx_v_offset = __Pyx_PyInt_As_int(__pyx_arg_offset); if (unlikely((__pyx_v_offset == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L3_error)
+    __pyx_v_offset = __Pyx_PyInt_As_int(__pyx_arg_offset); if (unlikely((__pyx_v_offset == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 319, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("gencodegenes.transcript.Transcript.genomic_offset.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -7113,38 +7032,38 @@
 }
 
 static int __pyx_pf_12gencodegenes_10transcript_10Transcript_14genomic_offset_2__set__(struct __pyx_obj_12gencodegenes_10transcript_Transcript *__pyx_v_self, int __pyx_v_offset) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "gencodegenes/transcript.pyx":324
+  /* "gencodegenes/transcript.pyx":320
  *     @genomic_offset.setter
  *     def genomic_offset(self, int offset):
  *         self.thisptr.set_genomic_offset(offset)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __pyx_v_self->thisptr->set_genomic_offset(__pyx_v_offset);
 
-  /* "gencodegenes/transcript.pyx":323
+  /* "gencodegenes/transcript.pyx":319
  * 
  *     @genomic_offset.setter
  *     def genomic_offset(self, int offset):             # <<<<<<<<<<<<<<
  *         self.thisptr.set_genomic_offset(offset)
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":327
+/* "gencodegenes/transcript.pyx":323
  * 
  *     @property
  *     def genomic_sequence(self):             # <<<<<<<<<<<<<<
  *         ''' genomic sequence spanning the transcript
  *         '''
  */
 
@@ -7166,29 +7085,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "gencodegenes/transcript.pyx":330
+  /* "gencodegenes/transcript.pyx":326
  *         ''' genomic sequence spanning the transcript
  *         '''
  *         return self.thisptr.get_genomic_sequence().decode('utf8')             # <<<<<<<<<<<<<<
  * 
  *     @genomic_sequence.setter
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_self->thisptr->get_genomic_sequence(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_self->thisptr->get_genomic_sequence(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":327
+  /* "gencodegenes/transcript.pyx":323
  * 
  *     @property
  *     def genomic_sequence(self):             # <<<<<<<<<<<<<<
  *         ''' genomic sequence spanning the transcript
  *         '''
  */
 
@@ -7199,15 +7118,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":333
+/* "gencodegenes/transcript.pyx":329
  * 
  *     @genomic_sequence.setter
  *     def genomic_sequence(self, str text):             # <<<<<<<<<<<<<<
  *         self.thisptr.add_genomic_sequence(text.encode('utf8'))
  * 
  */
 
@@ -7216,15 +7135,15 @@
 static int __pyx_pw_12gencodegenes_10transcript_10Transcript_16genomic_sequence_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_text) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 333, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 329, __pyx_L1_error)
   __pyx_r = __pyx_pf_12gencodegenes_10transcript_10Transcript_16genomic_sequence_2__set__(((struct __pyx_obj_12gencodegenes_10transcript_Transcript *)__pyx_v_self), ((PyObject*)__pyx_v_text));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -7238,37 +7157,37 @@
   PyObject *__pyx_t_1 = NULL;
   std::string __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "gencodegenes/transcript.pyx":334
+  /* "gencodegenes/transcript.pyx":330
  *     @genomic_sequence.setter
  *     def genomic_sequence(self, str text):
  *         self.thisptr.add_genomic_sequence(text.encode('utf8'))             # <<<<<<<<<<<<<<
  * 
  *     def _fix_cds_boundary(self, pos):
  */
   if (unlikely(__pyx_v_text == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 334, __pyx_L1_error)
+    __PYX_ERR(0, 330, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   try {
     __pyx_v_self->thisptr->add_genomic_sequence(__pyx_t_2);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 334, __pyx_L1_error)
+    __PYX_ERR(0, 330, __pyx_L1_error)
   }
 
-  /* "gencodegenes/transcript.pyx":333
+  /* "gencodegenes/transcript.pyx":329
  * 
  *     @genomic_sequence.setter
  *     def genomic_sequence(self, str text):             # <<<<<<<<<<<<<<
  *         self.thisptr.add_genomic_sequence(text.encode('utf8'))
  * 
  */
 
@@ -7280,15 +7199,15 @@
   __Pyx_AddTraceback("gencodegenes.transcript.Transcript.genomic_sequence.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":336
+/* "gencodegenes/transcript.pyx":332
  *         self.thisptr.add_genomic_sequence(text.encode('utf8'))
  * 
  *     def _fix_cds_boundary(self, pos):             # <<<<<<<<<<<<<<
  *         ''' adjust CDS boundary
  * 
  */
 
@@ -7313,36 +7232,36 @@
   struct Region __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_fix_cds_boundary", 0);
 
-  /* "gencodegenes/transcript.pyx":342
+  /* "gencodegenes/transcript.pyx":338
  *             pos: nucleotide position on chromosome
  *         '''
  *         return self.thisptr.fix_cds_boundary(pos)             # <<<<<<<<<<<<<<
  * 
  *     def in_exons(self, position):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 342, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 338, __pyx_L1_error)
   try {
     __pyx_t_2 = __pyx_v_self->thisptr->fix_cds_boundary(__pyx_t_1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 342, __pyx_L1_error)
+    __PYX_ERR(0, 338, __pyx_L1_error)
   }
-  __pyx_t_3 = __pyx_convert__to_py_struct__Region(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 342, __pyx_L1_error)
+  __pyx_t_3 = __pyx_convert__to_py_struct__Region(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":336
+  /* "gencodegenes/transcript.pyx":332
  *         self.thisptr.add_genomic_sequence(text.encode('utf8'))
  * 
  *     def _fix_cds_boundary(self, pos):             # <<<<<<<<<<<<<<
  *         ''' adjust CDS boundary
  * 
  */
 
@@ -7353,15 +7272,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":344
+/* "gencodegenes/transcript.pyx":340
  *         return self.thisptr.fix_cds_boundary(pos)
  * 
  *     def in_exons(self, position):             # <<<<<<<<<<<<<<
  *         ''' check if a site lies within the exon ranges
  * 
  */
 
@@ -7385,30 +7304,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("in_exons", 0);
 
-  /* "gencodegenes/transcript.pyx":351
+  /* "gencodegenes/transcript.pyx":347
  *         '''
  * 
  *         return self.thisptr.is_exonic(position)             # <<<<<<<<<<<<<<
  * 
  *     def get_closest_exon(self, pos):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_position); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 351, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->thisptr->is_exonic(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 351, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_position); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 347, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->thisptr->is_exonic(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":344
+  /* "gencodegenes/transcript.pyx":340
  *         return self.thisptr.fix_cds_boundary(pos)
  * 
  *     def in_exons(self, position):             # <<<<<<<<<<<<<<
  *         ''' check if a site lies within the exon ranges
  * 
  */
 
@@ -7419,15 +7338,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":353
+/* "gencodegenes/transcript.pyx":349
  *         return self.thisptr.is_exonic(position)
  * 
  *     def get_closest_exon(self, pos):             # <<<<<<<<<<<<<<
  *         ''' finds the the exon closest to a site
  * 
  */
 
@@ -7451,30 +7370,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_closest_exon", 0);
 
-  /* "gencodegenes/transcript.pyx":359
+  /* "gencodegenes/transcript.pyx":355
  *             pos: nucleotide position on chromosome
  *         '''
  *         return self.thisptr.get_closest_exon(pos)             # <<<<<<<<<<<<<<
  * 
  *     def in_coding_region(self, pos):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 359, __pyx_L1_error)
-  __pyx_t_2 = __pyx_convert__to_py_struct__Region(__pyx_v_self->thisptr->get_closest_exon(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert__to_py_struct__Region(__pyx_v_self->thisptr->get_closest_exon(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 355, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":353
+  /* "gencodegenes/transcript.pyx":349
  *         return self.thisptr.is_exonic(position)
  * 
  *     def get_closest_exon(self, pos):             # <<<<<<<<<<<<<<
  *         ''' finds the the exon closest to a site
  * 
  */
 
@@ -7485,15 +7404,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":361
+/* "gencodegenes/transcript.pyx":357
  *         return self.thisptr.get_closest_exon(pos)
  * 
  *     def in_coding_region(self, pos):             # <<<<<<<<<<<<<<
  *         ''' determine if a genomic position lies within the coding region
  * 
  */
 
@@ -7517,30 +7436,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("in_coding_region", 0);
 
-  /* "gencodegenes/transcript.pyx":367
+  /* "gencodegenes/transcript.pyx":363
  *             pos: nucleotide position on chromosome
  *         '''
  *         return self.thisptr.in_coding_region(pos)             # <<<<<<<<<<<<<<
  * 
  *     def get_coding_distance(self, pos):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 367, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->thisptr->in_coding_region(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->thisptr->in_coding_region(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":361
+  /* "gencodegenes/transcript.pyx":357
  *         return self.thisptr.get_closest_exon(pos)
  * 
  *     def in_coding_region(self, pos):             # <<<<<<<<<<<<<<
  *         ''' determine if a genomic position lies within the coding region
  * 
  */
 
@@ -7551,15 +7470,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":369
+/* "gencodegenes/transcript.pyx":365
  *         return self.thisptr.in_coding_region(pos)
  * 
  *     def get_coding_distance(self, pos):             # <<<<<<<<<<<<<<
  *         ''' get distance to CDS start (and intronic offset)
  * 
  */
 
@@ -7586,53 +7505,53 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_coding_distance", 0);
 
-  /* "gencodegenes/transcript.pyx":375
+  /* "gencodegenes/transcript.pyx":371
  *             pos: nucleotide position on chromosome
  *         '''
  *         coords = self.thisptr.get_coding_distance(pos)             # <<<<<<<<<<<<<<
  * 
  *         return {'pos': coords.position, 'offset': coords.offset}
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 371, __pyx_L1_error)
   try {
     __pyx_t_2 = __pyx_v_self->thisptr->get_coding_distance(__pyx_t_1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 375, __pyx_L1_error)
+    __PYX_ERR(0, 371, __pyx_L1_error)
   }
   __pyx_v_coords = __pyx_t_2;
 
-  /* "gencodegenes/transcript.pyx":377
+  /* "gencodegenes/transcript.pyx":373
  *         coords = self.thisptr.get_coding_distance(pos)
  * 
  *         return {'pos': coords.position, 'offset': coords.offset}             # <<<<<<<<<<<<<<
  * 
  *     def get_position_on_chrom(self, pos, offset=0):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_coords.position); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_coords.position); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_pos, __pyx_t_4) < 0) __PYX_ERR(0, 377, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_pos, __pyx_t_4) < 0) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_coords.offset); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_coords.offset); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_offset, __pyx_t_4) < 0) __PYX_ERR(0, 377, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_offset, __pyx_t_4) < 0) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":369
+  /* "gencodegenes/transcript.pyx":365
  *         return self.thisptr.in_coding_region(pos)
  * 
  *     def get_coding_distance(self, pos):             # <<<<<<<<<<<<<<
  *         ''' get distance to CDS start (and intronic offset)
  * 
  */
 
@@ -7644,15 +7563,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":379
+/* "gencodegenes/transcript.pyx":375
  *         return {'pos': coords.position, 'offset': coords.offset}
  * 
  *     def get_position_on_chrom(self, pos, offset=0):             # <<<<<<<<<<<<<<
  *         ''' convert CDS coordinate to position on chromosome
  * 
  */
 
@@ -7692,15 +7611,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_offset);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_position_on_chrom") < 0)) __PYX_ERR(0, 379, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_position_on_chrom") < 0)) __PYX_ERR(0, 375, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -7708,15 +7627,15 @@
       }
     }
     __pyx_v_pos = values[0];
     __pyx_v_offset = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_position_on_chrom", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 379, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_position_on_chrom", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 375, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gencodegenes.transcript.Transcript.get_position_on_chrom", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_12gencodegenes_10transcript_10Transcript_32get_position_on_chrom(((struct __pyx_obj_12gencodegenes_10transcript_Transcript *)__pyx_v_self), __pyx_v_pos, __pyx_v_offset);
 
@@ -7733,37 +7652,37 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_position_on_chrom", 0);
 
-  /* "gencodegenes/transcript.pyx":386
+  /* "gencodegenes/transcript.pyx":382
  *             offset: if intronic, number of bases into the intron
  *         '''
  *         return self.thisptr.get_position_on_chrom(pos, offset)             # <<<<<<<<<<<<<<
  * 
  *     def get_codon_number_for_cds_position(self, cds_pos):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 386, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_offset); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_offset); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L1_error)
   try {
     __pyx_t_3 = __pyx_v_self->thisptr->get_position_on_chrom(__pyx_t_1, __pyx_t_2);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 386, __pyx_L1_error)
+    __PYX_ERR(0, 382, __pyx_L1_error)
   }
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 382, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":379
+  /* "gencodegenes/transcript.pyx":375
  *         return {'pos': coords.position, 'offset': coords.offset}
  * 
  *     def get_position_on_chrom(self, pos, offset=0):             # <<<<<<<<<<<<<<
  *         ''' convert CDS coordinate to position on chromosome
  * 
  */
 
@@ -7774,15 +7693,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":388
+/* "gencodegenes/transcript.pyx":384
  *         return self.thisptr.get_position_on_chrom(pos, offset)
  * 
  *     def get_codon_number_for_cds_position(self, cds_pos):             # <<<<<<<<<<<<<<
  *         ''' find which codon number a CDS position is at
  * 
  */
 
@@ -7806,30 +7725,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_codon_number_for_cds_position", 0);
 
-  /* "gencodegenes/transcript.pyx":394
+  /* "gencodegenes/transcript.pyx":390
  *             cds_pos: CDS distance in bp to CDS start
  *         '''
  *         return self.thisptr.get_codon_number_for_cds_position(cds_pos)             # <<<<<<<<<<<<<<
  * 
  *     def get_position_within_codon(self, cds_pos):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_cds_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 394, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_codon_number_for_cds_position(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 394, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_cds_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_codon_number_for_cds_position(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 390, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":388
+  /* "gencodegenes/transcript.pyx":384
  *         return self.thisptr.get_position_on_chrom(pos, offset)
  * 
  *     def get_codon_number_for_cds_position(self, cds_pos):             # <<<<<<<<<<<<<<
  *         ''' find which codon number a CDS position is at
  * 
  */
 
@@ -7840,15 +7759,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":396
+/* "gencodegenes/transcript.pyx":392
  *         return self.thisptr.get_codon_number_for_cds_position(cds_pos)
  * 
  *     def get_position_within_codon(self, cds_pos):             # <<<<<<<<<<<<<<
  *         ''' find the position within
  * 
  */
 
@@ -7872,30 +7791,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_position_within_codon", 0);
 
-  /* "gencodegenes/transcript.pyx":402
+  /* "gencodegenes/transcript.pyx":398
  *             cds_pos: CDS distance in bp to CDS start
  *         '''
  *         return self.thisptr.get_position_within_codon(cds_pos)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_cds_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 402, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_position_within_codon(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 402, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_cds_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 398, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_position_within_codon(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":396
+  /* "gencodegenes/transcript.pyx":392
  *         return self.thisptr.get_codon_number_for_cds_position(cds_pos)
  * 
  *     def get_position_within_codon(self, cds_pos):             # <<<<<<<<<<<<<<
  *         ''' find the position within
  * 
  */
 
@@ -7906,15 +7825,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":405
+/* "gencodegenes/transcript.pyx":401
  * 
  * 
  *     def reverse_complement(self, text):             # <<<<<<<<<<<<<<
  *         ''' reverse complement a sequence
  * 
  */
 
@@ -7938,30 +7857,30 @@
   std::string __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("reverse_complement", 0);
 
-  /* "gencodegenes/transcript.pyx":411
+  /* "gencodegenes/transcript.pyx":407
  *             text: DNA sequence
  *         '''
  *         return self.thisptr.reverse_complement(text).decode('utf8')             # <<<<<<<<<<<<<<
  * 
  *     def get_centered_sequence(self, pos, length=3):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_v_text); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 411, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_v_self->thisptr->reverse_complement(__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_v_text); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_v_self->thisptr->reverse_complement(__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":405
+  /* "gencodegenes/transcript.pyx":401
  * 
  * 
  *     def reverse_complement(self, text):             # <<<<<<<<<<<<<<
  *         ''' reverse complement a sequence
  * 
  */
 
@@ -7972,15 +7891,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":413
+/* "gencodegenes/transcript.pyx":409
  *         return self.thisptr.reverse_complement(text).decode('utf8')
  * 
  *     def get_centered_sequence(self, pos, length=3):             # <<<<<<<<<<<<<<
  *         ''' get DNA sequence around a chromosome position
  * 
  */
 
@@ -8020,15 +7939,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_length);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_centered_sequence") < 0)) __PYX_ERR(0, 413, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_centered_sequence") < 0)) __PYX_ERR(0, 409, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -8036,15 +7955,15 @@
       }
     }
     __pyx_v_pos = values[0];
     __pyx_v_length = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_centered_sequence", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 413, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_centered_sequence", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 409, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gencodegenes.transcript.Transcript.get_centered_sequence", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_12gencodegenes_10transcript_10Transcript_40get_centered_sequence(((struct __pyx_obj_12gencodegenes_10transcript_Transcript *)__pyx_v_self), __pyx_v_pos, __pyx_v_length);
 
@@ -8061,37 +7980,37 @@
   std::string __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_centered_sequence", 0);
 
-  /* "gencodegenes/transcript.pyx":420
+  /* "gencodegenes/transcript.pyx":416
  *             length: number of bases to include
  *         '''
  *         return self.thisptr.get_centered_sequence(pos, length).decode('utf8')             # <<<<<<<<<<<<<<
  * 
  *     def get_codon_sequence(self, codon_num):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 420, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_length); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 416, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_length); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 416, __pyx_L1_error)
   try {
     __pyx_t_3 = __pyx_v_self->thisptr->get_centered_sequence(__pyx_t_1, __pyx_t_2);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 420, __pyx_L1_error)
+    __PYX_ERR(0, 416, __pyx_L1_error)
   }
-  __pyx_t_4 = __Pyx_decode_cpp_string(__pyx_t_3, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_decode_cpp_string(__pyx_t_3, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 416, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":413
+  /* "gencodegenes/transcript.pyx":409
  *         return self.thisptr.reverse_complement(text).decode('utf8')
  * 
  *     def get_centered_sequence(self, pos, length=3):             # <<<<<<<<<<<<<<
  *         ''' get DNA sequence around a chromosome position
  * 
  */
 
@@ -8102,15 +8021,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":422
+/* "gencodegenes/transcript.pyx":418
  *         return self.thisptr.get_centered_sequence(pos, length).decode('utf8')
  * 
  *     def get_codon_sequence(self, codon_num):             # <<<<<<<<<<<<<<
  *         ''' get the cDNA sequence for a codon
  * 
  */
 
@@ -8135,36 +8054,36 @@
   std::string __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_codon_sequence", 0);
 
-  /* "gencodegenes/transcript.pyx":428
+  /* "gencodegenes/transcript.pyx":424
  *             codon_num: number of codon to extract
  *         '''
  *         return self.thisptr.get_codon_sequence(codon_num).decode('utf8')             # <<<<<<<<<<<<<<
  * 
  *     def translate(self, text):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_codon_num); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_codon_num); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 424, __pyx_L1_error)
   try {
     __pyx_t_2 = __pyx_v_self->thisptr->get_codon_sequence(__pyx_t_1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 428, __pyx_L1_error)
+    __PYX_ERR(0, 424, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_decode_cpp_string(__pyx_t_2, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_decode_cpp_string(__pyx_t_2, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":422
+  /* "gencodegenes/transcript.pyx":418
  *         return self.thisptr.get_centered_sequence(pos, length).decode('utf8')
  * 
  *     def get_codon_sequence(self, codon_num):             # <<<<<<<<<<<<<<
  *         ''' get the cDNA sequence for a codon
  * 
  */
 
@@ -8175,15 +8094,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":430
+/* "gencodegenes/transcript.pyx":426
  *         return self.thisptr.get_codon_sequence(codon_num).decode('utf8')
  * 
  *     def translate(self, text):             # <<<<<<<<<<<<<<
  *         ''' translate DNA sequence to amino acid sequence
  * 
  */
 
@@ -8210,54 +8129,54 @@
   std::string __pyx_t_4;
   std::string __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("translate", 0);
 
-  /* "gencodegenes/transcript.pyx":436
+  /* "gencodegenes/transcript.pyx":432
  *             text: DNA/mRNA sequence
  *         '''
  *         return self.thisptr.translate(text.encode('utf8')).decode('utf8')             # <<<<<<<<<<<<<<
  * 
  *     def get_codon_info(self, pos):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_text, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_text, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_n_u_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_u_utf8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 436, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   try {
     __pyx_t_5 = __pyx_v_self->thisptr->translate(__pyx_t_4);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 436, __pyx_L1_error)
+    __PYX_ERR(0, 432, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_t_5, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_t_5, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":430
+  /* "gencodegenes/transcript.pyx":426
  *         return self.thisptr.get_codon_sequence(codon_num).decode('utf8')
  * 
  *     def translate(self, text):             # <<<<<<<<<<<<<<
  *         ''' translate DNA sequence to amino acid sequence
  * 
  */
 
@@ -8270,15 +8189,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":438
+/* "gencodegenes/transcript.pyx":434
  *         return self.thisptr.translate(text.encode('utf8')).decode('utf8')
  * 
  *     def get_codon_info(self, pos):             # <<<<<<<<<<<<<<
  *         ''' find information about the codon that a position occurs at
  * 
  */
 
@@ -8308,201 +8227,201 @@
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_codon_info", 0);
 
-  /* "gencodegenes/transcript.pyx":444
+  /* "gencodegenes/transcript.pyx":440
  *             pos: nucleotide position on chromosome
  *         '''
  *         codon = dict(self.thisptr.get_codon_info(pos))             # <<<<<<<<<<<<<<
  * 
  *         if codon['codon_number'] == -9999999:
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 440, __pyx_L1_error)
   try {
     __pyx_t_2 = __pyx_v_self->thisptr->get_codon_info(__pyx_t_1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 444, __pyx_L1_error)
+    __PYX_ERR(0, 440, __pyx_L1_error)
   }
-  __pyx_t_3 = __pyx_convert__to_py_struct__Codon(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_3 = __pyx_convert__to_py_struct__Codon(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 440, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 440, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_codon = ((PyObject*)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "gencodegenes/transcript.pyx":446
+  /* "gencodegenes/transcript.pyx":442
  *         codon = dict(self.thisptr.get_codon_info(pos))
  * 
  *         if codon['codon_number'] == -9999999:             # <<<<<<<<<<<<<<
  *             codon['codon_number'] = None
  *             codon['intra_codon'] = None
  */
-  __pyx_t_4 = __Pyx_PyDict_GetItem(__pyx_v_codon, __pyx_n_u_codon_number); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_GetItem(__pyx_v_codon, __pyx_n_u_codon_number); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 442, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_t_4, __pyx_int_neg_9999999, -9999999L, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_t_4, __pyx_int_neg_9999999, -9999999L, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 442, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 442, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_5) {
 
-    /* "gencodegenes/transcript.pyx":447
+    /* "gencodegenes/transcript.pyx":443
  * 
  *         if codon['codon_number'] == -9999999:
  *             codon['codon_number'] = None             # <<<<<<<<<<<<<<
  *             codon['intra_codon'] = None
  *             codon['codon_seq'] = None
  */
-    if (unlikely(PyDict_SetItem(__pyx_v_codon, __pyx_n_u_codon_number, Py_None) < 0)) __PYX_ERR(0, 447, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_codon, __pyx_n_u_codon_number, Py_None) < 0)) __PYX_ERR(0, 443, __pyx_L1_error)
 
-    /* "gencodegenes/transcript.pyx":448
+    /* "gencodegenes/transcript.pyx":444
  *         if codon['codon_number'] == -9999999:
  *             codon['codon_number'] = None
  *             codon['intra_codon'] = None             # <<<<<<<<<<<<<<
  *             codon['codon_seq'] = None
  *             codon['initial_aa'] = None
  */
-    if (unlikely(PyDict_SetItem(__pyx_v_codon, __pyx_n_u_intra_codon, Py_None) < 0)) __PYX_ERR(0, 448, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_codon, __pyx_n_u_intra_codon, Py_None) < 0)) __PYX_ERR(0, 444, __pyx_L1_error)
 
-    /* "gencodegenes/transcript.pyx":449
+    /* "gencodegenes/transcript.pyx":445
  *             codon['codon_number'] = None
  *             codon['intra_codon'] = None
  *             codon['codon_seq'] = None             # <<<<<<<<<<<<<<
  *             codon['initial_aa'] = None
  * 
  */
-    if (unlikely(PyDict_SetItem(__pyx_v_codon, __pyx_n_u_codon_seq, Py_None) < 0)) __PYX_ERR(0, 449, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_codon, __pyx_n_u_codon_seq, Py_None) < 0)) __PYX_ERR(0, 445, __pyx_L1_error)
 
-    /* "gencodegenes/transcript.pyx":450
+    /* "gencodegenes/transcript.pyx":446
  *             codon['intra_codon'] = None
  *             codon['codon_seq'] = None
  *             codon['initial_aa'] = None             # <<<<<<<<<<<<<<
  * 
  *         if codon['codon_seq'] is not None:
  */
-    if (unlikely(PyDict_SetItem(__pyx_v_codon, __pyx_n_u_initial_aa, Py_None) < 0)) __PYX_ERR(0, 450, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_codon, __pyx_n_u_initial_aa, Py_None) < 0)) __PYX_ERR(0, 446, __pyx_L1_error)
 
-    /* "gencodegenes/transcript.pyx":446
+    /* "gencodegenes/transcript.pyx":442
  *         codon = dict(self.thisptr.get_codon_info(pos))
  * 
  *         if codon['codon_number'] == -9999999:             # <<<<<<<<<<<<<<
  *             codon['codon_number'] = None
  *             codon['intra_codon'] = None
  */
   }
 
-  /* "gencodegenes/transcript.pyx":452
+  /* "gencodegenes/transcript.pyx":448
  *             codon['initial_aa'] = None
  * 
  *         if codon['codon_seq'] is not None:             # <<<<<<<<<<<<<<
  *             codon['codon_seq'] = codon['codon_seq'].decode('utf8')
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_codon, __pyx_n_u_codon_seq); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 452, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_codon, __pyx_n_u_codon_seq); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = (__pyx_t_3 != Py_None);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "gencodegenes/transcript.pyx":453
+    /* "gencodegenes/transcript.pyx":449
  * 
  *         if codon['codon_seq'] is not None:
  *             codon['codon_seq'] = codon['codon_seq'].decode('utf8')             # <<<<<<<<<<<<<<
  * 
  *         if codon['initial_aa'] is not None:
  */
-    __pyx_t_4 = __Pyx_PyDict_GetItem(__pyx_v_codon, __pyx_n_u_codon_seq); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 453, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_GetItem(__pyx_v_codon, __pyx_n_u_codon_seq); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_decode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 453, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_decode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_4, __pyx_n_u_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_n_u_utf8);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(PyDict_SetItem(__pyx_v_codon, __pyx_n_u_codon_seq, __pyx_t_3) < 0)) __PYX_ERR(0, 453, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_codon, __pyx_n_u_codon_seq, __pyx_t_3) < 0)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "gencodegenes/transcript.pyx":452
+    /* "gencodegenes/transcript.pyx":448
  *             codon['initial_aa'] = None
  * 
  *         if codon['codon_seq'] is not None:             # <<<<<<<<<<<<<<
  *             codon['codon_seq'] = codon['codon_seq'].decode('utf8')
  * 
  */
   }
 
-  /* "gencodegenes/transcript.pyx":455
+  /* "gencodegenes/transcript.pyx":451
  *             codon['codon_seq'] = codon['codon_seq'].decode('utf8')
  * 
  *         if codon['initial_aa'] is not None:             # <<<<<<<<<<<<<<
  *             codon['initial_aa'] = chr(codon['initial_aa'])
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_codon, __pyx_n_u_initial_aa); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 455, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_codon, __pyx_n_u_initial_aa); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_6 = (__pyx_t_3 != Py_None);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = (__pyx_t_6 != 0);
   if (__pyx_t_5) {
 
-    /* "gencodegenes/transcript.pyx":456
+    /* "gencodegenes/transcript.pyx":452
  * 
  *         if codon['initial_aa'] is not None:
  *             codon['initial_aa'] = chr(codon['initial_aa'])             # <<<<<<<<<<<<<<
  * 
  *         return codon
  */
-    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_codon, __pyx_n_u_initial_aa); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 456, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_codon, __pyx_n_u_initial_aa); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 452, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_chr, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 456, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_chr, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 452, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(PyDict_SetItem(__pyx_v_codon, __pyx_n_u_initial_aa, __pyx_t_7) < 0)) __PYX_ERR(0, 456, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_codon, __pyx_n_u_initial_aa, __pyx_t_7) < 0)) __PYX_ERR(0, 452, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "gencodegenes/transcript.pyx":455
+    /* "gencodegenes/transcript.pyx":451
  *             codon['codon_seq'] = codon['codon_seq'].decode('utf8')
  * 
  *         if codon['initial_aa'] is not None:             # <<<<<<<<<<<<<<
  *             codon['initial_aa'] = chr(codon['initial_aa'])
  * 
  */
   }
 
-  /* "gencodegenes/transcript.pyx":458
+  /* "gencodegenes/transcript.pyx":454
  *             codon['initial_aa'] = chr(codon['initial_aa'])
  * 
  *         return codon             # <<<<<<<<<<<<<<
  * 
  *     def get_boundary_distance(self, pos):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_codon);
   __pyx_r = __pyx_v_codon;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":438
+  /* "gencodegenes/transcript.pyx":434
  *         return self.thisptr.translate(text.encode('utf8')).decode('utf8')
  * 
  *     def get_codon_info(self, pos):             # <<<<<<<<<<<<<<
  *         ''' find information about the codon that a position occurs at
  * 
  */
 
@@ -8516,15 +8435,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_codon);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":460
+/* "gencodegenes/transcript.pyx":456
  *         return codon
  * 
  *     def get_boundary_distance(self, pos):             # <<<<<<<<<<<<<<
  *         ''' get the distance in bp between a site and the nearest exon boundary
  * 
  */
 
@@ -8549,36 +8468,36 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_boundary_distance", 0);
 
-  /* "gencodegenes/transcript.pyx":466
+  /* "gencodegenes/transcript.pyx":462
  *             pos: nucleotide position on chromosome
  *         '''
  *         return self.thisptr.get_boundary_distance(pos)             # <<<<<<<<<<<<<<
  * 
  *     def consequence(self, pos, ref, alt):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 466, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 462, __pyx_L1_error)
   try {
     __pyx_t_2 = __pyx_v_self->thisptr->get_boundary_distance(__pyx_t_1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 466, __pyx_L1_error)
+    __PYX_ERR(0, 462, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 466, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 462, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":460
+  /* "gencodegenes/transcript.pyx":456
  *         return codon
  * 
  *     def get_boundary_distance(self, pos):             # <<<<<<<<<<<<<<
  *         ''' get the distance in bp between a site and the nearest exon boundary
  * 
  */
 
@@ -8589,15 +8508,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "gencodegenes/transcript.pyx":468
+/* "gencodegenes/transcript.pyx":464
  *         return self.thisptr.get_boundary_distance(pos)
  * 
  *     def consequence(self, pos, ref, alt):             # <<<<<<<<<<<<<<
  *         ''' get consequence of variant on transcript
  * 
  */
 
@@ -8635,40 +8554,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pos)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ref)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("consequence", 1, 3, 3, 1); __PYX_ERR(0, 468, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("consequence", 1, 3, 3, 1); __PYX_ERR(0, 464, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_alt)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("consequence", 1, 3, 3, 2); __PYX_ERR(0, 468, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("consequence", 1, 3, 3, 2); __PYX_ERR(0, 464, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "consequence") < 0)) __PYX_ERR(0, 468, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "consequence") < 0)) __PYX_ERR(0, 464, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_pos = values[0];
     __pyx_v_ref = values[1];
     __pyx_v_alt = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("consequence", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 468, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("consequence", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 464, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("gencodegenes.transcript.Transcript.consequence", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_12gencodegenes_10transcript_10Transcript_50consequence(((struct __pyx_obj_12gencodegenes_10transcript_Transcript *)__pyx_v_self), __pyx_v_pos, __pyx_v_ref, __pyx_v_alt);
 
@@ -8689,80 +8608,80 @@
   std::string __pyx_t_6;
   std::string __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("consequence", 0);
 
-  /* "gencodegenes/transcript.pyx":476
+  /* "gencodegenes/transcript.pyx":472
  *             alt: alternate allele DNA sequence
  *         '''
  *         cq = self.thisptr.consequence(pos, ref.encode('utf8'), alt.encode('utf8'))             # <<<<<<<<<<<<<<
  *         return cq.decode('utf8')
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 476, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_ref, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_pos); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 472, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_ref, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_n_u_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_u_utf8);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 476, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __pyx_convert_string_from_py_std__in_string(__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_t_5 = __pyx_convert_string_from_py_std__in_string(__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_alt, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_alt, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_n_u_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_u_utf8);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 476, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   try {
     __pyx_t_7 = __pyx_v_self->thisptr->consequence(__pyx_t_1, __pyx_t_5, __pyx_t_6);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 476, __pyx_L1_error)
+    __PYX_ERR(0, 472, __pyx_L1_error)
   }
   __pyx_v_cq = __pyx_t_7;
 
-  /* "gencodegenes/transcript.pyx":477
+  /* "gencodegenes/transcript.pyx":473
  *         '''
  *         cq = self.thisptr.consequence(pos, ref.encode('utf8'), alt.encode('utf8'))
  *         return cq.decode('utf8')             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_v_cq, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 477, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_v_cq, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 473, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "gencodegenes/transcript.pyx":468
+  /* "gencodegenes/transcript.pyx":464
  *         return self.thisptr.get_boundary_distance(pos)
  * 
  *     def consequence(self, pos, ref, alt):             # <<<<<<<<<<<<<<
  *         ''' get consequence of variant on transcript
  * 
  */
 
@@ -9535,14 +9454,36 @@
     __pyx_pw_12gencodegenes_10transcript_10Transcript_3__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   (*Py_TYPE(o)->tp_free)(o);
 }
 
+static PyObject *__pyx_tp_richcompare_12gencodegenes_10transcript_Transcript(PyObject *o1, PyObject *o2, int op) {
+  switch (op) {
+    case Py_EQ: {
+      return __pyx_pw_12gencodegenes_10transcript_10Transcript_11__eq__(o1, o2);
+    }
+    case Py_NE: {
+      PyObject *ret;
+      ret = __pyx_pw_12gencodegenes_10transcript_10Transcript_11__eq__(o1, o2);
+      if (likely(ret && ret != Py_NotImplemented)) {
+        int b = __Pyx_PyObject_IsTrue(ret); Py_DECREF(ret);
+        if (unlikely(b < 0)) return NULL;
+        ret = (b) ? Py_False : Py_True;
+        Py_INCREF(ret);
+      }
+      return ret;
+    }
+    default: {
+      return __Pyx_NewRef(Py_NotImplemented);
+    }
+  }
+}
+
 static PyObject *__pyx_getprop_12gencodegenes_10transcript_10Transcript_name(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_12gencodegenes_10transcript_10Transcript_4name_1__get__(o);
 }
 
 static PyObject *__pyx_getprop_12gencodegenes_10transcript_10Transcript_chrom(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_12gencodegenes_10transcript_10Transcript_5chrom_1__get__(o);
 }
@@ -9640,16 +9581,16 @@
     return -1;
   }
 }
 
 static PyMethodDef __pyx_methods_12gencodegenes_10transcript_Transcript[] = {
   {"_get_overlaps", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12gencodegenes_10transcript_10Transcript_13_get_overlaps, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12gencodegenes_10transcript_10Transcript_12_get_overlaps},
   {"_insert_region", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12gencodegenes_10transcript_10Transcript_15_insert_region, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12gencodegenes_10transcript_10Transcript_14_insert_region},
-  {"merge_coordinates", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12gencodegenes_10transcript_10Transcript_17merge_coordinates, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12gencodegenes_10transcript_10Transcript_16merge_coordinates},
-  {"merge_genomic_seq", (PyCFunction)__pyx_pw_12gencodegenes_10transcript_10Transcript_19merge_genomic_seq, METH_O, __pyx_doc_12gencodegenes_10transcript_10Transcript_18merge_genomic_seq},
+  {"_merge_coordinates", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12gencodegenes_10transcript_10Transcript_17_merge_coordinates, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12gencodegenes_10transcript_10Transcript_16_merge_coordinates},
+  {"_merge_genomic_seq", (PyCFunction)__pyx_pw_12gencodegenes_10transcript_10Transcript_19_merge_genomic_seq, METH_O, __pyx_doc_12gencodegenes_10transcript_10Transcript_18_merge_genomic_seq},
   {"_fix_cds_boundary", (PyCFunction)__pyx_pw_12gencodegenes_10transcript_10Transcript_23_fix_cds_boundary, METH_O, __pyx_doc_12gencodegenes_10transcript_10Transcript_22_fix_cds_boundary},
   {"in_exons", (PyCFunction)__pyx_pw_12gencodegenes_10transcript_10Transcript_25in_exons, METH_O, __pyx_doc_12gencodegenes_10transcript_10Transcript_24in_exons},
   {"get_closest_exon", (PyCFunction)__pyx_pw_12gencodegenes_10transcript_10Transcript_27get_closest_exon, METH_O, __pyx_doc_12gencodegenes_10transcript_10Transcript_26get_closest_exon},
   {"in_coding_region", (PyCFunction)__pyx_pw_12gencodegenes_10transcript_10Transcript_29in_coding_region, METH_O, __pyx_doc_12gencodegenes_10transcript_10Transcript_28in_coding_region},
   {"get_coding_distance", (PyCFunction)__pyx_pw_12gencodegenes_10transcript_10Transcript_31get_coding_distance, METH_O, __pyx_doc_12gencodegenes_10transcript_10Transcript_30get_coding_distance},
   {"get_position_on_chrom", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_12gencodegenes_10transcript_10Transcript_33get_position_on_chrom, METH_VARARGS|METH_KEYWORDS, __pyx_doc_12gencodegenes_10transcript_10Transcript_32get_position_on_chrom},
   {"get_codon_number_for_cds_position", (PyCFunction)__pyx_pw_12gencodegenes_10transcript_10Transcript_35get_codon_number_for_cds_position, METH_O, __pyx_doc_12gencodegenes_10transcript_10Transcript_34get_codon_number_for_cds_position},
@@ -9775,15 +9716,15 @@
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE, /*tp_flags*/
   0, /*tp_doc*/
   0, /*tp_traverse*/
   0, /*tp_clear*/
-  __pyx_pw_12gencodegenes_10transcript_10Transcript_11__richcmp__, /*tp_richcompare*/
+  __pyx_tp_richcompare_12gencodegenes_10transcript_Transcript, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_12gencodegenes_10transcript_Transcript, /*tp_methods*/
   0, /*tp_members*/
   __pyx_getsets_12gencodegenes_10transcript_Transcript, /*tp_getset*/
   0, /*tp_base*/
@@ -10219,15 +10160,14 @@
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_u_N, __pyx_k_N, sizeof(__pyx_k_N), 0, 1, 0, 1},
-  {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
   {&__pyx_n_s_Transcript, __pyx_k_Transcript, sizeof(__pyx_k_Transcript), 0, 0, 1, 1},
   {&__pyx_kp_u_Transcript_name, __pyx_k_Transcript_name, sizeof(__pyx_k_Transcript_name), 0, 1, 0, 0},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
   {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
   {&__pyx_kp_u__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 1, 0, 0},
   {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
@@ -10284,15 +10224,14 @@
   {&__pyx_n_s_min, __pyx_k_min, sizeof(__pyx_k_min), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_offset, __pyx_k_offset, sizeof(__pyx_k_offset), 0, 0, 1, 1},
   {&__pyx_n_u_offset, __pyx_k_offset, sizeof(__pyx_k_offset), 0, 1, 0, 1},
   {&__pyx_kp_u_offset_2, __pyx_k_offset_2, sizeof(__pyx_k_offset_2), 0, 1, 0, 0},
-  {&__pyx_kp_u_op_0_isn_t_implemented_yet, __pyx_k_op_0_isn_t_implemented_yet, sizeof(__pyx_k_op_0_isn_t_implemented_yet), 0, 1, 0, 0},
   {&__pyx_n_s_pos, __pyx_k_pos, sizeof(__pyx_k_pos), 0, 0, 1, 1},
   {&__pyx_n_u_pos, __pyx_k_pos, sizeof(__pyx_k_pos), 0, 1, 0, 1},
   {&__pyx_n_u_protein_coding, __pyx_k_protein_coding, sizeof(__pyx_k_protein_coding), 0, 1, 0, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
@@ -10318,20 +10257,19 @@
   {&__pyx_n_s_transcript_type, __pyx_k_transcript_type, sizeof(__pyx_k_transcript_type), 0, 0, 1, 1},
   {&__pyx_kp_u_transcript_type_2, __pyx_k_transcript_type_2, sizeof(__pyx_k_transcript_type_2), 0, 1, 0, 0},
   {&__pyx_n_s_type, __pyx_k_type, sizeof(__pyx_k_type), 0, 0, 1, 1},
   {&__pyx_n_u_utf8, __pyx_k_utf8, sizeof(__pyx_k_utf8), 0, 1, 0, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 94, __pyx_L1_error)
-  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 99, __pyx_L1_error)
-  __pyx_builtin_min = __Pyx_GetBuiltinName(__pyx_n_s_min); if (!__pyx_builtin_min) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_builtin_max = __Pyx_GetBuiltinName(__pyx_n_s_max); if (!__pyx_builtin_max) __PYX_ERR(0, 115, __pyx_L1_error)
-  __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 117, __pyx_L1_error)
-  __pyx_builtin_chr = __Pyx_GetBuiltinName(__pyx_n_s_chr); if (!__pyx_builtin_chr) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_builtin_min = __Pyx_GetBuiltinName(__pyx_n_s_min); if (!__pyx_builtin_min) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_builtin_max = __Pyx_GetBuiltinName(__pyx_n_s_max); if (!__pyx_builtin_max) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_builtin_chr = __Pyx_GetBuiltinName(__pyx_n_s_chr); if (!__pyx_builtin_chr) __PYX_ERR(0, 277, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 61, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
@@ -10436,42 +10374,52 @@
   __pyx_type_12gencodegenes_10transcript_Transcript.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_12gencodegenes_10transcript_Transcript.tp_dictoffset && __pyx_type_12gencodegenes_10transcript_Transcript.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_12gencodegenes_10transcript_Transcript.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_12gencodegenes_10transcript_Transcript, "__eq__"); if (unlikely(!wrapper)) __PYX_ERR(0, 25, __pyx_L1_error)
+    if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
+      __pyx_wrapperbase_12gencodegenes_10transcript_10Transcript_10__eq__ = *((PyWrapperDescrObject *)wrapper)->d_base;
+      __pyx_wrapperbase_12gencodegenes_10transcript_10Transcript_10__eq__.doc = __pyx_doc_12gencodegenes_10transcript_10Transcript_10__eq__;
+      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_12gencodegenes_10transcript_10Transcript_10__eq__;
+    }
+  }
+  #endif
+  #if CYTHON_UPDATE_DESCRIPTOR_DOC
+  {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_12gencodegenes_10transcript_Transcript, "__add__"); if (unlikely(!wrapper)) __PYX_ERR(0, 25, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_12gencodegenes_10transcript_10Transcript_20__add__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_12gencodegenes_10transcript_10Transcript_20__add__.doc = __pyx_doc_12gencodegenes_10transcript_10Transcript_20__add__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_12gencodegenes_10transcript_10Transcript_20__add__;
     }
   }
   #endif
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Transcript, (PyObject *)&__pyx_type_12gencodegenes_10transcript_Transcript) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_12gencodegenes_10transcript_Transcript) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   __pyx_ptype_12gencodegenes_10transcript_Transcript = &__pyx_type_12gencodegenes_10transcript_Transcript;
-  if (PyType_Ready(&__pyx_type_12gencodegenes_10transcript___pyx_scope_struct___insert_region) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_12gencodegenes_10transcript___pyx_scope_struct___insert_region) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_12gencodegenes_10transcript___pyx_scope_struct___insert_region.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_12gencodegenes_10transcript___pyx_scope_struct___insert_region.tp_dictoffset && __pyx_type_12gencodegenes_10transcript___pyx_scope_struct___insert_region.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_12gencodegenes_10transcript___pyx_scope_struct___insert_region.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_12gencodegenes_10transcript___pyx_scope_struct___insert_region = &__pyx_type_12gencodegenes_10transcript___pyx_scope_struct___insert_region;
-  if (PyType_Ready(&__pyx_type_12gencodegenes_10transcript___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_12gencodegenes_10transcript___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_12gencodegenes_10transcript___pyx_scope_struct_1_genexpr.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_12gencodegenes_10transcript___pyx_scope_struct_1_genexpr.tp_dictoffset && __pyx_type_12gencodegenes_10transcript___pyx_scope_struct_1_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_12gencodegenes_10transcript___pyx_scope_struct_1_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_12gencodegenes_10transcript___pyx_scope_struct_1_genexpr = &__pyx_type_12gencodegenes_10transcript___pyx_scope_struct_1_genexpr;
-  if (PyType_Ready(&__pyx_type_12gencodegenes_10transcript___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_12gencodegenes_10transcript___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_12gencodegenes_10transcript___pyx_scope_struct_2_genexpr.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_12gencodegenes_10transcript___pyx_scope_struct_2_genexpr.tp_dictoffset && __pyx_type_12gencodegenes_10transcript___pyx_scope_struct_2_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_12gencodegenes_10transcript___pyx_scope_struct_2_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_12gencodegenes_10transcript___pyx_scope_struct_2_genexpr = &__pyx_type_12gencodegenes_10transcript___pyx_scope_struct_2_genexpr;
@@ -11634,264 +11582,14 @@
             return __Pyx_PyObject_CallMethO(func, NULL);
         }
     }
     return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
 }
 #endif
 
-/* PyIntCompare */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, CYTHON_UNUSED long inplace) {
-    if (op1 == op2) {
-        Py_RETURN_TRUE;
-    }
-    #if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_CheckExact(op1))) {
-        const long b = intval;
-        long a = PyInt_AS_LONG(op1);
-        if (a == b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
-    }
-    #endif
-    #if CYTHON_USE_PYLONG_INTERNALS
-    if (likely(PyLong_CheckExact(op1))) {
-        int unequal;
-        unsigned long uintval;
-        Py_ssize_t size = Py_SIZE(op1);
-        const digit* digits = ((PyLongObject*)op1)->ob_digit;
-        if (intval == 0) {
-            if (size == 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
-        } else if (intval < 0) {
-            if (size >= 0)
-                Py_RETURN_FALSE;
-            intval = -intval;
-            size = -size;
-        } else {
-            if (size <= 0)
-                Py_RETURN_FALSE;
-        }
-        uintval = (unsigned long) intval;
-#if PyLong_SHIFT * 4 < SIZEOF_LONG*8
-        if (uintval >> (PyLong_SHIFT * 4)) {
-            unequal = (size != 5) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
-                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[4] != ((uintval >> (4 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
-        } else
-#endif
-#if PyLong_SHIFT * 3 < SIZEOF_LONG*8
-        if (uintval >> (PyLong_SHIFT * 3)) {
-            unequal = (size != 4) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
-                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
-        } else
-#endif
-#if PyLong_SHIFT * 2 < SIZEOF_LONG*8
-        if (uintval >> (PyLong_SHIFT * 2)) {
-            unequal = (size != 3) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
-                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
-        } else
-#endif
-#if PyLong_SHIFT * 1 < SIZEOF_LONG*8
-        if (uintval >> (PyLong_SHIFT * 1)) {
-            unequal = (size != 2) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
-                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
-        } else
-#endif
-            unequal = (size != 1) || (((unsigned long) digits[0]) != (uintval & (unsigned long) PyLong_MASK));
-        if (unequal == 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
-    }
-    #endif
-    if (PyFloat_CheckExact(op1)) {
-        const long b = intval;
-        double a = PyFloat_AS_DOUBLE(op1);
-        if ((double)a == (double)b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
-    }
-    return (
-        PyObject_RichCompare(op1, op2, Py_EQ));
-}
-
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-}
-#endif
-
-/* RaiseException */
-#if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
-    }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
-        }
-    }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
-}
-#else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
-                }
-            }
-        }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
-        }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
-    }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
-    }
-    PyErr_SetObject(type, value);
-    if (tb) {
-#if CYTHON_FAST_THREAD_STATE
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
-        }
-#else
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#endif
-    }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
-}
-#endif
-
 /* PyIntBinop */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, int inplace, int zerodivision_check) {
     (void)inplace;
     (void)zerodivision_check;
     #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_CheckExact(op1))) {
@@ -12964,14 +12662,264 @@
     }
     PyErr_Format(PyExc_TypeError,
         "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
         name, type->tp_name, Py_TYPE(obj)->tp_name);
     return 0;
 }
 
+/* PyIntCompare */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, CYTHON_UNUSED long inplace) {
+    if (op1 == op2) {
+        Py_RETURN_TRUE;
+    }
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_CheckExact(op1))) {
+        const long b = intval;
+        long a = PyInt_AS_LONG(op1);
+        if (a == b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    #endif
+    #if CYTHON_USE_PYLONG_INTERNALS
+    if (likely(PyLong_CheckExact(op1))) {
+        int unequal;
+        unsigned long uintval;
+        Py_ssize_t size = Py_SIZE(op1);
+        const digit* digits = ((PyLongObject*)op1)->ob_digit;
+        if (intval == 0) {
+            if (size == 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+        } else if (intval < 0) {
+            if (size >= 0)
+                Py_RETURN_FALSE;
+            intval = -intval;
+            size = -size;
+        } else {
+            if (size <= 0)
+                Py_RETURN_FALSE;
+        }
+        uintval = (unsigned long) intval;
+#if PyLong_SHIFT * 4 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 4)) {
+            unequal = (size != 5) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[4] != ((uintval >> (4 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 3 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 3)) {
+            unequal = (size != 4) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 2 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 2)) {
+            unequal = (size != 3) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 1 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 1)) {
+            unequal = (size != 2) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+            unequal = (size != 1) || (((unsigned long) digits[0]) != (uintval & (unsigned long) PyLong_MASK));
+        if (unequal == 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    #endif
+    if (PyFloat_CheckExact(op1)) {
+        const long b = intval;
+        double a = PyFloat_AS_DOUBLE(op1);
+        if ((double)a == (double)b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    return (
+        PyObject_RichCompare(op1, op2, Py_EQ));
+}
+
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+}
+#endif
+
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
+                        CYTHON_UNUSED PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+#if CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
                  "'%.50s' object has no attribute '%U'",
                  tp->tp_name, attr_name);
@@ -13539,52 +13487,14 @@
   Py_DECREF(member);
   return res;
   bad:
   Py_XDECREF(member);
   Py_DECREF(res);
   return NULL;
 }
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
@@ -13774,14 +13684,52 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
+/* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const char neg_one = (char) -1, const_zero = (char) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
```

### Comparing `gencodegenes-1.0.7/src/gencodegenes/transcript.pxd` & `gencodegenes-1.0.8/src/gencodegenes/transcript.pxd`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/src/gencodegenes/transcript.pyx` & `gencodegenes-1.0.8/src/gencodegenes/transcript.pyx`

 * *Files 7% similar despite different names*

```diff
@@ -81,21 +81,17 @@
     
     def __str__(self):
         return self.__repr__()
     
     def __hash__(self):
         return hash((self.chrom, self.start, self.end))
     
-    def __richcmp__(self, other, op):
-        
-        if op == 2:
-            return self.__hash__() == other.__hash__()
-        else:
-            err_msg = "op {0} isn't implemented yet".format(op)
-            raise NotImplementedError(err_msg)
+    def __eq__(self, other):
+        ''' check if transcripts occupy exact same genomic region '''
+        return self.__hash__() == other.__hash__()
     
     def _get_overlaps(self, exon, regions):
         ''' find all regions which overlap a given region
         '''
         return [ i for i, x in enumerate(regions) if
             exon['start'] <= x['end'] and exon['end'] >= x['start'] ]
     
@@ -115,15 +111,15 @@
         end = max( x['end'] for x in overlaps + [region] )
         
         for i in sorted(indices, reverse=True):
             del coords[i]
         
         return coords + [{'start': start, 'end': end}]
     
-    def merge_coordinates(self, first, second):
+    def _merge_coordinates(self, first, second):
         ''' merge two sets of coordinates, to get the union of regions
         
         This uses an inefficient approach, looping over and over, but we won't
         need to perform this often.
         
         Args:
             first: list of {'start': x, 'end': y} dictionaries for first transcript
@@ -140,15 +136,15 @@
                 a, b = region, region
             
             coords = self._insert_region(coords, a)
             coords = self._insert_region(coords, b)
         
         return [ (x['start'], x['end']) for x in sorted(coords, key=lambda x: x['start']) ]
     
-    def merge_genomic_seq(self, other):
+    def _merge_genomic_seq(self, other):
         ''' merge the genomic sequence from two transcripts
         
         We have two transcripts A, and B. We need to get the contiguous sequence
         from the start of the first transcript on the chromosome to the end of
         the second transcript. The transcripts may or may not overlap. There are
         three scenarios we need to account for:
         
@@ -239,23 +235,23 @@
         if self is None:
             return other
         
         altered = Transcript('{}:{}'.format(self.name, other.name),
             self.chrom, min(self.start, other.start),
             max(self.end, other.end), self.strand, self.type)
         
-        exons = self.merge_coordinates(self.exons, other.exons)
-        cds = self.merge_coordinates(self.cds, other.cds)
+        exons = self._merge_coordinates(self.exons, other.exons)
+        cds = self._merge_coordinates(self.cds, other.cds)
         
         altered.exons = exons
         altered.cds = cds
         
         if self.genomic_sequence != "":
             altered.genomic_offset = self.genomic_offset
-            altered.genomic_sequence = self.merge_genomic_seq(other)
+            altered.genomic_sequence = self._merge_genomic_seq(other)
         
         return altered
     
     @property
     def name(self):
         '''transcript ID'''
         return self.thisptr.get_name().decode('utf8')
```

### Comparing `gencodegenes-1.0.7/src/gencodegenes/tx.cpp` & `gencodegenes-1.0.8/src/gencodegenes/tx.cpp`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/src/gencodegenes/tx.h` & `gencodegenes-1.0.8/src/gencodegenes/tx.h`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/src/gencodegenes.egg-info/PKG-INFO` & `gencodegenes-1.0.8/src/gencodegenes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gencodegenes
-Version: 1.0.7
+Version: 1.0.8
 Summary: Package to load genes from GENCODE GTF files
 Home-page: https://github.com/jeremymcrae/gencodegenes
 Author: Jeremy McRae
 Author-email: jeremy.mcrae@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `gencodegenes-1.0.7/src/gencodegenes.egg-info/SOURCES.txt` & `gencodegenes-1.0.8/src/gencodegenes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/src/gtf.cpp` & `gencodegenes-1.0.8/src/gtf.cpp`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/src/gtf.h` & `gencodegenes-1.0.8/src/gtf.h`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/src/gzstream/gzstream.C` & `gencodegenes-1.0.8/src/gzstream/gzstream.C`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/src/gzstream/gzstream.h` & `gencodegenes-1.0.8/src/gzstream/gzstream.h`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/src/tx.cpp` & `gencodegenes-1.0.8/src/tx.cpp`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/src/tx.h` & `gencodegenes-1.0.8/src/tx.h`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/tests/data/example.grch38.fa` & `gencodegenes-1.0.8/tests/data/example.grch38.fa`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/tests/data/example.grch38.gtf` & `gencodegenes-1.0.8/tests/data/example.grch38.gtf`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/tests/test_gencode.py` & `gencodegenes-1.0.8/tests/test_gencode.py`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/tests/test_sequence_methods.py` & `gencodegenes-1.0.8/tests/test_sequence_methods.py`

 * *Files identical despite different names*

### Comparing `gencodegenes-1.0.7/tests/test_transcript.py` & `gencodegenes-1.0.8/tests/test_transcript.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,16 +214,16 @@
         """
         
         a = Transcript("a", "1", 10, 20, "+")
         
         exons1 = [{'start': 10, 'end': 20}, {'start': 25, 'end': 40}]
         exons2 = [{'start': 10, 'end': 30}]
         
-        self.assertEqual(a.merge_coordinates(exons1, exons2),
-            a.merge_coordinates(exons2, exons1))
+        self.assertEqual(a._merge_coordinates(exons1, exons2),
+            a._merge_coordinates(exons2, exons1))
     
     def test_in_exons(self):
         """ test that in_exons() works correctly
         """
         
         # self.gene.exons = [(1000, 1200), (1800, 2000)]
```

