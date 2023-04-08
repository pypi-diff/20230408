# Comparing `tmp/cpprb-9.4.5.tar.gz` & `tmp/cpprb-9.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cpprb-9.4.5.tar", last modified: Sat Feb  6 15:12:05 2021, max compression
+gzip compressed data, was "dist/cpprb-9.4.6.tar", last modified: Tue Mar  2 14:29:48 2021, max compression
```

## Comparing `cpprb-9.4.5.tar` & `cpprb-9.4.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-06 15:12:05.000000 cpprb-9.4.5/
--rw-rw-rw-   0 root         (0) root         (0)       18 2021-02-06 15:11:27.000000 cpprb-9.4.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    16105 2021-02-06 15:12:05.000000 cpprb-9.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12194 2021-02-06 15:02:03.000000 cpprb-9.4.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-06 15:12:05.000000 cpprb-9.4.5/cpprb/
--rw-r--r--   0 root         (0) root         (0)  3006562 2021-02-06 15:11:33.000000 cpprb-9.4.5/cpprb/PyReplayBuffer.cpp
--rw-rw-rw-   0 root         (0) root         (0)    17708 2021-02-06 15:11:27.000000 cpprb-9.4.5/cpprb/ReplayBuffer.hh
--rw-rw-rw-   0 root         (0) root         (0)     5672 2021-02-06 15:11:27.000000 cpprb-9.4.5/cpprb/SegmentTree.hh
--rw-r--r--   0 root         (0) root         (0)   467742 2021-02-06 15:11:34.000000 cpprb-9.4.5/cpprb/VectorWrapper.cpp
--rw-rw-rw-   0 root         (0) root         (0)      401 2021-02-06 15:11:27.000000 cpprb-9.4.5/cpprb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3703 2021-02-06 15:11:27.000000 cpprb-9.4.5/cpprb/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-06 15:12:05.000000 cpprb-9.4.5/cpprb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16105 2021-02-06 15:12:05.000000 cpprb-9.4.5/cpprb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      298 2021-02-06 15:12:05.000000 cpprb-9.4.5/cpprb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-06 15:12:05.000000 cpprb-9.4.5/cpprb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      298 2021-02-06 15:12:05.000000 cpprb-9.4.5/cpprb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2021-02-06 15:12:05.000000 cpprb-9.4.5/cpprb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-02-06 15:12:05.000000 cpprb-9.4.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4088 2021-02-06 15:11:27.000000 cpprb-9.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-02 14:29:48.000000 cpprb-9.4.6/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2021-03-02 14:29:11.000000 cpprb-9.4.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    16105 2021-03-02 14:29:48.000000 cpprb-9.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12194 2021-03-02 14:09:10.000000 cpprb-9.4.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-02 14:29:48.000000 cpprb-9.4.6/cpprb/
+-rw-r--r--   0 root         (0) root         (0)  3014111 2021-03-02 14:29:17.000000 cpprb-9.4.6/cpprb/PyReplayBuffer.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    17708 2021-03-02 14:29:11.000000 cpprb-9.4.6/cpprb/ReplayBuffer.hh
+-rw-rw-rw-   0 root         (0) root         (0)     5672 2021-03-02 14:29:11.000000 cpprb-9.4.6/cpprb/SegmentTree.hh
+-rw-r--r--   0 root         (0) root         (0)   467742 2021-03-02 14:29:17.000000 cpprb-9.4.6/cpprb/VectorWrapper.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      401 2021-03-02 14:29:11.000000 cpprb-9.4.6/cpprb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3703 2021-03-02 14:29:11.000000 cpprb-9.4.6/cpprb/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-02 14:29:48.000000 cpprb-9.4.6/cpprb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16105 2021-03-02 14:29:47.000000 cpprb-9.4.6/cpprb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      298 2021-03-02 14:29:48.000000 cpprb-9.4.6/cpprb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-03-02 14:29:47.000000 cpprb-9.4.6/cpprb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      298 2021-03-02 14:29:47.000000 cpprb-9.4.6/cpprb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2021-03-02 14:29:47.000000 cpprb-9.4.6/cpprb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-03-02 14:29:48.000000 cpprb-9.4.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4088 2021-03-02 14:29:11.000000 cpprb-9.4.6/setup.py
```

### Comparing `cpprb-9.4.5/PKG-INFO` & `cpprb-9.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpprb
-Version: 9.4.5
+Version: 9.4.6
 Summary: ReplayBuffer for Reinforcement Learning written by C++ and Cython
 Home-page: https://ymd_h.gitlab.io/cpprb/
 Author: Yamada Hiroyuki
 License: UNKNOWN
 Description: ![img](https://img.shields.io/gitlab/pipeline/ymd_h/cpprb.svg)
         ![img](https://img.shields.io/pypi/v/cpprb.svg)
         ![img](https://img.shields.io/pypi/l/cpprb.svg)
```

### Comparing `cpprb-9.4.5/README.md` & `cpprb-9.4.6/README.md`

 * *Files identical despite different names*

### Comparing `cpprb-9.4.5/cpprb/PyReplayBuffer.cpp` & `cpprb-9.4.6/cpprb/PyReplayBuffer.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1524,15 +1524,15 @@
   struct __pyx_obj_5cpprb_14PyReplayBuffer_StepChecker *size_check;
   struct __pyx_obj_5cpprb_14PyReplayBuffer_NstepBuffer *nstep;
   bool use_nstep;
   size_t cache_size;
 };
 
 
-/* "cpprb/PyReplayBuffer.pyx":1313
+/* "cpprb/PyReplayBuffer.pyx":1330
  * 
  * @cython.embedsignature(True)
  * cdef class PrioritizedReplayBuffer(ReplayBuffer):             # <<<<<<<<<<<<<<
  *     r"""Prioritized replay buffer class to store transitions with priorities.
  * 
  */
 struct __pyx_obj_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer {
@@ -1545,15 +1545,15 @@
   bool check_for_update;
   __Pyx_memviewslice unchange_since_sample;
   std::vector<size_t>  idx_vec;
   std::vector<float>  ps_vec;
 };
 
 
-/* "cpprb/PyReplayBuffer.pyx":1586
+/* "cpprb/PyReplayBuffer.pyx":1603
  * 
  * @cython.embedsignature(True)
  * cdef class MPReplayBuffer:             # <<<<<<<<<<<<<<
  *     r"""Multi-process support Replay Buffer class to store transitions and to sample them randomly.
  * 
  */
 struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer {
@@ -1567,15 +1567,15 @@
   struct __pyx_obj_5cpprb_14PyReplayBuffer_StepChecker *size_check;
   PyObject *explorer_ready;
   PyObject *explorer_count;
   PyObject *learner_ready;
 };
 
 
-/* "cpprb/PyReplayBuffer.pyx":1859
+/* "cpprb/PyReplayBuffer.pyx":1876
  * 
  * 
  * cdef class ThreadSafePrioritizedSampler:             # <<<<<<<<<<<<<<
  *     cdef size_t size
  *     cdef float alpha
  */
 struct __pyx_obj_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler {
@@ -1589,15 +1589,15 @@
   PyObject *sum_a;
   PyObject *min;
   PyObject *min_a;
   ymd::CppThreadSafePrioritizedSampler<float>  *per;
 };
 
 
-/* "cpprb/PyReplayBuffer.pyx":1920
+/* "cpprb/PyReplayBuffer.pyx":1937
  * 
  * @cython.embedsignature(True)
  * cdef class MPPrioritizedReplayBuffer(MPReplayBuffer):             # <<<<<<<<<<<<<<
  *     r"""Multi-process support Prioritized Replay Buffer class to store transitions with priorities.
  * 
  */
 struct __pyx_obj_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer {
@@ -1921,37 +1921,38 @@
 
 struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer {
   void (*clear)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch);
   size_t (*get_stored_size)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch);
   size_t (*get_buffer_size)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch);
   size_t (*get_next_index)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch);
   void (*add_cache)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *);
+  void (*add_cache_i)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, size_t, size_t);
   void (*on_episode_end)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch);
   size_t (*get_current_episode_len)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch);
   bool (*is_Nstep)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *__pyx_vtabptr_5cpprb_14PyReplayBuffer_ReplayBuffer;
 
 
-/* "cpprb/PyReplayBuffer.pyx":1313
+/* "cpprb/PyReplayBuffer.pyx":1330
  * 
  * @cython.embedsignature(True)
  * cdef class PrioritizedReplayBuffer(ReplayBuffer):             # <<<<<<<<<<<<<<
  *     r"""Prioritized replay buffer class to store transitions with priorities.
  * 
  */
 
 struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer {
   struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer __pyx_base;
   float (*get_max_priority)(struct __pyx_obj_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *__pyx_vtabptr_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer;
 
 
-/* "cpprb/PyReplayBuffer.pyx":1586
+/* "cpprb/PyReplayBuffer.pyx":1603
  * 
  * @cython.embedsignature(True)
  * cdef class MPReplayBuffer:             # <<<<<<<<<<<<<<
  *     r"""Multi-process support Replay Buffer class to store transitions and to sample them randomly.
  * 
  */
 
@@ -1966,29 +1967,29 @@
   size_t (*get_next_index)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *, int __pyx_skip_dispatch);
   void (*on_episode_end)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *, int __pyx_skip_dispatch);
   bool (*is_Nstep)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *__pyx_vtabptr_5cpprb_14PyReplayBuffer_MPReplayBuffer;
 
 
-/* "cpprb/PyReplayBuffer.pyx":1859
+/* "cpprb/PyReplayBuffer.pyx":1876
  * 
  * 
  * cdef class ThreadSafePrioritizedSampler:             # <<<<<<<<<<<<<<
  *     cdef size_t size
  *     cdef float alpha
  */
 
 struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler {
   ymd::CppThreadSafePrioritizedSampler<float>  *(*ptr)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler *);
 };
 static struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler *__pyx_vtabptr_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler;
 
 
-/* "cpprb/PyReplayBuffer.pyx":1920
+/* "cpprb/PyReplayBuffer.pyx":1937
  * 
  * @cython.embedsignature(True)
  * cdef class MPPrioritizedReplayBuffer(MPReplayBuffer):             # <<<<<<<<<<<<<<
  *     r"""Multi-process support Prioritized Replay Buffer class to store transitions with priorities.
  * 
  */
 
@@ -3362,14 +3363,15 @@
 static void __pyx_f_5cpprb_14PyReplayBuffer_26ProcessSafeRingBufferIndex_clear(struct __pyx_obj_5cpprb_14PyReplayBuffer_ProcessSafeRingBufferIndex *__pyx_v_self); /* proto*/
 static size_t __pyx_f_5cpprb_14PyReplayBuffer_26ProcessSafeRingBufferIndex_get_stored_size(struct __pyx_obj_5cpprb_14PyReplayBuffer_ProcessSafeRingBufferIndex *__pyx_v_self); /* proto*/
 static void __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_clear(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
 static size_t __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_stored_size(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
 static size_t __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_buffer_size(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
 static size_t __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_next_index(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
 static void __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_add_cache(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *__pyx_v_self); /* proto*/
+static void __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_add_cache_i(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *__pyx_v_self, size_t __pyx_v_key, size_t __pyx_v_key_end); /* proto*/
 static void __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_on_episode_end(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
 static size_t __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_current_episode_len(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
 static bool __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_is_Nstep(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
 static void __pyx_f_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_clear(struct __pyx_obj_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
 static float __pyx_f_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_get_max_priority(struct __pyx_obj_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
 static void __pyx_f_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_on_episode_end(struct __pyx_obj_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
 static void __pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer__lock_explorer(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *__pyx_v_self); /* proto*/
@@ -3862,20 +3864,20 @@
 static const char __pyx_k_pyx_unpickle_StepChecker[] = "__pyx_unpickle_StepChecker";
 static const char __pyx_k_Invalid_shape_in_axis_d_d[] = "Invalid shape in axis %d: %d.";
 static const char __pyx_k_MPPrioritizedReplayBuffer[] = "MPPrioritizedReplayBuffer";
 static const char __pyx_k_ProcessSafeRingBufferIndex[] = "ProcessSafeRingBufferIndex";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_properties_must_not_be_None[] = "`properties` must not be `None`";
 static const char __pyx_k_pyx_unpickle_MPReplayBuffer[] = "__pyx_unpickle_MPReplayBuffer";
-static const char __pyx_k_ReplayBuffer_clear_line_1169[] = "ReplayBuffer.clear (line 1169)";
+static const char __pyx_k_ReplayBuffer_clear_line_1177[] = "ReplayBuffer.clear (line 1177)";
 static const char __pyx_k_ThreadSafePrioritizedSampler[] = "ThreadSafePrioritizedSampler";
 static const char __pyx_k_multiprocessing_sharedctypes[] = "multiprocessing.sharedctypes";
 static const char __pyx_k_pyx_unpickle_RingBufferIndex[] = "__pyx_unpickle_RingBufferIndex";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
-static const char __pyx_k_MPReplayBuffer_clear_line_1783[] = "MPReplayBuffer.clear (line 1783)";
+static const char __pyx_k_MPReplayBuffer_clear_line_1800[] = "MPReplayBuffer.clear (line 1800)";
 static const char __pyx_k_pyx_unpickle_MPPrioritizedRepl[] = "__pyx_unpickle_MPPrioritizedReplayBuffer";
 static const char __pyx_k_pyx_unpickle_ProcessSafeRingBu[] = "__pyx_unpickle_ProcessSafeRingBufferIndex";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_asctime_s_msecs_03d_levelname_s[] = "%(asctime)s.%(msecs)03d [%(levelname)s] (%(filename)s:%(lineno)s) %(message)s";
 static const char __pyx_k_cpprb_train_is_still_beta_relea[] = "`cpprb.train` is still beta release. API can be changed.";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_priorities_shape_is_imcompatibl[] = "`priorities` shape is imcompatible";
@@ -3938,15 +3940,15 @@
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
 static PyObject *__pyx_kp_s_Invalid_mode_expected_c_or_fortr;
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
 static PyObject *__pyx_n_s_Lock;
 static PyObject *__pyx_n_s_MPPrioritizedReplayBuffer;
 static PyObject *__pyx_n_s_MPReplayBuffer;
-static PyObject *__pyx_kp_u_MPReplayBuffer_clear_line_1783;
+static PyObject *__pyx_kp_u_MPReplayBuffer_clear_line_1800;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
 static PyObject *__pyx_n_s_Nepisodes;
 static PyObject *__pyx_kp_u_Non_native_byte_order_not_suppor;
 static PyObject *__pyx_kp_u_None;
 static PyObject *__pyx_n_s_NotImplementedError;
@@ -3962,15 +3964,15 @@
 static PyObject *__pyx_n_u_PrioritizedReplayBuffer;
 static PyObject *__pyx_n_s_Process;
 static PyObject *__pyx_n_s_ProcessSafeRingBufferIndex;
 static PyObject *__pyx_n_s_RawArray;
 static PyObject *__pyx_n_s_RawValue;
 static PyObject *__pyx_n_s_ReplayBuffer;
 static PyObject *__pyx_n_u_ReplayBuffer;
-static PyObject *__pyx_kp_u_ReplayBuffer_clear_line_1169;
+static PyObject *__pyx_kp_u_ReplayBuffer_clear_line_1177;
 static PyObject *__pyx_kp_u_Reward;
 static PyObject *__pyx_n_s_RingBufferIndex;
 static PyObject *__pyx_n_s_RuntimeError;
 static PyObject *__pyx_n_s_SPS;
 static PyObject *__pyx_n_s_SelectiveEnvironment;
 static PyObject *__pyx_n_s_SelectiveReplayBuffer;
 static PyObject *__pyx_n_s_SharedBuffer;
@@ -20366,16 +20368,18 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_5cpprb_14PyReplayBuffer_12ReplayBuffer_4add(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *__pyx_v_self, PyObject *__pyx_v_kwargs) {
   size_t __pyx_v_N;
   size_t __pyx_v_index;
   size_t __pyx_v_end;
-  CYTHON_UNUSED size_t __pyx_v_remain;
+  size_t __pyx_v_remain;
   PyObject *__pyx_v_add_idx = 0;
+  size_t __pyx_v_key_min;
+  size_t __pyx_v_key;
   PyObject *__pyx_v_name = NULL;
   PyObject *__pyx_v_b = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -20383,20 +20387,22 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   size_t __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
-  Py_ssize_t __pyx_t_11;
-  Py_ssize_t __pyx_t_12;
-  int __pyx_t_13;
-  PyObject *__pyx_t_14 = NULL;
-  PyObject *(*__pyx_t_15)(PyObject *);
-  int __pyx_t_16;
+  size_t __pyx_t_11;
+  size_t __pyx_t_12;
+  Py_ssize_t __pyx_t_13;
+  Py_ssize_t __pyx_t_14;
+  int __pyx_t_15;
+  PyObject *__pyx_t_16 = NULL;
+  PyObject *(*__pyx_t_17)(PyObject *);
+  int __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add", 0);
   __Pyx_TraceCall("add", __pyx_f[0], 1033, 0, __PYX_ERR(0, 1033, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_kwargs);
 
@@ -20509,25 +20515,25 @@
   __pyx_v_end = (__pyx_v_index + __pyx_v_N);
 
   /* "cpprb/PyReplayBuffer.pyx":1069
  *         cdef size_t index = self.index.fetch_add(N)
  *         cdef size_t end = index + N
  *         cdef size_t remain = 0             # <<<<<<<<<<<<<<
  *         cdef add_idx = np.arange(index,end)
- * 
+ *         cdef size_t key_min = 0
  */
   __Pyx_TraceLine(1069,0,__PYX_ERR(0, 1069, __pyx_L1_error))
   __pyx_v_remain = 0;
 
   /* "cpprb/PyReplayBuffer.pyx":1070
  *         cdef size_t end = index + N
  *         cdef size_t remain = 0
  *         cdef add_idx = np.arange(index,end)             # <<<<<<<<<<<<<<
+ *         cdef size_t key_min = 0
  * 
- *         if end > self.buffer_size:
  */
   __Pyx_TraceLine(1070,0,__PYX_ERR(0, 1070, __pyx_L1_error))
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1070, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_arange); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1070, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -20583,340 +20589,459 @@
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_add_idx = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1072
+  /* "cpprb/PyReplayBuffer.pyx":1071
+ *         cdef size_t remain = 0
  *         cdef add_idx = np.arange(index,end)
+ *         cdef size_t key_min = 0             # <<<<<<<<<<<<<<
+ * 
+ *         if end > self.buffer_size:
+ */
+  __Pyx_TraceLine(1071,0,__PYX_ERR(0, 1071, __pyx_L1_error))
+  __pyx_v_key_min = 0;
+
+  /* "cpprb/PyReplayBuffer.pyx":1073
+ *         cdef size_t key_min = 0
  * 
  *         if end > self.buffer_size:             # <<<<<<<<<<<<<<
  *             remain = end - self.buffer_size
  *             add_idx[add_idx >= self.buffer_size] -= self.buffer_size
  */
-  __Pyx_TraceLine(1072,0,__PYX_ERR(0, 1072, __pyx_L1_error))
+  __Pyx_TraceLine(1073,0,__PYX_ERR(0, 1073, __pyx_L1_error))
   __pyx_t_5 = ((__pyx_v_end > __pyx_v_self->buffer_size) != 0);
   if (__pyx_t_5) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1073
+    /* "cpprb/PyReplayBuffer.pyx":1074
  * 
  *         if end > self.buffer_size:
  *             remain = end - self.buffer_size             # <<<<<<<<<<<<<<
  *             add_idx[add_idx >= self.buffer_size] -= self.buffer_size
  * 
  */
-    __Pyx_TraceLine(1073,0,__PYX_ERR(0, 1073, __pyx_L1_error))
+    __Pyx_TraceLine(1074,0,__PYX_ERR(0, 1074, __pyx_L1_error))
     __pyx_v_remain = (__pyx_v_end - __pyx_v_self->buffer_size);
 
-    /* "cpprb/PyReplayBuffer.pyx":1074
+    /* "cpprb/PyReplayBuffer.pyx":1075
  *         if end > self.buffer_size:
  *             remain = end - self.buffer_size
  *             add_idx[add_idx >= self.buffer_size] -= self.buffer_size             # <<<<<<<<<<<<<<
  * 
- *         for name, b in self.buffer.items():
+ *         if self.compress_any and (remain or
  */
-    __Pyx_TraceLine(1074,0,__PYX_ERR(0, 1074, __pyx_L1_error))
-    __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_self->buffer_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1074, __pyx_L1_error)
+    __Pyx_TraceLine(1075,0,__PYX_ERR(0, 1075, __pyx_L1_error))
+    __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_self->buffer_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1075, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = PyObject_RichCompare(__pyx_v_add_idx, __pyx_t_4, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1074, __pyx_L1_error)
+    __pyx_t_2 = PyObject_RichCompare(__pyx_v_add_idx, __pyx_t_4, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1075, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_add_idx, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1074, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_add_idx, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1075, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_FromSize_t(__pyx_v_self->buffer_size); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1074, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_FromSize_t(__pyx_v_self->buffer_size); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1075, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_7 = PyNumber_InPlaceSubtract(__pyx_t_4, __pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1074, __pyx_L1_error)
+    __pyx_t_7 = PyNumber_InPlaceSubtract(__pyx_t_4, __pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1075, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(PyObject_SetItem(__pyx_v_add_idx, __pyx_t_2, __pyx_t_7) < 0)) __PYX_ERR(0, 1074, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_add_idx, __pyx_t_2, __pyx_t_7) < 0)) __PYX_ERR(0, 1075, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1072
- *         cdef add_idx = np.arange(index,end)
+    /* "cpprb/PyReplayBuffer.pyx":1073
+ *         cdef size_t key_min = 0
  * 
  *         if end > self.buffer_size:             # <<<<<<<<<<<<<<
  *             remain = end - self.buffer_size
  *             add_idx[add_idx >= self.buffer_size] -= self.buffer_size
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1076
+  /* "cpprb/PyReplayBuffer.pyx":1077
  *             add_idx[add_idx >= self.buffer_size] -= self.buffer_size
  * 
+ *         if self.compress_any and (remain or             # <<<<<<<<<<<<<<
+ *                                   self.get_stored_size() == self.buffer_size):
+ *             key_min = remain or end
+ */
+  __Pyx_TraceLine(1077,0,__PYX_ERR(0, 1077, __pyx_L1_error))
+  __pyx_t_1 = (__pyx_v_self->compress_any != 0);
+  if (__pyx_t_1) {
+  } else {
+    __pyx_t_5 = __pyx_t_1;
+    goto __pyx_L7_bool_binop_done;
+  }
+  __pyx_t_1 = (__pyx_v_remain != 0);
+  if (!__pyx_t_1) {
+  } else {
+    __pyx_t_5 = __pyx_t_1;
+    goto __pyx_L7_bool_binop_done;
+  }
+
+  /* "cpprb/PyReplayBuffer.pyx":1078
+ * 
+ *         if self.compress_any and (remain or
+ *                                   self.get_stored_size() == self.buffer_size):             # <<<<<<<<<<<<<<
+ *             key_min = remain or end
+ *             for key in range(key_min,
+ */
+  __Pyx_TraceLine(1078,0,__PYX_ERR(0, 1078, __pyx_L1_error))
+  __pyx_t_1 = ((((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_stored_size(__pyx_v_self, 0) == __pyx_v_self->buffer_size) != 0);
+  __pyx_t_5 = __pyx_t_1;
+  __pyx_L7_bool_binop_done:;
+
+  /* "cpprb/PyReplayBuffer.pyx":1077
+ *             add_idx[add_idx >= self.buffer_size] -= self.buffer_size
+ * 
+ *         if self.compress_any and (remain or             # <<<<<<<<<<<<<<
+ *                                   self.get_stored_size() == self.buffer_size):
+ *             key_min = remain or end
+ */
+  __Pyx_TraceLine(1077,0,__PYX_ERR(0, 1077, __pyx_L1_error))
+  if (__pyx_t_5) {
+
+    /* "cpprb/PyReplayBuffer.pyx":1079
+ *         if self.compress_any and (remain or
+ *                                   self.get_stored_size() == self.buffer_size):
+ *             key_min = remain or end             # <<<<<<<<<<<<<<
+ *             for key in range(key_min,
+ *                              min(key_min + self.cache_size, self.buffer_size)):
+ */
+    __Pyx_TraceLine(1079,0,__PYX_ERR(0, 1079, __pyx_L1_error))
+    if (!__pyx_v_remain) {
+    } else {
+      __pyx_t_6 = __pyx_v_remain;
+      goto __pyx_L10_bool_binop_done;
+    }
+    __pyx_t_6 = __pyx_v_end;
+    __pyx_L10_bool_binop_done:;
+    __pyx_v_key_min = __pyx_t_6;
+
+    /* "cpprb/PyReplayBuffer.pyx":1081
+ *             key_min = remain or end
+ *             for key in range(key_min,
+ *                              min(key_min + self.cache_size, self.buffer_size)):             # <<<<<<<<<<<<<<
+ *                 self.add_cache_i(key, index)
+ * 
+ */
+    __Pyx_TraceLine(1081,0,__PYX_ERR(0, 1081, __pyx_L1_error))
+    __pyx_t_6 = __pyx_v_self->buffer_size;
+    __pyx_t_11 = (__pyx_v_key_min + __pyx_v_self->cache_size);
+    if (((__pyx_t_6 < __pyx_t_11) != 0)) {
+      __pyx_t_12 = __pyx_t_6;
+    } else {
+      __pyx_t_12 = __pyx_t_11;
+    }
+    __pyx_t_6 = __pyx_t_12;
+
+    /* "cpprb/PyReplayBuffer.pyx":1080
+ *                                   self.get_stored_size() == self.buffer_size):
+ *             key_min = remain or end
+ *             for key in range(key_min,             # <<<<<<<<<<<<<<
+ *                              min(key_min + self.cache_size, self.buffer_size)):
+ *                 self.add_cache_i(key, index)
+ */
+    __Pyx_TraceLine(1080,0,__PYX_ERR(0, 1080, __pyx_L1_error))
+    __pyx_t_12 = __pyx_t_6;
+    for (__pyx_t_11 = __pyx_v_key_min; __pyx_t_11 < __pyx_t_12; __pyx_t_11+=1) {
+      __pyx_v_key = __pyx_t_11;
+
+      /* "cpprb/PyReplayBuffer.pyx":1082
+ *             for key in range(key_min,
+ *                              min(key_min + self.cache_size, self.buffer_size)):
+ *                 self.add_cache_i(key, index)             # <<<<<<<<<<<<<<
+ * 
+ *         for name, b in self.buffer.items():
+ */
+      __Pyx_TraceLine(1082,0,__PYX_ERR(0, 1082, __pyx_L1_error))
+      ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self->__pyx_vtab)->add_cache_i(__pyx_v_self, __pyx_v_key, __pyx_v_index);
+    }
+
+    /* "cpprb/PyReplayBuffer.pyx":1077
+ *             add_idx[add_idx >= self.buffer_size] -= self.buffer_size
+ * 
+ *         if self.compress_any and (remain or             # <<<<<<<<<<<<<<
+ *                                   self.get_stored_size() == self.buffer_size):
+ *             key_min = remain or end
+ */
+  }
+
+  /* "cpprb/PyReplayBuffer.pyx":1084
+ *                 self.add_cache_i(key, index)
+ * 
  *         for name, b in self.buffer.items():             # <<<<<<<<<<<<<<
  *             b[add_idx] = np.reshape(np.array(kwargs[name],copy=False,ndmin=2),
  *                                     self.env_dict[name]["add_shape"])
  */
-  __Pyx_TraceLine(1076,0,__PYX_ERR(0, 1076, __pyx_L1_error))
-  __pyx_t_11 = 0;
+  __Pyx_TraceLine(1084,0,__PYX_ERR(0, 1084, __pyx_L1_error))
+  __pyx_t_13 = 0;
   if (unlikely(__pyx_v_self->buffer == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-    __PYX_ERR(0, 1076, __pyx_L1_error)
+    __PYX_ERR(0, 1084, __pyx_L1_error)
   }
-  __pyx_t_7 = __Pyx_dict_iterator(__pyx_v_self->buffer, 0, __pyx_n_s_items, (&__pyx_t_12), (&__pyx_t_9)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1076, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_dict_iterator(__pyx_v_self->buffer, 0, __pyx_n_s_items, (&__pyx_t_14), (&__pyx_t_9)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1084, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_2);
   __pyx_t_2 = __pyx_t_7;
   __pyx_t_7 = 0;
   while (1) {
-    __pyx_t_13 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_12, &__pyx_t_11, &__pyx_t_7, &__pyx_t_10, NULL, __pyx_t_9);
-    if (unlikely(__pyx_t_13 == 0)) break;
-    if (unlikely(__pyx_t_13 == -1)) __PYX_ERR(0, 1076, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_14, &__pyx_t_13, &__pyx_t_7, &__pyx_t_10, NULL, __pyx_t_9);
+    if (unlikely(__pyx_t_15 == 0)) break;
+    if (unlikely(__pyx_t_15 == -1)) __PYX_ERR(0, 1084, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_XDECREF_SET(__pyx_v_b, __pyx_t_10);
     __pyx_t_10 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1077
+    /* "cpprb/PyReplayBuffer.pyx":1085
  * 
  *         for name, b in self.buffer.items():
  *             b[add_idx] = np.reshape(np.array(kwargs[name],copy=False,ndmin=2),             # <<<<<<<<<<<<<<
  *                                     self.env_dict[name]["add_shape"])
  * 
  */
-    __Pyx_TraceLine(1077,0,__PYX_ERR(0, 1077, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1077, __pyx_L1_error)
+    __Pyx_TraceLine(1085,0,__PYX_ERR(0, 1085, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1085, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_reshape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1077, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_reshape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1085, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1077, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1085, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1077, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1085, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_kwargs, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1077, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_kwargs, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1085, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1077, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1085, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7);
     __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1077, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1085, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1077, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_ndmin, __pyx_int_2) < 0) __PYX_ERR(0, 1077, __pyx_L1_error)
-    __pyx_t_14 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, __pyx_t_7); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1077, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_14);
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1085, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_ndmin, __pyx_int_2) < 0) __PYX_ERR(0, 1085, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, __pyx_t_7); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 1085, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_16);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1078
+    /* "cpprb/PyReplayBuffer.pyx":1086
  *         for name, b in self.buffer.items():
  *             b[add_idx] = np.reshape(np.array(kwargs[name],copy=False,ndmin=2),
  *                                     self.env_dict[name]["add_shape"])             # <<<<<<<<<<<<<<
  * 
  *         if self.has_next_of:
  */
-    __Pyx_TraceLine(1078,0,__PYX_ERR(0, 1078, __pyx_L1_error))
-    __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_self->env_dict, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1078, __pyx_L1_error)
+    __Pyx_TraceLine(1086,0,__PYX_ERR(0, 1086, __pyx_L1_error))
+    __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_self->env_dict, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1086, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_add_shape); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1078, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_add_shape); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1086, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = NULL;
-    __pyx_t_13 = 0;
+    __pyx_t_15 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
-        __pyx_t_13 = 1;
+        __pyx_t_15 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_4)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_14, __pyx_t_8};
-      __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_13, 2+__pyx_t_13); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1077, __pyx_L1_error)
+      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_16, __pyx_t_8};
+      __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1085, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_10);
-      __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+      __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_14, __pyx_t_8};
-      __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_13, 2+__pyx_t_13); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1077, __pyx_L1_error)
+      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_16, __pyx_t_8};
+      __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1085, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_10);
-      __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+      __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     } else
     #endif
     {
-      __pyx_t_3 = PyTuple_New(2+__pyx_t_13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1077, __pyx_L1_error)
+      __pyx_t_3 = PyTuple_New(2+__pyx_t_15); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1085, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       if (__pyx_t_7) {
         __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_7); __pyx_t_7 = NULL;
       }
-      __Pyx_GIVEREF(__pyx_t_14);
-      PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_13, __pyx_t_14);
+      __Pyx_GIVEREF(__pyx_t_16);
+      PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_15, __pyx_t_16);
       __Pyx_GIVEREF(__pyx_t_8);
-      PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_13, __pyx_t_8);
-      __pyx_t_14 = 0;
+      PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_15, __pyx_t_8);
+      __pyx_t_16 = 0;
       __pyx_t_8 = 0;
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1077, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1085, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1077
+    /* "cpprb/PyReplayBuffer.pyx":1085
  * 
  *         for name, b in self.buffer.items():
  *             b[add_idx] = np.reshape(np.array(kwargs[name],copy=False,ndmin=2),             # <<<<<<<<<<<<<<
  *                                     self.env_dict[name]["add_shape"])
  * 
  */
-    __Pyx_TraceLine(1077,0,__PYX_ERR(0, 1077, __pyx_L1_error))
-    if (unlikely(PyObject_SetItem(__pyx_v_b, __pyx_v_add_idx, __pyx_t_10) < 0)) __PYX_ERR(0, 1077, __pyx_L1_error)
+    __Pyx_TraceLine(1085,0,__PYX_ERR(0, 1085, __pyx_L1_error))
+    if (unlikely(PyObject_SetItem(__pyx_v_b, __pyx_v_add_idx, __pyx_t_10) < 0)) __PYX_ERR(0, 1085, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1080
+  /* "cpprb/PyReplayBuffer.pyx":1088
  *                                     self.env_dict[name]["add_shape"])
  * 
  *         if self.has_next_of:             # <<<<<<<<<<<<<<
  *             for name in self.next_of:
  *                 self.next_[name][...]=np.reshape(np.array(kwargs[f"next_{name}"],
  */
-  __Pyx_TraceLine(1080,0,__PYX_ERR(0, 1080, __pyx_L1_error))
+  __Pyx_TraceLine(1088,0,__PYX_ERR(0, 1088, __pyx_L1_error))
   __pyx_t_5 = (__pyx_v_self->has_next_of != 0);
   if (__pyx_t_5) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1081
+    /* "cpprb/PyReplayBuffer.pyx":1089
  * 
  *         if self.has_next_of:
  *             for name in self.next_of:             # <<<<<<<<<<<<<<
  *                 self.next_[name][...]=np.reshape(np.array(kwargs[f"next_{name}"],
  *                                                           copy=False,
  */
-    __Pyx_TraceLine(1081,0,__PYX_ERR(0, 1081, __pyx_L1_error))
+    __Pyx_TraceLine(1089,0,__PYX_ERR(0, 1089, __pyx_L1_error))
     if (likely(PyList_CheckExact(__pyx_v_self->next_of)) || PyTuple_CheckExact(__pyx_v_self->next_of)) {
-      __pyx_t_2 = __pyx_v_self->next_of; __Pyx_INCREF(__pyx_t_2); __pyx_t_12 = 0;
-      __pyx_t_15 = NULL;
+      __pyx_t_2 = __pyx_v_self->next_of; __Pyx_INCREF(__pyx_t_2); __pyx_t_14 = 0;
+      __pyx_t_17 = NULL;
     } else {
-      __pyx_t_12 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_self->next_of); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1081, __pyx_L1_error)
+      __pyx_t_14 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_self->next_of); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1089, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_15 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 1081, __pyx_L1_error)
+      __pyx_t_17 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1089, __pyx_L1_error)
     }
     for (;;) {
-      if (likely(!__pyx_t_15)) {
+      if (likely(!__pyx_t_17)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
-          if (__pyx_t_12 >= PyList_GET_SIZE(__pyx_t_2)) break;
+          if (__pyx_t_14 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_10 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_12); __Pyx_INCREF(__pyx_t_10); __pyx_t_12++; if (unlikely(0 < 0)) __PYX_ERR(0, 1081, __pyx_L1_error)
+          __pyx_t_10 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_14); __Pyx_INCREF(__pyx_t_10); __pyx_t_14++; if (unlikely(0 < 0)) __PYX_ERR(0, 1089, __pyx_L1_error)
           #else
-          __pyx_t_10 = PySequence_ITEM(__pyx_t_2, __pyx_t_12); __pyx_t_12++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1081, __pyx_L1_error)
+          __pyx_t_10 = PySequence_ITEM(__pyx_t_2, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1089, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_10);
           #endif
         } else {
-          if (__pyx_t_12 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+          if (__pyx_t_14 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_10 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_12); __Pyx_INCREF(__pyx_t_10); __pyx_t_12++; if (unlikely(0 < 0)) __PYX_ERR(0, 1081, __pyx_L1_error)
+          __pyx_t_10 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_14); __Pyx_INCREF(__pyx_t_10); __pyx_t_14++; if (unlikely(0 < 0)) __PYX_ERR(0, 1089, __pyx_L1_error)
           #else
-          __pyx_t_10 = PySequence_ITEM(__pyx_t_2, __pyx_t_12); __pyx_t_12++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1081, __pyx_L1_error)
+          __pyx_t_10 = PySequence_ITEM(__pyx_t_2, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1089, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_10);
           #endif
         }
       } else {
-        __pyx_t_10 = __pyx_t_15(__pyx_t_2);
+        __pyx_t_10 = __pyx_t_17(__pyx_t_2);
         if (unlikely(!__pyx_t_10)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 1081, __pyx_L1_error)
+            else __PYX_ERR(0, 1089, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_10);
       }
       __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_10);
       __pyx_t_10 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":1082
+      /* "cpprb/PyReplayBuffer.pyx":1090
  *         if self.has_next_of:
  *             for name in self.next_of:
  *                 self.next_[name][...]=np.reshape(np.array(kwargs[f"next_{name}"],             # <<<<<<<<<<<<<<
  *                                                           copy=False,
  *                                                           ndmin=2),
  */
-      __Pyx_TraceLine(1082,0,__PYX_ERR(0, 1082, __pyx_L1_error))
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1082, __pyx_L1_error)
+      __Pyx_TraceLine(1090,0,__PYX_ERR(0, 1090, __pyx_L1_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1090, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_reshape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1082, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_reshape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1090, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1082, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1090, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_array); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1082, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_array); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1090, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1082, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1090, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_14 = __Pyx_PyUnicode_Concat(__pyx_n_u_next, __pyx_t_4); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1082, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_14);
+      __pyx_t_16 = __Pyx_PyUnicode_Concat(__pyx_n_u_next, __pyx_t_4); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 1090, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_16);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_kwargs, __pyx_t_14); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1082, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_kwargs, __pyx_t_16); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1090, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-      __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1082, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_14);
+      __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+      __pyx_t_16 = PyTuple_New(1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 1090, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_16);
       __Pyx_GIVEREF(__pyx_t_4);
-      PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_4);
+      PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":1083
+      /* "cpprb/PyReplayBuffer.pyx":1091
  *             for name in self.next_of:
  *                 self.next_[name][...]=np.reshape(np.array(kwargs[f"next_{name}"],
  *                                                           copy=False,             # <<<<<<<<<<<<<<
  *                                                           ndmin=2),
  *                                                  self.env_dict[name]["add_shape"])[-1]
  */
-      __Pyx_TraceLine(1083,0,__PYX_ERR(0, 1083, __pyx_L1_error))
-      __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1083, __pyx_L1_error)
+      __Pyx_TraceLine(1091,0,__PYX_ERR(0, 1091, __pyx_L1_error))
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1091, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1083, __pyx_L1_error)
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_ndmin, __pyx_int_2) < 0) __PYX_ERR(0, 1083, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1091, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_ndmin, __pyx_int_2) < 0) __PYX_ERR(0, 1091, __pyx_L1_error)
 
-      /* "cpprb/PyReplayBuffer.pyx":1082
+      /* "cpprb/PyReplayBuffer.pyx":1090
  *         if self.has_next_of:
  *             for name in self.next_of:
  *                 self.next_[name][...]=np.reshape(np.array(kwargs[f"next_{name}"],             # <<<<<<<<<<<<<<
  *                                                           copy=False,
  *                                                           ndmin=2),
  */
-      __Pyx_TraceLine(1082,0,__PYX_ERR(0, 1082, __pyx_L1_error))
-      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_14, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1082, __pyx_L1_error)
+      __Pyx_TraceLine(1090,0,__PYX_ERR(0, 1090, __pyx_L1_error))
+      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_16, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1090, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+      __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":1085
+      /* "cpprb/PyReplayBuffer.pyx":1093
  *                                                           copy=False,
  *                                                           ndmin=2),
  *                                                  self.env_dict[name]["add_shape"])[-1]             # <<<<<<<<<<<<<<
  * 
  *         if (self.cache is not None) and (index in self.cache):
  */
-      __Pyx_TraceLine(1085,0,__PYX_ERR(0, 1085, __pyx_L1_error))
-      __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_self->env_dict, __pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1085, __pyx_L1_error)
+      __Pyx_TraceLine(1093,0,__PYX_ERR(0, 1093, __pyx_L1_error))
+      __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_self->env_dict, __pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1093, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_14 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_n_u_add_shape); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1085, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_14);
+      __pyx_t_16 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_n_u_add_shape); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 1093, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_16);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       __pyx_t_9 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -20924,150 +21049,150 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
           __pyx_t_9 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_3)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_7, __pyx_t_14};
-        __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1082, __pyx_L1_error)
+        PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_7, __pyx_t_16};
+        __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1090, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_7, __pyx_t_14};
-        __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1082, __pyx_L1_error)
+        PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_7, __pyx_t_16};
+        __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1090, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+        __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
       } else
       #endif
       {
-        __pyx_t_8 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1082, __pyx_L1_error)
+        __pyx_t_8 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1090, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         if (__pyx_t_4) {
           __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_4); __pyx_t_4 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_9, __pyx_t_7);
-        __Pyx_GIVEREF(__pyx_t_14);
-        PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_9, __pyx_t_14);
+        __Pyx_GIVEREF(__pyx_t_16);
+        PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_9, __pyx_t_16);
         __pyx_t_7 = 0;
-        __pyx_t_14 = 0;
-        __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1082, __pyx_L1_error)
+        __pyx_t_16 = 0;
+        __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1090, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_10, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1085, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_10, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1093, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":1082
+      /* "cpprb/PyReplayBuffer.pyx":1090
  *         if self.has_next_of:
  *             for name in self.next_of:
  *                 self.next_[name][...]=np.reshape(np.array(kwargs[f"next_{name}"],             # <<<<<<<<<<<<<<
  *                                                           copy=False,
  *                                                           ndmin=2),
  */
-      __Pyx_TraceLine(1082,0,__PYX_ERR(0, 1082, __pyx_L1_error))
-      __pyx_t_10 = __Pyx_PyObject_GetItem(__pyx_v_self->next_, __pyx_v_name); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1082, __pyx_L1_error)
+      __Pyx_TraceLine(1090,0,__PYX_ERR(0, 1090, __pyx_L1_error))
+      __pyx_t_10 = __Pyx_PyObject_GetItem(__pyx_v_self->next_, __pyx_v_name); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1090, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
-      if (unlikely(PyObject_SetItem(__pyx_t_10, Py_Ellipsis, __pyx_t_3) < 0)) __PYX_ERR(0, 1082, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(__pyx_t_10, Py_Ellipsis, __pyx_t_3) < 0)) __PYX_ERR(0, 1090, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":1081
+      /* "cpprb/PyReplayBuffer.pyx":1089
  * 
  *         if self.has_next_of:
  *             for name in self.next_of:             # <<<<<<<<<<<<<<
  *                 self.next_[name][...]=np.reshape(np.array(kwargs[f"next_{name}"],
  *                                                           copy=False,
  */
-      __Pyx_TraceLine(1081,0,__PYX_ERR(0, 1081, __pyx_L1_error))
+      __Pyx_TraceLine(1089,0,__PYX_ERR(0, 1089, __pyx_L1_error))
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1080
+    /* "cpprb/PyReplayBuffer.pyx":1088
  *                                     self.env_dict[name]["add_shape"])
  * 
  *         if self.has_next_of:             # <<<<<<<<<<<<<<
  *             for name in self.next_of:
  *                 self.next_[name][...]=np.reshape(np.array(kwargs[f"next_{name}"],
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1087
+  /* "cpprb/PyReplayBuffer.pyx":1095
  *                                                  self.env_dict[name]["add_shape"])[-1]
  * 
  *         if (self.cache is not None) and (index in self.cache):             # <<<<<<<<<<<<<<
  *             del self.cache[index]
  * 
  */
-  __Pyx_TraceLine(1087,0,__PYX_ERR(0, 1087, __pyx_L1_error))
+  __Pyx_TraceLine(1095,0,__PYX_ERR(0, 1095, __pyx_L1_error))
   __pyx_t_1 = (__pyx_v_self->cache != Py_None);
-  __pyx_t_16 = (__pyx_t_1 != 0);
-  if (__pyx_t_16) {
+  __pyx_t_18 = (__pyx_t_1 != 0);
+  if (__pyx_t_18) {
   } else {
-    __pyx_t_5 = __pyx_t_16;
-    goto __pyx_L12_bool_binop_done;
+    __pyx_t_5 = __pyx_t_18;
+    goto __pyx_L20_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1087, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1095, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_16 = (__Pyx_PySequence_ContainsTF(__pyx_t_2, __pyx_v_self->cache, Py_EQ)); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 1087, __pyx_L1_error)
+  __pyx_t_18 = (__Pyx_PySequence_ContainsTF(__pyx_t_2, __pyx_v_self->cache, Py_EQ)); if (unlikely(__pyx_t_18 < 0)) __PYX_ERR(0, 1095, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_1 = (__pyx_t_16 != 0);
+  __pyx_t_1 = (__pyx_t_18 != 0);
   __pyx_t_5 = __pyx_t_1;
-  __pyx_L12_bool_binop_done:;
+  __pyx_L20_bool_binop_done:;
   if (__pyx_t_5) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1088
+    /* "cpprb/PyReplayBuffer.pyx":1096
  * 
  *         if (self.cache is not None) and (index in self.cache):
  *             del self.cache[index]             # <<<<<<<<<<<<<<
  * 
  *         self.episode_len += N
  */
-    __Pyx_TraceLine(1088,0,__PYX_ERR(0, 1088, __pyx_L1_error))
-    if (unlikely(__Pyx_DelItemInt(__pyx_v_self->cache, __pyx_v_index, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1) < 0)) __PYX_ERR(0, 1088, __pyx_L1_error)
+    __Pyx_TraceLine(1096,0,__PYX_ERR(0, 1096, __pyx_L1_error))
+    if (unlikely(__Pyx_DelItemInt(__pyx_v_self->cache, __pyx_v_index, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1) < 0)) __PYX_ERR(0, 1096, __pyx_L1_error)
 
-    /* "cpprb/PyReplayBuffer.pyx":1087
+    /* "cpprb/PyReplayBuffer.pyx":1095
  *                                                  self.env_dict[name]["add_shape"])[-1]
  * 
  *         if (self.cache is not None) and (index in self.cache):             # <<<<<<<<<<<<<<
  *             del self.cache[index]
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1090
+  /* "cpprb/PyReplayBuffer.pyx":1098
  *             del self.cache[index]
  * 
  *         self.episode_len += N             # <<<<<<<<<<<<<<
  *         return index
  * 
  */
-  __Pyx_TraceLine(1090,0,__PYX_ERR(0, 1090, __pyx_L1_error))
+  __Pyx_TraceLine(1098,0,__PYX_ERR(0, 1098, __pyx_L1_error))
   __pyx_v_self->episode_len = (__pyx_v_self->episode_len + __pyx_v_N);
 
-  /* "cpprb/PyReplayBuffer.pyx":1091
+  /* "cpprb/PyReplayBuffer.pyx":1099
  * 
  *         self.episode_len += N
  *         return index             # <<<<<<<<<<<<<<
  * 
  *     def get_all_transitions(self,shuffle: bool=False):
  */
-  __Pyx_TraceLine(1091,0,__PYX_ERR(0, 1091, __pyx_L1_error))
+  __Pyx_TraceLine(1099,0,__PYX_ERR(0, 1099, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1091, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1099, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "cpprb/PyReplayBuffer.pyx":1033
  *         pass
@@ -21081,29 +21206,29 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_XDECREF(__pyx_t_14);
+  __Pyx_XDECREF(__pyx_t_16);
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.ReplayBuffer.add", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_XDECREF(__pyx_v_add_idx);
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_XDECREF(__pyx_v_b);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1093
+/* "cpprb/PyReplayBuffer.pyx":1101
  *         return index
  * 
  *     def get_all_transitions(self,shuffle: bool=False):             # <<<<<<<<<<<<<<
  *         r"""
  *         Get all transitions stored in replay buffer.
  */
 
@@ -21135,33 +21260,33 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_shuffle);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_all_transitions") < 0)) __PYX_ERR(0, 1093, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_all_transitions") < 0)) __PYX_ERR(0, 1101, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_shuffle = __Pyx_PyObject_IsTrue(values[0]); if (unlikely((__pyx_v_shuffle == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1093, __pyx_L3_error)
+      __pyx_v_shuffle = __Pyx_PyObject_IsTrue(values[0]); if (unlikely((__pyx_v_shuffle == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1101, __pyx_L3_error)
     } else {
       __pyx_v_shuffle = ((bool)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_all_transitions", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1093, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_all_transitions", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1101, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.ReplayBuffer.get_all_transitions", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_12ReplayBuffer_6get_all_transitions(((struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self), __pyx_v_shuffle);
 
@@ -21180,134 +21305,134 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_all_transitions", 0);
-  __Pyx_TraceCall("get_all_transitions", __pyx_f[0], 1093, 0, __PYX_ERR(0, 1093, __pyx_L1_error));
+  __Pyx_TraceCall("get_all_transitions", __pyx_f[0], 1101, 0, __PYX_ERR(0, 1101, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1107
+  /* "cpprb/PyReplayBuffer.pyx":1115
  *             All transitions stored in this replay buffer.
  *         """
  *         idx = np.arange(self.get_stored_size())             # <<<<<<<<<<<<<<
  * 
  *         if shuffle:
  */
-  __Pyx_TraceLine(1107,0,__PYX_ERR(0, 1107, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1107, __pyx_L1_error)
+  __Pyx_TraceLine(1115,0,__PYX_ERR(0, 1115, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1107, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_FromSize_t(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_stored_size(__pyx_v_self, 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1107, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_FromSize_t(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_stored_size(__pyx_v_self, 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1107, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_idx = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1109
+  /* "cpprb/PyReplayBuffer.pyx":1117
  *         idx = np.arange(self.get_stored_size())
  * 
  *         if shuffle:             # <<<<<<<<<<<<<<
  *             np.random.shuffle(idx)
  * 
  */
-  __Pyx_TraceLine(1109,0,__PYX_ERR(0, 1109, __pyx_L1_error))
+  __Pyx_TraceLine(1117,0,__PYX_ERR(0, 1117, __pyx_L1_error))
   __pyx_t_5 = (__pyx_v_shuffle != 0);
   if (__pyx_t_5) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1110
+    /* "cpprb/PyReplayBuffer.pyx":1118
  * 
  *         if shuffle:
  *             np.random.shuffle(idx)             # <<<<<<<<<<<<<<
  * 
  *         return self._encode_sample(idx)
  */
-    __Pyx_TraceLine(1110,0,__PYX_ERR(0, 1110, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1110, __pyx_L1_error)
+    __Pyx_TraceLine(1118,0,__PYX_ERR(0, 1118, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1118, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1110, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1118, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1110, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1118, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_idx) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_idx);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1110, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1118, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1109
+    /* "cpprb/PyReplayBuffer.pyx":1117
  *         idx = np.arange(self.get_stored_size())
  * 
  *         if shuffle:             # <<<<<<<<<<<<<<
  *             np.random.shuffle(idx)
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1112
+  /* "cpprb/PyReplayBuffer.pyx":1120
  *             np.random.shuffle(idx)
  * 
  *         return self._encode_sample(idx)             # <<<<<<<<<<<<<<
  * 
  *     def _encode_sample(self,idx):
  */
-  __Pyx_TraceLine(1112,0,__PYX_ERR(0, 1112, __pyx_L1_error))
+  __Pyx_TraceLine(1120,0,__PYX_ERR(0, 1120, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_encode_sample); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1112, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_encode_sample); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_idx) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_idx);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1112, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1093
+  /* "cpprb/PyReplayBuffer.pyx":1101
  *         return index
  * 
  *     def get_all_transitions(self,shuffle: bool=False):             # <<<<<<<<<<<<<<
  *         r"""
  *         Get all transitions stored in replay buffer.
  */
 
@@ -21323,15 +21448,15 @@
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1114
+/* "cpprb/PyReplayBuffer.pyx":1122
  *         return self._encode_sample(idx)
  * 
  *     def _encode_sample(self,idx):             # <<<<<<<<<<<<<<
  *         cdef sample = {}
  *         cdef next_idx
  */
 
@@ -21378,637 +21503,637 @@
   size_t __pyx_t_14;
   size_t __pyx_t_15;
   size_t __pyx_t_16;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_encode_sample", 0);
-  __Pyx_TraceCall("_encode_sample", __pyx_f[0], 1114, 0, __PYX_ERR(0, 1114, __pyx_L1_error));
+  __Pyx_TraceCall("_encode_sample", __pyx_f[0], 1122, 0, __PYX_ERR(0, 1122, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_idx);
 
-  /* "cpprb/PyReplayBuffer.pyx":1115
+  /* "cpprb/PyReplayBuffer.pyx":1123
  * 
  *     def _encode_sample(self,idx):
  *         cdef sample = {}             # <<<<<<<<<<<<<<
  *         cdef next_idx
  *         cdef cache_idx
  */
-  __Pyx_TraceLine(1115,0,__PYX_ERR(0, 1115, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1115, __pyx_L1_error)
+  __Pyx_TraceLine(1123,0,__PYX_ERR(0, 1123, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_sample = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1120
+  /* "cpprb/PyReplayBuffer.pyx":1128
  *         cdef bool use_cache
  * 
  *         idx = np.array(idx,copy=False,ndmin=1)             # <<<<<<<<<<<<<<
  *         for name, b in self.buffer.items():
  *             sample[name] = b[idx]
  */
-  __Pyx_TraceLine(1120,0,__PYX_ERR(0, 1120, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1120, __pyx_L1_error)
+  __Pyx_TraceLine(1128,0,__PYX_ERR(0, 1128, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1120, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1120, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_idx);
   __Pyx_GIVEREF(__pyx_v_idx);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_idx);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1120, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1120, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_ndmin, __pyx_int_1) < 0) __PYX_ERR(0, 1120, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1120, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1128, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_ndmin, __pyx_int_1) < 0) __PYX_ERR(0, 1128, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_idx, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1121
+  /* "cpprb/PyReplayBuffer.pyx":1129
  * 
  *         idx = np.array(idx,copy=False,ndmin=1)
  *         for name, b in self.buffer.items():             # <<<<<<<<<<<<<<
  *             sample[name] = b[idx]
  * 
  */
-  __Pyx_TraceLine(1121,0,__PYX_ERR(0, 1121, __pyx_L1_error))
+  __Pyx_TraceLine(1129,0,__PYX_ERR(0, 1129, __pyx_L1_error))
   __pyx_t_5 = 0;
   if (unlikely(__pyx_v_self->buffer == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-    __PYX_ERR(0, 1121, __pyx_L1_error)
+    __PYX_ERR(0, 1129, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_self->buffer, 0, __pyx_n_s_items, (&__pyx_t_6), (&__pyx_t_7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1121, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_self->buffer, 0, __pyx_n_s_items, (&__pyx_t_6), (&__pyx_t_7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __pyx_t_4 = __pyx_t_3;
   __pyx_t_3 = 0;
   while (1) {
     __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_4, __pyx_t_6, &__pyx_t_5, &__pyx_t_3, &__pyx_t_1, NULL, __pyx_t_7);
     if (unlikely(__pyx_t_8 == 0)) break;
-    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 1121, __pyx_L1_error)
+    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 1129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_3);
     __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_b, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1122
+    /* "cpprb/PyReplayBuffer.pyx":1130
  *         idx = np.array(idx,copy=False,ndmin=1)
  *         for name, b in self.buffer.items():
  *             sample[name] = b[idx]             # <<<<<<<<<<<<<<
  * 
  *         if self.has_next_of:
  */
-    __Pyx_TraceLine(1122,0,__PYX_ERR(0, 1122, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_b, __pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1122, __pyx_L1_error)
+    __Pyx_TraceLine(1130,0,__PYX_ERR(0, 1130, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_b, __pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(PyObject_SetItem(__pyx_v_sample, __pyx_v_name, __pyx_t_1) < 0)) __PYX_ERR(0, 1122, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_sample, __pyx_v_name, __pyx_t_1) < 0)) __PYX_ERR(0, 1130, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1124
+  /* "cpprb/PyReplayBuffer.pyx":1132
  *             sample[name] = b[idx]
  * 
  *         if self.has_next_of:             # <<<<<<<<<<<<<<
  *             next_idx = idx + 1
  *             next_idx[next_idx == self.get_buffer_size()] = 0
  */
-  __Pyx_TraceLine(1124,0,__PYX_ERR(0, 1124, __pyx_L1_error))
+  __Pyx_TraceLine(1132,0,__PYX_ERR(0, 1132, __pyx_L1_error))
   __pyx_t_9 = (__pyx_v_self->has_next_of != 0);
   if (__pyx_t_9) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1125
+    /* "cpprb/PyReplayBuffer.pyx":1133
  * 
  *         if self.has_next_of:
  *             next_idx = idx + 1             # <<<<<<<<<<<<<<
  *             next_idx[next_idx == self.get_buffer_size()] = 0
  *             cache_idx = (next_idx == self.get_next_index())
  */
-    __Pyx_TraceLine(1125,0,__PYX_ERR(0, 1125, __pyx_L1_error))
-    __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_v_idx, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1125, __pyx_L1_error)
+    __Pyx_TraceLine(1133,0,__PYX_ERR(0, 1133, __pyx_L1_error))
+    __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_v_idx, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_v_next_idx = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1126
+    /* "cpprb/PyReplayBuffer.pyx":1134
  *         if self.has_next_of:
  *             next_idx = idx + 1
  *             next_idx[next_idx == self.get_buffer_size()] = 0             # <<<<<<<<<<<<<<
  *             cache_idx = (next_idx == self.get_next_index())
  *             use_cache = cache_idx.any()
  */
-    __Pyx_TraceLine(1126,0,__PYX_ERR(0, 1126, __pyx_L1_error))
-    __pyx_t_4 = __Pyx_PyInt_FromSize_t(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_buffer_size(__pyx_v_self, 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1126, __pyx_L1_error)
+    __Pyx_TraceLine(1134,0,__PYX_ERR(0, 1134, __pyx_L1_error))
+    __pyx_t_4 = __Pyx_PyInt_FromSize_t(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_buffer_size(__pyx_v_self, 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyObject_RichCompare(__pyx_v_next_idx, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1126, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_v_next_idx, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1134, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(PyObject_SetItem(__pyx_v_next_idx, __pyx_t_1, __pyx_int_0) < 0)) __PYX_ERR(0, 1126, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_next_idx, __pyx_t_1, __pyx_int_0) < 0)) __PYX_ERR(0, 1134, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1127
+    /* "cpprb/PyReplayBuffer.pyx":1135
  *             next_idx = idx + 1
  *             next_idx[next_idx == self.get_buffer_size()] = 0
  *             cache_idx = (next_idx == self.get_next_index())             # <<<<<<<<<<<<<<
  *             use_cache = cache_idx.any()
  * 
  */
-    __Pyx_TraceLine(1127,0,__PYX_ERR(0, 1127, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_PyInt_FromSize_t(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_next_index(__pyx_v_self, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1127, __pyx_L1_error)
+    __Pyx_TraceLine(1135,0,__PYX_ERR(0, 1135, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_PyInt_FromSize_t(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_next_index(__pyx_v_self, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1135, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyObject_RichCompare(__pyx_v_next_idx, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1127, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_v_next_idx, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1135, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_cache_idx = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1128
+    /* "cpprb/PyReplayBuffer.pyx":1136
  *             next_idx[next_idx == self.get_buffer_size()] = 0
  *             cache_idx = (next_idx == self.get_next_index())
  *             use_cache = cache_idx.any()             # <<<<<<<<<<<<<<
  * 
  *             for name in self.next_of:
  */
-    __Pyx_TraceLine(1128,0,__PYX_ERR(0, 1128, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cache_idx, __pyx_n_s_any); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1128, __pyx_L1_error)
+    __Pyx_TraceLine(1136,0,__PYX_ERR(0, 1136, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cache_idx, __pyx_n_s_any); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1136, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1128, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1136, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_10 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1128, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_10 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1136, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_use_cache = __pyx_t_10;
 
-    /* "cpprb/PyReplayBuffer.pyx":1130
+    /* "cpprb/PyReplayBuffer.pyx":1138
  *             use_cache = cache_idx.any()
  * 
  *             for name in self.next_of:             # <<<<<<<<<<<<<<
  *                 sample[f"next_{name}"] = self.buffer[name][next_idx]
  *                 if use_cache:
  */
-    __Pyx_TraceLine(1130,0,__PYX_ERR(0, 1130, __pyx_L1_error))
+    __Pyx_TraceLine(1138,0,__PYX_ERR(0, 1138, __pyx_L1_error))
     if (likely(PyList_CheckExact(__pyx_v_self->next_of)) || PyTuple_CheckExact(__pyx_v_self->next_of)) {
       __pyx_t_4 = __pyx_v_self->next_of; __Pyx_INCREF(__pyx_t_4); __pyx_t_6 = 0;
       __pyx_t_11 = NULL;
     } else {
-      __pyx_t_6 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_self->next_of); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1130, __pyx_L1_error)
+      __pyx_t_6 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_self->next_of); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1138, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_11 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1130, __pyx_L1_error)
+      __pyx_t_11 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1138, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_11)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_1 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1130, __pyx_L1_error)
+          __pyx_t_1 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1138, __pyx_L1_error)
           #else
-          __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1130, __pyx_L1_error)
+          __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1138, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           #endif
         } else {
           if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1130, __pyx_L1_error)
+          __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1138, __pyx_L1_error)
           #else
-          __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1130, __pyx_L1_error)
+          __pyx_t_1 = PySequence_ITEM(__pyx_t_4, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1138, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           #endif
         }
       } else {
         __pyx_t_1 = __pyx_t_11(__pyx_t_4);
         if (unlikely(!__pyx_t_1)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 1130, __pyx_L1_error)
+            else __PYX_ERR(0, 1138, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_1);
       }
       __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":1131
+      /* "cpprb/PyReplayBuffer.pyx":1139
  * 
  *             for name in self.next_of:
  *                 sample[f"next_{name}"] = self.buffer[name][next_idx]             # <<<<<<<<<<<<<<
  *                 if use_cache:
  *                     # Cache for the latest "next_***" stored at `self.next_`
  */
-      __Pyx_TraceLine(1131,0,__PYX_ERR(0, 1131, __pyx_L1_error))
-      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->buffer, __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1131, __pyx_L1_error)
+      __Pyx_TraceLine(1139,0,__PYX_ERR(0, 1139, __pyx_L1_error))
+      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->buffer, __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_next_idx); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1131, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_next_idx); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1131, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_n_u_next, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1131, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_n_u_next, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(PyObject_SetItem(__pyx_v_sample, __pyx_t_2, __pyx_t_3) < 0)) __PYX_ERR(0, 1131, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(__pyx_v_sample, __pyx_t_2, __pyx_t_3) < 0)) __PYX_ERR(0, 1139, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":1132
+      /* "cpprb/PyReplayBuffer.pyx":1140
  *             for name in self.next_of:
  *                 sample[f"next_{name}"] = self.buffer[name][next_idx]
  *                 if use_cache:             # <<<<<<<<<<<<<<
  *                     # Cache for the latest "next_***" stored at `self.next_`
  *                     sample[f"next_{name}"][cache_idx] = self.next_[name]
  */
-      __Pyx_TraceLine(1132,0,__PYX_ERR(0, 1132, __pyx_L1_error))
+      __Pyx_TraceLine(1140,0,__PYX_ERR(0, 1140, __pyx_L1_error))
       __pyx_t_9 = (__pyx_v_use_cache != 0);
       if (__pyx_t_9) {
 
-        /* "cpprb/PyReplayBuffer.pyx":1134
+        /* "cpprb/PyReplayBuffer.pyx":1142
  *                 if use_cache:
  *                     # Cache for the latest "next_***" stored at `self.next_`
  *                     sample[f"next_{name}"][cache_idx] = self.next_[name]             # <<<<<<<<<<<<<<
  * 
  *         cdef size_t i,_i
  */
-        __Pyx_TraceLine(1134,0,__PYX_ERR(0, 1134, __pyx_L1_error))
-        __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_self->next_, __pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1134, __pyx_L1_error)
+        __Pyx_TraceLine(1142,0,__PYX_ERR(0, 1142, __pyx_L1_error))
+        __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_self->next_, __pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1142, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1134, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1142, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_n_u_next, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1134, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_n_u_next, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1142, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_sample, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1134, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_sample, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1142, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (unlikely(PyObject_SetItem(__pyx_t_2, __pyx_v_cache_idx, __pyx_t_3) < 0)) __PYX_ERR(0, 1134, __pyx_L1_error)
+        if (unlikely(PyObject_SetItem(__pyx_t_2, __pyx_v_cache_idx, __pyx_t_3) < 0)) __PYX_ERR(0, 1142, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "cpprb/PyReplayBuffer.pyx":1132
+        /* "cpprb/PyReplayBuffer.pyx":1140
  *             for name in self.next_of:
  *                 sample[f"next_{name}"] = self.buffer[name][next_idx]
  *                 if use_cache:             # <<<<<<<<<<<<<<
  *                     # Cache for the latest "next_***" stored at `self.next_`
  *                     sample[f"next_{name}"][cache_idx] = self.next_[name]
  */
       }
 
-      /* "cpprb/PyReplayBuffer.pyx":1130
+      /* "cpprb/PyReplayBuffer.pyx":1138
  *             use_cache = cache_idx.any()
  * 
  *             for name in self.next_of:             # <<<<<<<<<<<<<<
  *                 sample[f"next_{name}"] = self.buffer[name][next_idx]
  *                 if use_cache:
  */
-      __Pyx_TraceLine(1130,0,__PYX_ERR(0, 1130, __pyx_L1_error))
+      __Pyx_TraceLine(1138,0,__PYX_ERR(0, 1138, __pyx_L1_error))
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1124
+    /* "cpprb/PyReplayBuffer.pyx":1132
  *             sample[name] = b[idx]
  * 
  *         if self.has_next_of:             # <<<<<<<<<<<<<<
  *             next_idx = idx + 1
  *             next_idx[next_idx == self.get_buffer_size()] = 0
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1137
+  /* "cpprb/PyReplayBuffer.pyx":1145
  * 
  *         cdef size_t i,_i
  *         cdef size_t N = idx.shape[0]             # <<<<<<<<<<<<<<
  *         if self.cache is not None:
  *             # Cache for episode ends stored at `self.cache`
  */
-  __Pyx_TraceLine(1137,0,__PYX_ERR(0, 1137, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_idx, __pyx_n_s_shape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1137, __pyx_L1_error)
+  __Pyx_TraceLine(1145,0,__PYX_ERR(0, 1145, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_idx, __pyx_n_s_shape); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_4, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1137, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_4, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_t_3); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1137, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_t_3); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1145, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_N = __pyx_t_12;
 
-  /* "cpprb/PyReplayBuffer.pyx":1138
+  /* "cpprb/PyReplayBuffer.pyx":1146
  *         cdef size_t i,_i
  *         cdef size_t N = idx.shape[0]
  *         if self.cache is not None:             # <<<<<<<<<<<<<<
  *             # Cache for episode ends stored at `self.cache`
  *             for _i in range(N):
  */
-  __Pyx_TraceLine(1138,0,__PYX_ERR(0, 1138, __pyx_L1_error))
+  __Pyx_TraceLine(1146,0,__PYX_ERR(0, 1146, __pyx_L1_error))
   __pyx_t_9 = (__pyx_v_self->cache != Py_None);
   __pyx_t_13 = (__pyx_t_9 != 0);
   if (__pyx_t_13) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1140
+    /* "cpprb/PyReplayBuffer.pyx":1148
  *         if self.cache is not None:
  *             # Cache for episode ends stored at `self.cache`
  *             for _i in range(N):             # <<<<<<<<<<<<<<
  *                 i = idx[_i]
  *                 if i in self.cache:
  */
-    __Pyx_TraceLine(1140,0,__PYX_ERR(0, 1140, __pyx_L1_error))
+    __Pyx_TraceLine(1148,0,__PYX_ERR(0, 1148, __pyx_L1_error))
     __pyx_t_12 = __pyx_v_N;
     __pyx_t_14 = __pyx_t_12;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v__i = __pyx_t_15;
 
-      /* "cpprb/PyReplayBuffer.pyx":1141
+      /* "cpprb/PyReplayBuffer.pyx":1149
  *             # Cache for episode ends stored at `self.cache`
  *             for _i in range(N):
  *                 i = idx[_i]             # <<<<<<<<<<<<<<
  *                 if i in self.cache:
  *                     if self.has_next_of:
  */
-      __Pyx_TraceLine(1141,0,__PYX_ERR(0, 1141, __pyx_L1_error))
-      __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_idx, __pyx_v__i, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1141, __pyx_L1_error)
+      __Pyx_TraceLine(1149,0,__PYX_ERR(0, 1149, __pyx_L1_error))
+      __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_idx, __pyx_v__i, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1149, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_16 = __Pyx_PyInt_As_size_t(__pyx_t_3); if (unlikely((__pyx_t_16 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1141, __pyx_L1_error)
+      __pyx_t_16 = __Pyx_PyInt_As_size_t(__pyx_t_3); if (unlikely((__pyx_t_16 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1149, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_v_i = __pyx_t_16;
 
-      /* "cpprb/PyReplayBuffer.pyx":1142
+      /* "cpprb/PyReplayBuffer.pyx":1150
  *             for _i in range(N):
  *                 i = idx[_i]
  *                 if i in self.cache:             # <<<<<<<<<<<<<<
  *                     if self.has_next_of:
  *                         for name in self.next_of:
  */
-      __Pyx_TraceLine(1142,0,__PYX_ERR(0, 1142, __pyx_L1_error))
-      __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1142, __pyx_L1_error)
+      __Pyx_TraceLine(1150,0,__PYX_ERR(0, 1150, __pyx_L1_error))
+      __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1150, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_13 = (__Pyx_PySequence_ContainsTF(__pyx_t_3, __pyx_v_self->cache, Py_EQ)); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 1142, __pyx_L1_error)
+      __pyx_t_13 = (__Pyx_PySequence_ContainsTF(__pyx_t_3, __pyx_v_self->cache, Py_EQ)); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 1150, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_9 = (__pyx_t_13 != 0);
       if (__pyx_t_9) {
 
-        /* "cpprb/PyReplayBuffer.pyx":1143
+        /* "cpprb/PyReplayBuffer.pyx":1151
  *                 i = idx[_i]
  *                 if i in self.cache:
  *                     if self.has_next_of:             # <<<<<<<<<<<<<<
  *                         for name in self.next_of:
  *                             sample[f"next_{name}"][_i] = self.cache[i][f"next_{name}"]
  */
-        __Pyx_TraceLine(1143,0,__PYX_ERR(0, 1143, __pyx_L1_error))
+        __Pyx_TraceLine(1151,0,__PYX_ERR(0, 1151, __pyx_L1_error))
         __pyx_t_9 = (__pyx_v_self->has_next_of != 0);
         if (__pyx_t_9) {
 
-          /* "cpprb/PyReplayBuffer.pyx":1144
+          /* "cpprb/PyReplayBuffer.pyx":1152
  *                 if i in self.cache:
  *                     if self.has_next_of:
  *                         for name in self.next_of:             # <<<<<<<<<<<<<<
  *                             sample[f"next_{name}"][_i] = self.cache[i][f"next_{name}"]
  *                     if self.compress_any:
  */
-          __Pyx_TraceLine(1144,0,__PYX_ERR(0, 1144, __pyx_L1_error))
+          __Pyx_TraceLine(1152,0,__PYX_ERR(0, 1152, __pyx_L1_error))
           if (likely(PyList_CheckExact(__pyx_v_self->next_of)) || PyTuple_CheckExact(__pyx_v_self->next_of)) {
             __pyx_t_3 = __pyx_v_self->next_of; __Pyx_INCREF(__pyx_t_3); __pyx_t_6 = 0;
             __pyx_t_11 = NULL;
           } else {
-            __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_self->next_of); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1144, __pyx_L1_error)
+            __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_self->next_of); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1152, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_3);
-            __pyx_t_11 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1144, __pyx_L1_error)
+            __pyx_t_11 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1152, __pyx_L1_error)
           }
           for (;;) {
             if (likely(!__pyx_t_11)) {
               if (likely(PyList_CheckExact(__pyx_t_3))) {
                 if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_3)) break;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                __pyx_t_4 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1144, __pyx_L1_error)
+                __pyx_t_4 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1152, __pyx_L1_error)
                 #else
-                __pyx_t_4 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1144, __pyx_L1_error)
+                __pyx_t_4 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1152, __pyx_L1_error)
                 __Pyx_GOTREF(__pyx_t_4);
                 #endif
               } else {
                 if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1144, __pyx_L1_error)
+                __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1152, __pyx_L1_error)
                 #else
-                __pyx_t_4 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1144, __pyx_L1_error)
+                __pyx_t_4 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1152, __pyx_L1_error)
                 __Pyx_GOTREF(__pyx_t_4);
                 #endif
               }
             } else {
               __pyx_t_4 = __pyx_t_11(__pyx_t_3);
               if (unlikely(!__pyx_t_4)) {
                 PyObject* exc_type = PyErr_Occurred();
                 if (exc_type) {
                   if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                  else __PYX_ERR(0, 1144, __pyx_L1_error)
+                  else __PYX_ERR(0, 1152, __pyx_L1_error)
                 }
                 break;
               }
               __Pyx_GOTREF(__pyx_t_4);
             }
             __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_4);
             __pyx_t_4 = 0;
 
-            /* "cpprb/PyReplayBuffer.pyx":1145
+            /* "cpprb/PyReplayBuffer.pyx":1153
  *                     if self.has_next_of:
  *                         for name in self.next_of:
  *                             sample[f"next_{name}"][_i] = self.cache[i][f"next_{name}"]             # <<<<<<<<<<<<<<
  *                     if self.compress_any:
  *                         for name in self.stack_compress:
  */
-            __Pyx_TraceLine(1145,0,__PYX_ERR(0, 1145, __pyx_L1_error))
-            __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_self->cache, __pyx_v_i, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1145, __pyx_L1_error)
+            __Pyx_TraceLine(1153,0,__PYX_ERR(0, 1153, __pyx_L1_error))
+            __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_self->cache, __pyx_v_i, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1153, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_4);
-            __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1145, __pyx_L1_error)
+            __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1153, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_n_u_next, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1145, __pyx_L1_error)
+            __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_n_u_next, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1153, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-            __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1145, __pyx_L1_error)
+            __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1153, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-            __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1145, __pyx_L1_error)
+            __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1153, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
-            __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_n_u_next, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1145, __pyx_L1_error)
+            __pyx_t_4 = __Pyx_PyUnicode_Concat(__pyx_n_u_next, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1153, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_4);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-            __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_sample, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1145, __pyx_L1_error)
+            __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_sample, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1153, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-            if (unlikely(__Pyx_SetItemInt(__pyx_t_1, __pyx_v__i, __pyx_t_2, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1) < 0)) __PYX_ERR(0, 1145, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_t_1, __pyx_v__i, __pyx_t_2, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1) < 0)) __PYX_ERR(0, 1153, __pyx_L1_error)
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-            /* "cpprb/PyReplayBuffer.pyx":1144
+            /* "cpprb/PyReplayBuffer.pyx":1152
  *                 if i in self.cache:
  *                     if self.has_next_of:
  *                         for name in self.next_of:             # <<<<<<<<<<<<<<
  *                             sample[f"next_{name}"][_i] = self.cache[i][f"next_{name}"]
  *                     if self.compress_any:
  */
-            __Pyx_TraceLine(1144,0,__PYX_ERR(0, 1144, __pyx_L1_error))
+            __Pyx_TraceLine(1152,0,__PYX_ERR(0, 1152, __pyx_L1_error))
           }
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          /* "cpprb/PyReplayBuffer.pyx":1143
+          /* "cpprb/PyReplayBuffer.pyx":1151
  *                 i = idx[_i]
  *                 if i in self.cache:
  *                     if self.has_next_of:             # <<<<<<<<<<<<<<
  *                         for name in self.next_of:
  *                             sample[f"next_{name}"][_i] = self.cache[i][f"next_{name}"]
  */
         }
 
-        /* "cpprb/PyReplayBuffer.pyx":1146
+        /* "cpprb/PyReplayBuffer.pyx":1154
  *                         for name in self.next_of:
  *                             sample[f"next_{name}"][_i] = self.cache[i][f"next_{name}"]
  *                     if self.compress_any:             # <<<<<<<<<<<<<<
  *                         for name in self.stack_compress:
  *                             sample[name][_i] = self.cache[i][name]
  */
-        __Pyx_TraceLine(1146,0,__PYX_ERR(0, 1146, __pyx_L1_error))
+        __Pyx_TraceLine(1154,0,__PYX_ERR(0, 1154, __pyx_L1_error))
         __pyx_t_9 = (__pyx_v_self->compress_any != 0);
         if (__pyx_t_9) {
 
-          /* "cpprb/PyReplayBuffer.pyx":1147
+          /* "cpprb/PyReplayBuffer.pyx":1155
  *                             sample[f"next_{name}"][_i] = self.cache[i][f"next_{name}"]
  *                     if self.compress_any:
  *                         for name in self.stack_compress:             # <<<<<<<<<<<<<<
  *                             sample[name][_i] = self.cache[i][name]
  * 
  */
-          __Pyx_TraceLine(1147,0,__PYX_ERR(0, 1147, __pyx_L1_error))
+          __Pyx_TraceLine(1155,0,__PYX_ERR(0, 1155, __pyx_L1_error))
           if (likely(PyList_CheckExact(__pyx_v_self->stack_compress)) || PyTuple_CheckExact(__pyx_v_self->stack_compress)) {
             __pyx_t_3 = __pyx_v_self->stack_compress; __Pyx_INCREF(__pyx_t_3); __pyx_t_6 = 0;
             __pyx_t_11 = NULL;
           } else {
-            __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_self->stack_compress); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1147, __pyx_L1_error)
+            __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_self->stack_compress); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1155, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_3);
-            __pyx_t_11 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1147, __pyx_L1_error)
+            __pyx_t_11 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1155, __pyx_L1_error)
           }
           for (;;) {
             if (likely(!__pyx_t_11)) {
               if (likely(PyList_CheckExact(__pyx_t_3))) {
                 if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_3)) break;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1147, __pyx_L1_error)
+                __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1155, __pyx_L1_error)
                 #else
-                __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1147, __pyx_L1_error)
+                __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1155, __pyx_L1_error)
                 __Pyx_GOTREF(__pyx_t_2);
                 #endif
               } else {
                 if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1147, __pyx_L1_error)
+                __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 1155, __pyx_L1_error)
                 #else
-                __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1147, __pyx_L1_error)
+                __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1155, __pyx_L1_error)
                 __Pyx_GOTREF(__pyx_t_2);
                 #endif
               }
             } else {
               __pyx_t_2 = __pyx_t_11(__pyx_t_3);
               if (unlikely(!__pyx_t_2)) {
                 PyObject* exc_type = PyErr_Occurred();
                 if (exc_type) {
                   if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                  else __PYX_ERR(0, 1147, __pyx_L1_error)
+                  else __PYX_ERR(0, 1155, __pyx_L1_error)
                 }
                 break;
               }
               __Pyx_GOTREF(__pyx_t_2);
             }
             __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_2);
             __pyx_t_2 = 0;
 
-            /* "cpprb/PyReplayBuffer.pyx":1148
+            /* "cpprb/PyReplayBuffer.pyx":1156
  *                     if self.compress_any:
  *                         for name in self.stack_compress:
  *                             sample[name][_i] = self.cache[i][name]             # <<<<<<<<<<<<<<
  * 
  *         return sample
  */
-            __Pyx_TraceLine(1148,0,__PYX_ERR(0, 1148, __pyx_L1_error))
-            __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_self->cache, __pyx_v_i, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1148, __pyx_L1_error)
+            __Pyx_TraceLine(1156,0,__PYX_ERR(0, 1156, __pyx_L1_error))
+            __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_self->cache, __pyx_v_i, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1156, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1148, __pyx_L1_error)
+            __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1156, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-            __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_sample, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1148, __pyx_L1_error)
+            __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_sample, __pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1156, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
-            if (unlikely(__Pyx_SetItemInt(__pyx_t_2, __pyx_v__i, __pyx_t_1, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1) < 0)) __PYX_ERR(0, 1148, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_t_2, __pyx_v__i, __pyx_t_1, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1) < 0)) __PYX_ERR(0, 1156, __pyx_L1_error)
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-            /* "cpprb/PyReplayBuffer.pyx":1147
+            /* "cpprb/PyReplayBuffer.pyx":1155
  *                             sample[f"next_{name}"][_i] = self.cache[i][f"next_{name}"]
  *                     if self.compress_any:
  *                         for name in self.stack_compress:             # <<<<<<<<<<<<<<
  *                             sample[name][_i] = self.cache[i][name]
  * 
  */
-            __Pyx_TraceLine(1147,0,__PYX_ERR(0, 1147, __pyx_L1_error))
+            __Pyx_TraceLine(1155,0,__PYX_ERR(0, 1155, __pyx_L1_error))
           }
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          /* "cpprb/PyReplayBuffer.pyx":1146
+          /* "cpprb/PyReplayBuffer.pyx":1154
  *                         for name in self.next_of:
  *                             sample[f"next_{name}"][_i] = self.cache[i][f"next_{name}"]
  *                     if self.compress_any:             # <<<<<<<<<<<<<<
  *                         for name in self.stack_compress:
  *                             sample[name][_i] = self.cache[i][name]
  */
         }
 
-        /* "cpprb/PyReplayBuffer.pyx":1142
+        /* "cpprb/PyReplayBuffer.pyx":1150
  *             for _i in range(N):
  *                 i = idx[_i]
  *                 if i in self.cache:             # <<<<<<<<<<<<<<
  *                     if self.has_next_of:
  *                         for name in self.next_of:
  */
       }
     }
 
-    /* "cpprb/PyReplayBuffer.pyx":1138
+    /* "cpprb/PyReplayBuffer.pyx":1146
  *         cdef size_t i,_i
  *         cdef size_t N = idx.shape[0]
  *         if self.cache is not None:             # <<<<<<<<<<<<<<
  *             # Cache for episode ends stored at `self.cache`
  *             for _i in range(N):
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1150
+  /* "cpprb/PyReplayBuffer.pyx":1158
  *                             sample[name][_i] = self.cache[i][name]
  * 
  *         return sample             # <<<<<<<<<<<<<<
  * 
  *     def sample(self,batch_size):
  */
-  __Pyx_TraceLine(1150,0,__PYX_ERR(0, 1150, __pyx_L1_error))
+  __Pyx_TraceLine(1158,0,__PYX_ERR(0, 1158, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_sample);
   __pyx_r = __pyx_v_sample;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1114
+  /* "cpprb/PyReplayBuffer.pyx":1122
  *         return self._encode_sample(idx)
  * 
  *     def _encode_sample(self,idx):             # <<<<<<<<<<<<<<
  *         cdef sample = {}
  *         cdef next_idx
  */
 
@@ -22029,15 +22154,15 @@
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1152
+/* "cpprb/PyReplayBuffer.pyx":1160
  *         return sample
  * 
  *     def sample(self,batch_size):             # <<<<<<<<<<<<<<
  *         r"""Sample the stored transitions randomly with speciped size
  * 
  */
 
@@ -22066,33 +22191,33 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sample", 0);
-  __Pyx_TraceCall("sample", __pyx_f[0], 1152, 0, __PYX_ERR(0, 1152, __pyx_L1_error));
+  __Pyx_TraceCall("sample", __pyx_f[0], 1160, 0, __PYX_ERR(0, 1160, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1166
+  /* "cpprb/PyReplayBuffer.pyx":1174
  *             the same transition multiple times.
  *         """
  *         cdef idx = np.random.randint(0,self.get_stored_size(),batch_size)             # <<<<<<<<<<<<<<
  *         return self._encode_sample(idx)
  * 
  */
-  __Pyx_TraceLine(1166,0,__PYX_ERR(0, 1166, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __Pyx_TraceLine(1174,0,__PYX_ERR(0, 1174, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_randint); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_randint); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_FromSize_t(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_stored_size(__pyx_v_self, 0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_FromSize_t(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_stored_size(__pyx_v_self, 0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -22101,83 +22226,83 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_int_0, __pyx_t_3, __pyx_v_batch_size};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1166, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1174, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_int_0, __pyx_t_3, __pyx_v_batch_size};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1166, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1174, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1166, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1174, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_int_0);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_t_3);
     __Pyx_INCREF(__pyx_v_batch_size);
     __Pyx_GIVEREF(__pyx_v_batch_size);
     PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_5, __pyx_v_batch_size);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1166, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1174, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_idx = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1167
+  /* "cpprb/PyReplayBuffer.pyx":1175
  *         """
  *         cdef idx = np.random.randint(0,self.get_stored_size(),batch_size)
  *         return self._encode_sample(idx)             # <<<<<<<<<<<<<<
  * 
  *     cpdef void clear(self) except *:
  */
-  __Pyx_TraceLine(1167,0,__PYX_ERR(0, 1167, __pyx_L1_error))
+  __Pyx_TraceLine(1175,0,__PYX_ERR(0, 1175, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_encode_sample); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1167, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_encode_sample); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_v_idx) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_idx);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1167, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1152
+  /* "cpprb/PyReplayBuffer.pyx":1160
  *         return sample
  * 
  *     def sample(self,batch_size):             # <<<<<<<<<<<<<<
  *         r"""Sample the stored transitions randomly with speciped size
  * 
  */
 
@@ -22194,15 +22319,15 @@
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1169
+/* "cpprb/PyReplayBuffer.pyx":1177
  *         return self._encode_sample(idx)
  * 
  *     cpdef void clear(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Clear replay buffer.
  * 
  */
 
@@ -22216,25 +22341,25 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear", 0);
-  __Pyx_TraceCall("clear", __pyx_f[0], 1169, 0, __PYX_ERR(0, 1169, __pyx_L1_error));
+  __Pyx_TraceCall("clear", __pyx_f[0], 1177, 0, __PYX_ERR(0, 1177, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1169, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_12ReplayBuffer_13clear)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -22242,15 +22367,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1169, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1177, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
@@ -22262,97 +22387,97 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1188
+  /* "cpprb/PyReplayBuffer.pyx":1196
  *         0
  *         """
  *         self.index.clear()             # <<<<<<<<<<<<<<
  *         self.episode_len = 0
  * 
  */
-  __Pyx_TraceLine(1188,0,__PYX_ERR(0, 1188, __pyx_L1_error))
+  __Pyx_TraceLine(1196,0,__PYX_ERR(0, 1196, __pyx_L1_error))
   ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_RingBufferIndex *)__pyx_v_self->index->__pyx_vtab)->clear(__pyx_v_self->index);
 
-  /* "cpprb/PyReplayBuffer.pyx":1189
+  /* "cpprb/PyReplayBuffer.pyx":1197
  *         """
  *         self.index.clear()
  *         self.episode_len = 0             # <<<<<<<<<<<<<<
  * 
  *         self.cache = {} if (self.has_next_of or self.compress_any) else None
  */
-  __Pyx_TraceLine(1189,0,__PYX_ERR(0, 1189, __pyx_L1_error))
+  __Pyx_TraceLine(1197,0,__PYX_ERR(0, 1197, __pyx_L1_error))
   __pyx_v_self->episode_len = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1191
+  /* "cpprb/PyReplayBuffer.pyx":1199
  *         self.episode_len = 0
  * 
  *         self.cache = {} if (self.has_next_of or self.compress_any) else None             # <<<<<<<<<<<<<<
  * 
  *         if self.use_nstep:
  */
-  __Pyx_TraceLine(1191,0,__PYX_ERR(0, 1191, __pyx_L1_error))
+  __Pyx_TraceLine(1199,0,__PYX_ERR(0, 1199, __pyx_L1_error))
   __pyx_t_6 = (__pyx_v_self->has_next_of != 0);
   if (!__pyx_t_6) {
   } else {
     __pyx_t_5 = __pyx_t_6;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_6 = (__pyx_v_self->compress_any != 0);
   __pyx_t_5 = __pyx_t_6;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_5) {
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1191, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
   } else {
     __Pyx_INCREF(Py_None);
     __pyx_t_1 = Py_None;
   }
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->cache);
   __Pyx_DECREF(__pyx_v_self->cache);
   __pyx_v_self->cache = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1193
+  /* "cpprb/PyReplayBuffer.pyx":1201
  *         self.cache = {} if (self.has_next_of or self.compress_any) else None
  * 
  *         if self.use_nstep:             # <<<<<<<<<<<<<<
  *             self.nstep.clear()
  * 
  */
-  __Pyx_TraceLine(1193,0,__PYX_ERR(0, 1193, __pyx_L1_error))
+  __Pyx_TraceLine(1201,0,__PYX_ERR(0, 1201, __pyx_L1_error))
   __pyx_t_5 = (__pyx_v_self->use_nstep != 0);
   if (__pyx_t_5) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1194
+    /* "cpprb/PyReplayBuffer.pyx":1202
  * 
  *         if self.use_nstep:
  *             self.nstep.clear()             # <<<<<<<<<<<<<<
  * 
  *     cpdef size_t get_stored_size(self):
  */
-    __Pyx_TraceLine(1194,0,__PYX_ERR(0, 1194, __pyx_L1_error))
+    __Pyx_TraceLine(1202,0,__PYX_ERR(0, 1202, __pyx_L1_error))
     ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_NstepBuffer *)__pyx_v_self->nstep->__pyx_vtab)->clear(__pyx_v_self->nstep, 0);
 
-    /* "cpprb/PyReplayBuffer.pyx":1193
+    /* "cpprb/PyReplayBuffer.pyx":1201
  *         self.cache = {} if (self.has_next_of or self.compress_any) else None
  * 
  *         if self.use_nstep:             # <<<<<<<<<<<<<<
  *             self.nstep.clear()
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1169
+  /* "cpprb/PyReplayBuffer.pyx":1177
  *         return self._encode_sample(idx)
  * 
  *     cpdef void clear(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Clear replay buffer.
  * 
  */
 
@@ -22388,18 +22513,18 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear", 0);
-  __Pyx_TraceCall("clear (wrapper)", __pyx_f[0], 1169, 0, __PYX_ERR(0, 1169, __pyx_L1_error));
+  __Pyx_TraceCall("clear (wrapper)", __pyx_f[0], 1177, 0, __PYX_ERR(0, 1177, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_clear(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1169, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1169, __pyx_L1_error)
+  __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_clear(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1177, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -22409,15 +22534,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1196
+/* "cpprb/PyReplayBuffer.pyx":1204
  *             self.nstep.clear()
  * 
  *     cpdef size_t get_stored_size(self):             # <<<<<<<<<<<<<<
  *         r"""Get stored size
  * 
  */
 
@@ -22431,25 +22556,25 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   size_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_stored_size", 0);
-  __Pyx_TraceCall("get_stored_size", __pyx_f[0], 1196, 0, __PYX_ERR(0, 1196, __pyx_L1_error));
+  __Pyx_TraceCall("get_stored_size", __pyx_f[0], 1204, 0, __PYX_ERR(0, 1204, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_stored_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1196, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_stored_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1204, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_12ReplayBuffer_15get_stored_size)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -22457,18 +22582,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1196, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1204, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1196, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1204, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -22479,26 +22604,26 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1204
+  /* "cpprb/PyReplayBuffer.pyx":1212
  *             stored size
  *         """
  *         return self.index.get_stored_size()             # <<<<<<<<<<<<<<
  * 
  *     cpdef size_t get_buffer_size(self):
  */
-  __Pyx_TraceLine(1204,0,__PYX_ERR(0, 1204, __pyx_L1_error))
+  __Pyx_TraceLine(1212,0,__PYX_ERR(0, 1212, __pyx_L1_error))
   __pyx_r = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_RingBufferIndex *)__pyx_v_self->index->__pyx_vtab)->get_stored_size(__pyx_v_self->index);
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1196
+  /* "cpprb/PyReplayBuffer.pyx":1204
  *             self.nstep.clear()
  * 
  *     cpdef size_t get_stored_size(self):             # <<<<<<<<<<<<<<
  *         r"""Get stored size
  * 
  */
 
@@ -22535,17 +22660,17 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_stored_size", 0);
-  __Pyx_TraceCall("get_stored_size (wrapper)", __pyx_f[0], 1196, 0, __PYX_ERR(0, 1196, __pyx_L1_error));
+  __Pyx_TraceCall("get_stored_size (wrapper)", __pyx_f[0], 1204, 0, __PYX_ERR(0, 1204, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_stored_size(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1196, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_stored_size(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -22555,15 +22680,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1206
+/* "cpprb/PyReplayBuffer.pyx":1214
  *         return self.index.get_stored_size()
  * 
  *     cpdef size_t get_buffer_size(self):             # <<<<<<<<<<<<<<
  *         r"""Get buffer size
  * 
  */
 
@@ -22577,25 +22702,25 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   size_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_buffer_size", 0);
-  __Pyx_TraceCall("get_buffer_size", __pyx_f[0], 1206, 0, __PYX_ERR(0, 1206, __pyx_L1_error));
+  __Pyx_TraceCall("get_buffer_size", __pyx_f[0], 1214, 0, __PYX_ERR(0, 1214, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_buffer_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1206, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_buffer_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1214, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_12ReplayBuffer_17get_buffer_size)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -22603,18 +22728,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1206, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1214, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1206, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1214, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -22625,26 +22750,26 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1214
+  /* "cpprb/PyReplayBuffer.pyx":1222
  *             buffer size
  *         """
  *         return self.buffer_size             # <<<<<<<<<<<<<<
  * 
  *     cpdef size_t get_next_index(self):
  */
-  __Pyx_TraceLine(1214,0,__PYX_ERR(0, 1214, __pyx_L1_error))
+  __Pyx_TraceLine(1222,0,__PYX_ERR(0, 1222, __pyx_L1_error))
   __pyx_r = __pyx_v_self->buffer_size;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1206
+  /* "cpprb/PyReplayBuffer.pyx":1214
  *         return self.index.get_stored_size()
  * 
  *     cpdef size_t get_buffer_size(self):             # <<<<<<<<<<<<<<
  *         r"""Get buffer size
  * 
  */
 
@@ -22681,17 +22806,17 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_buffer_size", 0);
-  __Pyx_TraceCall("get_buffer_size (wrapper)", __pyx_f[0], 1206, 0, __PYX_ERR(0, 1206, __pyx_L1_error));
+  __Pyx_TraceCall("get_buffer_size (wrapper)", __pyx_f[0], 1214, 0, __PYX_ERR(0, 1214, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_buffer_size(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1206, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_buffer_size(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -22701,15 +22826,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1216
+/* "cpprb/PyReplayBuffer.pyx":1224
  *         return self.buffer_size
  * 
  *     cpdef size_t get_next_index(self):             # <<<<<<<<<<<<<<
  *         r"""Get the next index to store
  * 
  */
 
@@ -22723,25 +22848,25 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   size_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_next_index", 0);
-  __Pyx_TraceCall("get_next_index", __pyx_f[0], 1216, 0, __PYX_ERR(0, 1216, __pyx_L1_error));
+  __Pyx_TraceCall("get_next_index", __pyx_f[0], 1224, 0, __PYX_ERR(0, 1224, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_next_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1216, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_next_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1224, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_12ReplayBuffer_19get_next_index)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -22749,18 +22874,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1216, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1224, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1216, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1224, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -22771,26 +22896,26 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1224
+  /* "cpprb/PyReplayBuffer.pyx":1232
  *             the next index to store
  *         """
  *         return self.index.get_next_index()             # <<<<<<<<<<<<<<
  * 
  *     cdef void add_cache(self):
  */
-  __Pyx_TraceLine(1224,0,__PYX_ERR(0, 1224, __pyx_L1_error))
+  __Pyx_TraceLine(1232,0,__PYX_ERR(0, 1232, __pyx_L1_error))
   __pyx_r = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_RingBufferIndex *)__pyx_v_self->index->__pyx_vtab)->get_next_index(__pyx_v_self->index);
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1216
+  /* "cpprb/PyReplayBuffer.pyx":1224
  *         return self.buffer_size
  * 
  *     cpdef size_t get_next_index(self):             # <<<<<<<<<<<<<<
  *         r"""Get the next index to store
  * 
  */
 
@@ -22827,17 +22952,17 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_next_index", 0);
-  __Pyx_TraceCall("get_next_index (wrapper)", __pyx_f[0], 1216, 0, __PYX_ERR(0, 1216, __pyx_L1_error));
+  __Pyx_TraceCall("get_next_index (wrapper)", __pyx_f[0], 1224, 0, __PYX_ERR(0, 1224, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_next_index(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1216, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_next_index(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -22847,574 +22972,655 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1226
+/* "cpprb/PyReplayBuffer.pyx":1234
  *         return self.index.get_next_index()
  * 
  *     cdef void add_cache(self):             # <<<<<<<<<<<<<<
  *         r"""Add last items into cache
  * 
  */
 
 static void __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_add_cache(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *__pyx_v_self) {
   size_t __pyx_v_key_end;
   size_t __pyx_v_key_min;
   size_t __pyx_v_max_cache;
   size_t __pyx_v_key;
-  size_t __pyx_v_next_key;
-  PyObject *__pyx_v_cache_key = NULL;
-  PyObject *__pyx_v_name = NULL;
-  PyObject *__pyx_v_value = NULL;
+  CYTHON_UNUSED size_t __pyx_v_next_key;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   size_t __pyx_t_3;
   size_t __pyx_t_4;
   size_t __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  Py_ssize_t __pyx_t_7;
-  Py_ssize_t __pyx_t_8;
-  int __pyx_t_9;
-  PyObject *__pyx_t_10 = NULL;
-  PyObject *__pyx_t_11 = NULL;
-  int __pyx_t_12;
-  PyObject *__pyx_t_13 = NULL;
-  PyObject *(*__pyx_t_14)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_cache", 0);
-  __Pyx_TraceCall("add_cache", __pyx_f[0], 1226, 0, __PYX_ERR(0, 1226, __pyx_L1_error));
+  __Pyx_TraceCall("add_cache", __pyx_f[0], 1234, 0, __PYX_ERR(0, 1234, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1237
+  /* "cpprb/PyReplayBuffer.pyx":1245
  * 
  *         # If no cache configuration, do nothing
  *         if self.cache is None:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
-  __Pyx_TraceLine(1237,0,__PYX_ERR(0, 1237, __pyx_L1_error))
+  __Pyx_TraceLine(1245,0,__PYX_ERR(0, 1245, __pyx_L1_error))
   __pyx_t_1 = (__pyx_v_self->cache == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1238
+    /* "cpprb/PyReplayBuffer.pyx":1246
  *         # If no cache configuration, do nothing
  *         if self.cache is None:
  *             return             # <<<<<<<<<<<<<<
  * 
  *         # If nothing are stored, do nothing
  */
-    __Pyx_TraceLine(1238,0,__PYX_ERR(0, 1238, __pyx_L1_error))
+    __Pyx_TraceLine(1246,0,__PYX_ERR(0, 1246, __pyx_L1_error))
     goto __pyx_L0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1237
+    /* "cpprb/PyReplayBuffer.pyx":1245
  * 
  *         # If no cache configuration, do nothing
  *         if self.cache is None:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1241
+  /* "cpprb/PyReplayBuffer.pyx":1249
  * 
  *         # If nothing are stored, do nothing
  *         if self.get_stored_size() == 0:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
-  __Pyx_TraceLine(1241,0,__PYX_ERR(0, 1241, __pyx_L1_error))
+  __Pyx_TraceLine(1249,0,__PYX_ERR(0, 1249, __pyx_L1_error))
   __pyx_t_2 = ((((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_stored_size(__pyx_v_self, 0) == 0) != 0);
   if (__pyx_t_2) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1242
+    /* "cpprb/PyReplayBuffer.pyx":1250
  *         # If nothing are stored, do nothing
  *         if self.get_stored_size() == 0:
  *             return             # <<<<<<<<<<<<<<
  * 
  *         cdef size_t key_end = (self.get_next_index() or self.buffer_size)
  */
-    __Pyx_TraceLine(1242,0,__PYX_ERR(0, 1242, __pyx_L1_error))
+    __Pyx_TraceLine(1250,0,__PYX_ERR(0, 1250, __pyx_L1_error))
     goto __pyx_L0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1241
+    /* "cpprb/PyReplayBuffer.pyx":1249
  * 
  *         # If nothing are stored, do nothing
  *         if self.get_stored_size() == 0:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1244
+  /* "cpprb/PyReplayBuffer.pyx":1252
  *             return
  * 
  *         cdef size_t key_end = (self.get_next_index() or self.buffer_size)             # <<<<<<<<<<<<<<
  *         # Next index (without wraparounding): key_end in [1,...,self.buffer_size]
  * 
  */
-  __Pyx_TraceLine(1244,0,__PYX_ERR(0, 1244, __pyx_L1_error))
+  __Pyx_TraceLine(1252,0,__PYX_ERR(0, 1252, __pyx_L1_error))
   __pyx_t_4 = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_next_index(__pyx_v_self, 0);
   if (!__pyx_t_4) {
   } else {
     __pyx_t_3 = __pyx_t_4;
     goto __pyx_L5_bool_binop_done;
   }
   __pyx_t_3 = __pyx_v_self->buffer_size;
   __pyx_L5_bool_binop_done:;
   __pyx_v_key_end = __pyx_t_3;
 
-  /* "cpprb/PyReplayBuffer.pyx":1247
+  /* "cpprb/PyReplayBuffer.pyx":1255
  *         # Next index (without wraparounding): key_end in [1,...,self.buffer_size]
  * 
  *         cdef size_t key_min = 0             # <<<<<<<<<<<<<<
  *         cdef size_t max_cache = min(self.cache_size,self.episode_len)
  *         if key_end > max_cache:
  */
-  __Pyx_TraceLine(1247,0,__PYX_ERR(0, 1247, __pyx_L1_error))
+  __Pyx_TraceLine(1255,0,__PYX_ERR(0, 1255, __pyx_L1_error))
   __pyx_v_key_min = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1248
+  /* "cpprb/PyReplayBuffer.pyx":1256
  * 
  *         cdef size_t key_min = 0
  *         cdef size_t max_cache = min(self.cache_size,self.episode_len)             # <<<<<<<<<<<<<<
  *         if key_end > max_cache:
  *             key_min = key_end - max_cache
  */
-  __Pyx_TraceLine(1248,0,__PYX_ERR(0, 1248, __pyx_L1_error))
+  __Pyx_TraceLine(1256,0,__PYX_ERR(0, 1256, __pyx_L1_error))
   __pyx_t_3 = __pyx_v_self->episode_len;
   __pyx_t_4 = __pyx_v_self->cache_size;
   if (((__pyx_t_3 < __pyx_t_4) != 0)) {
     __pyx_t_5 = __pyx_t_3;
   } else {
     __pyx_t_5 = __pyx_t_4;
   }
   __pyx_v_max_cache = __pyx_t_5;
 
-  /* "cpprb/PyReplayBuffer.pyx":1249
+  /* "cpprb/PyReplayBuffer.pyx":1257
  *         cdef size_t key_min = 0
  *         cdef size_t max_cache = min(self.cache_size,self.episode_len)
  *         if key_end > max_cache:             # <<<<<<<<<<<<<<
  *             key_min = key_end - max_cache
  * 
  */
-  __Pyx_TraceLine(1249,0,__PYX_ERR(0, 1249, __pyx_L1_error))
+  __Pyx_TraceLine(1257,0,__PYX_ERR(0, 1257, __pyx_L1_error))
   __pyx_t_2 = ((__pyx_v_key_end > __pyx_v_max_cache) != 0);
   if (__pyx_t_2) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1250
+    /* "cpprb/PyReplayBuffer.pyx":1258
  *         cdef size_t max_cache = min(self.cache_size,self.episode_len)
  *         if key_end > max_cache:
  *             key_min = key_end - max_cache             # <<<<<<<<<<<<<<
  * 
  *         cdef size_t key = 0
  */
-    __Pyx_TraceLine(1250,0,__PYX_ERR(0, 1250, __pyx_L1_error))
+    __Pyx_TraceLine(1258,0,__PYX_ERR(0, 1258, __pyx_L1_error))
     __pyx_v_key_min = (__pyx_v_key_end - __pyx_v_max_cache);
 
-    /* "cpprb/PyReplayBuffer.pyx":1249
+    /* "cpprb/PyReplayBuffer.pyx":1257
  *         cdef size_t key_min = 0
  *         cdef size_t max_cache = min(self.cache_size,self.episode_len)
  *         if key_end > max_cache:             # <<<<<<<<<<<<<<
  *             key_min = key_end - max_cache
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1252
+  /* "cpprb/PyReplayBuffer.pyx":1260
  *             key_min = key_end - max_cache
  * 
  *         cdef size_t key = 0             # <<<<<<<<<<<<<<
  *         cdef size_t next_key = 0
  *         for key in range(key_min, key_end): # key_end is excluded
  */
-  __Pyx_TraceLine(1252,0,__PYX_ERR(0, 1252, __pyx_L1_error))
+  __Pyx_TraceLine(1260,0,__PYX_ERR(0, 1260, __pyx_L1_error))
   __pyx_v_key = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1253
+  /* "cpprb/PyReplayBuffer.pyx":1261
  * 
  *         cdef size_t key = 0
  *         cdef size_t next_key = 0             # <<<<<<<<<<<<<<
  *         for key in range(key_min, key_end): # key_end is excluded
- *             next_key = key + 1
+ *             self.add_cache_i(key, key_end)
  */
-  __Pyx_TraceLine(1253,0,__PYX_ERR(0, 1253, __pyx_L1_error))
+  __Pyx_TraceLine(1261,0,__PYX_ERR(0, 1261, __pyx_L1_error))
   __pyx_v_next_key = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1254
+  /* "cpprb/PyReplayBuffer.pyx":1262
  *         cdef size_t key = 0
  *         cdef size_t next_key = 0
  *         for key in range(key_min, key_end): # key_end is excluded             # <<<<<<<<<<<<<<
- *             next_key = key + 1
- *             cache_key = {}
+ *             self.add_cache_i(key, key_end)
+ * 
  */
-  __Pyx_TraceLine(1254,0,__PYX_ERR(0, 1254, __pyx_L1_error))
+  __Pyx_TraceLine(1262,0,__PYX_ERR(0, 1262, __pyx_L1_error))
   __pyx_t_5 = __pyx_v_key_end;
   __pyx_t_3 = __pyx_t_5;
   for (__pyx_t_4 = __pyx_v_key_min; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_key = __pyx_t_4;
 
-    /* "cpprb/PyReplayBuffer.pyx":1255
+    /* "cpprb/PyReplayBuffer.pyx":1263
  *         cdef size_t next_key = 0
  *         for key in range(key_min, key_end): # key_end is excluded
- *             next_key = key + 1             # <<<<<<<<<<<<<<
- *             cache_key = {}
+ *             self.add_cache_i(key, key_end)             # <<<<<<<<<<<<<<
  * 
+ *     cdef void add_cache_i(self, size_t key, size_t key_end):
  */
-    __Pyx_TraceLine(1255,0,__PYX_ERR(0, 1255, __pyx_L1_error))
-    __pyx_v_next_key = (__pyx_v_key + 1);
+    __Pyx_TraceLine(1263,0,__PYX_ERR(0, 1263, __pyx_L1_error))
+    ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self->__pyx_vtab)->add_cache_i(__pyx_v_self, __pyx_v_key, __pyx_v_key_end);
+  }
 
-    /* "cpprb/PyReplayBuffer.pyx":1256
- *         for key in range(key_min, key_end): # key_end is excluded
- *             next_key = key + 1
- *             cache_key = {}             # <<<<<<<<<<<<<<
+  /* "cpprb/PyReplayBuffer.pyx":1234
+ *         return self.index.get_next_index()
+ * 
+ *     cdef void add_cache(self):             # <<<<<<<<<<<<<<
+ *         r"""Add last items into cache
  * 
- *             if self.has_next_of:
  */
-    __Pyx_TraceLine(1256,0,__PYX_ERR(0, 1256, __pyx_L1_error))
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1256, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_XDECREF_SET(__pyx_v_cache_key, ((PyObject*)__pyx_t_6));
-    __pyx_t_6 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1258
- *             cache_key = {}
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("cpprb.PyReplayBuffer.ReplayBuffer.add_cache", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
+  __Pyx_RefNannyFinishContext();
+}
+
+/* "cpprb/PyReplayBuffer.pyx":1265
+ *             self.add_cache_i(key, key_end)
  * 
- *             if self.has_next_of:             # <<<<<<<<<<<<<<
- *                 if next_key == key_end:
- *                     for name, value in self.next_.items():
+ *     cdef void add_cache_i(self, size_t key, size_t key_end):             # <<<<<<<<<<<<<<
+ *         # If key is already cached, don't do anything
+ *         if key in self.cache:
  */
-    __Pyx_TraceLine(1258,0,__PYX_ERR(0, 1258, __pyx_L1_error))
-    __pyx_t_2 = (__pyx_v_self->has_next_of != 0);
-    if (__pyx_t_2) {
 
-      /* "cpprb/PyReplayBuffer.pyx":1259
+static void __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_add_cache_i(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *__pyx_v_self, size_t __pyx_v_key, size_t __pyx_v_key_end) {
+  size_t __pyx_v_next_key;
+  PyObject *__pyx_v_cache_key = 0;
+  PyObject *__pyx_v_name = NULL;
+  PyObject *__pyx_v_value = NULL;
+  __Pyx_TraceDeclarations
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_t_9;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *(*__pyx_t_11)(PyObject *);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("add_cache_i", 0);
+  __Pyx_TraceCall("add_cache_i", __pyx_f[0], 1265, 0, __PYX_ERR(0, 1265, __pyx_L1_error));
+
+  /* "cpprb/PyReplayBuffer.pyx":1267
+ *     cdef void add_cache_i(self, size_t key, size_t key_end):
+ *         # If key is already cached, don't do anything
+ *         if key in self.cache:             # <<<<<<<<<<<<<<
+ *             return
  * 
- *             if self.has_next_of:
- *                 if next_key == key_end:             # <<<<<<<<<<<<<<
- *                     for name, value in self.next_.items():
- *                         cache_key[f"next_{name}"] = value.copy()
  */
-      __Pyx_TraceLine(1259,0,__PYX_ERR(0, 1259, __pyx_L1_error))
-      __pyx_t_2 = ((__pyx_v_next_key == __pyx_v_key_end) != 0);
-      if (__pyx_t_2) {
+  __Pyx_TraceLine(1267,0,__PYX_ERR(0, 1267, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1267, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_v_self->cache, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1267, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
-        /* "cpprb/PyReplayBuffer.pyx":1260
- *             if self.has_next_of:
- *                 if next_key == key_end:
- *                     for name, value in self.next_.items():             # <<<<<<<<<<<<<<
- *                         cache_key[f"next_{name}"] = value.copy()
- *                 else:
+    /* "cpprb/PyReplayBuffer.pyx":1268
+ *         # If key is already cached, don't do anything
+ *         if key in self.cache:
+ *             return             # <<<<<<<<<<<<<<
+ * 
+ *         cdef size_t next_key = key + 1
  */
-        __Pyx_TraceLine(1260,0,__PYX_ERR(0, 1260, __pyx_L1_error))
-        __pyx_t_7 = 0;
-        if (unlikely(__pyx_v_self->next_ == Py_None)) {
-          PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-          __PYX_ERR(0, 1260, __pyx_L1_error)
-        }
-        __pyx_t_10 = __Pyx_dict_iterator(__pyx_v_self->next_, 0, __pyx_n_s_items, (&__pyx_t_8), (&__pyx_t_9)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1260, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_10);
-        __Pyx_XDECREF(__pyx_t_6);
-        __pyx_t_6 = __pyx_t_10;
-        __pyx_t_10 = 0;
-        while (1) {
-          __pyx_t_12 = __Pyx_dict_iter_next(__pyx_t_6, __pyx_t_8, &__pyx_t_7, &__pyx_t_10, &__pyx_t_11, NULL, __pyx_t_9);
-          if (unlikely(__pyx_t_12 == 0)) break;
-          if (unlikely(__pyx_t_12 == -1)) __PYX_ERR(0, 1260, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_10);
-          __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_10);
-          __pyx_t_10 = 0;
-          __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_11);
-          __pyx_t_11 = 0;
+    __Pyx_TraceLine(1268,0,__PYX_ERR(0, 1268, __pyx_L1_error))
+    goto __pyx_L0;
 
-          /* "cpprb/PyReplayBuffer.pyx":1261
- *                 if next_key == key_end:
- *                     for name, value in self.next_.items():
- *                         cache_key[f"next_{name}"] = value.copy()             # <<<<<<<<<<<<<<
- *                 else:
- *                     for name in self.next_.keys():
+    /* "cpprb/PyReplayBuffer.pyx":1267
+ *     cdef void add_cache_i(self, size_t key, size_t key_end):
+ *         # If key is already cached, don't do anything
+ *         if key in self.cache:             # <<<<<<<<<<<<<<
+ *             return
+ * 
  */
-          __Pyx_TraceLine(1261,0,__PYX_ERR(0, 1261, __pyx_L1_error))
-          __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_copy); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1261, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_13 = NULL;
-          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
-            __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_10);
-            if (likely(__pyx_t_13)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
-              __Pyx_INCREF(__pyx_t_13);
-              __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_10, function);
-            }
-          }
-          __pyx_t_11 = (__pyx_t_13) ? __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_13) : __Pyx_PyObject_CallNoArg(__pyx_t_10);
-          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1261, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          __pyx_t_10 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1261, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_13 = __Pyx_PyUnicode_Concat(__pyx_n_u_next, __pyx_t_10); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1261, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_13);
-          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          if (unlikely(PyDict_SetItem(__pyx_v_cache_key, __pyx_t_13, __pyx_t_11) < 0)) __PYX_ERR(0, 1261, __pyx_L1_error)
-          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        }
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  }
 
-        /* "cpprb/PyReplayBuffer.pyx":1259
+  /* "cpprb/PyReplayBuffer.pyx":1270
+ *             return
+ * 
+ *         cdef size_t next_key = key + 1             # <<<<<<<<<<<<<<
+ *         cdef cache_key = {}
  * 
- *             if self.has_next_of:
- *                 if next_key == key_end:             # <<<<<<<<<<<<<<
- *                     for name, value in self.next_.items():
- *                         cache_key[f"next_{name}"] = value.copy()
  */
-        goto __pyx_L11;
-      }
+  __Pyx_TraceLine(1270,0,__PYX_ERR(0, 1270, __pyx_L1_error))
+  __pyx_v_next_key = (__pyx_v_key + 1);
 
-      /* "cpprb/PyReplayBuffer.pyx":1263
- *                         cache_key[f"next_{name}"] = value.copy()
- *                 else:
- *                     for name in self.next_.keys():             # <<<<<<<<<<<<<<
- *                         cache_key[f"next_{name}"] = self.buffer[name][next_key].copy()
+  /* "cpprb/PyReplayBuffer.pyx":1271
+ * 
+ *         cdef size_t next_key = key + 1
+ *         cdef cache_key = {}             # <<<<<<<<<<<<<<
  * 
+ *         if self.has_next_of:
  */
-      __Pyx_TraceLine(1263,0,__PYX_ERR(0, 1263, __pyx_L1_error))
-      /*else*/ {
-        __pyx_t_8 = 0;
-        if (unlikely(__pyx_v_self->next_ == Py_None)) {
-          PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "keys");
-          __PYX_ERR(0, 1263, __pyx_L1_error)
-        }
-        __pyx_t_11 = __Pyx_dict_iterator(__pyx_v_self->next_, 0, __pyx_n_s_keys, (&__pyx_t_7), (&__pyx_t_9)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1263, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_11);
-        __Pyx_XDECREF(__pyx_t_6);
-        __pyx_t_6 = __pyx_t_11;
-        __pyx_t_11 = 0;
-        while (1) {
-          __pyx_t_12 = __Pyx_dict_iter_next(__pyx_t_6, __pyx_t_7, &__pyx_t_8, &__pyx_t_11, NULL, NULL, __pyx_t_9);
-          if (unlikely(__pyx_t_12 == 0)) break;
-          if (unlikely(__pyx_t_12 == -1)) __PYX_ERR(0, 1263, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_11);
-          __pyx_t_11 = 0;
+  __Pyx_TraceLine(1271,0,__PYX_ERR(0, 1271, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1271, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_cache_key = __pyx_t_1;
+  __pyx_t_1 = 0;
 
-          /* "cpprb/PyReplayBuffer.pyx":1264
- *                 else:
- *                     for name in self.next_.keys():
- *                         cache_key[f"next_{name}"] = self.buffer[name][next_key].copy()             # <<<<<<<<<<<<<<
+  /* "cpprb/PyReplayBuffer.pyx":1273
+ *         cdef cache_key = {}
  * 
- *             if self.compress_any:
+ *         if self.has_next_of:             # <<<<<<<<<<<<<<
+ *             if next_key == key_end:
+ *                 for name, value in self.next_.items():
  */
-          __Pyx_TraceLine(1264,0,__PYX_ERR(0, 1264, __pyx_L1_error))
-          __pyx_t_13 = __Pyx_PyObject_GetItem(__pyx_v_self->buffer, __pyx_v_name); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1264, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_13);
-          __pyx_t_10 = __Pyx_GetItemInt(__pyx_t_13, __pyx_v_next_key, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1264, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_10);
-          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_copy); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1264, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_13);
-          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          __pyx_t_10 = NULL;
-          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
-            __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_13);
-            if (likely(__pyx_t_10)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
-              __Pyx_INCREF(__pyx_t_10);
-              __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_13, function);
-            }
+  __Pyx_TraceLine(1273,0,__PYX_ERR(0, 1273, __pyx_L1_error))
+  __pyx_t_3 = (__pyx_v_self->has_next_of != 0);
+  if (__pyx_t_3) {
+
+    /* "cpprb/PyReplayBuffer.pyx":1274
+ * 
+ *         if self.has_next_of:
+ *             if next_key == key_end:             # <<<<<<<<<<<<<<
+ *                 for name, value in self.next_.items():
+ *                     cache_key[f"next_{name}"] = value.copy()
+ */
+    __Pyx_TraceLine(1274,0,__PYX_ERR(0, 1274, __pyx_L1_error))
+    __pyx_t_3 = ((__pyx_v_next_key == __pyx_v_key_end) != 0);
+    if (__pyx_t_3) {
+
+      /* "cpprb/PyReplayBuffer.pyx":1275
+ *         if self.has_next_of:
+ *             if next_key == key_end:
+ *                 for name, value in self.next_.items():             # <<<<<<<<<<<<<<
+ *                     cache_key[f"next_{name}"] = value.copy()
+ *             else:
+ */
+      __Pyx_TraceLine(1275,0,__PYX_ERR(0, 1275, __pyx_L1_error))
+      __pyx_t_4 = 0;
+      if (unlikely(__pyx_v_self->next_ == Py_None)) {
+        PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
+        __PYX_ERR(0, 1275, __pyx_L1_error)
+      }
+      __pyx_t_7 = __Pyx_dict_iterator(__pyx_v_self->next_, 0, __pyx_n_s_items, (&__pyx_t_5), (&__pyx_t_6)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1275, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_XDECREF(__pyx_t_1);
+      __pyx_t_1 = __pyx_t_7;
+      __pyx_t_7 = 0;
+      while (1) {
+        __pyx_t_9 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_5, &__pyx_t_4, &__pyx_t_7, &__pyx_t_8, NULL, __pyx_t_6);
+        if (unlikely(__pyx_t_9 == 0)) break;
+        if (unlikely(__pyx_t_9 == -1)) __PYX_ERR(0, 1275, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_7);
+        __pyx_t_7 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_8);
+        __pyx_t_8 = 0;
+
+        /* "cpprb/PyReplayBuffer.pyx":1276
+ *             if next_key == key_end:
+ *                 for name, value in self.next_.items():
+ *                     cache_key[f"next_{name}"] = value.copy()             # <<<<<<<<<<<<<<
+ *             else:
+ *                 for name in self.next_.keys():
+ */
+        __Pyx_TraceLine(1276,0,__PYX_ERR(0, 1276, __pyx_L1_error))
+        __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_copy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1276, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        __pyx_t_10 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+          __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_7);
+          if (likely(__pyx_t_10)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+            __Pyx_INCREF(__pyx_t_10);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_7, function);
           }
-          __pyx_t_11 = (__pyx_t_10) ? __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_t_10) : __Pyx_PyObject_CallNoArg(__pyx_t_13);
-          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1264, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-          __pyx_t_13 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1264, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_13);
-          __pyx_t_10 = __Pyx_PyUnicode_Concat(__pyx_n_u_next, __pyx_t_13); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1264, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_10);
-          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-          if (unlikely(PyDict_SetItem(__pyx_v_cache_key, __pyx_t_10, __pyx_t_11) < 0)) __PYX_ERR(0, 1264, __pyx_L1_error)
-          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         }
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __pyx_t_8 = (__pyx_t_10) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_10) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
+        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1276, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1276, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        __pyx_t_10 = __Pyx_PyUnicode_Concat(__pyx_n_u_next, __pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1276, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        if (unlikely(PyObject_SetItem(__pyx_v_cache_key, __pyx_t_10, __pyx_t_8) < 0)) __PYX_ERR(0, 1276, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
-      __pyx_L11:;
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":1258
- *             cache_key = {}
+      /* "cpprb/PyReplayBuffer.pyx":1274
  * 
- *             if self.has_next_of:             # <<<<<<<<<<<<<<
- *                 if next_key == key_end:
- *                     for name, value in self.next_.items():
+ *         if self.has_next_of:
+ *             if next_key == key_end:             # <<<<<<<<<<<<<<
+ *                 for name, value in self.next_.items():
+ *                     cache_key[f"next_{name}"] = value.copy()
  */
+      goto __pyx_L5;
     }
 
-    /* "cpprb/PyReplayBuffer.pyx":1266
- *                         cache_key[f"next_{name}"] = self.buffer[name][next_key].copy()
- * 
- *             if self.compress_any:             # <<<<<<<<<<<<<<
- *                 for name in self.stack_compress:
- *                     cache_key[name] = self.buffer[name][key].copy()
- */
-    __Pyx_TraceLine(1266,0,__PYX_ERR(0, 1266, __pyx_L1_error))
-    __pyx_t_2 = (__pyx_v_self->compress_any != 0);
-    if (__pyx_t_2) {
-
-      /* "cpprb/PyReplayBuffer.pyx":1267
- * 
- *             if self.compress_any:
- *                 for name in self.stack_compress:             # <<<<<<<<<<<<<<
- *                     cache_key[name] = self.buffer[name][key].copy()
+    /* "cpprb/PyReplayBuffer.pyx":1278
+ *                     cache_key[f"next_{name}"] = value.copy()
+ *             else:
+ *                 for name in self.next_.keys():             # <<<<<<<<<<<<<<
+ *                     cache_key[f"next_{name}"] = self.buffer[name][next_key].copy()
  * 
  */
-      __Pyx_TraceLine(1267,0,__PYX_ERR(0, 1267, __pyx_L1_error))
-      if (likely(PyList_CheckExact(__pyx_v_self->stack_compress)) || PyTuple_CheckExact(__pyx_v_self->stack_compress)) {
-        __pyx_t_6 = __pyx_v_self->stack_compress; __Pyx_INCREF(__pyx_t_6); __pyx_t_7 = 0;
-        __pyx_t_14 = NULL;
-      } else {
-        __pyx_t_7 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_self->stack_compress); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1267, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_14 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1267, __pyx_L1_error)
+    __Pyx_TraceLine(1278,0,__PYX_ERR(0, 1278, __pyx_L1_error))
+    /*else*/ {
+      __pyx_t_5 = 0;
+      if (unlikely(__pyx_v_self->next_ == Py_None)) {
+        PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "keys");
+        __PYX_ERR(0, 1278, __pyx_L1_error)
       }
-      for (;;) {
-        if (likely(!__pyx_t_14)) {
-          if (likely(PyList_CheckExact(__pyx_t_6))) {
-            if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_6)) break;
-            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_11 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_11); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 1267, __pyx_L1_error)
-            #else
-            __pyx_t_11 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1267, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_11);
-            #endif
-          } else {
-            if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
-            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_11 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_11); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 1267, __pyx_L1_error)
-            #else
-            __pyx_t_11 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1267, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_11);
-            #endif
-          }
-        } else {
-          __pyx_t_11 = __pyx_t_14(__pyx_t_6);
-          if (unlikely(!__pyx_t_11)) {
-            PyObject* exc_type = PyErr_Occurred();
-            if (exc_type) {
-              if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 1267, __pyx_L1_error)
-            }
-            break;
-          }
-          __Pyx_GOTREF(__pyx_t_11);
-        }
-        __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_11);
-        __pyx_t_11 = 0;
+      __pyx_t_8 = __Pyx_dict_iterator(__pyx_v_self->next_, 0, __pyx_n_s_keys, (&__pyx_t_4), (&__pyx_t_6)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1278, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_XDECREF(__pyx_t_1);
+      __pyx_t_1 = __pyx_t_8;
+      __pyx_t_8 = 0;
+      while (1) {
+        __pyx_t_9 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_4, &__pyx_t_5, &__pyx_t_8, NULL, NULL, __pyx_t_6);
+        if (unlikely(__pyx_t_9 == 0)) break;
+        if (unlikely(__pyx_t_9 == -1)) __PYX_ERR(0, 1278, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_8);
+        __pyx_t_8 = 0;
 
-        /* "cpprb/PyReplayBuffer.pyx":1268
- *             if self.compress_any:
- *                 for name in self.stack_compress:
- *                     cache_key[name] = self.buffer[name][key].copy()             # <<<<<<<<<<<<<<
+        /* "cpprb/PyReplayBuffer.pyx":1279
+ *             else:
+ *                 for name in self.next_.keys():
+ *                     cache_key[f"next_{name}"] = self.buffer[name][next_key].copy()             # <<<<<<<<<<<<<<
  * 
- *             self.cache[key] = cache_key
+ *         if self.compress_any:
  */
-        __Pyx_TraceLine(1268,0,__PYX_ERR(0, 1268, __pyx_L1_error))
-        __pyx_t_10 = __Pyx_PyObject_GetItem(__pyx_v_self->buffer, __pyx_v_name); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1268, __pyx_L1_error)
+        __Pyx_TraceLine(1279,0,__PYX_ERR(0, 1279, __pyx_L1_error))
+        __pyx_t_10 = __Pyx_PyObject_GetItem(__pyx_v_self->buffer, __pyx_v_name); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1279, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
-        __pyx_t_13 = __Pyx_GetItemInt(__pyx_t_10, __pyx_v_key, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1268, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_13);
+        __pyx_t_7 = __Pyx_GetItemInt(__pyx_t_10, __pyx_v_next_key, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1279, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_copy); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1268, __pyx_L1_error)
+        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_copy); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1279, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
-        __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-        __pyx_t_13 = NULL;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __pyx_t_7 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
-          __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_10);
-          if (likely(__pyx_t_13)) {
+          __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_10);
+          if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
-            __Pyx_INCREF(__pyx_t_13);
+            __Pyx_INCREF(__pyx_t_7);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_10, function);
           }
         }
-        __pyx_t_11 = (__pyx_t_13) ? __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_13) : __Pyx_PyObject_CallNoArg(__pyx_t_10);
-        __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1268, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_11);
+        __pyx_t_8 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_10);
+        __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1279, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        if (unlikely(PyDict_SetItem(__pyx_v_cache_key, __pyx_v_name, __pyx_t_11) < 0)) __PYX_ERR(0, 1268, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+        __pyx_t_10 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1279, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_n_u_next, __pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1279, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        if (unlikely(PyObject_SetItem(__pyx_v_cache_key, __pyx_t_7, __pyx_t_8) < 0)) __PYX_ERR(0, 1279, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      }
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    }
+    __pyx_L5:;
 
-        /* "cpprb/PyReplayBuffer.pyx":1267
+    /* "cpprb/PyReplayBuffer.pyx":1273
+ *         cdef cache_key = {}
  * 
- *             if self.compress_any:
- *                 for name in self.stack_compress:             # <<<<<<<<<<<<<<
- *                     cache_key[name] = self.buffer[name][key].copy()
+ *         if self.has_next_of:             # <<<<<<<<<<<<<<
+ *             if next_key == key_end:
+ *                 for name, value in self.next_.items():
+ */
+  }
+
+  /* "cpprb/PyReplayBuffer.pyx":1281
+ *                     cache_key[f"next_{name}"] = self.buffer[name][next_key].copy()
  * 
+ *         if self.compress_any:             # <<<<<<<<<<<<<<
+ *             for name in self.stack_compress:
+ *                 cache_key[name] = self.buffer[name][key].copy()
  */
-        __Pyx_TraceLine(1267,0,__PYX_ERR(0, 1267, __pyx_L1_error))
-      }
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_TraceLine(1281,0,__PYX_ERR(0, 1281, __pyx_L1_error))
+  __pyx_t_3 = (__pyx_v_self->compress_any != 0);
+  if (__pyx_t_3) {
 
-      /* "cpprb/PyReplayBuffer.pyx":1266
- *                         cache_key[f"next_{name}"] = self.buffer[name][next_key].copy()
+    /* "cpprb/PyReplayBuffer.pyx":1282
+ * 
+ *         if self.compress_any:
+ *             for name in self.stack_compress:             # <<<<<<<<<<<<<<
+ *                 cache_key[name] = self.buffer[name][key].copy()
  * 
- *             if self.compress_any:             # <<<<<<<<<<<<<<
- *                 for name in self.stack_compress:
- *                     cache_key[name] = self.buffer[name][key].copy()
  */
+    __Pyx_TraceLine(1282,0,__PYX_ERR(0, 1282, __pyx_L1_error))
+    if (likely(PyList_CheckExact(__pyx_v_self->stack_compress)) || PyTuple_CheckExact(__pyx_v_self->stack_compress)) {
+      __pyx_t_1 = __pyx_v_self->stack_compress; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
+      __pyx_t_11 = NULL;
+    } else {
+      __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_self->stack_compress); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1282, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_11 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 1282, __pyx_L1_error)
     }
+    for (;;) {
+      if (likely(!__pyx_t_11)) {
+        if (likely(PyList_CheckExact(__pyx_t_1))) {
+          if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_1)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_8 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_8); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 1282, __pyx_L1_error)
+          #else
+          __pyx_t_8 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1282, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_8);
+          #endif
+        } else {
+          if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_8); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 1282, __pyx_L1_error)
+          #else
+          __pyx_t_8 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1282, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_8);
+          #endif
+        }
+      } else {
+        __pyx_t_8 = __pyx_t_11(__pyx_t_1);
+        if (unlikely(!__pyx_t_8)) {
+          PyObject* exc_type = PyErr_Occurred();
+          if (exc_type) {
+            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+            else __PYX_ERR(0, 1282, __pyx_L1_error)
+          }
+          break;
+        }
+        __Pyx_GOTREF(__pyx_t_8);
+      }
+      __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_8);
+      __pyx_t_8 = 0;
+
+      /* "cpprb/PyReplayBuffer.pyx":1283
+ *         if self.compress_any:
+ *             for name in self.stack_compress:
+ *                 cache_key[name] = self.buffer[name][key].copy()             # <<<<<<<<<<<<<<
+ * 
+ *         self.cache[key] = cache_key
+ */
+      __Pyx_TraceLine(1283,0,__PYX_ERR(0, 1283, __pyx_L1_error))
+      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_self->buffer, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1283, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_10 = __Pyx_GetItemInt(__pyx_t_7, __pyx_v_key, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1283, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_copy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1283, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __pyx_t_10 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+        __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_7);
+        if (likely(__pyx_t_10)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+          __Pyx_INCREF(__pyx_t_10);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_7, function);
+        }
+      }
+      __pyx_t_8 = (__pyx_t_10) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_10) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
+      __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1283, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(PyObject_SetItem(__pyx_v_cache_key, __pyx_v_name, __pyx_t_8) < 0)) __PYX_ERR(0, 1283, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1270
- *                     cache_key[name] = self.buffer[name][key].copy()
+      /* "cpprb/PyReplayBuffer.pyx":1282
  * 
- *             self.cache[key] = cache_key             # <<<<<<<<<<<<<<
+ *         if self.compress_any:
+ *             for name in self.stack_compress:             # <<<<<<<<<<<<<<
+ *                 cache_key[name] = self.buffer[name][key].copy()
  * 
- *     cpdef void on_episode_end(self) except *:
  */
-    __Pyx_TraceLine(1270,0,__PYX_ERR(0, 1270, __pyx_L1_error))
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_self->cache, __pyx_v_key, __pyx_v_cache_key, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1) < 0)) __PYX_ERR(0, 1270, __pyx_L1_error)
+      __Pyx_TraceLine(1282,0,__PYX_ERR(0, 1282, __pyx_L1_error))
+    }
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "cpprb/PyReplayBuffer.pyx":1281
+ *                     cache_key[f"next_{name}"] = self.buffer[name][next_key].copy()
+ * 
+ *         if self.compress_any:             # <<<<<<<<<<<<<<
+ *             for name in self.stack_compress:
+ *                 cache_key[name] = self.buffer[name][key].copy()
+ */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1226
- *         return self.index.get_next_index()
+  /* "cpprb/PyReplayBuffer.pyx":1285
+ *                 cache_key[name] = self.buffer[name][key].copy()
+ * 
+ *         self.cache[key] = cache_key             # <<<<<<<<<<<<<<
  * 
- *     cdef void add_cache(self):             # <<<<<<<<<<<<<<
- *         r"""Add last items into cache
  * 
  */
+  __Pyx_TraceLine(1285,0,__PYX_ERR(0, 1285, __pyx_L1_error))
+  if (unlikely(__Pyx_SetItemInt(__pyx_v_self->cache, __pyx_v_key, __pyx_v_cache_key, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1) < 0)) __PYX_ERR(0, 1285, __pyx_L1_error)
+
+  /* "cpprb/PyReplayBuffer.pyx":1265
+ *             self.add_cache_i(key, key_end)
+ * 
+ *     cdef void add_cache_i(self, size_t key, size_t key_end):             # <<<<<<<<<<<<<<
+ *         # If key is already cached, don't do anything
+ *         if key in self.cache:
+ */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_XDECREF(__pyx_t_13);
-  __Pyx_WriteUnraisable("cpprb.PyReplayBuffer.ReplayBuffer.add_cache", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_WriteUnraisable("cpprb.PyReplayBuffer.ReplayBuffer.add_cache_i", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_cache_key);
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1272
- *             self.cache[key] = cache_key
+/* "cpprb/PyReplayBuffer.pyx":1289
+ * 
  * 
  *     cpdef void on_episode_end(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Call on episode end
  * 
  */
 
 static PyObject *__pyx_pw_5cpprb_14PyReplayBuffer_12ReplayBuffer_21on_episode_end(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
@@ -23426,25 +23632,25 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_episode_end", 0);
-  __Pyx_TraceCall("on_episode_end", __pyx_f[0], 1272, 0, __PYX_ERR(0, 1272, __pyx_L1_error));
+  __Pyx_TraceCall("on_episode_end", __pyx_f[0], 1289, 0, __PYX_ERR(0, 1289, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_episode_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1272, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_episode_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1289, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_12ReplayBuffer_21on_episode_end)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -23452,15 +23658,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1272, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1289, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
@@ -23472,107 +23678,107 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1285
+  /* "cpprb/PyReplayBuffer.pyx":1302
  *         even though any `done` flags from environment is not set.
  *         """
  *         if self.use_nstep:             # <<<<<<<<<<<<<<
  *             self.use_nstep = False
  *             self.add(**self.nstep.on_episode_end())
  */
-  __Pyx_TraceLine(1285,0,__PYX_ERR(0, 1285, __pyx_L1_error))
+  __Pyx_TraceLine(1302,0,__PYX_ERR(0, 1302, __pyx_L1_error))
   __pyx_t_5 = (__pyx_v_self->use_nstep != 0);
   if (__pyx_t_5) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1286
+    /* "cpprb/PyReplayBuffer.pyx":1303
  *         """
  *         if self.use_nstep:
  *             self.use_nstep = False             # <<<<<<<<<<<<<<
  *             self.add(**self.nstep.on_episode_end())
  *             self.use_nstep = True
  */
-    __Pyx_TraceLine(1286,0,__PYX_ERR(0, 1286, __pyx_L1_error))
+    __Pyx_TraceLine(1303,0,__PYX_ERR(0, 1303, __pyx_L1_error))
     __pyx_v_self->use_nstep = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1287
+    /* "cpprb/PyReplayBuffer.pyx":1304
  *         if self.use_nstep:
  *             self.use_nstep = False
  *             self.add(**self.nstep.on_episode_end())             # <<<<<<<<<<<<<<
  *             self.use_nstep = True
  * 
  */
-    __Pyx_TraceLine(1287,0,__PYX_ERR(0, 1287, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1287, __pyx_L1_error)
+    __Pyx_TraceLine(1304,0,__PYX_ERR(0, 1304, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1304, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_NstepBuffer *)__pyx_v_self->nstep->__pyx_vtab)->on_episode_end(__pyx_v_self->nstep, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1287, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_NstepBuffer *)__pyx_v_self->nstep->__pyx_vtab)->on_episode_end(__pyx_v_self->nstep, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1304, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (unlikely(__pyx_t_3 == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-      __PYX_ERR(0, 1287, __pyx_L1_error)
+      __PYX_ERR(0, 1304, __pyx_L1_error)
     }
     if (likely(PyDict_CheckExact(__pyx_t_3))) {
-      __pyx_t_2 = PyDict_Copy(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1287, __pyx_L1_error)
+      __pyx_t_2 = PyDict_Copy(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1304, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else {
-      __pyx_t_2 = PyObject_CallFunctionObjArgs((PyObject*)&PyDict_Type, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1287, __pyx_L1_error)
+      __pyx_t_2 = PyObject_CallFunctionObjArgs((PyObject*)&PyDict_Type, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1304, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1287, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1304, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1288
+    /* "cpprb/PyReplayBuffer.pyx":1305
  *             self.use_nstep = False
  *             self.add(**self.nstep.on_episode_end())
  *             self.use_nstep = True             # <<<<<<<<<<<<<<
  * 
  *         self.add_cache()
  */
-    __Pyx_TraceLine(1288,0,__PYX_ERR(0, 1288, __pyx_L1_error))
+    __Pyx_TraceLine(1305,0,__PYX_ERR(0, 1305, __pyx_L1_error))
     __pyx_v_self->use_nstep = 1;
 
-    /* "cpprb/PyReplayBuffer.pyx":1285
+    /* "cpprb/PyReplayBuffer.pyx":1302
  *         even though any `done` flags from environment is not set.
  *         """
  *         if self.use_nstep:             # <<<<<<<<<<<<<<
  *             self.use_nstep = False
  *             self.add(**self.nstep.on_episode_end())
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1290
+  /* "cpprb/PyReplayBuffer.pyx":1307
  *             self.use_nstep = True
  * 
  *         self.add_cache()             # <<<<<<<<<<<<<<
  * 
  *         self.episode_len = 0
  */
-  __Pyx_TraceLine(1290,0,__PYX_ERR(0, 1290, __pyx_L1_error))
+  __Pyx_TraceLine(1307,0,__PYX_ERR(0, 1307, __pyx_L1_error))
   ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self->__pyx_vtab)->add_cache(__pyx_v_self);
 
-  /* "cpprb/PyReplayBuffer.pyx":1292
+  /* "cpprb/PyReplayBuffer.pyx":1309
  *         self.add_cache()
  * 
  *         self.episode_len = 0             # <<<<<<<<<<<<<<
  * 
  *     cpdef size_t get_current_episode_len(self):
  */
-  __Pyx_TraceLine(1292,0,__PYX_ERR(0, 1292, __pyx_L1_error))
+  __Pyx_TraceLine(1309,0,__PYX_ERR(0, 1309, __pyx_L1_error))
   __pyx_v_self->episode_len = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1272
- *             self.cache[key] = cache_key
+  /* "cpprb/PyReplayBuffer.pyx":1289
+ * 
  * 
  *     cpdef void on_episode_end(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Call on episode end
  * 
  */
 
   /* function exit code */
@@ -23607,18 +23813,18 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_episode_end", 0);
-  __Pyx_TraceCall("on_episode_end (wrapper)", __pyx_f[0], 1272, 0, __PYX_ERR(0, 1272, __pyx_L1_error));
+  __Pyx_TraceCall("on_episode_end (wrapper)", __pyx_f[0], 1289, 0, __PYX_ERR(0, 1289, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_on_episode_end(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1272, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1272, __pyx_L1_error)
+  __pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_on_episode_end(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1289, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -23628,15 +23834,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1294
+/* "cpprb/PyReplayBuffer.pyx":1311
  *         self.episode_len = 0
  * 
  *     cpdef size_t get_current_episode_len(self):             # <<<<<<<<<<<<<<
  *         r"""Get current episode length
  * 
  */
 
@@ -23650,25 +23856,25 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   size_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_current_episode_len", 0);
-  __Pyx_TraceCall("get_current_episode_len", __pyx_f[0], 1294, 0, __PYX_ERR(0, 1294, __pyx_L1_error));
+  __Pyx_TraceCall("get_current_episode_len", __pyx_f[0], 1311, 0, __PYX_ERR(0, 1311, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_episode_len); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1294, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_episode_len); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1311, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_12ReplayBuffer_23get_current_episode_len)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -23676,18 +23882,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1294, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1311, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1294, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1311, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -23698,26 +23904,26 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1301
+  /* "cpprb/PyReplayBuffer.pyx":1318
  *         episode_len : size_t
  *         """
  *         return self.episode_len             # <<<<<<<<<<<<<<
  * 
  *     cpdef bool is_Nstep(self):
  */
-  __Pyx_TraceLine(1301,0,__PYX_ERR(0, 1301, __pyx_L1_error))
+  __Pyx_TraceLine(1318,0,__PYX_ERR(0, 1318, __pyx_L1_error))
   __pyx_r = __pyx_v_self->episode_len;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1294
+  /* "cpprb/PyReplayBuffer.pyx":1311
  *         self.episode_len = 0
  * 
  *     cpdef size_t get_current_episode_len(self):             # <<<<<<<<<<<<<<
  *         r"""Get current episode length
  * 
  */
 
@@ -23754,17 +23960,17 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_current_episode_len", 0);
-  __Pyx_TraceCall("get_current_episode_len (wrapper)", __pyx_f[0], 1294, 0, __PYX_ERR(0, 1294, __pyx_L1_error));
+  __Pyx_TraceCall("get_current_episode_len (wrapper)", __pyx_f[0], 1311, 0, __PYX_ERR(0, 1311, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_current_episode_len(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1294, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_current_episode_len(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1311, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -23774,15 +23980,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1303
+/* "cpprb/PyReplayBuffer.pyx":1320
  *         return self.episode_len
  * 
  *     cpdef bool is_Nstep(self):             # <<<<<<<<<<<<<<
  *         r"""Get whether use Nstep or not
  * 
  */
 
@@ -23796,25 +24002,25 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   bool __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_Nstep", 0);
-  __Pyx_TraceCall("is_Nstep", __pyx_f[0], 1303, 0, __PYX_ERR(0, 1303, __pyx_L1_error));
+  __Pyx_TraceCall("is_Nstep", __pyx_f[0], 1320, 0, __PYX_ERR(0, 1320, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_is_Nstep); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1303, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_is_Nstep); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1320, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_12ReplayBuffer_25is_Nstep)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -23822,18 +24028,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1303, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1320, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1303, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1320, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -23844,26 +24050,26 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1310
+  /* "cpprb/PyReplayBuffer.pyx":1327
  *         use_nstep : bool
  *         """
  *         return self.use_nstep             # <<<<<<<<<<<<<<
  * 
  * @cython.embedsignature(True)
  */
-  __Pyx_TraceLine(1310,0,__PYX_ERR(0, 1310, __pyx_L1_error))
+  __Pyx_TraceLine(1327,0,__PYX_ERR(0, 1327, __pyx_L1_error))
   __pyx_r = __pyx_v_self->use_nstep;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1303
+  /* "cpprb/PyReplayBuffer.pyx":1320
  *         return self.episode_len
  * 
  *     cpdef bool is_Nstep(self):             # <<<<<<<<<<<<<<
  *         r"""Get whether use Nstep or not
  * 
  */
 
@@ -23900,17 +24106,17 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_Nstep", 0);
-  __Pyx_TraceCall("is_Nstep (wrapper)", __pyx_f[0], 1303, 0, __PYX_ERR(0, 1303, __pyx_L1_error));
+  __Pyx_TraceCall("is_Nstep (wrapper)", __pyx_f[0], 1320, 0, __PYX_ERR(0, 1320, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_is_Nstep(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1303, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_is_Nstep(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1320, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -24043,15 +24249,15 @@
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1328
+/* "cpprb/PyReplayBuffer.pyx":1345
  *     cdef vector[float] ps_vec
  * 
  *     def __cinit__(self,size,env_dict=None,*,alpha=0.6,Nstep=None,eps=1e-4,             # <<<<<<<<<<<<<<
  *                   check_for_update=False,**kwrags):
  *         self.alpha = alpha
  */
 
@@ -24077,15 +24283,15 @@
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_size,&__pyx_n_s_env_dict,&__pyx_n_s_alpha,&__pyx_n_s_Nstep,&__pyx_n_s_eps,&__pyx_n_s_check_for_update,0};
     PyObject* values[6] = {0,0,0,0,0,0};
     values[1] = ((PyObject *)Py_None);
     values[2] = ((PyObject *)__pyx_float_0_6);
     values[3] = ((PyObject *)Py_None);
     values[4] = ((PyObject *)__pyx_float_1eneg_4);
 
-    /* "cpprb/PyReplayBuffer.pyx":1329
+    /* "cpprb/PyReplayBuffer.pyx":1346
  * 
  *     def __cinit__(self,size,env_dict=None,*,alpha=0.6,Nstep=None,eps=1e-4,
  *                   check_for_update=False,**kwrags):             # <<<<<<<<<<<<<<
  *         self.alpha = alpha
  *         self.per = new CppPrioritizedSampler[float](size,alpha)
  */
     values[5] = ((PyObject *)Py_False);
@@ -24116,15 +24322,15 @@
         Py_ssize_t index;
         for (index = 2; index < 6 && kw_args > 0; index++) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwrags, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 1328, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwrags, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 1345, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -24136,24 +24342,24 @@
     __pyx_v_alpha = values[2];
     __pyx_v_Nstep = values[3];
     __pyx_v_eps = values[4];
     __pyx_v_check_for_update = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1328, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1345, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwrags); __pyx_v_kwrags = 0;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.PrioritizedReplayBuffer.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer___cinit__(((struct __pyx_obj_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *)__pyx_v_self), __pyx_v_size, __pyx_v_env_dict, __pyx_v_alpha, __pyx_v_Nstep, __pyx_v_eps, __pyx_v_check_for_update, __pyx_v_kwrags);
 
-  /* "cpprb/PyReplayBuffer.pyx":1328
+  /* "cpprb/PyReplayBuffer.pyx":1345
  *     cdef vector[float] ps_vec
  * 
  *     def __cinit__(self,size,env_dict=None,*,alpha=0.6,Nstep=None,eps=1e-4,             # <<<<<<<<<<<<<<
  *                   check_for_update=False,**kwrags):
  *         self.alpha = alpha
  */
 
@@ -24180,335 +24386,335 @@
   __Pyx_memviewslice __pyx_t_11 = { 0, 0, { 0 }, { 0 }, { 0 } };
   std::vector<size_t>  __pyx_t_12;
   std::vector<float>  __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
-  __Pyx_TraceCall("__cinit__", __pyx_f[0], 1328, 0, __PYX_ERR(0, 1328, __pyx_L1_error));
+  __Pyx_TraceCall("__cinit__", __pyx_f[0], 1345, 0, __PYX_ERR(0, 1345, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1330
+  /* "cpprb/PyReplayBuffer.pyx":1347
  *     def __cinit__(self,size,env_dict=None,*,alpha=0.6,Nstep=None,eps=1e-4,
  *                   check_for_update=False,**kwrags):
  *         self.alpha = alpha             # <<<<<<<<<<<<<<
  *         self.per = new CppPrioritizedSampler[float](size,alpha)
  *         self.per.set_eps(eps)
  */
-  __Pyx_TraceLine(1330,0,__PYX_ERR(0, 1330, __pyx_L1_error))
-  __pyx_t_1 = __pyx_PyFloat_AsFloat(__pyx_v_alpha); if (unlikely((__pyx_t_1 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1330, __pyx_L1_error)
+  __Pyx_TraceLine(1347,0,__PYX_ERR(0, 1347, __pyx_L1_error))
+  __pyx_t_1 = __pyx_PyFloat_AsFloat(__pyx_v_alpha); if (unlikely((__pyx_t_1 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1347, __pyx_L1_error)
   __pyx_v_self->alpha = __pyx_t_1;
 
-  /* "cpprb/PyReplayBuffer.pyx":1331
+  /* "cpprb/PyReplayBuffer.pyx":1348
  *                   check_for_update=False,**kwrags):
  *         self.alpha = alpha
  *         self.per = new CppPrioritizedSampler[float](size,alpha)             # <<<<<<<<<<<<<<
  *         self.per.set_eps(eps)
  *         self.weights = VectorFloat()
  */
-  __Pyx_TraceLine(1331,0,__PYX_ERR(0, 1331, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyInt_As_size_t(__pyx_v_size); if (unlikely((__pyx_t_2 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1331, __pyx_L1_error)
-  __pyx_t_1 = __pyx_PyFloat_AsFloat(__pyx_v_alpha); if (unlikely((__pyx_t_1 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1331, __pyx_L1_error)
+  __Pyx_TraceLine(1348,0,__PYX_ERR(0, 1348, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyInt_As_size_t(__pyx_v_size); if (unlikely((__pyx_t_2 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1348, __pyx_L1_error)
+  __pyx_t_1 = __pyx_PyFloat_AsFloat(__pyx_v_alpha); if (unlikely((__pyx_t_1 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1348, __pyx_L1_error)
   try {
     __pyx_t_3 = new ymd::CppPrioritizedSampler<float> (__pyx_t_2, __pyx_t_1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 1331, __pyx_L1_error)
+    __PYX_ERR(0, 1348, __pyx_L1_error)
   }
   __pyx_v_self->per = __pyx_t_3;
 
-  /* "cpprb/PyReplayBuffer.pyx":1332
+  /* "cpprb/PyReplayBuffer.pyx":1349
  *         self.alpha = alpha
  *         self.per = new CppPrioritizedSampler[float](size,alpha)
  *         self.per.set_eps(eps)             # <<<<<<<<<<<<<<
  *         self.weights = VectorFloat()
  *         self.indexes = VectorSize_t()
  */
-  __Pyx_TraceLine(1332,0,__PYX_ERR(0, 1332, __pyx_L1_error))
-  __pyx_t_1 = __pyx_PyFloat_AsFloat(__pyx_v_eps); if (unlikely((__pyx_t_1 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1332, __pyx_L1_error)
+  __Pyx_TraceLine(1349,0,__PYX_ERR(0, 1349, __pyx_L1_error))
+  __pyx_t_1 = __pyx_PyFloat_AsFloat(__pyx_v_eps); if (unlikely((__pyx_t_1 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1349, __pyx_L1_error)
   __pyx_v_self->per->set_eps(__pyx_t_1);
 
-  /* "cpprb/PyReplayBuffer.pyx":1333
+  /* "cpprb/PyReplayBuffer.pyx":1350
  *         self.per = new CppPrioritizedSampler[float](size,alpha)
  *         self.per.set_eps(eps)
  *         self.weights = VectorFloat()             # <<<<<<<<<<<<<<
  *         self.indexes = VectorSize_t()
  * 
  */
-  __Pyx_TraceLine(1333,0,__PYX_ERR(0, 1333, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_5cpprb_13VectorWrapper_VectorFloat)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1333, __pyx_L1_error)
+  __Pyx_TraceLine(1350,0,__PYX_ERR(0, 1350, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_5cpprb_13VectorWrapper_VectorFloat)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   __Pyx_GOTREF(__pyx_v_self->weights);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->weights));
   __pyx_v_self->weights = ((struct __pyx_obj_5cpprb_13VectorWrapper_VectorFloat *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1334
+  /* "cpprb/PyReplayBuffer.pyx":1351
  *         self.per.set_eps(eps)
  *         self.weights = VectorFloat()
  *         self.indexes = VectorSize_t()             # <<<<<<<<<<<<<<
  * 
  *         if self.use_nstep:
  */
-  __Pyx_TraceLine(1334,0,__PYX_ERR(0, 1334, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_5cpprb_13VectorWrapper_VectorSize_t)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1334, __pyx_L1_error)
+  __Pyx_TraceLine(1351,0,__PYX_ERR(0, 1351, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_5cpprb_13VectorWrapper_VectorSize_t)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1351, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   __Pyx_GOTREF(__pyx_v_self->indexes);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->indexes));
   __pyx_v_self->indexes = ((struct __pyx_obj_5cpprb_13VectorWrapper_VectorSize_t *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1336
+  /* "cpprb/PyReplayBuffer.pyx":1353
  *         self.indexes = VectorSize_t()
  * 
  *         if self.use_nstep:             # <<<<<<<<<<<<<<
  *             self.priorities_nstep = NstepBuffer({"priorities": {"dtype": np.single},
  *                                                  "done": {}},
  */
-  __Pyx_TraceLine(1336,0,__PYX_ERR(0, 1336, __pyx_L1_error))
+  __Pyx_TraceLine(1353,0,__PYX_ERR(0, 1353, __pyx_L1_error))
   __pyx_t_5 = (__pyx_v_self->__pyx_base.use_nstep != 0);
   if (__pyx_t_5) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1337
+    /* "cpprb/PyReplayBuffer.pyx":1354
  * 
  *         if self.use_nstep:
  *             self.priorities_nstep = NstepBuffer({"priorities": {"dtype": np.single},             # <<<<<<<<<<<<<<
  *                                                  "done": {}},
  *                                                 {"size": Nstep["size"]})
  */
-    __Pyx_TraceLine(1337,0,__PYX_ERR(0, 1337, __pyx_L1_error))
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1337, __pyx_L1_error)
+    __Pyx_TraceLine(1354,0,__PYX_ERR(0, 1354, __pyx_L1_error))
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1337, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1337, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_single); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1337, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_single); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 1337, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 1354, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_priorities, __pyx_t_6) < 0) __PYX_ERR(0, 1337, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_priorities, __pyx_t_6) < 0) __PYX_ERR(0, 1354, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1338
+    /* "cpprb/PyReplayBuffer.pyx":1355
  *         if self.use_nstep:
  *             self.priorities_nstep = NstepBuffer({"priorities": {"dtype": np.single},
  *                                                  "done": {}},             # <<<<<<<<<<<<<<
  *                                                 {"size": Nstep["size"]})
  * 
  */
-    __Pyx_TraceLine(1338,0,__PYX_ERR(0, 1338, __pyx_L1_error))
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1338, __pyx_L1_error)
+    __Pyx_TraceLine(1355,0,__PYX_ERR(0, 1355, __pyx_L1_error))
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1355, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_done, __pyx_t_6) < 0) __PYX_ERR(0, 1337, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_done, __pyx_t_6) < 0) __PYX_ERR(0, 1354, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1339
+    /* "cpprb/PyReplayBuffer.pyx":1356
  *             self.priorities_nstep = NstepBuffer({"priorities": {"dtype": np.single},
  *                                                  "done": {}},
  *                                                 {"size": Nstep["size"]})             # <<<<<<<<<<<<<<
  * 
  *         self.check_for_update = check_for_update
  */
-    __Pyx_TraceLine(1339,0,__PYX_ERR(0, 1339, __pyx_L1_error))
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1339, __pyx_L1_error)
+    __Pyx_TraceLine(1356,0,__PYX_ERR(0, 1356, __pyx_L1_error))
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1356, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_Nstep, __pyx_n_u_size); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1339, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_Nstep, __pyx_n_u_size); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1356, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_size, __pyx_t_8) < 0) __PYX_ERR(0, 1339, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_size, __pyx_t_8) < 0) __PYX_ERR(0, 1356, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1337
+    /* "cpprb/PyReplayBuffer.pyx":1354
  * 
  *         if self.use_nstep:
  *             self.priorities_nstep = NstepBuffer({"priorities": {"dtype": np.single},             # <<<<<<<<<<<<<<
  *                                                  "done": {}},
  *                                                 {"size": Nstep["size"]})
  */
-    __Pyx_TraceLine(1337,0,__PYX_ERR(0, 1337, __pyx_L1_error))
-    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1337, __pyx_L1_error)
+    __Pyx_TraceLine(1354,0,__PYX_ERR(0, 1354, __pyx_L1_error))
+    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_6);
     __pyx_t_4 = 0;
     __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_NstepBuffer), __pyx_t_8, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1337, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_NstepBuffer), __pyx_t_8, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GIVEREF(__pyx_t_6);
     __Pyx_GOTREF(__pyx_v_self->priorities_nstep);
     __Pyx_DECREF(((PyObject *)__pyx_v_self->priorities_nstep));
     __pyx_v_self->priorities_nstep = ((struct __pyx_obj_5cpprb_14PyReplayBuffer_NstepBuffer *)__pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1336
+    /* "cpprb/PyReplayBuffer.pyx":1353
  *         self.indexes = VectorSize_t()
  * 
  *         if self.use_nstep:             # <<<<<<<<<<<<<<
  *             self.priorities_nstep = NstepBuffer({"priorities": {"dtype": np.single},
  *                                                  "done": {}},
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1341
+  /* "cpprb/PyReplayBuffer.pyx":1358
  *                                                 {"size": Nstep["size"]})
  * 
  *         self.check_for_update = check_for_update             # <<<<<<<<<<<<<<
  *         if self.check_for_update:
  *             self.unchange_since_sample = np.ones(np.array(size,
  */
-  __Pyx_TraceLine(1341,0,__PYX_ERR(0, 1341, __pyx_L1_error))
-  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_v_check_for_update); if (unlikely((__pyx_t_9 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1341, __pyx_L1_error)
+  __Pyx_TraceLine(1358,0,__PYX_ERR(0, 1358, __pyx_L1_error))
+  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_v_check_for_update); if (unlikely((__pyx_t_9 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1358, __pyx_L1_error)
   __pyx_v_self->check_for_update = __pyx_t_9;
 
-  /* "cpprb/PyReplayBuffer.pyx":1342
+  /* "cpprb/PyReplayBuffer.pyx":1359
  * 
  *         self.check_for_update = check_for_update
  *         if self.check_for_update:             # <<<<<<<<<<<<<<
  *             self.unchange_since_sample = np.ones(np.array(size,
  *                                                           copy=False,
  */
-  __Pyx_TraceLine(1342,0,__PYX_ERR(0, 1342, __pyx_L1_error))
+  __Pyx_TraceLine(1359,0,__PYX_ERR(0, 1359, __pyx_L1_error))
   __pyx_t_5 = (__pyx_v_self->check_for_update != 0);
   if (__pyx_t_5) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1343
+    /* "cpprb/PyReplayBuffer.pyx":1360
  *         self.check_for_update = check_for_update
  *         if self.check_for_update:
  *             self.unchange_since_sample = np.ones(np.array(size,             # <<<<<<<<<<<<<<
  *                                                           copy=False,
  *                                                           dtype='int'),
  */
-    __Pyx_TraceLine(1343,0,__PYX_ERR(0, 1343, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1343, __pyx_L1_error)
+    __Pyx_TraceLine(1360,0,__PYX_ERR(0, 1360, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_ones); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1343, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_ones); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1343, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_array); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1343, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_array); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1343, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_v_size);
     __Pyx_GIVEREF(__pyx_v_size);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_size);
 
-    /* "cpprb/PyReplayBuffer.pyx":1344
+    /* "cpprb/PyReplayBuffer.pyx":1361
  *         if self.check_for_update:
  *             self.unchange_since_sample = np.ones(np.array(size,
  *                                                           copy=False,             # <<<<<<<<<<<<<<
  *                                                           dtype='int'),
  *                                                  dtype='bool')
  */
-    __Pyx_TraceLine(1344,0,__PYX_ERR(0, 1344, __pyx_L1_error))
-    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1344, __pyx_L1_error)
+    __Pyx_TraceLine(1361,0,__PYX_ERR(0, 1361, __pyx_L1_error))
+    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1361, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1344, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_n_u_int) < 0) __PYX_ERR(0, 1344, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1361, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_n_u_int) < 0) __PYX_ERR(0, 1361, __pyx_L1_error)
 
-    /* "cpprb/PyReplayBuffer.pyx":1343
+    /* "cpprb/PyReplayBuffer.pyx":1360
  *         self.check_for_update = check_for_update
  *         if self.check_for_update:
  *             self.unchange_since_sample = np.ones(np.array(size,             # <<<<<<<<<<<<<<
  *                                                           copy=False,
  *                                                           dtype='int'),
  */
-    __Pyx_TraceLine(1343,0,__PYX_ERR(0, 1343, __pyx_L1_error))
-    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1343, __pyx_L1_error)
+    __Pyx_TraceLine(1360,0,__PYX_ERR(0, 1360, __pyx_L1_error))
+    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1343, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_10);
     PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_10);
     __pyx_t_10 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1346
+    /* "cpprb/PyReplayBuffer.pyx":1363
  *                                                           copy=False,
  *                                                           dtype='int'),
  *                                                  dtype='bool')             # <<<<<<<<<<<<<<
  * 
  *         self.idx_vec = vector[size_t]()
  */
-    __Pyx_TraceLine(1346,0,__PYX_ERR(0, 1346, __pyx_L1_error))
-    __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1346, __pyx_L1_error)
+    __Pyx_TraceLine(1363,0,__PYX_ERR(0, 1363, __pyx_L1_error))
+    __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1363, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_dtype, __pyx_n_u_bool) < 0) __PYX_ERR(0, 1346, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_dtype, __pyx_n_u_bool) < 0) __PYX_ERR(0, 1363, __pyx_L1_error)
 
-    /* "cpprb/PyReplayBuffer.pyx":1343
+    /* "cpprb/PyReplayBuffer.pyx":1360
  *         self.check_for_update = check_for_update
  *         if self.check_for_update:
  *             self.unchange_since_sample = np.ones(np.array(size,             # <<<<<<<<<<<<<<
  *                                                           copy=False,
  *                                                           dtype='int'),
  */
-    __Pyx_TraceLine(1343,0,__PYX_ERR(0, 1343, __pyx_L1_error))
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_7, __pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1343, __pyx_L1_error)
+    __Pyx_TraceLine(1360,0,__PYX_ERR(0, 1360, __pyx_L1_error))
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_7, __pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_bool(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 1343, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_bool(__pyx_t_6, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 1360, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __PYX_XDEC_MEMVIEW(&__pyx_v_self->unchange_since_sample, 0);
     __pyx_v_self->unchange_since_sample = __pyx_t_11;
     __pyx_t_11.memview = NULL;
     __pyx_t_11.data = NULL;
 
-    /* "cpprb/PyReplayBuffer.pyx":1342
+    /* "cpprb/PyReplayBuffer.pyx":1359
  * 
  *         self.check_for_update = check_for_update
  *         if self.check_for_update:             # <<<<<<<<<<<<<<
  *             self.unchange_since_sample = np.ones(np.array(size,
  *                                                           copy=False,
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1348
+  /* "cpprb/PyReplayBuffer.pyx":1365
  *                                                  dtype='bool')
  * 
  *         self.idx_vec = vector[size_t]()             # <<<<<<<<<<<<<<
  *         self.ps_vec = vector[float]()
  * 
  */
-  __Pyx_TraceLine(1348,0,__PYX_ERR(0, 1348, __pyx_L1_error))
+  __Pyx_TraceLine(1365,0,__PYX_ERR(0, 1365, __pyx_L1_error))
   try {
     __pyx_t_12 = std::vector<size_t> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 1348, __pyx_L1_error)
+    __PYX_ERR(0, 1365, __pyx_L1_error)
   }
   __pyx_v_self->idx_vec = __pyx_t_12;
 
-  /* "cpprb/PyReplayBuffer.pyx":1349
+  /* "cpprb/PyReplayBuffer.pyx":1366
  * 
  *         self.idx_vec = vector[size_t]()
  *         self.ps_vec = vector[float]()             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self,size,env_dict=None,*,alpha=0.6,Nstep=None,eps=1e-4,
  */
-  __Pyx_TraceLine(1349,0,__PYX_ERR(0, 1349, __pyx_L1_error))
+  __Pyx_TraceLine(1366,0,__PYX_ERR(0, 1366, __pyx_L1_error))
   try {
     __pyx_t_13 = std::vector<float> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 1349, __pyx_L1_error)
+    __PYX_ERR(0, 1366, __pyx_L1_error)
   }
   __pyx_v_self->ps_vec = __pyx_t_13;
 
-  /* "cpprb/PyReplayBuffer.pyx":1328
+  /* "cpprb/PyReplayBuffer.pyx":1345
  *     cdef vector[float] ps_vec
  * 
  *     def __cinit__(self,size,env_dict=None,*,alpha=0.6,Nstep=None,eps=1e-4,             # <<<<<<<<<<<<<<
  *                   check_for_update=False,**kwrags):
  *         self.alpha = alpha
  */
 
@@ -24526,15 +24732,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1351
+/* "cpprb/PyReplayBuffer.pyx":1368
  *         self.ps_vec = vector[float]()
  * 
  *     def __init__(self,size,env_dict=None,*,alpha=0.6,Nstep=None,eps=1e-4,             # <<<<<<<<<<<<<<
  *                  check_for_update=False,**kwargs):
  *         r"""Initialize PrioritizedReplayBuffer
  */
 
@@ -24564,15 +24770,15 @@
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_size,&__pyx_n_s_env_dict,&__pyx_n_s_alpha,&__pyx_n_s_Nstep,&__pyx_n_s_eps,&__pyx_n_s_check_for_update,0};
     PyObject* values[6] = {0,0,0,0,0,0};
     values[1] = ((PyObject *)Py_None);
     values[2] = ((PyObject *)__pyx_float_0_6);
     values[3] = ((PyObject *)Py_None);
     values[4] = ((PyObject *)__pyx_float_1eneg_4);
 
-    /* "cpprb/PyReplayBuffer.pyx":1352
+    /* "cpprb/PyReplayBuffer.pyx":1369
  * 
  *     def __init__(self,size,env_dict=None,*,alpha=0.6,Nstep=None,eps=1e-4,
  *                  check_for_update=False,**kwargs):             # <<<<<<<<<<<<<<
  *         r"""Initialize PrioritizedReplayBuffer
  * 
  */
     values[5] = ((PyObject *)Py_False);
@@ -24603,15 +24809,15 @@
         Py_ssize_t index;
         for (index = 2; index < 6 && kw_args > 0; index++) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1351, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1368, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -24623,24 +24829,24 @@
     __pyx_v_alpha = values[2];
     __pyx_v_Nstep = values[3];
     __pyx_v_eps = values[4];
     __pyx_v_check_for_update = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1351, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1368, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.PrioritizedReplayBuffer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_2__init__(((struct __pyx_obj_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *)__pyx_v_self), __pyx_v_size, __pyx_v_env_dict, __pyx_v_alpha, __pyx_v_Nstep, __pyx_v_eps, __pyx_v_check_for_update, __pyx_v_kwargs);
 
-  /* "cpprb/PyReplayBuffer.pyx":1351
+  /* "cpprb/PyReplayBuffer.pyx":1368
  *         self.ps_vec = vector[float]()
  * 
  *     def __init__(self,size,env_dict=None,*,alpha=0.6,Nstep=None,eps=1e-4,             # <<<<<<<<<<<<<<
  *                  check_for_update=False,**kwargs):
  *         r"""Initialize PrioritizedReplayBuffer
  */
 
@@ -24654,29 +24860,29 @@
   int __pyx_r;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
-  __Pyx_TraceCall("__init__", __pyx_f[0], 1351, 0, __PYX_ERR(0, 1351, __pyx_L1_error));
+  __Pyx_TraceCall("__init__", __pyx_f[0], 1368, 0, __PYX_ERR(0, 1368, __pyx_L1_error));
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.PrioritizedReplayBuffer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1388
+/* "cpprb/PyReplayBuffer.pyx":1405
  *         pass
  * 
  *     def add(self,*,priorities = None,**kwargs):             # <<<<<<<<<<<<<<
  *         r"""Add transition(s) into replay buffer.
  * 
  */
 
@@ -24708,25 +24914,25 @@
       kw_args = PyDict_Size(__pyx_kwds);
       if (kw_args == 1) {
         const Py_ssize_t index = 0;
         PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
         if (value) { values[index] = value; kw_args--; }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, 0, "add") < 0)) __PYX_ERR(0, 1388, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, 0, "add") < 0)) __PYX_ERR(0, 1405, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 0) {
       goto __pyx_L5_argtuple_error;
     } else {
     }
     __pyx_v_priorities = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("add", 1, 0, 0, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1388, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("add", 1, 0, 0, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1405, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.PrioritizedReplayBuffer.add", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_4add(((struct __pyx_obj_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *)__pyx_v_self), __pyx_v_priorities, __pyx_v_kwargs);
@@ -24759,93 +24965,93 @@
   Py_ssize_t __pyx_t_12;
   int __pyx_t_13;
   __Pyx_memviewslice __pyx_t_14 = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add", 0);
-  __Pyx_TraceCall("add", __pyx_f[0], 1388, 0, __PYX_ERR(0, 1388, __pyx_L1_error));
+  __Pyx_TraceCall("add", __pyx_f[0], 1405, 0, __PYX_ERR(0, 1405, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_priorities);
 
-  /* "cpprb/PyReplayBuffer.pyx":1418
+  /* "cpprb/PyReplayBuffer.pyx":1435
  *         It is user responsibility that all the values have the same step-size.
  *         """
  *         cdef size_t N = self.size_check.step_size(kwargs)             # <<<<<<<<<<<<<<
  *         if priorities is not None:
  *             priorities = np.ravel(np.array(priorities,copy=False,
  */
-  __Pyx_TraceLine(1418,0,__PYX_ERR(0, 1418, __pyx_L1_error))
-  __pyx_t_1 = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_StepChecker *)__pyx_v_self->__pyx_base.size_check->__pyx_vtab)->step_size(__pyx_v_self->__pyx_base.size_check, __pyx_v_kwargs); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1418, __pyx_L1_error)
+  __Pyx_TraceLine(1435,0,__PYX_ERR(0, 1435, __pyx_L1_error))
+  __pyx_t_1 = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_StepChecker *)__pyx_v_self->__pyx_base.size_check->__pyx_vtab)->step_size(__pyx_v_self->__pyx_base.size_check, __pyx_v_kwargs); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1435, __pyx_L1_error)
   __pyx_v_N = __pyx_t_1;
 
-  /* "cpprb/PyReplayBuffer.pyx":1419
+  /* "cpprb/PyReplayBuffer.pyx":1436
  *         """
  *         cdef size_t N = self.size_check.step_size(kwargs)
  *         if priorities is not None:             # <<<<<<<<<<<<<<
  *             priorities = np.ravel(np.array(priorities,copy=False,
  *                                            ndmin=1,dtype=np.single))
  */
-  __Pyx_TraceLine(1419,0,__PYX_ERR(0, 1419, __pyx_L1_error))
+  __Pyx_TraceLine(1436,0,__PYX_ERR(0, 1436, __pyx_L1_error))
   __pyx_t_2 = (__pyx_v_priorities != Py_None);
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1420
+    /* "cpprb/PyReplayBuffer.pyx":1437
  *         cdef size_t N = self.size_check.step_size(kwargs)
  *         if priorities is not None:
  *             priorities = np.ravel(np.array(priorities,copy=False,             # <<<<<<<<<<<<<<
  *                                            ndmin=1,dtype=np.single))
  *             if N != priorities.shape[0]:
  */
-    __Pyx_TraceLine(1420,0,__PYX_ERR(0, 1420, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1420, __pyx_L1_error)
+    __Pyx_TraceLine(1437,0,__PYX_ERR(0, 1437, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ravel); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1420, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ravel); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1420, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1420, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1420, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_v_priorities);
     __Pyx_GIVEREF(__pyx_v_priorities);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_priorities);
-    __pyx_t_8 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1420, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1420, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_ndmin, __pyx_int_1) < 0) __PYX_ERR(0, 1420, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1437, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_ndmin, __pyx_int_1) < 0) __PYX_ERR(0, 1437, __pyx_L1_error)
 
-    /* "cpprb/PyReplayBuffer.pyx":1421
+    /* "cpprb/PyReplayBuffer.pyx":1438
  *         if priorities is not None:
  *             priorities = np.ravel(np.array(priorities,copy=False,
  *                                            ndmin=1,dtype=np.single))             # <<<<<<<<<<<<<<
  *             if N != priorities.shape[0]:
  *                 raise ValueError("`priorities` shape is imcompatible")
  */
-    __Pyx_TraceLine(1421,0,__PYX_ERR(0, 1421, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1421, __pyx_L1_error)
+    __Pyx_TraceLine(1438,0,__PYX_ERR(0, 1438, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1438, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_single); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1421, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_single); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1438, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_10) < 0) __PYX_ERR(0, 1420, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_10) < 0) __PYX_ERR(0, 1437, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1420
+    /* "cpprb/PyReplayBuffer.pyx":1437
  *         cdef size_t N = self.size_check.step_size(kwargs)
  *         if priorities is not None:
  *             priorities = np.ravel(np.array(priorities,copy=False,             # <<<<<<<<<<<<<<
  *                                            ndmin=1,dtype=np.single))
  *             if N != priorities.shape[0]:
  */
-    __Pyx_TraceLine(1420,0,__PYX_ERR(0, 1420, __pyx_L1_error))
-    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_5, __pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1420, __pyx_L1_error)
+    __Pyx_TraceLine(1437,0,__PYX_ERR(0, 1437, __pyx_L1_error))
+    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_5, __pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
@@ -24855,426 +25061,426 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_8, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_10);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1420, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF_SET(__pyx_v_priorities, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1422
+    /* "cpprb/PyReplayBuffer.pyx":1439
  *             priorities = np.ravel(np.array(priorities,copy=False,
  *                                            ndmin=1,dtype=np.single))
  *             if N != priorities.shape[0]:             # <<<<<<<<<<<<<<
  *                 raise ValueError("`priorities` shape is imcompatible")
  * 
  */
-    __Pyx_TraceLine(1422,0,__PYX_ERR(0, 1422, __pyx_L1_error))
-    __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1422, __pyx_L1_error)
+    __Pyx_TraceLine(1439,0,__PYX_ERR(0, 1439, __pyx_L1_error))
+    __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1439, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_priorities, __pyx_n_s_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1422, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_priorities, __pyx_n_s_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1439, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_10 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1422, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1439, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PyObject_RichCompare(__pyx_t_4, __pyx_t_10, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1422, __pyx_L1_error)
+    __pyx_t_6 = PyObject_RichCompare(__pyx_t_4, __pyx_t_10, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1439, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 1422, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 1439, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "cpprb/PyReplayBuffer.pyx":1423
+      /* "cpprb/PyReplayBuffer.pyx":1440
  *                                            ndmin=1,dtype=np.single))
  *             if N != priorities.shape[0]:
  *                 raise ValueError("`priorities` shape is imcompatible")             # <<<<<<<<<<<<<<
  * 
  *         if self.use_nstep:
  */
-      __Pyx_TraceLine(1423,0,__PYX_ERR(0, 1423, __pyx_L1_error))
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1423, __pyx_L1_error)
+      __Pyx_TraceLine(1440,0,__PYX_ERR(0, 1440, __pyx_L1_error))
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1440, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 1423, __pyx_L1_error)
+      __PYX_ERR(0, 1440, __pyx_L1_error)
 
-      /* "cpprb/PyReplayBuffer.pyx":1422
+      /* "cpprb/PyReplayBuffer.pyx":1439
  *             priorities = np.ravel(np.array(priorities,copy=False,
  *                                            ndmin=1,dtype=np.single))
  *             if N != priorities.shape[0]:             # <<<<<<<<<<<<<<
  *                 raise ValueError("`priorities` shape is imcompatible")
  * 
  */
     }
 
-    /* "cpprb/PyReplayBuffer.pyx":1419
+    /* "cpprb/PyReplayBuffer.pyx":1436
  *         """
  *         cdef size_t N = self.size_check.step_size(kwargs)
  *         if priorities is not None:             # <<<<<<<<<<<<<<
  *             priorities = np.ravel(np.array(priorities,copy=False,
  *                                            ndmin=1,dtype=np.single))
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1425
+  /* "cpprb/PyReplayBuffer.pyx":1442
  *                 raise ValueError("`priorities` shape is imcompatible")
  * 
  *         if self.use_nstep:             # <<<<<<<<<<<<<<
  *             if priorities is None:
  *                 priorities = np.full((N),self.get_max_priority(),dtype=np.single)
  */
-  __Pyx_TraceLine(1425,0,__PYX_ERR(0, 1425, __pyx_L1_error))
+  __Pyx_TraceLine(1442,0,__PYX_ERR(0, 1442, __pyx_L1_error))
   __pyx_t_3 = (__pyx_v_self->__pyx_base.use_nstep != 0);
   if (__pyx_t_3) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1426
+    /* "cpprb/PyReplayBuffer.pyx":1443
  * 
  *         if self.use_nstep:
  *             if priorities is None:             # <<<<<<<<<<<<<<
  *                 priorities = np.full((N),self.get_max_priority(),dtype=np.single)
  * 
  */
-    __Pyx_TraceLine(1426,0,__PYX_ERR(0, 1426, __pyx_L1_error))
+    __Pyx_TraceLine(1443,0,__PYX_ERR(0, 1443, __pyx_L1_error))
     __pyx_t_3 = (__pyx_v_priorities == Py_None);
     __pyx_t_2 = (__pyx_t_3 != 0);
     if (__pyx_t_2) {
 
-      /* "cpprb/PyReplayBuffer.pyx":1427
+      /* "cpprb/PyReplayBuffer.pyx":1444
  *         if self.use_nstep:
  *             if priorities is None:
  *                 priorities = np.full((N),self.get_max_priority(),dtype=np.single)             # <<<<<<<<<<<<<<
  * 
  *             priorities = self.priorities_nstep.add(priorities=priorities,
  */
-      __Pyx_TraceLine(1427,0,__PYX_ERR(0, 1427, __pyx_L1_error))
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1427, __pyx_L1_error)
+      __Pyx_TraceLine(1444,0,__PYX_ERR(0, 1444, __pyx_L1_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1444, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_full); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1427, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_full); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1444, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyInt_FromSize_t(__pyx_v_N); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1427, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_FromSize_t(__pyx_v_N); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1444, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_4 = PyFloat_FromDouble(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->get_max_priority(__pyx_v_self, 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1427, __pyx_L1_error)
+      __pyx_t_4 = PyFloat_FromDouble(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->get_max_priority(__pyx_v_self, 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1444, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1427, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1444, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_4);
       __pyx_t_6 = 0;
       __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1427, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1444, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1427, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1444, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_single); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1427, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_single); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1444, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1427, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1444, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_8, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1427, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_8, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1444, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF_SET(__pyx_v_priorities, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":1426
+      /* "cpprb/PyReplayBuffer.pyx":1443
  * 
  *         if self.use_nstep:
  *             if priorities is None:             # <<<<<<<<<<<<<<
  *                 priorities = np.full((N),self.get_max_priority(),dtype=np.single)
  * 
  */
     }
 
-    /* "cpprb/PyReplayBuffer.pyx":1429
+    /* "cpprb/PyReplayBuffer.pyx":1446
  *                 priorities = np.full((N),self.get_max_priority(),dtype=np.single)
  * 
  *             priorities = self.priorities_nstep.add(priorities=priorities,             # <<<<<<<<<<<<<<
  *                                                    done=np.array(kwargs["done"],
  *                                                                  copy=True))
  */
-    __Pyx_TraceLine(1429,0,__PYX_ERR(0, 1429, __pyx_L1_error))
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->priorities_nstep), __pyx_n_s_add); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1429, __pyx_L1_error)
+    __Pyx_TraceLine(1446,0,__PYX_ERR(0, 1446, __pyx_L1_error))
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->priorities_nstep), __pyx_n_s_add); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1446, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1429, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1446, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_priorities, __pyx_v_priorities) < 0) __PYX_ERR(0, 1429, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_priorities, __pyx_v_priorities) < 0) __PYX_ERR(0, 1446, __pyx_L1_error)
 
-    /* "cpprb/PyReplayBuffer.pyx":1430
+    /* "cpprb/PyReplayBuffer.pyx":1447
  * 
  *             priorities = self.priorities_nstep.add(priorities=priorities,
  *                                                    done=np.array(kwargs["done"],             # <<<<<<<<<<<<<<
  *                                                                  copy=True))
  *             if priorities is not None:
  */
-    __Pyx_TraceLine(1430,0,__PYX_ERR(0, 1430, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1430, __pyx_L1_error)
+    __Pyx_TraceLine(1447,0,__PYX_ERR(0, 1447, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_array); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1430, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_array); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_u_done); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1430, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_u_done); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1430, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_8);
     __pyx_t_8 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1431
+    /* "cpprb/PyReplayBuffer.pyx":1448
  *             priorities = self.priorities_nstep.add(priorities=priorities,
  *                                                    done=np.array(kwargs["done"],
  *                                                                  copy=True))             # <<<<<<<<<<<<<<
  *             if priorities is not None:
  *                 priorities = np.ravel(priorities["priorities"])
  */
-    __Pyx_TraceLine(1431,0,__PYX_ERR(0, 1431, __pyx_L1_error))
-    __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1431, __pyx_L1_error)
+    __Pyx_TraceLine(1448,0,__PYX_ERR(0, 1448, __pyx_L1_error))
+    __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1448, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_copy, Py_True) < 0) __PYX_ERR(0, 1431, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_copy, Py_True) < 0) __PYX_ERR(0, 1448, __pyx_L1_error)
 
-    /* "cpprb/PyReplayBuffer.pyx":1430
+    /* "cpprb/PyReplayBuffer.pyx":1447
  * 
  *             priorities = self.priorities_nstep.add(priorities=priorities,
  *                                                    done=np.array(kwargs["done"],             # <<<<<<<<<<<<<<
  *                                                                  copy=True))
  *             if priorities is not None:
  */
-    __Pyx_TraceLine(1430,0,__PYX_ERR(0, 1430, __pyx_L1_error))
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_6, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1430, __pyx_L1_error)
+    __Pyx_TraceLine(1447,0,__PYX_ERR(0, 1447, __pyx_L1_error))
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_6, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_done, __pyx_t_7) < 0) __PYX_ERR(0, 1429, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_done, __pyx_t_7) < 0) __PYX_ERR(0, 1446, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1429
+    /* "cpprb/PyReplayBuffer.pyx":1446
  *                 priorities = np.full((N),self.get_max_priority(),dtype=np.single)
  * 
  *             priorities = self.priorities_nstep.add(priorities=priorities,             # <<<<<<<<<<<<<<
  *                                                    done=np.array(kwargs["done"],
  *                                                                  copy=True))
  */
-    __Pyx_TraceLine(1429,0,__PYX_ERR(0, 1429, __pyx_L1_error))
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1429, __pyx_L1_error)
+    __Pyx_TraceLine(1446,0,__PYX_ERR(0, 1446, __pyx_L1_error))
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1446, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_priorities, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1432
+    /* "cpprb/PyReplayBuffer.pyx":1449
  *                                                    done=np.array(kwargs["done"],
  *                                                                  copy=True))
  *             if priorities is not None:             # <<<<<<<<<<<<<<
  *                 priorities = np.ravel(priorities["priorities"])
  *                 N = priorities.shape[0]
  */
-    __Pyx_TraceLine(1432,0,__PYX_ERR(0, 1432, __pyx_L1_error))
+    __Pyx_TraceLine(1449,0,__PYX_ERR(0, 1449, __pyx_L1_error))
     __pyx_t_2 = (__pyx_v_priorities != Py_None);
     __pyx_t_3 = (__pyx_t_2 != 0);
     if (__pyx_t_3) {
 
-      /* "cpprb/PyReplayBuffer.pyx":1433
+      /* "cpprb/PyReplayBuffer.pyx":1450
  *                                                                  copy=True))
  *             if priorities is not None:
  *                 priorities = np.ravel(priorities["priorities"])             # <<<<<<<<<<<<<<
  *                 N = priorities.shape[0]
  * 
  */
-      __Pyx_TraceLine(1433,0,__PYX_ERR(0, 1433, __pyx_L1_error))
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1433, __pyx_L1_error)
+      __Pyx_TraceLine(1450,0,__PYX_ERR(0, 1450, __pyx_L1_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1450, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ravel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1433, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ravel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1450, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_priorities, __pyx_n_u_priorities); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1433, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_priorities, __pyx_n_u_priorities); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1450, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_8 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_7 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_8, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1433, __pyx_L1_error)
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1450, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF_SET(__pyx_v_priorities, __pyx_t_7);
       __pyx_t_7 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":1434
+      /* "cpprb/PyReplayBuffer.pyx":1451
  *             if priorities is not None:
  *                 priorities = np.ravel(priorities["priorities"])
  *                 N = priorities.shape[0]             # <<<<<<<<<<<<<<
  * 
  *         cdef maybe_index = super().add(**kwargs)
  */
-      __Pyx_TraceLine(1434,0,__PYX_ERR(0, 1434, __pyx_L1_error))
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_priorities, __pyx_n_s_shape); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1434, __pyx_L1_error)
+      __Pyx_TraceLine(1451,0,__PYX_ERR(0, 1451, __pyx_L1_error))
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_priorities, __pyx_n_s_shape); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1451, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_7, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1434, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_7, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1451, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_t_5); if (unlikely((__pyx_t_1 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1434, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_t_5); if (unlikely((__pyx_t_1 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1451, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_N = __pyx_t_1;
 
-      /* "cpprb/PyReplayBuffer.pyx":1432
+      /* "cpprb/PyReplayBuffer.pyx":1449
  *                                                    done=np.array(kwargs["done"],
  *                                                                  copy=True))
  *             if priorities is not None:             # <<<<<<<<<<<<<<
  *                 priorities = np.ravel(priorities["priorities"])
  *                 N = priorities.shape[0]
  */
     }
 
-    /* "cpprb/PyReplayBuffer.pyx":1425
+    /* "cpprb/PyReplayBuffer.pyx":1442
  *                 raise ValueError("`priorities` shape is imcompatible")
  * 
  *         if self.use_nstep:             # <<<<<<<<<<<<<<
  *             if priorities is None:
  *                 priorities = np.full((N),self.get_max_priority(),dtype=np.single)
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1436
+  /* "cpprb/PyReplayBuffer.pyx":1453
  *                 N = priorities.shape[0]
  * 
  *         cdef maybe_index = super().add(**kwargs)             # <<<<<<<<<<<<<<
  *         if maybe_index is None:
  *             return None
  */
-  __Pyx_TraceLine(1436,0,__PYX_ERR(0, 1436, __pyx_L1_error))
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1436, __pyx_L1_error)
+  __Pyx_TraceLine(1453,0,__PYX_ERR(0, 1453, __pyx_L1_error))
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer));
   PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer));
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_5, 1, ((PyObject *)__pyx_v_self));
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_5, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1436, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_5, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_add); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1436, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_add); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_v_kwargs); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1436, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_v_kwargs); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_maybe_index = __pyx_t_7;
   __pyx_t_7 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1437
+  /* "cpprb/PyReplayBuffer.pyx":1454
  * 
  *         cdef maybe_index = super().add(**kwargs)
  *         if maybe_index is None:             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
-  __Pyx_TraceLine(1437,0,__PYX_ERR(0, 1437, __pyx_L1_error))
+  __Pyx_TraceLine(1454,0,__PYX_ERR(0, 1454, __pyx_L1_error))
   __pyx_t_3 = (__pyx_v_maybe_index == Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
   if (__pyx_t_2) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1438
+    /* "cpprb/PyReplayBuffer.pyx":1455
  *         cdef maybe_index = super().add(**kwargs)
  *         if maybe_index is None:
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         cdef size_t index = maybe_index
  */
-    __Pyx_TraceLine(1438,0,__PYX_ERR(0, 1438, __pyx_L1_error))
+    __Pyx_TraceLine(1455,0,__PYX_ERR(0, 1455, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1437
+    /* "cpprb/PyReplayBuffer.pyx":1454
  * 
  *         cdef maybe_index = super().add(**kwargs)
  *         if maybe_index is None:             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1440
+  /* "cpprb/PyReplayBuffer.pyx":1457
  *             return None
  * 
  *         cdef size_t index = maybe_index             # <<<<<<<<<<<<<<
  *         cdef const float [:] ps
  * 
  */
-  __Pyx_TraceLine(1440,0,__PYX_ERR(0, 1440, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_maybe_index); if (unlikely((__pyx_t_1 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1440, __pyx_L1_error)
+  __Pyx_TraceLine(1457,0,__PYX_ERR(0, 1457, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_maybe_index); if (unlikely((__pyx_t_1 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1457, __pyx_L1_error)
   __pyx_v_index = __pyx_t_1;
 
-  /* "cpprb/PyReplayBuffer.pyx":1443
+  /* "cpprb/PyReplayBuffer.pyx":1460
  *         cdef const float [:] ps
  * 
  *         if priorities is not None:             # <<<<<<<<<<<<<<
  *             ps = np.ravel(np.array(priorities,copy=False,ndmin=1,dtype=np.single))
  *             self.per.set_priorities(index,&ps[0],N,self.get_buffer_size())
  */
-  __Pyx_TraceLine(1443,0,__PYX_ERR(0, 1443, __pyx_L1_error))
+  __Pyx_TraceLine(1460,0,__PYX_ERR(0, 1460, __pyx_L1_error))
   __pyx_t_2 = (__pyx_v_priorities != Py_None);
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1444
+    /* "cpprb/PyReplayBuffer.pyx":1461
  * 
  *         if priorities is not None:
  *             ps = np.ravel(np.array(priorities,copy=False,ndmin=1,dtype=np.single))             # <<<<<<<<<<<<<<
  *             self.per.set_priorities(index,&ps[0],N,self.get_buffer_size())
  *         else:
  */
-    __Pyx_TraceLine(1444,0,__PYX_ERR(0, 1444, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1444, __pyx_L1_error)
+    __Pyx_TraceLine(1461,0,__PYX_ERR(0, 1461, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1461, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ravel); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1444, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ravel); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1461, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1444, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1461, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1444, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1461, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1444, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1461, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_v_priorities);
     __Pyx_GIVEREF(__pyx_v_priorities);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_priorities);
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1444, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1461, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1444, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_ndmin, __pyx_int_1) < 0) __PYX_ERR(0, 1444, __pyx_L1_error)
-    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1444, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1461, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_ndmin, __pyx_int_1) < 0) __PYX_ERR(0, 1461, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1461, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_single); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1444, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_single); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1461, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 1444, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 1461, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1444, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1461, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
@@ -25284,97 +25490,97 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_7 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_6, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_9);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1444, __pyx_L1_error)
+    if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1461, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_float__const__(__pyx_t_7, 0); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 1444, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_float__const__(__pyx_t_7, 0); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 1461, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_v_ps = __pyx_t_11;
     __pyx_t_11.memview = NULL;
     __pyx_t_11.data = NULL;
 
-    /* "cpprb/PyReplayBuffer.pyx":1445
+    /* "cpprb/PyReplayBuffer.pyx":1462
  *         if priorities is not None:
  *             ps = np.ravel(np.array(priorities,copy=False,ndmin=1,dtype=np.single))
  *             self.per.set_priorities(index,&ps[0],N,self.get_buffer_size())             # <<<<<<<<<<<<<<
  *         else:
  *             self.per.set_priorities(index,N,self.get_buffer_size())
  */
-    __Pyx_TraceLine(1445,0,__PYX_ERR(0, 1445, __pyx_L1_error))
+    __Pyx_TraceLine(1462,0,__PYX_ERR(0, 1462, __pyx_L1_error))
     __pyx_t_12 = 0;
     __pyx_t_13 = -1;
     if (__pyx_t_12 < 0) {
       __pyx_t_12 += __pyx_v_ps.shape[0];
       if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 0;
     } else if (unlikely(__pyx_t_12 >= __pyx_v_ps.shape[0])) __pyx_t_13 = 0;
     if (unlikely(__pyx_t_13 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_13);
-      __PYX_ERR(0, 1445, __pyx_L1_error)
+      __PYX_ERR(0, 1462, __pyx_L1_error)
     }
     __pyx_v_self->per->set_priorities(__pyx_v_index, (&(*((float const  *) ( /* dim=0 */ (__pyx_v_ps.data + __pyx_t_12 * __pyx_v_ps.strides[0]) )))), __pyx_v_N, ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_buffer_size(((struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self), 0));
 
-    /* "cpprb/PyReplayBuffer.pyx":1443
+    /* "cpprb/PyReplayBuffer.pyx":1460
  *         cdef const float [:] ps
  * 
  *         if priorities is not None:             # <<<<<<<<<<<<<<
  *             ps = np.ravel(np.array(priorities,copy=False,ndmin=1,dtype=np.single))
  *             self.per.set_priorities(index,&ps[0],N,self.get_buffer_size())
  */
     goto __pyx_L9;
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1447
+  /* "cpprb/PyReplayBuffer.pyx":1464
  *             self.per.set_priorities(index,&ps[0],N,self.get_buffer_size())
  *         else:
  *             self.per.set_priorities(index,N,self.get_buffer_size())             # <<<<<<<<<<<<<<
  * 
  *         if self.check_for_update:
  */
-  __Pyx_TraceLine(1447,0,__PYX_ERR(0, 1447, __pyx_L1_error))
+  __Pyx_TraceLine(1464,0,__PYX_ERR(0, 1464, __pyx_L1_error))
   /*else*/ {
     __pyx_v_self->per->set_priorities(__pyx_v_index, __pyx_v_N, ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_buffer_size(((struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self), 0));
   }
   __pyx_L9:;
 
-  /* "cpprb/PyReplayBuffer.pyx":1449
+  /* "cpprb/PyReplayBuffer.pyx":1466
  *             self.per.set_priorities(index,N,self.get_buffer_size())
  * 
  *         if self.check_for_update:             # <<<<<<<<<<<<<<
  *             if index+N <= self.buffer_size:
  *                 self.unchange_since_sample[index:index+N] = False
  */
-  __Pyx_TraceLine(1449,0,__PYX_ERR(0, 1449, __pyx_L1_error))
+  __Pyx_TraceLine(1466,0,__PYX_ERR(0, 1466, __pyx_L1_error))
   __pyx_t_3 = (__pyx_v_self->check_for_update != 0);
   if (__pyx_t_3) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1450
+    /* "cpprb/PyReplayBuffer.pyx":1467
  * 
  *         if self.check_for_update:
  *             if index+N <= self.buffer_size:             # <<<<<<<<<<<<<<
  *                 self.unchange_since_sample[index:index+N] = False
  *             else:
  */
-    __Pyx_TraceLine(1450,0,__PYX_ERR(0, 1450, __pyx_L1_error))
+    __Pyx_TraceLine(1467,0,__PYX_ERR(0, 1467, __pyx_L1_error))
     __pyx_t_3 = (((__pyx_v_index + __pyx_v_N) <= __pyx_v_self->__pyx_base.buffer_size) != 0);
     if (__pyx_t_3) {
 
-      /* "cpprb/PyReplayBuffer.pyx":1451
+      /* "cpprb/PyReplayBuffer.pyx":1468
  *         if self.check_for_update:
  *             if index+N <= self.buffer_size:
  *                 self.unchange_since_sample[index:index+N] = False             # <<<<<<<<<<<<<<
  *             else:
  *                 self.unchange_since_sample[index:] = False
  */
-      __Pyx_TraceLine(1451,0,__PYX_ERR(0, 1451, __pyx_L1_error))
-      if (unlikely(!__pyx_v_self->unchange_since_sample.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1451, __pyx_L1_error)}
+      __Pyx_TraceLine(1468,0,__PYX_ERR(0, 1468, __pyx_L1_error))
+      if (unlikely(!__pyx_v_self->unchange_since_sample.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1468, __pyx_L1_error)}
       __pyx_t_14.data = __pyx_v_self->unchange_since_sample.data;
       __pyx_t_14.memview = __pyx_v_self->unchange_since_sample.memview;
       __PYX_INC_MEMVIEW(&__pyx_t_14, 0);
       __pyx_t_13 = -1;
       if (unlikely(__pyx_memoryview_slice_memviewslice(
     &__pyx_t_14,
     __pyx_v_self->unchange_since_sample.shape[0], __pyx_v_self->unchange_since_sample.strides[0], __pyx_v_self->unchange_since_sample.suboffsets[0],
@@ -25385,15 +25591,15 @@
     (__pyx_v_index + __pyx_v_N),
     0,
     1,
     1,
     0,
     1) < 0))
 {
-    __PYX_ERR(0, 1451, __pyx_L1_error)
+    __PYX_ERR(0, 1468, __pyx_L1_error)
 }
 
 {
           bool __pyx_temp_scalar = 0;
           {
               Py_ssize_t __pyx_temp_extent_0 = __pyx_t_14.shape[0];
               Py_ssize_t __pyx_temp_stride_0 = __pyx_t_14.strides[0];
@@ -25406,34 +25612,34 @@
               }
           }
       }
       __PYX_XDEC_MEMVIEW(&__pyx_t_14, 1);
       __pyx_t_14.memview = NULL;
       __pyx_t_14.data = NULL;
 
-      /* "cpprb/PyReplayBuffer.pyx":1450
+      /* "cpprb/PyReplayBuffer.pyx":1467
  * 
  *         if self.check_for_update:
  *             if index+N <= self.buffer_size:             # <<<<<<<<<<<<<<
  *                 self.unchange_since_sample[index:index+N] = False
  *             else:
  */
       goto __pyx_L11;
     }
 
-    /* "cpprb/PyReplayBuffer.pyx":1453
+    /* "cpprb/PyReplayBuffer.pyx":1470
  *                 self.unchange_since_sample[index:index+N] = False
  *             else:
  *                 self.unchange_since_sample[index:] = False             # <<<<<<<<<<<<<<
  *                 self.unchange_since_sample[:index+N-self.buffer_size] = False
  * 
  */
-    __Pyx_TraceLine(1453,0,__PYX_ERR(0, 1453, __pyx_L1_error))
+    __Pyx_TraceLine(1470,0,__PYX_ERR(0, 1470, __pyx_L1_error))
     /*else*/ {
-      if (unlikely(!__pyx_v_self->unchange_since_sample.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1453, __pyx_L1_error)}
+      if (unlikely(!__pyx_v_self->unchange_since_sample.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1470, __pyx_L1_error)}
       __pyx_t_14.data = __pyx_v_self->unchange_since_sample.data;
       __pyx_t_14.memview = __pyx_v_self->unchange_since_sample.memview;
       __PYX_INC_MEMVIEW(&__pyx_t_14, 0);
       __pyx_t_13 = -1;
       if (unlikely(__pyx_memoryview_slice_memviewslice(
     &__pyx_t_14,
     __pyx_v_self->unchange_since_sample.shape[0], __pyx_v_self->unchange_since_sample.strides[0], __pyx_v_self->unchange_since_sample.suboffsets[0],
@@ -25444,15 +25650,15 @@
     0,
     0,
     1,
     0,
     0,
     1) < 0))
 {
-    __PYX_ERR(0, 1453, __pyx_L1_error)
+    __PYX_ERR(0, 1470, __pyx_L1_error)
 }
 
 {
           bool __pyx_temp_scalar = 0;
           {
               Py_ssize_t __pyx_temp_extent_0 = __pyx_t_14.shape[0];
               Py_ssize_t __pyx_temp_stride_0 = __pyx_t_14.strides[0];
@@ -25465,23 +25671,23 @@
               }
           }
       }
       __PYX_XDEC_MEMVIEW(&__pyx_t_14, 1);
       __pyx_t_14.memview = NULL;
       __pyx_t_14.data = NULL;
 
-      /* "cpprb/PyReplayBuffer.pyx":1454
+      /* "cpprb/PyReplayBuffer.pyx":1471
  *             else:
  *                 self.unchange_since_sample[index:] = False
  *                 self.unchange_since_sample[:index+N-self.buffer_size] = False             # <<<<<<<<<<<<<<
  * 
  *         return index
  */
-      __Pyx_TraceLine(1454,0,__PYX_ERR(0, 1454, __pyx_L1_error))
-      if (unlikely(!__pyx_v_self->unchange_since_sample.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1454, __pyx_L1_error)}
+      __Pyx_TraceLine(1471,0,__PYX_ERR(0, 1471, __pyx_L1_error))
+      if (unlikely(!__pyx_v_self->unchange_since_sample.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1471, __pyx_L1_error)}
       __pyx_t_14.data = __pyx_v_self->unchange_since_sample.data;
       __pyx_t_14.memview = __pyx_v_self->unchange_since_sample.memview;
       __PYX_INC_MEMVIEW(&__pyx_t_14, 0);
       __pyx_t_13 = -1;
       if (unlikely(__pyx_memoryview_slice_memviewslice(
     &__pyx_t_14,
     __pyx_v_self->unchange_since_sample.shape[0], __pyx_v_self->unchange_since_sample.strides[0], __pyx_v_self->unchange_since_sample.suboffsets[0],
@@ -25492,15 +25698,15 @@
     ((__pyx_v_index + __pyx_v_N) - __pyx_v_self->__pyx_base.buffer_size),
     0,
     0,
     1,
     0,
     1) < 0))
 {
-    __PYX_ERR(0, 1454, __pyx_L1_error)
+    __PYX_ERR(0, 1471, __pyx_L1_error)
 }
 
 {
           bool __pyx_temp_scalar = 0;
           {
               Py_ssize_t __pyx_temp_extent_0 = __pyx_t_14.shape[0];
               Py_ssize_t __pyx_temp_stride_0 = __pyx_t_14.strides[0];
@@ -25515,39 +25721,39 @@
       }
       __PYX_XDEC_MEMVIEW(&__pyx_t_14, 1);
       __pyx_t_14.memview = NULL;
       __pyx_t_14.data = NULL;
     }
     __pyx_L11:;
 
-    /* "cpprb/PyReplayBuffer.pyx":1449
+    /* "cpprb/PyReplayBuffer.pyx":1466
  *             self.per.set_priorities(index,N,self.get_buffer_size())
  * 
  *         if self.check_for_update:             # <<<<<<<<<<<<<<
  *             if index+N <= self.buffer_size:
  *                 self.unchange_since_sample[index:index+N] = False
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1456
+  /* "cpprb/PyReplayBuffer.pyx":1473
  *                 self.unchange_since_sample[:index+N-self.buffer_size] = False
  * 
  *         return index             # <<<<<<<<<<<<<<
  * 
  *     def sample(self,batch_size,beta = 0.4):
  */
-  __Pyx_TraceLine(1456,0,__PYX_ERR(0, 1456, __pyx_L1_error))
+  __Pyx_TraceLine(1473,0,__PYX_ERR(0, 1473, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_7 = __Pyx_PyInt_FromSize_t(__pyx_v_index); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1456, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_FromSize_t(__pyx_v_index); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1473, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_r = __pyx_t_7;
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1388
+  /* "cpprb/PyReplayBuffer.pyx":1405
  *         pass
  * 
  *     def add(self,*,priorities = None,**kwargs):             # <<<<<<<<<<<<<<
  *         r"""Add transition(s) into replay buffer.
  * 
  */
 
@@ -25570,15 +25776,15 @@
   __Pyx_XDECREF(__pyx_v_priorities);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1458
+/* "cpprb/PyReplayBuffer.pyx":1475
  *         return index
  * 
  *     def sample(self,batch_size,beta = 0.4):             # <<<<<<<<<<<<<<
  *         r"""Sample the stored transitions.
  * 
  */
 
@@ -25618,15 +25824,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_beta);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "sample") < 0)) __PYX_ERR(0, 1458, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "sample") < 0)) __PYX_ERR(0, 1475, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -25634,15 +25840,15 @@
       }
     }
     __pyx_v_batch_size = values[0];
     __pyx_v_beta = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("sample", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1458, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("sample", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1475, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.PrioritizedReplayBuffer.sample", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_6sample(((struct __pyx_obj_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *)__pyx_v_self), __pyx_v_batch_size, __pyx_v_beta);
 
@@ -25663,151 +25869,151 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sample", 0);
-  __Pyx_TraceCall("sample", __pyx_f[0], 1458, 0, __PYX_ERR(0, 1458, __pyx_L1_error));
+  __Pyx_TraceCall("sample", __pyx_f[0], 1475, 0, __PYX_ERR(0, 1475, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1484
+  /* "cpprb/PyReplayBuffer.pyx":1501
  *         (:math:`= w_{i}/\max_{j}(w_{j})`), which ensure the weights :math:`\leq` 1.
  *         """
  *         self.per.sample(batch_size,beta,             # <<<<<<<<<<<<<<
  *                         self.weights.vec,self.indexes.vec,
  *                         self.get_stored_size())
  */
-  __Pyx_TraceLine(1484,0,__PYX_ERR(0, 1484, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_batch_size); if (unlikely((__pyx_t_1 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1484, __pyx_L1_error)
-  __pyx_t_2 = __pyx_PyFloat_AsFloat(__pyx_v_beta); if (unlikely((__pyx_t_2 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1484, __pyx_L1_error)
+  __Pyx_TraceLine(1501,0,__PYX_ERR(0, 1501, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_batch_size); if (unlikely((__pyx_t_1 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1501, __pyx_L1_error)
+  __pyx_t_2 = __pyx_PyFloat_AsFloat(__pyx_v_beta); if (unlikely((__pyx_t_2 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1501, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":1486
+  /* "cpprb/PyReplayBuffer.pyx":1503
  *         self.per.sample(batch_size,beta,
  *                         self.weights.vec,self.indexes.vec,
  *                         self.get_stored_size())             # <<<<<<<<<<<<<<
  *         cdef idx = self.indexes.as_numpy()
  *         samples = self._encode_sample(idx)
  */
-  __Pyx_TraceLine(1486,0,__PYX_ERR(0, 1486, __pyx_L1_error))
+  __Pyx_TraceLine(1503,0,__PYX_ERR(0, 1503, __pyx_L1_error))
   __pyx_v_self->per->sample(__pyx_t_1, __pyx_t_2, __pyx_v_self->weights->vec, __pyx_v_self->indexes->vec, ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_stored_size(((struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self), 0));
 
-  /* "cpprb/PyReplayBuffer.pyx":1487
+  /* "cpprb/PyReplayBuffer.pyx":1504
  *                         self.weights.vec,self.indexes.vec,
  *                         self.get_stored_size())
  *         cdef idx = self.indexes.as_numpy()             # <<<<<<<<<<<<<<
  *         samples = self._encode_sample(idx)
  *         samples['weights'] = self.weights.as_numpy()
  */
-  __Pyx_TraceLine(1487,0,__PYX_ERR(0, 1487, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->indexes), __pyx_n_s_as_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1487, __pyx_L1_error)
+  __Pyx_TraceLine(1504,0,__PYX_ERR(0, 1504, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->indexes), __pyx_n_s_as_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1504, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1487, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1504, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_idx = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1488
+  /* "cpprb/PyReplayBuffer.pyx":1505
  *                         self.get_stored_size())
  *         cdef idx = self.indexes.as_numpy()
  *         samples = self._encode_sample(idx)             # <<<<<<<<<<<<<<
  *         samples['weights'] = self.weights.as_numpy()
  *         samples['indexes'] = idx
  */
-  __Pyx_TraceLine(1488,0,__PYX_ERR(0, 1488, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_encode_sample); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1488, __pyx_L1_error)
+  __Pyx_TraceLine(1505,0,__PYX_ERR(0, 1505, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_encode_sample); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1505, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_idx) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_idx);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1488, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1505, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_samples = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1489
+  /* "cpprb/PyReplayBuffer.pyx":1506
  *         cdef idx = self.indexes.as_numpy()
  *         samples = self._encode_sample(idx)
  *         samples['weights'] = self.weights.as_numpy()             # <<<<<<<<<<<<<<
  *         samples['indexes'] = idx
  * 
  */
-  __Pyx_TraceLine(1489,0,__PYX_ERR(0, 1489, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->weights), __pyx_n_s_as_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1489, __pyx_L1_error)
+  __Pyx_TraceLine(1506,0,__PYX_ERR(0, 1506, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->weights), __pyx_n_s_as_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1489, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_samples, __pyx_n_u_weights, __pyx_t_3) < 0)) __PYX_ERR(0, 1489, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_samples, __pyx_n_u_weights, __pyx_t_3) < 0)) __PYX_ERR(0, 1506, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1490
+  /* "cpprb/PyReplayBuffer.pyx":1507
  *         samples = self._encode_sample(idx)
  *         samples['weights'] = self.weights.as_numpy()
  *         samples['indexes'] = idx             # <<<<<<<<<<<<<<
  * 
  *         if self.check_for_update:
  */
-  __Pyx_TraceLine(1490,0,__PYX_ERR(0, 1490, __pyx_L1_error))
-  if (unlikely(PyObject_SetItem(__pyx_v_samples, __pyx_n_u_indexes, __pyx_v_idx) < 0)) __PYX_ERR(0, 1490, __pyx_L1_error)
+  __Pyx_TraceLine(1507,0,__PYX_ERR(0, 1507, __pyx_L1_error))
+  if (unlikely(PyObject_SetItem(__pyx_v_samples, __pyx_n_u_indexes, __pyx_v_idx) < 0)) __PYX_ERR(0, 1507, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":1492
+  /* "cpprb/PyReplayBuffer.pyx":1509
  *         samples['indexes'] = idx
  * 
  *         if self.check_for_update:             # <<<<<<<<<<<<<<
  *             self.unchange_since_sample[:] = True
  * 
  */
-  __Pyx_TraceLine(1492,0,__PYX_ERR(0, 1492, __pyx_L1_error))
+  __Pyx_TraceLine(1509,0,__PYX_ERR(0, 1509, __pyx_L1_error))
   __pyx_t_6 = (__pyx_v_self->check_for_update != 0);
   if (__pyx_t_6) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1493
+    /* "cpprb/PyReplayBuffer.pyx":1510
  * 
  *         if self.check_for_update:
  *             self.unchange_since_sample[:] = True             # <<<<<<<<<<<<<<
  * 
  *         return samples
  */
-    __Pyx_TraceLine(1493,0,__PYX_ERR(0, 1493, __pyx_L1_error))
-    if (unlikely(!__pyx_v_self->unchange_since_sample.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1493, __pyx_L1_error)}
+    __Pyx_TraceLine(1510,0,__PYX_ERR(0, 1510, __pyx_L1_error))
+    if (unlikely(!__pyx_v_self->unchange_since_sample.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1510, __pyx_L1_error)}
     {
         bool __pyx_temp_scalar = 1;
         {
             Py_ssize_t __pyx_temp_extent_0 = __pyx_v_self->unchange_since_sample.shape[0];
             Py_ssize_t __pyx_temp_stride_0 = __pyx_v_self->unchange_since_sample.strides[0];
             char *__pyx_temp_pointer_0;
             Py_ssize_t __pyx_temp_idx_0;
@@ -25815,37 +26021,37 @@
             for (__pyx_temp_idx_0 = 0; __pyx_temp_idx_0 < __pyx_temp_extent_0; __pyx_temp_idx_0++) {
               *((bool *) __pyx_temp_pointer_0) = __pyx_temp_scalar;
               __pyx_temp_pointer_0 += __pyx_temp_stride_0;
             }
         }
     }
 
-    /* "cpprb/PyReplayBuffer.pyx":1492
+    /* "cpprb/PyReplayBuffer.pyx":1509
  *         samples['indexes'] = idx
  * 
  *         if self.check_for_update:             # <<<<<<<<<<<<<<
  *             self.unchange_since_sample[:] = True
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1495
+  /* "cpprb/PyReplayBuffer.pyx":1512
  *             self.unchange_since_sample[:] = True
  * 
  *         return samples             # <<<<<<<<<<<<<<
  * 
  *     def update_priorities(self,indexes,priorities):
  */
-  __Pyx_TraceLine(1495,0,__PYX_ERR(0, 1495, __pyx_L1_error))
+  __Pyx_TraceLine(1512,0,__PYX_ERR(0, 1512, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_samples);
   __pyx_r = __pyx_v_samples;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1458
+  /* "cpprb/PyReplayBuffer.pyx":1475
  *         return index
  * 
  *     def sample(self,batch_size,beta = 0.4):             # <<<<<<<<<<<<<<
  *         r"""Sample the stored transitions.
  * 
  */
 
@@ -25861,15 +26067,15 @@
   __Pyx_XDECREF(__pyx_v_samples);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1497
+/* "cpprb/PyReplayBuffer.pyx":1514
  *         return samples
  * 
  *     def update_priorities(self,indexes,priorities):             # <<<<<<<<<<<<<<
  *         r"""Update priorities
  * 
  */
 
@@ -25904,32 +26110,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indexes)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_priorities)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("update_priorities", 1, 2, 2, 1); __PYX_ERR(0, 1497, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("update_priorities", 1, 2, 2, 1); __PYX_ERR(0, 1514, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "update_priorities") < 0)) __PYX_ERR(0, 1497, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "update_priorities") < 0)) __PYX_ERR(0, 1514, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_indexes = values[0];
     __pyx_v_priorities = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("update_priorities", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1497, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("update_priorities", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1514, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.PrioritizedReplayBuffer.update_priorities", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_8update_priorities(((struct __pyx_obj_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *)__pyx_v_self), __pyx_v_indexes, __pyx_v_priorities);
 
@@ -25958,348 +26164,348 @@
   Py_ssize_t __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   size_t __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("update_priorities", 0);
-  __Pyx_TraceCall("update_priorities", __pyx_f[0], 1497, 0, __PYX_ERR(0, 1497, __pyx_L1_error));
+  __Pyx_TraceCall("update_priorities", __pyx_f[0], 1514, 0, __PYX_ERR(0, 1514, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1517
+  /* "cpprb/PyReplayBuffer.pyx":1534
  *         """
  * 
  *         if priorities is None:             # <<<<<<<<<<<<<<
  *             raise TypeError("`properties` must not be `None`")
  * 
  */
-  __Pyx_TraceLine(1517,0,__PYX_ERR(0, 1517, __pyx_L1_error))
+  __Pyx_TraceLine(1534,0,__PYX_ERR(0, 1534, __pyx_L1_error))
   __pyx_t_1 = (__pyx_v_priorities == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1518
+    /* "cpprb/PyReplayBuffer.pyx":1535
  * 
  *         if priorities is None:
  *             raise TypeError("`properties` must not be `None`")             # <<<<<<<<<<<<<<
  * 
  *         cdef const size_t [:] idx = Csize(indexes)
  */
-    __Pyx_TraceLine(1518,0,__PYX_ERR(0, 1518, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1518, __pyx_L1_error)
+    __Pyx_TraceLine(1535,0,__PYX_ERR(0, 1535, __pyx_L1_error))
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1535, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 1518, __pyx_L1_error)
+    __PYX_ERR(0, 1535, __pyx_L1_error)
 
-    /* "cpprb/PyReplayBuffer.pyx":1517
+    /* "cpprb/PyReplayBuffer.pyx":1534
  *         """
  * 
  *         if priorities is None:             # <<<<<<<<<<<<<<
  *             raise TypeError("`properties` must not be `None`")
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1520
+  /* "cpprb/PyReplayBuffer.pyx":1537
  *             raise TypeError("`properties` must not be `None`")
  * 
  *         cdef const size_t [:] idx = Csize(indexes)             # <<<<<<<<<<<<<<
  *         cdef const float [:] ps = Cfloat(priorities)
  * 
  */
-  __Pyx_TraceLine(1520,0,__PYX_ERR(0, 1520, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_5cpprb_14PyReplayBuffer_Csize(__pyx_v_indexes); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 1520, __pyx_L1_error)
+  __Pyx_TraceLine(1537,0,__PYX_ERR(0, 1537, __pyx_L1_error))
+  __pyx_t_4 = __pyx_f_5cpprb_14PyReplayBuffer_Csize(__pyx_v_indexes); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 1537, __pyx_L1_error)
   __pyx_v_idx = __pyx_t_4;
   __pyx_t_4.memview = NULL;
   __pyx_t_4.data = NULL;
 
-  /* "cpprb/PyReplayBuffer.pyx":1521
+  /* "cpprb/PyReplayBuffer.pyx":1538
  * 
  *         cdef const size_t [:] idx = Csize(indexes)
  *         cdef const float [:] ps = Cfloat(priorities)             # <<<<<<<<<<<<<<
  * 
  *         if not self.check_for_update:
  */
-  __Pyx_TraceLine(1521,0,__PYX_ERR(0, 1521, __pyx_L1_error))
-  __pyx_t_5 = __pyx_f_5cpprb_14PyReplayBuffer_Cfloat(__pyx_v_priorities); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 1521, __pyx_L1_error)
+  __Pyx_TraceLine(1538,0,__PYX_ERR(0, 1538, __pyx_L1_error))
+  __pyx_t_5 = __pyx_f_5cpprb_14PyReplayBuffer_Cfloat(__pyx_v_priorities); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 1538, __pyx_L1_error)
   __pyx_v_ps = __pyx_t_5;
   __pyx_t_5.memview = NULL;
   __pyx_t_5.data = NULL;
 
-  /* "cpprb/PyReplayBuffer.pyx":1523
+  /* "cpprb/PyReplayBuffer.pyx":1540
  *         cdef const float [:] ps = Cfloat(priorities)
  * 
  *         if not self.check_for_update:             # <<<<<<<<<<<<<<
  *             self.per.update_priorities(&idx[0],&ps[0],idx.shape[0])
  *             return None
  */
-  __Pyx_TraceLine(1523,0,__PYX_ERR(0, 1523, __pyx_L1_error))
+  __Pyx_TraceLine(1540,0,__PYX_ERR(0, 1540, __pyx_L1_error))
   __pyx_t_2 = ((!(__pyx_v_self->check_for_update != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1524
+    /* "cpprb/PyReplayBuffer.pyx":1541
  * 
  *         if not self.check_for_update:
  *             self.per.update_priorities(&idx[0],&ps[0],idx.shape[0])             # <<<<<<<<<<<<<<
  *             return None
  * 
  */
-    __Pyx_TraceLine(1524,0,__PYX_ERR(0, 1524, __pyx_L1_error))
+    __Pyx_TraceLine(1541,0,__PYX_ERR(0, 1541, __pyx_L1_error))
     __pyx_t_6 = 0;
     __pyx_t_7 = -1;
     if (__pyx_t_6 < 0) {
       __pyx_t_6 += __pyx_v_idx.shape[0];
       if (unlikely(__pyx_t_6 < 0)) __pyx_t_7 = 0;
     } else if (unlikely(__pyx_t_6 >= __pyx_v_idx.shape[0])) __pyx_t_7 = 0;
     if (unlikely(__pyx_t_7 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_7);
-      __PYX_ERR(0, 1524, __pyx_L1_error)
+      __PYX_ERR(0, 1541, __pyx_L1_error)
     }
     __pyx_t_8 = 0;
     __pyx_t_7 = -1;
     if (__pyx_t_8 < 0) {
       __pyx_t_8 += __pyx_v_ps.shape[0];
       if (unlikely(__pyx_t_8 < 0)) __pyx_t_7 = 0;
     } else if (unlikely(__pyx_t_8 >= __pyx_v_ps.shape[0])) __pyx_t_7 = 0;
     if (unlikely(__pyx_t_7 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_7);
-      __PYX_ERR(0, 1524, __pyx_L1_error)
+      __PYX_ERR(0, 1541, __pyx_L1_error)
     }
     __pyx_v_self->per->update_priorities((&(*((size_t const  *) ( /* dim=0 */ (__pyx_v_idx.data + __pyx_t_6 * __pyx_v_idx.strides[0]) )))), (&(*((float const  *) ( /* dim=0 */ (__pyx_v_ps.data + __pyx_t_8 * __pyx_v_ps.strides[0]) )))), (__pyx_v_idx.shape[0]));
 
-    /* "cpprb/PyReplayBuffer.pyx":1525
+    /* "cpprb/PyReplayBuffer.pyx":1542
  *         if not self.check_for_update:
  *             self.per.update_priorities(&idx[0],&ps[0],idx.shape[0])
  *             return None             # <<<<<<<<<<<<<<
  * 
  *         self.idx_vec.clear()
  */
-    __Pyx_TraceLine(1525,0,__PYX_ERR(0, 1525, __pyx_L1_error))
+    __Pyx_TraceLine(1542,0,__PYX_ERR(0, 1542, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1523
+    /* "cpprb/PyReplayBuffer.pyx":1540
  *         cdef const float [:] ps = Cfloat(priorities)
  * 
  *         if not self.check_for_update:             # <<<<<<<<<<<<<<
  *             self.per.update_priorities(&idx[0],&ps[0],idx.shape[0])
  *             return None
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1527
+  /* "cpprb/PyReplayBuffer.pyx":1544
  *             return None
  * 
  *         self.idx_vec.clear()             # <<<<<<<<<<<<<<
  *         self.idx_vec.reserve(idx.shape[0])
  * 
  */
-  __Pyx_TraceLine(1527,0,__PYX_ERR(0, 1527, __pyx_L1_error))
+  __Pyx_TraceLine(1544,0,__PYX_ERR(0, 1544, __pyx_L1_error))
   __pyx_v_self->idx_vec.clear();
 
-  /* "cpprb/PyReplayBuffer.pyx":1528
+  /* "cpprb/PyReplayBuffer.pyx":1545
  * 
  *         self.idx_vec.clear()
  *         self.idx_vec.reserve(idx.shape[0])             # <<<<<<<<<<<<<<
  * 
  *         self.ps_vec.clear()
  */
-  __Pyx_TraceLine(1528,0,__PYX_ERR(0, 1528, __pyx_L1_error))
+  __Pyx_TraceLine(1545,0,__PYX_ERR(0, 1545, __pyx_L1_error))
   __pyx_v_self->idx_vec.reserve((__pyx_v_idx.shape[0]));
 
-  /* "cpprb/PyReplayBuffer.pyx":1530
+  /* "cpprb/PyReplayBuffer.pyx":1547
  *         self.idx_vec.reserve(idx.shape[0])
  * 
  *         self.ps_vec.clear()             # <<<<<<<<<<<<<<
  *         self.ps_vec.reserve(ps.shape[0])
  * 
  */
-  __Pyx_TraceLine(1530,0,__PYX_ERR(0, 1530, __pyx_L1_error))
+  __Pyx_TraceLine(1547,0,__PYX_ERR(0, 1547, __pyx_L1_error))
   __pyx_v_self->ps_vec.clear();
 
-  /* "cpprb/PyReplayBuffer.pyx":1531
+  /* "cpprb/PyReplayBuffer.pyx":1548
  * 
  *         self.ps_vec.clear()
  *         self.ps_vec.reserve(ps.shape[0])             # <<<<<<<<<<<<<<
  * 
  *         if self.check_for_update:
  */
-  __Pyx_TraceLine(1531,0,__PYX_ERR(0, 1531, __pyx_L1_error))
+  __Pyx_TraceLine(1548,0,__PYX_ERR(0, 1548, __pyx_L1_error))
   __pyx_v_self->ps_vec.reserve((__pyx_v_ps.shape[0]));
 
-  /* "cpprb/PyReplayBuffer.pyx":1533
+  /* "cpprb/PyReplayBuffer.pyx":1550
  *         self.ps_vec.reserve(ps.shape[0])
  * 
  *         if self.check_for_update:             # <<<<<<<<<<<<<<
  *             for _i in range(idx.shape[0]):
  *                 if self.unchange_since_sample[idx[_i]]:
  */
-  __Pyx_TraceLine(1533,0,__PYX_ERR(0, 1533, __pyx_L1_error))
+  __Pyx_TraceLine(1550,0,__PYX_ERR(0, 1550, __pyx_L1_error))
   __pyx_t_2 = (__pyx_v_self->check_for_update != 0);
   if (__pyx_t_2) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1534
+    /* "cpprb/PyReplayBuffer.pyx":1551
  * 
  *         if self.check_for_update:
  *             for _i in range(idx.shape[0]):             # <<<<<<<<<<<<<<
  *                 if self.unchange_since_sample[idx[_i]]:
  *                     self.idx_vec.push_back(idx[_i])
  */
-    __Pyx_TraceLine(1534,0,__PYX_ERR(0, 1534, __pyx_L1_error))
+    __Pyx_TraceLine(1551,0,__PYX_ERR(0, 1551, __pyx_L1_error))
     __pyx_t_9 = (__pyx_v_idx.shape[0]);
     __pyx_t_10 = __pyx_t_9;
     for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
       __pyx_v__i = __pyx_t_11;
 
-      /* "cpprb/PyReplayBuffer.pyx":1535
+      /* "cpprb/PyReplayBuffer.pyx":1552
  *         if self.check_for_update:
  *             for _i in range(idx.shape[0]):
  *                 if self.unchange_since_sample[idx[_i]]:             # <<<<<<<<<<<<<<
  *                     self.idx_vec.push_back(idx[_i])
  *                     self.ps_vec.push_back(ps[_i])
  */
-      __Pyx_TraceLine(1535,0,__PYX_ERR(0, 1535, __pyx_L1_error))
-      if (unlikely(!__pyx_v_self->unchange_since_sample.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1535, __pyx_L1_error)}
+      __Pyx_TraceLine(1552,0,__PYX_ERR(0, 1552, __pyx_L1_error))
+      if (unlikely(!__pyx_v_self->unchange_since_sample.memview)) {PyErr_SetString(PyExc_AttributeError,"Memoryview is not initialized");__PYX_ERR(0, 1552, __pyx_L1_error)}
       __pyx_t_8 = __pyx_v__i;
       __pyx_t_7 = -1;
       if (__pyx_t_8 < 0) {
         __pyx_t_8 += __pyx_v_idx.shape[0];
         if (unlikely(__pyx_t_8 < 0)) __pyx_t_7 = 0;
       } else if (unlikely(__pyx_t_8 >= __pyx_v_idx.shape[0])) __pyx_t_7 = 0;
       if (unlikely(__pyx_t_7 != -1)) {
         __Pyx_RaiseBufferIndexError(__pyx_t_7);
-        __PYX_ERR(0, 1535, __pyx_L1_error)
+        __PYX_ERR(0, 1552, __pyx_L1_error)
       }
       __pyx_t_12 = (*((size_t const  *) ( /* dim=0 */ (__pyx_v_idx.data + __pyx_t_8 * __pyx_v_idx.strides[0]) )));
       __pyx_t_7 = -1;
       if (unlikely(__pyx_t_12 >= (size_t)__pyx_v_self->unchange_since_sample.shape[0])) __pyx_t_7 = 0;
       if (unlikely(__pyx_t_7 != -1)) {
         __Pyx_RaiseBufferIndexError(__pyx_t_7);
-        __PYX_ERR(0, 1535, __pyx_L1_error)
+        __PYX_ERR(0, 1552, __pyx_L1_error)
       }
       __pyx_t_2 = ((*((bool *) ( /* dim=0 */ (__pyx_v_self->unchange_since_sample.data + __pyx_t_12 * __pyx_v_self->unchange_since_sample.strides[0]) ))) != 0);
       if (__pyx_t_2) {
 
-        /* "cpprb/PyReplayBuffer.pyx":1536
+        /* "cpprb/PyReplayBuffer.pyx":1553
  *             for _i in range(idx.shape[0]):
  *                 if self.unchange_since_sample[idx[_i]]:
  *                     self.idx_vec.push_back(idx[_i])             # <<<<<<<<<<<<<<
  *                     self.ps_vec.push_back(ps[_i])
  * 
  */
-        __Pyx_TraceLine(1536,0,__PYX_ERR(0, 1536, __pyx_L1_error))
+        __Pyx_TraceLine(1553,0,__PYX_ERR(0, 1553, __pyx_L1_error))
         __pyx_t_8 = __pyx_v__i;
         __pyx_t_7 = -1;
         if (__pyx_t_8 < 0) {
           __pyx_t_8 += __pyx_v_idx.shape[0];
           if (unlikely(__pyx_t_8 < 0)) __pyx_t_7 = 0;
         } else if (unlikely(__pyx_t_8 >= __pyx_v_idx.shape[0])) __pyx_t_7 = 0;
         if (unlikely(__pyx_t_7 != -1)) {
           __Pyx_RaiseBufferIndexError(__pyx_t_7);
-          __PYX_ERR(0, 1536, __pyx_L1_error)
+          __PYX_ERR(0, 1553, __pyx_L1_error)
         }
         try {
           __pyx_v_self->idx_vec.push_back((*((size_t const  *) ( /* dim=0 */ (__pyx_v_idx.data + __pyx_t_8 * __pyx_v_idx.strides[0]) ))));
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 1536, __pyx_L1_error)
+          __PYX_ERR(0, 1553, __pyx_L1_error)
         }
 
-        /* "cpprb/PyReplayBuffer.pyx":1537
+        /* "cpprb/PyReplayBuffer.pyx":1554
  *                 if self.unchange_since_sample[idx[_i]]:
  *                     self.idx_vec.push_back(idx[_i])
  *                     self.ps_vec.push_back(ps[_i])             # <<<<<<<<<<<<<<
  * 
  *         cdef N = self.idx_vec.size()
  */
-        __Pyx_TraceLine(1537,0,__PYX_ERR(0, 1537, __pyx_L1_error))
+        __Pyx_TraceLine(1554,0,__PYX_ERR(0, 1554, __pyx_L1_error))
         __pyx_t_8 = __pyx_v__i;
         __pyx_t_7 = -1;
         if (__pyx_t_8 < 0) {
           __pyx_t_8 += __pyx_v_ps.shape[0];
           if (unlikely(__pyx_t_8 < 0)) __pyx_t_7 = 0;
         } else if (unlikely(__pyx_t_8 >= __pyx_v_ps.shape[0])) __pyx_t_7 = 0;
         if (unlikely(__pyx_t_7 != -1)) {
           __Pyx_RaiseBufferIndexError(__pyx_t_7);
-          __PYX_ERR(0, 1537, __pyx_L1_error)
+          __PYX_ERR(0, 1554, __pyx_L1_error)
         }
         try {
           __pyx_v_self->ps_vec.push_back((*((float const  *) ( /* dim=0 */ (__pyx_v_ps.data + __pyx_t_8 * __pyx_v_ps.strides[0]) ))));
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 1537, __pyx_L1_error)
+          __PYX_ERR(0, 1554, __pyx_L1_error)
         }
 
-        /* "cpprb/PyReplayBuffer.pyx":1535
+        /* "cpprb/PyReplayBuffer.pyx":1552
  *         if self.check_for_update:
  *             for _i in range(idx.shape[0]):
  *                 if self.unchange_since_sample[idx[_i]]:             # <<<<<<<<<<<<<<
  *                     self.idx_vec.push_back(idx[_i])
  *                     self.ps_vec.push_back(ps[_i])
  */
       }
     }
 
-    /* "cpprb/PyReplayBuffer.pyx":1533
+    /* "cpprb/PyReplayBuffer.pyx":1550
  *         self.ps_vec.reserve(ps.shape[0])
  * 
  *         if self.check_for_update:             # <<<<<<<<<<<<<<
  *             for _i in range(idx.shape[0]):
  *                 if self.unchange_since_sample[idx[_i]]:
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1539
+  /* "cpprb/PyReplayBuffer.pyx":1556
  *                     self.ps_vec.push_back(ps[_i])
  * 
  *         cdef N = self.idx_vec.size()             # <<<<<<<<<<<<<<
  *         if N > 0:
  *             self.per.update_priorities(self.idx_vec.data(),self.ps_vec.data(),N)
  */
-  __Pyx_TraceLine(1539,0,__PYX_ERR(0, 1539, __pyx_L1_error))
-  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_self->idx_vec.size()); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1539, __pyx_L1_error)
+  __Pyx_TraceLine(1556,0,__PYX_ERR(0, 1556, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_self->idx_vec.size()); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1556, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_N = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1540
+  /* "cpprb/PyReplayBuffer.pyx":1557
  * 
  *         cdef N = self.idx_vec.size()
  *         if N > 0:             # <<<<<<<<<<<<<<
  *             self.per.update_priorities(self.idx_vec.data(),self.ps_vec.data(),N)
  * 
  */
-  __Pyx_TraceLine(1540,0,__PYX_ERR(0, 1540, __pyx_L1_error))
-  __pyx_t_3 = PyObject_RichCompare(__pyx_v_N, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1540, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1540, __pyx_L1_error)
+  __Pyx_TraceLine(1557,0,__PYX_ERR(0, 1557, __pyx_L1_error))
+  __pyx_t_3 = PyObject_RichCompare(__pyx_v_N, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1557, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1557, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_2) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1541
+    /* "cpprb/PyReplayBuffer.pyx":1558
  *         cdef N = self.idx_vec.size()
  *         if N > 0:
  *             self.per.update_priorities(self.idx_vec.data(),self.ps_vec.data(),N)             # <<<<<<<<<<<<<<
  * 
  *     cpdef void clear(self) except *:
  */
-    __Pyx_TraceLine(1541,0,__PYX_ERR(0, 1541, __pyx_L1_error))
-    __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_v_N); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1541, __pyx_L1_error)
+    __Pyx_TraceLine(1558,0,__PYX_ERR(0, 1558, __pyx_L1_error))
+    __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_v_N); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1558, __pyx_L1_error)
     __pyx_v_self->per->update_priorities(__pyx_v_self->idx_vec.data(), __pyx_v_self->ps_vec.data(), __pyx_t_12);
 
-    /* "cpprb/PyReplayBuffer.pyx":1540
+    /* "cpprb/PyReplayBuffer.pyx":1557
  * 
  *         cdef N = self.idx_vec.size()
  *         if N > 0:             # <<<<<<<<<<<<<<
  *             self.per.update_priorities(self.idx_vec.data(),self.ps_vec.data(),N)
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1497
+  /* "cpprb/PyReplayBuffer.pyx":1514
  *         return samples
  * 
  *     def update_priorities(self,indexes,priorities):             # <<<<<<<<<<<<<<
  *         r"""Update priorities
  * 
  */
 
@@ -26318,15 +26524,15 @@
   __Pyx_XDECREF(__pyx_v_N);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1543
+/* "cpprb/PyReplayBuffer.pyx":1560
  *             self.per.update_priorities(self.idx_vec.data(),self.ps_vec.data(),N)
  * 
  *     cpdef void clear(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Clear replay buffer
  *         """
  */
 
@@ -26339,25 +26545,25 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear", 0);
-  __Pyx_TraceCall("clear", __pyx_f[0], 1543, 0, __PYX_ERR(0, 1543, __pyx_L1_error));
+  __Pyx_TraceCall("clear", __pyx_f[0], 1560, 0, __PYX_ERR(0, 1560, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1543, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1560, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_11clear)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -26365,15 +26571,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1543, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1560, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
@@ -26385,94 +26591,94 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1546
+  /* "cpprb/PyReplayBuffer.pyx":1563
  *         r"""Clear replay buffer
  *         """
  *         super(PrioritizedReplayBuffer,self).clear()             # <<<<<<<<<<<<<<
  *         clear(self.per)
  *         if self.use_nstep:
  */
-  __Pyx_TraceLine(1546,0,__PYX_ERR(0, 1546, __pyx_L1_error))
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1546, __pyx_L1_error)
+  __Pyx_TraceLine(1563,0,__PYX_ERR(0, 1563, __pyx_L1_error))
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1563, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer));
   PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer));
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)__pyx_v_self));
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1546, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1563, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1546, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1563, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1546, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1563, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1547
+  /* "cpprb/PyReplayBuffer.pyx":1564
  *         """
  *         super(PrioritizedReplayBuffer,self).clear()
  *         clear(self.per)             # <<<<<<<<<<<<<<
  *         if self.use_nstep:
  *             self.priorities_nstep.clear()
  */
-  __Pyx_TraceLine(1547,0,__PYX_ERR(0, 1547, __pyx_L1_error))
+  __Pyx_TraceLine(1564,0,__PYX_ERR(0, 1564, __pyx_L1_error))
   ymd::clear<ymd::CppPrioritizedSampler<float> >(__pyx_v_self->per);
 
-  /* "cpprb/PyReplayBuffer.pyx":1548
+  /* "cpprb/PyReplayBuffer.pyx":1565
  *         super(PrioritizedReplayBuffer,self).clear()
  *         clear(self.per)
  *         if self.use_nstep:             # <<<<<<<<<<<<<<
  *             self.priorities_nstep.clear()
  * 
  */
-  __Pyx_TraceLine(1548,0,__PYX_ERR(0, 1548, __pyx_L1_error))
+  __Pyx_TraceLine(1565,0,__PYX_ERR(0, 1565, __pyx_L1_error))
   __pyx_t_5 = (__pyx_v_self->__pyx_base.use_nstep != 0);
   if (__pyx_t_5) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1549
+    /* "cpprb/PyReplayBuffer.pyx":1566
  *         clear(self.per)
  *         if self.use_nstep:
  *             self.priorities_nstep.clear()             # <<<<<<<<<<<<<<
  * 
  *     cpdef float get_max_priority(self):
  */
-    __Pyx_TraceLine(1549,0,__PYX_ERR(0, 1549, __pyx_L1_error))
+    __Pyx_TraceLine(1566,0,__PYX_ERR(0, 1566, __pyx_L1_error))
     ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_NstepBuffer *)__pyx_v_self->priorities_nstep->__pyx_vtab)->clear(__pyx_v_self->priorities_nstep, 0);
 
-    /* "cpprb/PyReplayBuffer.pyx":1548
+    /* "cpprb/PyReplayBuffer.pyx":1565
  *         super(PrioritizedReplayBuffer,self).clear()
  *         clear(self.per)
  *         if self.use_nstep:             # <<<<<<<<<<<<<<
  *             self.priorities_nstep.clear()
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1543
+  /* "cpprb/PyReplayBuffer.pyx":1560
  *             self.per.update_priorities(self.idx_vec.data(),self.ps_vec.data(),N)
  * 
  *     cpdef void clear(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Clear replay buffer
  *         """
  */
 
@@ -26508,18 +26714,18 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear", 0);
-  __Pyx_TraceCall("clear (wrapper)", __pyx_f[0], 1543, 0, __PYX_ERR(0, 1543, __pyx_L1_error));
+  __Pyx_TraceCall("clear (wrapper)", __pyx_f[0], 1560, 0, __PYX_ERR(0, 1560, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_f_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_clear(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1543, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1543, __pyx_L1_error)
+  __pyx_f_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_clear(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1560, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -26529,15 +26735,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1551
+/* "cpprb/PyReplayBuffer.pyx":1568
  *             self.priorities_nstep.clear()
  * 
  *     cpdef float get_max_priority(self):             # <<<<<<<<<<<<<<
  *         r"""Get the max priority of stored priorities
  * 
  */
 
@@ -26551,25 +26757,25 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   float __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_max_priority", 0);
-  __Pyx_TraceCall("get_max_priority", __pyx_f[0], 1551, 0, __PYX_ERR(0, 1551, __pyx_L1_error));
+  __Pyx_TraceCall("get_max_priority", __pyx_f[0], 1568, 0, __PYX_ERR(0, 1568, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_max_priority); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1551, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_max_priority); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1568, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_13get_max_priority)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -26577,18 +26783,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1551, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1568, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __pyx_PyFloat_AsFloat(__pyx_t_2); if (unlikely((__pyx_t_5 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1551, __pyx_L1_error)
+        __pyx_t_5 = __pyx_PyFloat_AsFloat(__pyx_t_2); if (unlikely((__pyx_t_5 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1568, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -26599,26 +26805,26 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1559
+  /* "cpprb/PyReplayBuffer.pyx":1576
  *             the max priority of stored priorities
  *         """
  *         return self.per.get_max_priority()             # <<<<<<<<<<<<<<
  * 
  *     cpdef void on_episode_end(self) except *:
  */
-  __Pyx_TraceLine(1559,0,__PYX_ERR(0, 1559, __pyx_L1_error))
+  __Pyx_TraceLine(1576,0,__PYX_ERR(0, 1576, __pyx_L1_error))
   __pyx_r = __pyx_v_self->per->get_max_priority();
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1551
+  /* "cpprb/PyReplayBuffer.pyx":1568
  *             self.priorities_nstep.clear()
  * 
  *     cpdef float get_max_priority(self):             # <<<<<<<<<<<<<<
  *         r"""Get the max priority of stored priorities
  * 
  */
 
@@ -26655,17 +26861,17 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_max_priority", 0);
-  __Pyx_TraceCall("get_max_priority (wrapper)", __pyx_f[0], 1551, 0, __PYX_ERR(0, 1551, __pyx_L1_error));
+  __Pyx_TraceCall("get_max_priority (wrapper)", __pyx_f[0], 1568, 0, __PYX_ERR(0, 1568, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_get_max_priority(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1551, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_get_max_priority(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -26675,15 +26881,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1561
+/* "cpprb/PyReplayBuffer.pyx":1578
  *         return self.per.get_max_priority()
  * 
  *     cpdef void on_episode_end(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Call on episode end
  * 
  */
 
@@ -26696,25 +26902,25 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_episode_end", 0);
-  __Pyx_TraceCall("on_episode_end", __pyx_f[0], 1561, 0, __PYX_ERR(0, 1561, __pyx_L1_error));
+  __Pyx_TraceCall("on_episode_end", __pyx_f[0], 1578, 0, __PYX_ERR(0, 1578, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_episode_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1561, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_episode_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1578, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_15on_episode_end)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -26722,15 +26928,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1561, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1578, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
@@ -26742,134 +26948,134 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1574
+  /* "cpprb/PyReplayBuffer.pyx":1591
  *         even though any `done` flags from environment is not set.
  *         """
  *         if self.use_nstep:             # <<<<<<<<<<<<<<
  *             self.use_nstep = False
  *             self.add(**self.nstep.on_episode_end(),
  */
-  __Pyx_TraceLine(1574,0,__PYX_ERR(0, 1574, __pyx_L1_error))
+  __Pyx_TraceLine(1591,0,__PYX_ERR(0, 1591, __pyx_L1_error))
   __pyx_t_5 = (__pyx_v_self->__pyx_base.use_nstep != 0);
   if (__pyx_t_5) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1575
+    /* "cpprb/PyReplayBuffer.pyx":1592
  *         """
  *         if self.use_nstep:
  *             self.use_nstep = False             # <<<<<<<<<<<<<<
  *             self.add(**self.nstep.on_episode_end(),
  *                      priorities=self.priorities_nstep.on_episode_end()["priorities"])
  */
-    __Pyx_TraceLine(1575,0,__PYX_ERR(0, 1575, __pyx_L1_error))
+    __Pyx_TraceLine(1592,0,__PYX_ERR(0, 1592, __pyx_L1_error))
     __pyx_v_self->__pyx_base.use_nstep = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1576
+    /* "cpprb/PyReplayBuffer.pyx":1593
  *         if self.use_nstep:
  *             self.use_nstep = False
  *             self.add(**self.nstep.on_episode_end(),             # <<<<<<<<<<<<<<
  *                      priorities=self.priorities_nstep.on_episode_end()["priorities"])
  *             self.use_nstep = True
  */
-    __Pyx_TraceLine(1576,0,__PYX_ERR(0, 1576, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1576, __pyx_L1_error)
+    __Pyx_TraceLine(1593,0,__PYX_ERR(0, 1593, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1593, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_NstepBuffer *)__pyx_v_self->__pyx_base.nstep->__pyx_vtab)->on_episode_end(__pyx_v_self->__pyx_base.nstep, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1576, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_NstepBuffer *)__pyx_v_self->__pyx_base.nstep->__pyx_vtab)->on_episode_end(__pyx_v_self->__pyx_base.nstep, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1593, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (unlikely(__pyx_t_3 == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-      __PYX_ERR(0, 1576, __pyx_L1_error)
+      __PYX_ERR(0, 1593, __pyx_L1_error)
     }
     if (likely(PyDict_CheckExact(__pyx_t_3))) {
-      __pyx_t_2 = PyDict_Copy(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1576, __pyx_L1_error)
+      __pyx_t_2 = PyDict_Copy(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1593, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else {
-      __pyx_t_2 = PyObject_CallFunctionObjArgs((PyObject*)&PyDict_Type, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1576, __pyx_L1_error)
+      __pyx_t_2 = PyObject_CallFunctionObjArgs((PyObject*)&PyDict_Type, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1593, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
 
-    /* "cpprb/PyReplayBuffer.pyx":1577
+    /* "cpprb/PyReplayBuffer.pyx":1594
  *             self.use_nstep = False
  *             self.add(**self.nstep.on_episode_end(),
  *                      priorities=self.priorities_nstep.on_episode_end()["priorities"])             # <<<<<<<<<<<<<<
  *             self.use_nstep = True
  * 
  */
-    __Pyx_TraceLine(1577,0,__PYX_ERR(0, 1577, __pyx_L1_error))
-    __pyx_t_3 = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_NstepBuffer *)__pyx_v_self->priorities_nstep->__pyx_vtab)->on_episode_end(__pyx_v_self->priorities_nstep, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1577, __pyx_L1_error)
+    __Pyx_TraceLine(1594,0,__PYX_ERR(0, 1594, __pyx_L1_error))
+    __pyx_t_3 = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_NstepBuffer *)__pyx_v_self->priorities_nstep->__pyx_vtab)->on_episode_end(__pyx_v_self->priorities_nstep, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1594, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_priorities); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1577, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_priorities); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1594, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(PyDict_Contains(__pyx_t_2, __pyx_n_s_priorities))) {
-      __Pyx_RaiseDoubleKeywordsError("function", __pyx_n_s_priorities); __PYX_ERR(0, 1576, __pyx_L1_error)
+      __Pyx_RaiseDoubleKeywordsError("function", __pyx_n_s_priorities); __PYX_ERR(0, 1593, __pyx_L1_error)
     }
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_priorities, __pyx_t_4) < 0) __PYX_ERR(0, 1577, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_priorities, __pyx_t_4) < 0) __PYX_ERR(0, 1594, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1576
+    /* "cpprb/PyReplayBuffer.pyx":1593
  *         if self.use_nstep:
  *             self.use_nstep = False
  *             self.add(**self.nstep.on_episode_end(),             # <<<<<<<<<<<<<<
  *                      priorities=self.priorities_nstep.on_episode_end()["priorities"])
  *             self.use_nstep = True
  */
-    __Pyx_TraceLine(1576,0,__PYX_ERR(0, 1576, __pyx_L1_error))
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1576, __pyx_L1_error)
+    __Pyx_TraceLine(1593,0,__PYX_ERR(0, 1593, __pyx_L1_error))
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1593, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1578
+    /* "cpprb/PyReplayBuffer.pyx":1595
  *             self.add(**self.nstep.on_episode_end(),
  *                      priorities=self.priorities_nstep.on_episode_end()["priorities"])
  *             self.use_nstep = True             # <<<<<<<<<<<<<<
  * 
  *         self.add_cache()
  */
-    __Pyx_TraceLine(1578,0,__PYX_ERR(0, 1578, __pyx_L1_error))
+    __Pyx_TraceLine(1595,0,__PYX_ERR(0, 1595, __pyx_L1_error))
     __pyx_v_self->__pyx_base.use_nstep = 1;
 
-    /* "cpprb/PyReplayBuffer.pyx":1574
+    /* "cpprb/PyReplayBuffer.pyx":1591
  *         even though any `done` flags from environment is not set.
  *         """
  *         if self.use_nstep:             # <<<<<<<<<<<<<<
  *             self.use_nstep = False
  *             self.add(**self.nstep.on_episode_end(),
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1580
+  /* "cpprb/PyReplayBuffer.pyx":1597
  *             self.use_nstep = True
  * 
  *         self.add_cache()             # <<<<<<<<<<<<<<
  * 
  *         self.episode_len = 0
  */
-  __Pyx_TraceLine(1580,0,__PYX_ERR(0, 1580, __pyx_L1_error))
+  __Pyx_TraceLine(1597,0,__PYX_ERR(0, 1597, __pyx_L1_error))
   ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.add_cache(((struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_self));
 
-  /* "cpprb/PyReplayBuffer.pyx":1582
+  /* "cpprb/PyReplayBuffer.pyx":1599
  *         self.add_cache()
  * 
  *         self.episode_len = 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1582,0,__PYX_ERR(0, 1582, __pyx_L1_error))
+  __Pyx_TraceLine(1599,0,__PYX_ERR(0, 1599, __pyx_L1_error))
   __pyx_v_self->__pyx_base.episode_len = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1561
+  /* "cpprb/PyReplayBuffer.pyx":1578
  *         return self.per.get_max_priority()
  * 
  *     cpdef void on_episode_end(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Call on episode end
  * 
  */
 
@@ -26905,18 +27111,18 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_episode_end", 0);
-  __Pyx_TraceCall("on_episode_end (wrapper)", __pyx_f[0], 1561, 0, __PYX_ERR(0, 1561, __pyx_L1_error));
+  __Pyx_TraceCall("on_episode_end (wrapper)", __pyx_f[0], 1578, 0, __PYX_ERR(0, 1578, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_f_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_on_episode_end(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1561, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1561, __pyx_L1_error)
+  __pyx_f_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_on_episode_end(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1578, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1578, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -27049,15 +27255,15 @@
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1622
+/* "cpprb/PyReplayBuffer.pyx":1639
  *     cdef learner_ready
  * 
  *     def __init__(self,size,env_dict=None,*,default_dtype=None,logger=None,**kwargs):             # <<<<<<<<<<<<<<
  *         r"""Initialize ReplayBuffer
  * 
  */
 
@@ -27114,15 +27320,15 @@
         Py_ssize_t index;
         for (index = 2; index < 4 && kw_args > 0; index++) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1622, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1639, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -27132,15 +27338,15 @@
     __pyx_v_size = values[0];
     __pyx_v_env_dict = values[1];
     __pyx_v_default_dtype = values[2];
     __pyx_v_logger = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1622, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1639, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPReplayBuffer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_14MPReplayBuffer___init__(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self), __pyx_v_size, __pyx_v_env_dict, __pyx_v_default_dtype, __pyx_v_logger, __pyx_v_kwargs);
@@ -27164,346 +27370,346 @@
   size_t __pyx_t_6;
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
-  __Pyx_TraceCall("__init__", __pyx_f[0], 1622, 0, __PYX_ERR(0, 1622, __pyx_L1_error));
+  __Pyx_TraceCall("__init__", __pyx_f[0], 1639, 0, __PYX_ERR(0, 1639, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1636
+  /* "cpprb/PyReplayBuffer.pyx":1653
  *             fallback dtype for not specified in `env_dict`. default is numpy.single
  *         """
  *         self.env_dict = env_dict.copy() if env_dict else {}             # <<<<<<<<<<<<<<
  *         cdef special_keys = []
  * 
  */
-  __Pyx_TraceLine(1636,0,__PYX_ERR(0, 1636, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_env_dict); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1636, __pyx_L1_error)
+  __Pyx_TraceLine(1653,0,__PYX_ERR(0, 1653, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_env_dict); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1653, __pyx_L1_error)
   if (__pyx_t_2) {
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_env_dict, __pyx_n_s_copy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1636, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_env_dict, __pyx_n_s_copy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1653, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1636, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1653, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1636, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1653, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   }
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->env_dict);
   __Pyx_DECREF(__pyx_v_self->env_dict);
   __pyx_v_self->env_dict = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1637
+  /* "cpprb/PyReplayBuffer.pyx":1654
  *         """
  *         self.env_dict = env_dict.copy() if env_dict else {}
  *         cdef special_keys = []             # <<<<<<<<<<<<<<
  * 
  *         self.buffer_size = size
  */
-  __Pyx_TraceLine(1637,0,__PYX_ERR(0, 1637, __pyx_L1_error))
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1637, __pyx_L1_error)
+  __Pyx_TraceLine(1654,0,__PYX_ERR(0, 1654, __pyx_L1_error))
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_special_keys = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1639
+  /* "cpprb/PyReplayBuffer.pyx":1656
  *         cdef special_keys = []
  * 
  *         self.buffer_size = size             # <<<<<<<<<<<<<<
  *         self.index = ProcessSafeRingBufferIndex(self.buffer_size)
  * 
  */
-  __Pyx_TraceLine(1639,0,__PYX_ERR(0, 1639, __pyx_L1_error))
-  __pyx_t_6 = __Pyx_PyInt_As_size_t(__pyx_v_size); if (unlikely((__pyx_t_6 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1639, __pyx_L1_error)
+  __Pyx_TraceLine(1656,0,__PYX_ERR(0, 1656, __pyx_L1_error))
+  __pyx_t_6 = __Pyx_PyInt_As_size_t(__pyx_v_size); if (unlikely((__pyx_t_6 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1656, __pyx_L1_error)
   __pyx_v_self->buffer_size = __pyx_t_6;
 
-  /* "cpprb/PyReplayBuffer.pyx":1640
+  /* "cpprb/PyReplayBuffer.pyx":1657
  * 
  *         self.buffer_size = size
  *         self.index = ProcessSafeRingBufferIndex(self.buffer_size)             # <<<<<<<<<<<<<<
  * 
  *         self.default_dtype = default_dtype or np.single
  */
-  __Pyx_TraceLine(1640,0,__PYX_ERR(0, 1640, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_self->buffer_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1640, __pyx_L1_error)
+  __Pyx_TraceLine(1657,0,__PYX_ERR(0, 1657, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_self->buffer_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1657, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_ProcessSafeRingBufferIndex), __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1640, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_ProcessSafeRingBufferIndex), __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1657, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->index);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->index));
   __pyx_v_self->index = ((struct __pyx_obj_5cpprb_14PyReplayBuffer_ProcessSafeRingBufferIndex *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1642
+  /* "cpprb/PyReplayBuffer.pyx":1659
  *         self.index = ProcessSafeRingBufferIndex(self.buffer_size)
  * 
  *         self.default_dtype = default_dtype or np.single             # <<<<<<<<<<<<<<
  * 
  *         # side effect: Add "add_shape" key into self.env_dict
  */
-  __Pyx_TraceLine(1642,0,__PYX_ERR(0, 1642, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_default_dtype); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1642, __pyx_L1_error)
+  __Pyx_TraceLine(1659,0,__PYX_ERR(0, 1659, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_default_dtype); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 1659, __pyx_L1_error)
   if (!__pyx_t_2) {
   } else {
     __Pyx_INCREF(__pyx_v_default_dtype);
     __pyx_t_3 = __pyx_v_default_dtype;
     goto __pyx_L3_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1642, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1659, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_single); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1642, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_single); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1659, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_INCREF(__pyx_t_4);
   __pyx_t_3 = __pyx_t_4;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_L3_bool_binop_done:;
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->default_dtype);
   __Pyx_DECREF(__pyx_v_self->default_dtype);
   __pyx_v_self->default_dtype = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1645
+  /* "cpprb/PyReplayBuffer.pyx":1662
  * 
  *         # side effect: Add "add_shape" key into self.env_dict
  *         self.buffer = dict2buffer(self.buffer_size,self.env_dict,             # <<<<<<<<<<<<<<
  *                                   default_dtype = self.default_dtype,
  *                                   shared = True)
  */
-  __Pyx_TraceLine(1645,0,__PYX_ERR(0, 1645, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_dict2buffer); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1645, __pyx_L1_error)
+  __Pyx_TraceLine(1662,0,__PYX_ERR(0, 1662, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_dict2buffer); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1662, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_self->buffer_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1645, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_self->buffer_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1662, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1645, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1662, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
   __Pyx_INCREF(__pyx_v_self->env_dict);
   __Pyx_GIVEREF(__pyx_v_self->env_dict);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_self->env_dict);
   __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1646
+  /* "cpprb/PyReplayBuffer.pyx":1663
  *         # side effect: Add "add_shape" key into self.env_dict
  *         self.buffer = dict2buffer(self.buffer_size,self.env_dict,
  *                                   default_dtype = self.default_dtype,             # <<<<<<<<<<<<<<
  *                                   shared = True)
  * 
  */
-  __Pyx_TraceLine(1646,0,__PYX_ERR(0, 1646, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1646, __pyx_L1_error)
+  __Pyx_TraceLine(1663,0,__PYX_ERR(0, 1663, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_default_dtype, __pyx_v_self->default_dtype) < 0) __PYX_ERR(0, 1646, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_default_dtype, __pyx_v_self->default_dtype) < 0) __PYX_ERR(0, 1663, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":1647
+  /* "cpprb/PyReplayBuffer.pyx":1664
  *         self.buffer = dict2buffer(self.buffer_size,self.env_dict,
  *                                   default_dtype = self.default_dtype,
  *                                   shared = True)             # <<<<<<<<<<<<<<
  * 
  *         self.size_check = StepChecker(self.env_dict,special_keys)
  */
-  __Pyx_TraceLine(1647,0,__PYX_ERR(0, 1647, __pyx_L1_error))
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_shared, Py_True) < 0) __PYX_ERR(0, 1646, __pyx_L1_error)
+  __Pyx_TraceLine(1664,0,__PYX_ERR(0, 1664, __pyx_L1_error))
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_shared, Py_True) < 0) __PYX_ERR(0, 1663, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":1645
+  /* "cpprb/PyReplayBuffer.pyx":1662
  * 
  *         # side effect: Add "add_shape" key into self.env_dict
  *         self.buffer = dict2buffer(self.buffer_size,self.env_dict,             # <<<<<<<<<<<<<<
  *                                   default_dtype = self.default_dtype,
  *                                   shared = True)
  */
-  __Pyx_TraceLine(1645,0,__PYX_ERR(0, 1645, __pyx_L1_error))
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1645, __pyx_L1_error)
+  __Pyx_TraceLine(1662,0,__PYX_ERR(0, 1662, __pyx_L1_error))
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1662, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_GIVEREF(__pyx_t_5);
   __Pyx_GOTREF(__pyx_v_self->buffer);
   __Pyx_DECREF(__pyx_v_self->buffer);
   __pyx_v_self->buffer = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1649
+  /* "cpprb/PyReplayBuffer.pyx":1666
  *                                   shared = True)
  * 
  *         self.size_check = StepChecker(self.env_dict,special_keys)             # <<<<<<<<<<<<<<
  * 
  *         self.learner_ready = Event()
  */
-  __Pyx_TraceLine(1649,0,__PYX_ERR(0, 1649, __pyx_L1_error))
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1649, __pyx_L1_error)
+  __Pyx_TraceLine(1666,0,__PYX_ERR(0, 1666, __pyx_L1_error))
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1666, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_self->env_dict);
   __Pyx_GIVEREF(__pyx_v_self->env_dict);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_self->env_dict);
   __Pyx_INCREF(__pyx_v_special_keys);
   __Pyx_GIVEREF(__pyx_v_special_keys);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_special_keys);
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_StepChecker), __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1649, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_StepChecker), __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1666, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_GIVEREF(__pyx_t_4);
   __Pyx_GOTREF(__pyx_v_self->size_check);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->size_check));
   __pyx_v_self->size_check = ((struct __pyx_obj_5cpprb_14PyReplayBuffer_StepChecker *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1651
+  /* "cpprb/PyReplayBuffer.pyx":1668
  *         self.size_check = StepChecker(self.env_dict,special_keys)
  * 
  *         self.learner_ready = Event()             # <<<<<<<<<<<<<<
  *         self.learner_ready.clear()
  *         self.explorer_ready = Event()
  */
-  __Pyx_TraceLine(1651,0,__PYX_ERR(0, 1651, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Event); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1651, __pyx_L1_error)
+  __Pyx_TraceLine(1668,0,__PYX_ERR(0, 1668, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Event); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1668, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1651, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1668, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_GIVEREF(__pyx_t_4);
   __Pyx_GOTREF(__pyx_v_self->learner_ready);
   __Pyx_DECREF(__pyx_v_self->learner_ready);
   __pyx_v_self->learner_ready = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1652
+  /* "cpprb/PyReplayBuffer.pyx":1669
  * 
  *         self.learner_ready = Event()
  *         self.learner_ready.clear()             # <<<<<<<<<<<<<<
  *         self.explorer_ready = Event()
  *         self.explorer_ready.set()
  */
-  __Pyx_TraceLine(1652,0,__PYX_ERR(0, 1652, __pyx_L1_error))
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_ready, __pyx_n_s_clear); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1652, __pyx_L1_error)
+  __Pyx_TraceLine(1669,0,__PYX_ERR(0, 1669, __pyx_L1_error))
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_ready, __pyx_n_s_clear); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1669, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1652, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1669, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1653
+  /* "cpprb/PyReplayBuffer.pyx":1670
  *         self.learner_ready = Event()
  *         self.learner_ready.clear()
  *         self.explorer_ready = Event()             # <<<<<<<<<<<<<<
  *         self.explorer_ready.set()
  * 
  */
-  __Pyx_TraceLine(1653,0,__PYX_ERR(0, 1653, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Event); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1653, __pyx_L1_error)
+  __Pyx_TraceLine(1670,0,__PYX_ERR(0, 1670, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Event); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1670, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1653, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1670, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_GIVEREF(__pyx_t_4);
   __Pyx_GOTREF(__pyx_v_self->explorer_ready);
   __Pyx_DECREF(__pyx_v_self->explorer_ready);
   __pyx_v_self->explorer_ready = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1654
+  /* "cpprb/PyReplayBuffer.pyx":1671
  *         self.learner_ready.clear()
  *         self.explorer_ready = Event()
  *         self.explorer_ready.set()             # <<<<<<<<<<<<<<
  * 
  *         self.explorer_count = Value(ctypes.c_size_t,0)
  */
-  __Pyx_TraceLine(1654,0,__PYX_ERR(0, 1654, __pyx_L1_error))
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_ready, __pyx_n_s_set); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1654, __pyx_L1_error)
+  __Pyx_TraceLine(1671,0,__PYX_ERR(0, 1671, __pyx_L1_error))
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_ready, __pyx_n_s_set); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1671, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1654, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1671, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1656
+  /* "cpprb/PyReplayBuffer.pyx":1673
  *         self.explorer_ready.set()
  * 
  *         self.explorer_count = Value(ctypes.c_size_t,0)             # <<<<<<<<<<<<<<
  * 
  *     cdef void _lock_explorer(self) except *:
  */
-  __Pyx_TraceLine(1656,0,__PYX_ERR(0, 1656, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Value); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1656, __pyx_L1_error)
+  __Pyx_TraceLine(1673,0,__PYX_ERR(0, 1673, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Value); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1673, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1656, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1673, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_c_size_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1656, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_c_size_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1673, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_1)) {
@@ -27513,53 +27719,53 @@
       __Pyx_DECREF_SET(__pyx_t_5, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_t_3, __pyx_int_0};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1656, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1673, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_t_3, __pyx_int_0};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1656, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1673, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1656, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1673, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_1) {
       __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1); __pyx_t_1 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_int_0);
     __pyx_t_3 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1656, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1673, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_GIVEREF(__pyx_t_4);
   __Pyx_GOTREF(__pyx_v_self->explorer_count);
   __Pyx_DECREF(__pyx_v_self->explorer_count);
   __pyx_v_self->explorer_count = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1622
+  /* "cpprb/PyReplayBuffer.pyx":1639
  *     cdef learner_ready
  * 
  *     def __init__(self,size,env_dict=None,*,default_dtype=None,logger=None,**kwargs):             # <<<<<<<<<<<<<<
  *         r"""Initialize ReplayBuffer
  * 
  */
 
@@ -27577,15 +27783,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_special_keys);
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1658
+/* "cpprb/PyReplayBuffer.pyx":1675
  *         self.explorer_count = Value(ctypes.c_size_t,0)
  * 
  *     cdef void _lock_explorer(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_ready.wait() # Wait permission
  *         self.learner_ready.clear()  # Block learner
  */
 
@@ -27603,147 +27809,147 @@
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_lock_explorer", 0);
-  __Pyx_TraceCall("_lock_explorer", __pyx_f[0], 1658, 0, __PYX_ERR(0, 1658, __pyx_L1_error));
+  __Pyx_TraceCall("_lock_explorer", __pyx_f[0], 1675, 0, __PYX_ERR(0, 1675, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1659
+  /* "cpprb/PyReplayBuffer.pyx":1676
  * 
  *     cdef void _lock_explorer(self) except *:
  *         self.explorer_ready.wait() # Wait permission             # <<<<<<<<<<<<<<
  *         self.learner_ready.clear()  # Block learner
  *         with self.explorer_count.get_lock():
  */
-  __Pyx_TraceLine(1659,0,__PYX_ERR(0, 1659, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_ready, __pyx_n_s_wait); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1659, __pyx_L1_error)
+  __Pyx_TraceLine(1676,0,__PYX_ERR(0, 1676, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_ready, __pyx_n_s_wait); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1676, __pyx_L1_error)
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1659, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1676, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1660
+  /* "cpprb/PyReplayBuffer.pyx":1677
  *     cdef void _lock_explorer(self) except *:
  *         self.explorer_ready.wait() # Wait permission
  *         self.learner_ready.clear()  # Block learner             # <<<<<<<<<<<<<<
  *         with self.explorer_count.get_lock():
  *             self.explorer_count.value += 1
  */
-  __Pyx_TraceLine(1660,0,__PYX_ERR(0, 1660, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_ready, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1660, __pyx_L1_error)
+  __Pyx_TraceLine(1677,0,__PYX_ERR(0, 1677, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_ready, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1677, __pyx_L1_error)
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1660, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1677, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1661
+  /* "cpprb/PyReplayBuffer.pyx":1678
  *         self.explorer_ready.wait() # Wait permission
  *         self.learner_ready.clear()  # Block learner
  *         with self.explorer_count.get_lock():             # <<<<<<<<<<<<<<
  *             self.explorer_count.value += 1
  * 
  */
-  __Pyx_TraceLine(1661,0,__PYX_ERR(0, 1661, __pyx_L1_error))
+  __Pyx_TraceLine(1678,0,__PYX_ERR(0, 1678, __pyx_L1_error))
   /*with:*/ {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_count, __pyx_n_s_get_lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1661, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_count, __pyx_n_s_get_lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1678, __pyx_L1_error)
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
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1661, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1678, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1661, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1678, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1661, __pyx_L3_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1678, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1661, __pyx_L3_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1678, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     /*try:*/ {
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
 
-          /* "cpprb/PyReplayBuffer.pyx":1662
+          /* "cpprb/PyReplayBuffer.pyx":1679
  *         self.learner_ready.clear()  # Block learner
  *         with self.explorer_count.get_lock():
  *             self.explorer_count.value += 1             # <<<<<<<<<<<<<<
  * 
  *     cdef void _unlock_explorer(self) except *:
  */
-          __Pyx_TraceLine(1662,0,__PYX_ERR(0, 1662, __pyx_L7_error))
+          __Pyx_TraceLine(1679,0,__PYX_ERR(0, 1679, __pyx_L7_error))
           __Pyx_INCREF(__pyx_v_self->explorer_count);
           __pyx_t_1 = __pyx_v_self->explorer_count;
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1662, __pyx_L7_error)
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1679, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1662, __pyx_L7_error)
+          __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1679, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_value, __pyx_t_3) < 0) __PYX_ERR(0, 1662, __pyx_L7_error)
+          if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_value, __pyx_t_3) < 0) __PYX_ERR(0, 1679, __pyx_L7_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-          /* "cpprb/PyReplayBuffer.pyx":1661
+          /* "cpprb/PyReplayBuffer.pyx":1678
  *         self.explorer_ready.wait() # Wait permission
  *         self.learner_ready.clear()  # Block learner
  *         with self.explorer_count.get_lock():             # <<<<<<<<<<<<<<
  *             self.explorer_count.value += 1
  * 
  */
         }
@@ -27754,36 +27960,36 @@
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPReplayBuffer._lock_explorer", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 1661, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 1678, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1661, __pyx_L9_except_error)
+          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1678, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1661, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1678, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_9);
           __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-          if (__pyx_t_10 < 0) __PYX_ERR(0, 1661, __pyx_L9_except_error)
+          if (__pyx_t_10 < 0) __PYX_ERR(0, 1678, __pyx_L9_except_error)
           __pyx_t_11 = ((!(__pyx_t_10 != 0)) != 0);
           if (__pyx_t_11) {
             __Pyx_GIVEREF(__pyx_t_1);
             __Pyx_GIVEREF(__pyx_t_3);
             __Pyx_XGIVEREF(__pyx_t_2);
             __Pyx_ErrRestoreWithState(__pyx_t_1, __pyx_t_3, __pyx_t_2);
             __pyx_t_1 = 0; __pyx_t_3 = 0; __pyx_t_2 = 0; 
-            __PYX_ERR(0, 1661, __pyx_L9_except_error)
+            __PYX_ERR(0, 1678, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -27801,30 +28007,30 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_4) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__21, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1661, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1678, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L16;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L1_error;
     __pyx_L16:;
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1658
+  /* "cpprb/PyReplayBuffer.pyx":1675
  *         self.explorer_count = Value(ctypes.c_size_t,0)
  * 
  *     cdef void _lock_explorer(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_ready.wait() # Wait permission
  *         self.learner_ready.clear()  # Block learner
  */
 
@@ -27837,15 +28043,15 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPReplayBuffer._lock_explorer", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1664
+/* "cpprb/PyReplayBuffer.pyx":1681
  *             self.explorer_count.value += 1
  * 
  *     cdef void _unlock_explorer(self) except *:             # <<<<<<<<<<<<<<
  *         with self.explorer_count.get_lock():
  *             self.explorer_count.value -= 1
  */
 
@@ -27863,93 +28069,93 @@
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_unlock_explorer", 0);
-  __Pyx_TraceCall("_unlock_explorer", __pyx_f[0], 1664, 0, __PYX_ERR(0, 1664, __pyx_L1_error));
+  __Pyx_TraceCall("_unlock_explorer", __pyx_f[0], 1681, 0, __PYX_ERR(0, 1681, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1665
+  /* "cpprb/PyReplayBuffer.pyx":1682
  * 
  *     cdef void _unlock_explorer(self) except *:
  *         with self.explorer_count.get_lock():             # <<<<<<<<<<<<<<
  *             self.explorer_count.value -= 1
  *         if self.explorer_count.value == 0:
  */
-  __Pyx_TraceLine(1665,0,__PYX_ERR(0, 1665, __pyx_L1_error))
+  __Pyx_TraceLine(1682,0,__PYX_ERR(0, 1682, __pyx_L1_error))
   /*with:*/ {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_count, __pyx_n_s_get_lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1665, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_count, __pyx_n_s_get_lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1682, __pyx_L1_error)
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
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1665, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1682, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1665, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1682, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1665, __pyx_L3_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1682, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1665, __pyx_L3_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1682, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     /*try:*/ {
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
 
-          /* "cpprb/PyReplayBuffer.pyx":1666
+          /* "cpprb/PyReplayBuffer.pyx":1683
  *     cdef void _unlock_explorer(self) except *:
  *         with self.explorer_count.get_lock():
  *             self.explorer_count.value -= 1             # <<<<<<<<<<<<<<
  *         if self.explorer_count.value == 0:
  *             self.learner_ready.set()
  */
-          __Pyx_TraceLine(1666,0,__PYX_ERR(0, 1666, __pyx_L7_error))
+          __Pyx_TraceLine(1683,0,__PYX_ERR(0, 1683, __pyx_L7_error))
           __Pyx_INCREF(__pyx_v_self->explorer_count);
           __pyx_t_1 = __pyx_v_self->explorer_count;
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1666, __pyx_L7_error)
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1683, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_t_2, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1666, __pyx_L7_error)
+          __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_t_2, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1683, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_value, __pyx_t_3) < 0) __PYX_ERR(0, 1666, __pyx_L7_error)
+          if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_value, __pyx_t_3) < 0) __PYX_ERR(0, 1683, __pyx_L7_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-          /* "cpprb/PyReplayBuffer.pyx":1665
+          /* "cpprb/PyReplayBuffer.pyx":1682
  * 
  *     cdef void _unlock_explorer(self) except *:
  *         with self.explorer_count.get_lock():             # <<<<<<<<<<<<<<
  *             self.explorer_count.value -= 1
  *         if self.explorer_count.value == 0:
  */
         }
@@ -27960,36 +28166,36 @@
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPReplayBuffer._unlock_explorer", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 1665, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 1682, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1665, __pyx_L9_except_error)
+          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1682, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1665, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1682, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_9);
           __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-          if (__pyx_t_10 < 0) __PYX_ERR(0, 1665, __pyx_L9_except_error)
+          if (__pyx_t_10 < 0) __PYX_ERR(0, 1682, __pyx_L9_except_error)
           __pyx_t_11 = ((!(__pyx_t_10 != 0)) != 0);
           if (__pyx_t_11) {
             __Pyx_GIVEREF(__pyx_t_1);
             __Pyx_GIVEREF(__pyx_t_3);
             __Pyx_XGIVEREF(__pyx_t_2);
             __Pyx_ErrRestoreWithState(__pyx_t_1, __pyx_t_3, __pyx_t_2);
             __pyx_t_1 = 0; __pyx_t_3 = 0; __pyx_t_2 = 0; 
-            __PYX_ERR(0, 1665, __pyx_L9_except_error)
+            __PYX_ERR(0, 1682, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -28007,83 +28213,83 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_4) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__21, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1665, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1682, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L16;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L1_error;
     __pyx_L16:;
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1667
+  /* "cpprb/PyReplayBuffer.pyx":1684
  *         with self.explorer_count.get_lock():
  *             self.explorer_count.value -= 1
  *         if self.explorer_count.value == 0:             # <<<<<<<<<<<<<<
  *             self.learner_ready.set()
  * 
  */
-  __Pyx_TraceLine(1667,0,__PYX_ERR(0, 1667, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_count, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1667, __pyx_L1_error)
+  __Pyx_TraceLine(1684,0,__PYX_ERR(0, 1684, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_count, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_t_2, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1667, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_t_2, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 1667, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 1684, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_11) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1668
+    /* "cpprb/PyReplayBuffer.pyx":1685
  *             self.explorer_count.value -= 1
  *         if self.explorer_count.value == 0:
  *             self.learner_ready.set()             # <<<<<<<<<<<<<<
  * 
  *     cdef void _lock_learner(self) except *:
  */
-    __Pyx_TraceLine(1668,0,__PYX_ERR(0, 1668, __pyx_L1_error))
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_ready, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1668, __pyx_L1_error)
+    __Pyx_TraceLine(1685,0,__PYX_ERR(0, 1685, __pyx_L1_error))
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_ready, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1685, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1668, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1685, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1667
+    /* "cpprb/PyReplayBuffer.pyx":1684
  *         with self.explorer_count.get_lock():
  *             self.explorer_count.value -= 1
  *         if self.explorer_count.value == 0:             # <<<<<<<<<<<<<<
  *             self.learner_ready.set()
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1664
+  /* "cpprb/PyReplayBuffer.pyx":1681
  *             self.explorer_count.value += 1
  * 
  *     cdef void _unlock_explorer(self) except *:             # <<<<<<<<<<<<<<
  *         with self.explorer_count.get_lock():
  *             self.explorer_count.value -= 1
  */
 
@@ -28096,15 +28302,15 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPReplayBuffer._unlock_explorer", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1670
+/* "cpprb/PyReplayBuffer.pyx":1687
  *             self.learner_ready.set()
  * 
  *     cdef void _lock_learner(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_ready.clear() # New explorer cannot enter into critical section
  *         self.learner_ready.wait() # Wait until all explorer exit from critical section
  */
 
@@ -28114,71 +28320,71 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_lock_learner", 0);
-  __Pyx_TraceCall("_lock_learner", __pyx_f[0], 1670, 0, __PYX_ERR(0, 1670, __pyx_L1_error));
+  __Pyx_TraceCall("_lock_learner", __pyx_f[0], 1687, 0, __PYX_ERR(0, 1687, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1671
+  /* "cpprb/PyReplayBuffer.pyx":1688
  * 
  *     cdef void _lock_learner(self) except *:
  *         self.explorer_ready.clear() # New explorer cannot enter into critical section             # <<<<<<<<<<<<<<
  *         self.learner_ready.wait() # Wait until all explorer exit from critical section
  * 
  */
-  __Pyx_TraceLine(1671,0,__PYX_ERR(0, 1671, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_ready, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1671, __pyx_L1_error)
+  __Pyx_TraceLine(1688,0,__PYX_ERR(0, 1688, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_ready, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1688, __pyx_L1_error)
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1671, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1688, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1672
+  /* "cpprb/PyReplayBuffer.pyx":1689
  *     cdef void _lock_learner(self) except *:
  *         self.explorer_ready.clear() # New explorer cannot enter into critical section
  *         self.learner_ready.wait() # Wait until all explorer exit from critical section             # <<<<<<<<<<<<<<
  * 
  *     cdef void _unlock_learner(self) except *:
  */
-  __Pyx_TraceLine(1672,0,__PYX_ERR(0, 1672, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_ready, __pyx_n_s_wait); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1672, __pyx_L1_error)
+  __Pyx_TraceLine(1689,0,__PYX_ERR(0, 1689, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_ready, __pyx_n_s_wait); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1689, __pyx_L1_error)
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1672, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1689, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1670
+  /* "cpprb/PyReplayBuffer.pyx":1687
  *             self.learner_ready.set()
  * 
  *     cdef void _lock_learner(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_ready.clear() # New explorer cannot enter into critical section
  *         self.learner_ready.wait() # Wait until all explorer exit from critical section
  */
 
@@ -28190,15 +28396,15 @@
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPReplayBuffer._lock_learner", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1674
+/* "cpprb/PyReplayBuffer.pyx":1691
  *         self.learner_ready.wait() # Wait until all explorer exit from critical section
  * 
  *     cdef void _unlock_learner(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_ready.set() # Allow workers to enter into critical section
  * 
  */
 
@@ -28208,44 +28414,44 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_unlock_learner", 0);
-  __Pyx_TraceCall("_unlock_learner", __pyx_f[0], 1674, 0, __PYX_ERR(0, 1674, __pyx_L1_error));
+  __Pyx_TraceCall("_unlock_learner", __pyx_f[0], 1691, 0, __PYX_ERR(0, 1691, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1675
+  /* "cpprb/PyReplayBuffer.pyx":1692
  * 
  *     cdef void _unlock_learner(self) except *:
  *         self.explorer_ready.set() # Allow workers to enter into critical section             # <<<<<<<<<<<<<<
  * 
  *     def add(self,*,**kwargs):
  */
-  __Pyx_TraceLine(1675,0,__PYX_ERR(0, 1675, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_ready, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1675, __pyx_L1_error)
+  __Pyx_TraceLine(1692,0,__PYX_ERR(0, 1692, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_ready, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1692, __pyx_L1_error)
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1675, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1692, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1674
+  /* "cpprb/PyReplayBuffer.pyx":1691
  *         self.learner_ready.wait() # Wait until all explorer exit from critical section
  * 
  *     cdef void _unlock_learner(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_ready.set() # Allow workers to enter into critical section
  * 
  */
 
@@ -28257,15 +28463,15 @@
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPReplayBuffer._unlock_learner", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1677
+/* "cpprb/PyReplayBuffer.pyx":1694
  *         self.explorer_ready.set() # Allow workers to enter into critical section
  * 
  *     def add(self,*,**kwargs):             # <<<<<<<<<<<<<<
  *         r"""Add transition(s) into replay buffer.
  * 
  */
 
@@ -28313,63 +28519,63 @@
   Py_ssize_t __pyx_t_11;
   int __pyx_t_12;
   PyObject *__pyx_t_13 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add", 0);
-  __Pyx_TraceCall("add", __pyx_f[0], 1677, 0, __PYX_ERR(0, 1677, __pyx_L1_error));
+  __Pyx_TraceCall("add", __pyx_f[0], 1694, 0, __PYX_ERR(0, 1694, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1705
+  /* "cpprb/PyReplayBuffer.pyx":1722
  *         It is user responsibility that all the values have the same step-size.
  *         """
  *         cdef size_t N = self.size_check.step_size(kwargs)             # <<<<<<<<<<<<<<
  * 
  *         cdef size_t index = self.index.fetch_add(N)
  */
-  __Pyx_TraceLine(1705,0,__PYX_ERR(0, 1705, __pyx_L1_error))
-  __pyx_t_1 = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_StepChecker *)__pyx_v_self->size_check->__pyx_vtab)->step_size(__pyx_v_self->size_check, __pyx_v_kwargs); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1705, __pyx_L1_error)
+  __Pyx_TraceLine(1722,0,__PYX_ERR(0, 1722, __pyx_L1_error))
+  __pyx_t_1 = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_StepChecker *)__pyx_v_self->size_check->__pyx_vtab)->step_size(__pyx_v_self->size_check, __pyx_v_kwargs); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1722, __pyx_L1_error)
   __pyx_v_N = __pyx_t_1;
 
-  /* "cpprb/PyReplayBuffer.pyx":1707
+  /* "cpprb/PyReplayBuffer.pyx":1724
  *         cdef size_t N = self.size_check.step_size(kwargs)
  * 
  *         cdef size_t index = self.index.fetch_add(N)             # <<<<<<<<<<<<<<
  *         cdef size_t end = index + N
  *         cdef add_idx = np.arange(index,end)
  */
-  __Pyx_TraceLine(1707,0,__PYX_ERR(0, 1707, __pyx_L1_error))
+  __Pyx_TraceLine(1724,0,__PYX_ERR(0, 1724, __pyx_L1_error))
   __pyx_v_index = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ProcessSafeRingBufferIndex *)__pyx_v_self->index->__pyx_base.__pyx_vtab)->__pyx_base.fetch_add(((struct __pyx_obj_5cpprb_14PyReplayBuffer_RingBufferIndex *)__pyx_v_self->index), __pyx_v_N);
 
-  /* "cpprb/PyReplayBuffer.pyx":1708
+  /* "cpprb/PyReplayBuffer.pyx":1725
  * 
  *         cdef size_t index = self.index.fetch_add(N)
  *         cdef size_t end = index + N             # <<<<<<<<<<<<<<
  *         cdef add_idx = np.arange(index,end)
  * 
  */
-  __Pyx_TraceLine(1708,0,__PYX_ERR(0, 1708, __pyx_L1_error))
+  __Pyx_TraceLine(1725,0,__PYX_ERR(0, 1725, __pyx_L1_error))
   __pyx_v_end = (__pyx_v_index + __pyx_v_N);
 
-  /* "cpprb/PyReplayBuffer.pyx":1709
+  /* "cpprb/PyReplayBuffer.pyx":1726
  *         cdef size_t index = self.index.fetch_add(N)
  *         cdef size_t end = index + N
  *         cdef add_idx = np.arange(index,end)             # <<<<<<<<<<<<<<
  * 
  *         if end > self.buffer_size:
  */
-  __Pyx_TraceLine(1709,0,__PYX_ERR(0, 1709, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1709, __pyx_L1_error)
+  __Pyx_TraceLine(1726,0,__PYX_ERR(0, 1726, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1726, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_arange); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1709, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_arange); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1726, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1709, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1726, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_FromSize_t(__pyx_v_end); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1709, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_FromSize_t(__pyx_v_end); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1726, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -28378,180 +28584,180 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_5};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1709, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1726, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_5};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1709, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1726, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1709, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1726, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_5);
     __pyx_t_3 = 0;
     __pyx_t_5 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1709, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1726, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_add_idx = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1711
+  /* "cpprb/PyReplayBuffer.pyx":1728
  *         cdef add_idx = np.arange(index,end)
  * 
  *         if end > self.buffer_size:             # <<<<<<<<<<<<<<
  *             add_idx[add_idx >= self.buffer_size] -= self.buffer_size
  * 
  */
-  __Pyx_TraceLine(1711,0,__PYX_ERR(0, 1711, __pyx_L1_error))
+  __Pyx_TraceLine(1728,0,__PYX_ERR(0, 1728, __pyx_L1_error))
   __pyx_t_9 = ((__pyx_v_end > __pyx_v_self->buffer_size) != 0);
   if (__pyx_t_9) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1712
+    /* "cpprb/PyReplayBuffer.pyx":1729
  * 
  *         if end > self.buffer_size:
  *             add_idx[add_idx >= self.buffer_size] -= self.buffer_size             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_TraceLine(1712,0,__PYX_ERR(0, 1712, __pyx_L1_error))
-    __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_self->buffer_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1712, __pyx_L1_error)
+    __Pyx_TraceLine(1729,0,__PYX_ERR(0, 1729, __pyx_L1_error))
+    __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_self->buffer_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1729, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyObject_RichCompare(__pyx_v_add_idx, __pyx_t_2, Py_GE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1712, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_v_add_idx, __pyx_t_2, Py_GE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1729, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_add_idx, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1712, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_add_idx, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1729, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = __Pyx_PyInt_FromSize_t(__pyx_v_self->buffer_size); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1712, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_FromSize_t(__pyx_v_self->buffer_size); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1729, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_5 = PyNumber_InPlaceSubtract(__pyx_t_2, __pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1712, __pyx_L1_error)
+    __pyx_t_5 = PyNumber_InPlaceSubtract(__pyx_t_2, __pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1729, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(PyObject_SetItem(__pyx_v_add_idx, __pyx_t_4, __pyx_t_5) < 0)) __PYX_ERR(0, 1712, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_add_idx, __pyx_t_4, __pyx_t_5) < 0)) __PYX_ERR(0, 1729, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1711
+    /* "cpprb/PyReplayBuffer.pyx":1728
  *         cdef add_idx = np.arange(index,end)
  * 
  *         if end > self.buffer_size:             # <<<<<<<<<<<<<<
  *             add_idx[add_idx >= self.buffer_size] -= self.buffer_size
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1715
+  /* "cpprb/PyReplayBuffer.pyx":1732
  * 
  * 
  *         self._lock_explorer()             # <<<<<<<<<<<<<<
  * 
  *         for name, b in self.buffer.items():
  */
-  __Pyx_TraceLine(1715,0,__PYX_ERR(0, 1715, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->_lock_explorer(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1715, __pyx_L1_error)
+  __Pyx_TraceLine(1732,0,__PYX_ERR(0, 1732, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->_lock_explorer(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1732, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":1717
+  /* "cpprb/PyReplayBuffer.pyx":1734
  *         self._lock_explorer()
  * 
  *         for name, b in self.buffer.items():             # <<<<<<<<<<<<<<
  *             b[add_idx] = np.reshape(np.array(kwargs[name],copy=False,ndmin=2),
  *                                     self.env_dict[name]["add_shape"])
  */
-  __Pyx_TraceLine(1717,0,__PYX_ERR(0, 1717, __pyx_L1_error))
+  __Pyx_TraceLine(1734,0,__PYX_ERR(0, 1734, __pyx_L1_error))
   __pyx_t_10 = 0;
   if (unlikely(__pyx_v_self->buffer == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-    __PYX_ERR(0, 1717, __pyx_L1_error)
+    __PYX_ERR(0, 1734, __pyx_L1_error)
   }
-  __pyx_t_5 = __Pyx_dict_iterator(__pyx_v_self->buffer, 0, __pyx_n_s_items, (&__pyx_t_11), (&__pyx_t_7)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1717, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_dict_iterator(__pyx_v_self->buffer, 0, __pyx_n_s_items, (&__pyx_t_11), (&__pyx_t_7)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1734, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_4);
   __pyx_t_4 = __pyx_t_5;
   __pyx_t_5 = 0;
   while (1) {
     __pyx_t_12 = __Pyx_dict_iter_next(__pyx_t_4, __pyx_t_11, &__pyx_t_10, &__pyx_t_5, &__pyx_t_8, NULL, __pyx_t_7);
     if (unlikely(__pyx_t_12 == 0)) break;
-    if (unlikely(__pyx_t_12 == -1)) __PYX_ERR(0, 1717, __pyx_L1_error)
+    if (unlikely(__pyx_t_12 == -1)) __PYX_ERR(0, 1734, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_XDECREF_SET(__pyx_v_b, __pyx_t_8);
     __pyx_t_8 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1718
+    /* "cpprb/PyReplayBuffer.pyx":1735
  * 
  *         for name, b in self.buffer.items():
  *             b[add_idx] = np.reshape(np.array(kwargs[name],copy=False,ndmin=2),             # <<<<<<<<<<<<<<
  *                                     self.env_dict[name]["add_shape"])
  * 
  */
-    __Pyx_TraceLine(1718,0,__PYX_ERR(0, 1718, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1718, __pyx_L1_error)
+    __Pyx_TraceLine(1735,0,__PYX_ERR(0, 1735, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1735, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_reshape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1718, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_reshape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1735, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1718, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1735, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1718, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1735, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_v_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1718, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_v_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1735, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1718, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1735, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1718, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1735, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1718, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_ndmin, __pyx_int_2) < 0) __PYX_ERR(0, 1718, __pyx_L1_error)
-    __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1718, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1735, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_ndmin, __pyx_int_2) < 0) __PYX_ERR(0, 1735, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1735, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1719
+    /* "cpprb/PyReplayBuffer.pyx":1736
  *         for name, b in self.buffer.items():
  *             b[add_idx] = np.reshape(np.array(kwargs[name],copy=False,ndmin=2),
  *                                     self.env_dict[name]["add_shape"])             # <<<<<<<<<<<<<<
  * 
  *         self._unlock_explorer()
  */
-    __Pyx_TraceLine(1719,0,__PYX_ERR(0, 1719, __pyx_L1_error))
-    __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_self->env_dict, __pyx_v_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1719, __pyx_L1_error)
+    __Pyx_TraceLine(1736,0,__PYX_ERR(0, 1736, __pyx_L1_error))
+    __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_self->env_dict, __pyx_v_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1736, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_n_u_add_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1719, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_n_u_add_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1736, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     __pyx_t_12 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_5)) {
@@ -28561,88 +28767,88 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_12 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_13, __pyx_t_6};
-      __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1718, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1735, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_13, __pyx_t_6};
-      __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1718, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1735, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_3 = PyTuple_New(2+__pyx_t_12); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1718, __pyx_L1_error)
+      __pyx_t_3 = PyTuple_New(2+__pyx_t_12); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1735, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_13);
       PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_12, __pyx_t_13);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_12, __pyx_t_6);
       __pyx_t_13 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1718, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1735, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1718
+    /* "cpprb/PyReplayBuffer.pyx":1735
  * 
  *         for name, b in self.buffer.items():
  *             b[add_idx] = np.reshape(np.array(kwargs[name],copy=False,ndmin=2),             # <<<<<<<<<<<<<<
  *                                     self.env_dict[name]["add_shape"])
  * 
  */
-    __Pyx_TraceLine(1718,0,__PYX_ERR(0, 1718, __pyx_L1_error))
-    if (unlikely(PyObject_SetItem(__pyx_v_b, __pyx_v_add_idx, __pyx_t_8) < 0)) __PYX_ERR(0, 1718, __pyx_L1_error)
+    __Pyx_TraceLine(1735,0,__PYX_ERR(0, 1735, __pyx_L1_error))
+    if (unlikely(PyObject_SetItem(__pyx_v_b, __pyx_v_add_idx, __pyx_t_8) < 0)) __PYX_ERR(0, 1735, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1721
+  /* "cpprb/PyReplayBuffer.pyx":1738
  *                                     self.env_dict[name]["add_shape"])
  * 
  *         self._unlock_explorer()             # <<<<<<<<<<<<<<
  *         return index
  * 
  */
-  __Pyx_TraceLine(1721,0,__PYX_ERR(0, 1721, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->_unlock_explorer(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1721, __pyx_L1_error)
+  __Pyx_TraceLine(1738,0,__PYX_ERR(0, 1738, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->_unlock_explorer(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1738, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":1722
+  /* "cpprb/PyReplayBuffer.pyx":1739
  * 
  *         self._unlock_explorer()
  *         return index             # <<<<<<<<<<<<<<
  * 
  *     def get_all_transitions(self,shuffle: bool=False):
  */
-  __Pyx_TraceLine(1722,0,__PYX_ERR(0, 1722, __pyx_L1_error))
+  __Pyx_TraceLine(1739,0,__PYX_ERR(0, 1739, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1722, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1677
+  /* "cpprb/PyReplayBuffer.pyx":1694
  *         self.explorer_ready.set() # Allow workers to enter into critical section
  * 
  *     def add(self,*,**kwargs):             # <<<<<<<<<<<<<<
  *         r"""Add transition(s) into replay buffer.
  * 
  */
 
@@ -28663,15 +28869,15 @@
   __Pyx_XDECREF(__pyx_v_b);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1724
+/* "cpprb/PyReplayBuffer.pyx":1741
  *         return index
  * 
  *     def get_all_transitions(self,shuffle: bool=False):             # <<<<<<<<<<<<<<
  *         r"""
  *         Get all transitions stored in replay buffer.
  */
 
@@ -28703,33 +28909,33 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_shuffle);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_all_transitions") < 0)) __PYX_ERR(0, 1724, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_all_transitions") < 0)) __PYX_ERR(0, 1741, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_shuffle = __Pyx_PyObject_IsTrue(values[0]); if (unlikely((__pyx_v_shuffle == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1724, __pyx_L3_error)
+      __pyx_v_shuffle = __Pyx_PyObject_IsTrue(values[0]); if (unlikely((__pyx_v_shuffle == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1741, __pyx_L3_error)
     } else {
       __pyx_v_shuffle = ((bool)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_all_transitions", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1724, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_all_transitions", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1741, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPReplayBuffer.get_all_transitions", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_14MPReplayBuffer_4get_all_transitions(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self), __pyx_v_shuffle);
 
@@ -28749,165 +28955,165 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_all_transitions", 0);
-  __Pyx_TraceCall("get_all_transitions", __pyx_f[0], 1724, 0, __PYX_ERR(0, 1724, __pyx_L1_error));
+  __Pyx_TraceCall("get_all_transitions", __pyx_f[0], 1741, 0, __PYX_ERR(0, 1741, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1738
+  /* "cpprb/PyReplayBuffer.pyx":1755
  *             All transitions stored in this replay buffer.
  *         """
  *         idx = np.arange(self.get_stored_size())             # <<<<<<<<<<<<<<
  * 
  *         if shuffle:
  */
-  __Pyx_TraceLine(1738,0,__PYX_ERR(0, 1738, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1738, __pyx_L1_error)
+  __Pyx_TraceLine(1755,0,__PYX_ERR(0, 1755, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1738, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_FromSize_t(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_stored_size(__pyx_v_self, 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1738, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_FromSize_t(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_stored_size(__pyx_v_self, 0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1738, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_idx = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1740
+  /* "cpprb/PyReplayBuffer.pyx":1757
  *         idx = np.arange(self.get_stored_size())
  * 
  *         if shuffle:             # <<<<<<<<<<<<<<
  *             np.random.shuffle(idx)
  * 
  */
-  __Pyx_TraceLine(1740,0,__PYX_ERR(0, 1740, __pyx_L1_error))
+  __Pyx_TraceLine(1757,0,__PYX_ERR(0, 1757, __pyx_L1_error))
   __pyx_t_5 = (__pyx_v_shuffle != 0);
   if (__pyx_t_5) {
 
-    /* "cpprb/PyReplayBuffer.pyx":1741
+    /* "cpprb/PyReplayBuffer.pyx":1758
  * 
  *         if shuffle:
  *             np.random.shuffle(idx)             # <<<<<<<<<<<<<<
  * 
  *         self._lock_learner()
  */
-    __Pyx_TraceLine(1741,0,__PYX_ERR(0, 1741, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1741, __pyx_L1_error)
+    __Pyx_TraceLine(1758,0,__PYX_ERR(0, 1758, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1758, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1741, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1758, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1741, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1758, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_idx) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_idx);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1741, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1758, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1740
+    /* "cpprb/PyReplayBuffer.pyx":1757
  *         idx = np.arange(self.get_stored_size())
  * 
  *         if shuffle:             # <<<<<<<<<<<<<<
  *             np.random.shuffle(idx)
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1743
+  /* "cpprb/PyReplayBuffer.pyx":1760
  *             np.random.shuffle(idx)
  * 
  *         self._lock_learner()             # <<<<<<<<<<<<<<
  *         ret = self._encode_sample(idx)
  *         self._unlock_learner()
  */
-  __Pyx_TraceLine(1743,0,__PYX_ERR(0, 1743, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->_lock_learner(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1743, __pyx_L1_error)
+  __Pyx_TraceLine(1760,0,__PYX_ERR(0, 1760, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->_lock_learner(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1760, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":1744
+  /* "cpprb/PyReplayBuffer.pyx":1761
  * 
  *         self._lock_learner()
  *         ret = self._encode_sample(idx)             # <<<<<<<<<<<<<<
  *         self._unlock_learner()
  * 
  */
-  __Pyx_TraceLine(1744,0,__PYX_ERR(0, 1744, __pyx_L1_error))
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_encode_sample); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1744, __pyx_L1_error)
+  __Pyx_TraceLine(1761,0,__PYX_ERR(0, 1761, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_encode_sample); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1761, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_idx) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_idx);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1744, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1761, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_ret = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1745
+  /* "cpprb/PyReplayBuffer.pyx":1762
  *         self._lock_learner()
  *         ret = self._encode_sample(idx)
  *         self._unlock_learner()             # <<<<<<<<<<<<<<
  * 
  *         return ret
  */
-  __Pyx_TraceLine(1745,0,__PYX_ERR(0, 1745, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->_unlock_learner(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1745, __pyx_L1_error)
+  __Pyx_TraceLine(1762,0,__PYX_ERR(0, 1762, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->_unlock_learner(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1762, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":1747
+  /* "cpprb/PyReplayBuffer.pyx":1764
  *         self._unlock_learner()
  * 
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     def _encode_sample(self,idx):
  */
-  __Pyx_TraceLine(1747,0,__PYX_ERR(0, 1747, __pyx_L1_error))
+  __Pyx_TraceLine(1764,0,__PYX_ERR(0, 1764, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_ret);
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1724
+  /* "cpprb/PyReplayBuffer.pyx":1741
  *         return index
  * 
  *     def get_all_transitions(self,shuffle: bool=False):             # <<<<<<<<<<<<<<
  *         r"""
  *         Get all transitions stored in replay buffer.
  */
 
@@ -28924,15 +29130,15 @@
   __Pyx_XDECREF(__pyx_v_ret);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1749
+/* "cpprb/PyReplayBuffer.pyx":1766
  *         return ret
  * 
  *     def _encode_sample(self,idx):             # <<<<<<<<<<<<<<
  *         cdef sample = {}
  * 
  */
 
@@ -28965,118 +29171,118 @@
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_encode_sample", 0);
-  __Pyx_TraceCall("_encode_sample", __pyx_f[0], 1749, 0, __PYX_ERR(0, 1749, __pyx_L1_error));
+  __Pyx_TraceCall("_encode_sample", __pyx_f[0], 1766, 0, __PYX_ERR(0, 1766, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_idx);
 
-  /* "cpprb/PyReplayBuffer.pyx":1750
+  /* "cpprb/PyReplayBuffer.pyx":1767
  * 
  *     def _encode_sample(self,idx):
  *         cdef sample = {}             # <<<<<<<<<<<<<<
  * 
  *         idx = np.array(idx,copy=False,ndmin=1)
  */
-  __Pyx_TraceLine(1750,0,__PYX_ERR(0, 1750, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1750, __pyx_L1_error)
+  __Pyx_TraceLine(1767,0,__PYX_ERR(0, 1767, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1767, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_sample = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1752
+  /* "cpprb/PyReplayBuffer.pyx":1769
  *         cdef sample = {}
  * 
  *         idx = np.array(idx,copy=False,ndmin=1)             # <<<<<<<<<<<<<<
  * 
  *         for name, b in self.buffer.items():
  */
-  __Pyx_TraceLine(1752,0,__PYX_ERR(0, 1752, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1752, __pyx_L1_error)
+  __Pyx_TraceLine(1769,0,__PYX_ERR(0, 1769, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1769, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1752, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1769, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1752, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1769, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_idx);
   __Pyx_GIVEREF(__pyx_v_idx);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_idx);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1752, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1769, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1752, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_ndmin, __pyx_int_1) < 0) __PYX_ERR(0, 1752, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1752, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1769, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_ndmin, __pyx_int_1) < 0) __PYX_ERR(0, 1769, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1769, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_idx, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1754
+  /* "cpprb/PyReplayBuffer.pyx":1771
  *         idx = np.array(idx,copy=False,ndmin=1)
  * 
  *         for name, b in self.buffer.items():             # <<<<<<<<<<<<<<
  *             sample[name] = b[idx]
  * 
  */
-  __Pyx_TraceLine(1754,0,__PYX_ERR(0, 1754, __pyx_L1_error))
+  __Pyx_TraceLine(1771,0,__PYX_ERR(0, 1771, __pyx_L1_error))
   __pyx_t_5 = 0;
   if (unlikely(__pyx_v_self->buffer == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-    __PYX_ERR(0, 1754, __pyx_L1_error)
+    __PYX_ERR(0, 1771, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_self->buffer, 0, __pyx_n_s_items, (&__pyx_t_6), (&__pyx_t_7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1754, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_self->buffer, 0, __pyx_n_s_items, (&__pyx_t_6), (&__pyx_t_7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1771, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __pyx_t_4 = __pyx_t_3;
   __pyx_t_3 = 0;
   while (1) {
     __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_4, __pyx_t_6, &__pyx_t_5, &__pyx_t_3, &__pyx_t_1, NULL, __pyx_t_7);
     if (unlikely(__pyx_t_8 == 0)) break;
-    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 1754, __pyx_L1_error)
+    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 1771, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_3);
     __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_b, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":1755
+    /* "cpprb/PyReplayBuffer.pyx":1772
  * 
  *         for name, b in self.buffer.items():
  *             sample[name] = b[idx]             # <<<<<<<<<<<<<<
  * 
  *         return sample
  */
-    __Pyx_TraceLine(1755,0,__PYX_ERR(0, 1755, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_b, __pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1755, __pyx_L1_error)
+    __Pyx_TraceLine(1772,0,__PYX_ERR(0, 1772, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_b, __pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1772, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(PyObject_SetItem(__pyx_v_sample, __pyx_v_name, __pyx_t_1) < 0)) __PYX_ERR(0, 1755, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_sample, __pyx_v_name, __pyx_t_1) < 0)) __PYX_ERR(0, 1772, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1757
+  /* "cpprb/PyReplayBuffer.pyx":1774
  *             sample[name] = b[idx]
  * 
  *         return sample             # <<<<<<<<<<<<<<
  * 
  *     def sample(self,batch_size):
  */
-  __Pyx_TraceLine(1757,0,__PYX_ERR(0, 1757, __pyx_L1_error))
+  __Pyx_TraceLine(1774,0,__PYX_ERR(0, 1774, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_sample);
   __pyx_r = __pyx_v_sample;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1749
+  /* "cpprb/PyReplayBuffer.pyx":1766
  *         return ret
  * 
  *     def _encode_sample(self,idx):             # <<<<<<<<<<<<<<
  *         cdef sample = {}
  * 
  */
 
@@ -29095,15 +29301,15 @@
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1759
+/* "cpprb/PyReplayBuffer.pyx":1776
  *         return sample
  * 
  *     def sample(self,batch_size):             # <<<<<<<<<<<<<<
  *         r"""Sample the stored transitions randomly with speciped size
  * 
  */
 
@@ -29133,33 +29339,33 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sample", 0);
-  __Pyx_TraceCall("sample", __pyx_f[0], 1759, 0, __PYX_ERR(0, 1759, __pyx_L1_error));
+  __Pyx_TraceCall("sample", __pyx_f[0], 1776, 0, __PYX_ERR(0, 1776, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1775
+  /* "cpprb/PyReplayBuffer.pyx":1792
  *             the same transition multiple times.
  *         """
  *         cdef idx = np.random.randint(0,self.get_stored_size(),batch_size)             # <<<<<<<<<<<<<<
  * 
  *         self._lock_learner()
  */
-  __Pyx_TraceLine(1775,0,__PYX_ERR(0, 1775, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1775, __pyx_L1_error)
+  __Pyx_TraceLine(1792,0,__PYX_ERR(0, 1792, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1775, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_randint); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1775, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_randint); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_FromSize_t(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_stored_size(__pyx_v_self, 0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1775, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_FromSize_t(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->get_stored_size(__pyx_v_self, 0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -29168,114 +29374,114 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_int_0, __pyx_t_3, __pyx_v_batch_size};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1775, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1792, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_int_0, __pyx_t_3, __pyx_v_batch_size};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1775, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1792, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1775, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1792, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_int_0);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_t_3);
     __Pyx_INCREF(__pyx_v_batch_size);
     __Pyx_GIVEREF(__pyx_v_batch_size);
     PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_5, __pyx_v_batch_size);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1775, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1792, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_idx = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1777
+  /* "cpprb/PyReplayBuffer.pyx":1794
  *         cdef idx = np.random.randint(0,self.get_stored_size(),batch_size)
  * 
  *         self._lock_learner()             # <<<<<<<<<<<<<<
  *         ret =  self._encode_sample(idx)
  *         self._unlock_learner()
  */
-  __Pyx_TraceLine(1777,0,__PYX_ERR(0, 1777, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->_lock_learner(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1777, __pyx_L1_error)
+  __Pyx_TraceLine(1794,0,__PYX_ERR(0, 1794, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->_lock_learner(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1794, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":1778
+  /* "cpprb/PyReplayBuffer.pyx":1795
  * 
  *         self._lock_learner()
  *         ret =  self._encode_sample(idx)             # <<<<<<<<<<<<<<
  *         self._unlock_learner()
  * 
  */
-  __Pyx_TraceLine(1778,0,__PYX_ERR(0, 1778, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_encode_sample); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1778, __pyx_L1_error)
+  __Pyx_TraceLine(1795,0,__PYX_ERR(0, 1795, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_encode_sample); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1795, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_v_idx) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_idx);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1778, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1795, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_ret = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1779
+  /* "cpprb/PyReplayBuffer.pyx":1796
  *         self._lock_learner()
  *         ret =  self._encode_sample(idx)
  *         self._unlock_learner()             # <<<<<<<<<<<<<<
  * 
  *         return ret
  */
-  __Pyx_TraceLine(1779,0,__PYX_ERR(0, 1779, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->_unlock_learner(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1779, __pyx_L1_error)
+  __Pyx_TraceLine(1796,0,__PYX_ERR(0, 1796, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self->__pyx_vtab)->_unlock_learner(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1796, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":1781
+  /* "cpprb/PyReplayBuffer.pyx":1798
  *         self._unlock_learner()
  * 
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef void clear(self) except *:
  */
-  __Pyx_TraceLine(1781,0,__PYX_ERR(0, 1781, __pyx_L1_error))
+  __Pyx_TraceLine(1798,0,__PYX_ERR(0, 1798, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_ret);
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1759
+  /* "cpprb/PyReplayBuffer.pyx":1776
  *         return sample
  * 
  *     def sample(self,batch_size):             # <<<<<<<<<<<<<<
  *         r"""Sample the stored transitions randomly with speciped size
  * 
  */
 
@@ -29293,15 +29499,15 @@
   __Pyx_XDECREF(__pyx_v_ret);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1783
+/* "cpprb/PyReplayBuffer.pyx":1800
  *         return ret
  * 
  *     cpdef void clear(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Clear replay buffer.
  * 
  */
 
@@ -29313,25 +29519,25 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear", 0);
-  __Pyx_TraceCall("clear", __pyx_f[0], 1783, 0, __PYX_ERR(0, 1783, __pyx_L1_error));
+  __Pyx_TraceCall("clear", __pyx_f[0], 1800, 0, __PYX_ERR(0, 1800, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1783, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1800, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_14MPReplayBuffer_11clear)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -29339,15 +29545,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1783, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1800, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
@@ -29359,25 +29565,25 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1802
+  /* "cpprb/PyReplayBuffer.pyx":1819
  *         0
  *         """
  *         self.index.clear()             # <<<<<<<<<<<<<<
  * 
  *     cpdef size_t get_stored_size(self):
  */
-  __Pyx_TraceLine(1802,0,__PYX_ERR(0, 1802, __pyx_L1_error))
+  __Pyx_TraceLine(1819,0,__PYX_ERR(0, 1819, __pyx_L1_error))
   ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ProcessSafeRingBufferIndex *)__pyx_v_self->index->__pyx_base.__pyx_vtab)->__pyx_base.clear(((struct __pyx_obj_5cpprb_14PyReplayBuffer_RingBufferIndex *)__pyx_v_self->index));
 
-  /* "cpprb/PyReplayBuffer.pyx":1783
+  /* "cpprb/PyReplayBuffer.pyx":1800
  *         return ret
  * 
  *     cpdef void clear(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Clear replay buffer.
  * 
  */
 
@@ -29413,18 +29619,18 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear", 0);
-  __Pyx_TraceCall("clear (wrapper)", __pyx_f[0], 1783, 0, __PYX_ERR(0, 1783, __pyx_L1_error));
+  __Pyx_TraceCall("clear (wrapper)", __pyx_f[0], 1800, 0, __PYX_ERR(0, 1800, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_clear(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1783, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1783, __pyx_L1_error)
+  __pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_clear(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1800, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1800, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -29434,15 +29640,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1804
+/* "cpprb/PyReplayBuffer.pyx":1821
  *         self.index.clear()
  * 
  *     cpdef size_t get_stored_size(self):             # <<<<<<<<<<<<<<
  *         r"""Get stored size
  * 
  */
 
@@ -29456,25 +29662,25 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   size_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_stored_size", 0);
-  __Pyx_TraceCall("get_stored_size", __pyx_f[0], 1804, 0, __PYX_ERR(0, 1804, __pyx_L1_error));
+  __Pyx_TraceCall("get_stored_size", __pyx_f[0], 1821, 0, __PYX_ERR(0, 1821, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_stored_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1804, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_stored_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1821, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_14MPReplayBuffer_13get_stored_size)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -29482,18 +29688,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1804, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1821, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1804, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1821, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -29504,26 +29710,26 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1812
+  /* "cpprb/PyReplayBuffer.pyx":1829
  *             stored size
  *         """
  *         return self.index.get_stored_size()             # <<<<<<<<<<<<<<
  * 
  *     cpdef size_t get_buffer_size(self):
  */
-  __Pyx_TraceLine(1812,0,__PYX_ERR(0, 1812, __pyx_L1_error))
+  __Pyx_TraceLine(1829,0,__PYX_ERR(0, 1829, __pyx_L1_error))
   __pyx_r = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ProcessSafeRingBufferIndex *)__pyx_v_self->index->__pyx_base.__pyx_vtab)->__pyx_base.get_stored_size(((struct __pyx_obj_5cpprb_14PyReplayBuffer_RingBufferIndex *)__pyx_v_self->index));
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1804
+  /* "cpprb/PyReplayBuffer.pyx":1821
  *         self.index.clear()
  * 
  *     cpdef size_t get_stored_size(self):             # <<<<<<<<<<<<<<
  *         r"""Get stored size
  * 
  */
 
@@ -29560,17 +29766,17 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_stored_size", 0);
-  __Pyx_TraceCall("get_stored_size (wrapper)", __pyx_f[0], 1804, 0, __PYX_ERR(0, 1804, __pyx_L1_error));
+  __Pyx_TraceCall("get_stored_size (wrapper)", __pyx_f[0], 1821, 0, __PYX_ERR(0, 1821, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_get_stored_size(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1804, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_get_stored_size(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1821, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -29580,15 +29786,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1814
+/* "cpprb/PyReplayBuffer.pyx":1831
  *         return self.index.get_stored_size()
  * 
  *     cpdef size_t get_buffer_size(self):             # <<<<<<<<<<<<<<
  *         r"""Get buffer size
  * 
  */
 
@@ -29602,25 +29808,25 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   size_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_buffer_size", 0);
-  __Pyx_TraceCall("get_buffer_size", __pyx_f[0], 1814, 0, __PYX_ERR(0, 1814, __pyx_L1_error));
+  __Pyx_TraceCall("get_buffer_size", __pyx_f[0], 1831, 0, __PYX_ERR(0, 1831, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_buffer_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1814, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_buffer_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1831, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_14MPReplayBuffer_15get_buffer_size)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -29628,18 +29834,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1814, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1831, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1814, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1831, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -29650,26 +29856,26 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1822
+  /* "cpprb/PyReplayBuffer.pyx":1839
  *             buffer size
  *         """
  *         return self.buffer_size             # <<<<<<<<<<<<<<
  * 
  *     cpdef size_t get_next_index(self):
  */
-  __Pyx_TraceLine(1822,0,__PYX_ERR(0, 1822, __pyx_L1_error))
+  __Pyx_TraceLine(1839,0,__PYX_ERR(0, 1839, __pyx_L1_error))
   __pyx_r = __pyx_v_self->buffer_size;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1814
+  /* "cpprb/PyReplayBuffer.pyx":1831
  *         return self.index.get_stored_size()
  * 
  *     cpdef size_t get_buffer_size(self):             # <<<<<<<<<<<<<<
  *         r"""Get buffer size
  * 
  */
 
@@ -29706,17 +29912,17 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_buffer_size", 0);
-  __Pyx_TraceCall("get_buffer_size (wrapper)", __pyx_f[0], 1814, 0, __PYX_ERR(0, 1814, __pyx_L1_error));
+  __Pyx_TraceCall("get_buffer_size (wrapper)", __pyx_f[0], 1831, 0, __PYX_ERR(0, 1831, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_get_buffer_size(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1814, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_get_buffer_size(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1831, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -29726,15 +29932,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1824
+/* "cpprb/PyReplayBuffer.pyx":1841
  *         return self.buffer_size
  * 
  *     cpdef size_t get_next_index(self):             # <<<<<<<<<<<<<<
  *         r"""Get the next index to store
  * 
  */
 
@@ -29748,25 +29954,25 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   size_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_next_index", 0);
-  __Pyx_TraceCall("get_next_index", __pyx_f[0], 1824, 0, __PYX_ERR(0, 1824, __pyx_L1_error));
+  __Pyx_TraceCall("get_next_index", __pyx_f[0], 1841, 0, __PYX_ERR(0, 1841, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_next_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1824, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_next_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1841, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_14MPReplayBuffer_17get_next_index)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -29774,18 +29980,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1824, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1841, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1824, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1841, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -29796,26 +30002,26 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1832
+  /* "cpprb/PyReplayBuffer.pyx":1849
  *             the next index to store
  *         """
  *         return self.index.get_next_index()             # <<<<<<<<<<<<<<
  * 
  *     cpdef void on_episode_end(self) except *:
  */
-  __Pyx_TraceLine(1832,0,__PYX_ERR(0, 1832, __pyx_L1_error))
+  __Pyx_TraceLine(1849,0,__PYX_ERR(0, 1849, __pyx_L1_error))
   __pyx_r = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ProcessSafeRingBufferIndex *)__pyx_v_self->index->__pyx_base.__pyx_vtab)->__pyx_base.get_next_index(((struct __pyx_obj_5cpprb_14PyReplayBuffer_RingBufferIndex *)__pyx_v_self->index));
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1824
+  /* "cpprb/PyReplayBuffer.pyx":1841
  *         return self.buffer_size
  * 
  *     cpdef size_t get_next_index(self):             # <<<<<<<<<<<<<<
  *         r"""Get the next index to store
  * 
  */
 
@@ -29852,17 +30058,17 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_next_index", 0);
-  __Pyx_TraceCall("get_next_index (wrapper)", __pyx_f[0], 1824, 0, __PYX_ERR(0, 1824, __pyx_L1_error));
+  __Pyx_TraceCall("get_next_index (wrapper)", __pyx_f[0], 1841, 0, __PYX_ERR(0, 1841, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_get_next_index(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1824, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_get_next_index(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1841, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -29872,15 +30078,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1834
+/* "cpprb/PyReplayBuffer.pyx":1851
  *         return self.index.get_next_index()
  * 
  *     cpdef void on_episode_end(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Call on episode end
  * 
  */
 
@@ -29892,25 +30098,25 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_episode_end", 0);
-  __Pyx_TraceCall("on_episode_end", __pyx_f[0], 1834, 0, __PYX_ERR(0, 1834, __pyx_L1_error));
+  __Pyx_TraceCall("on_episode_end", __pyx_f[0], 1851, 0, __PYX_ERR(0, 1851, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_episode_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1834, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_episode_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1851, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_14MPReplayBuffer_19on_episode_end)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -29918,15 +30124,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1834, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1851, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
@@ -29938,37 +30144,37 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1835
+  /* "cpprb/PyReplayBuffer.pyx":1852
  * 
  *     cpdef void on_episode_end(self) except *:
  *         r"""Call on episode end             # <<<<<<<<<<<<<<
  * 
  *         Finalize the current episode by moving remaining Nstep buffer transitions,
  */
-  __Pyx_TraceLine(1835,0,__PYX_ERR(0, 1835, __pyx_L1_error))
+  __Pyx_TraceLine(1852,0,__PYX_ERR(0, 1852, __pyx_L1_error))
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPReplayBuffer.on_episode_end", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1834
+/* "cpprb/PyReplayBuffer.pyx":1851
  *         return self.index.get_next_index()
  * 
  *     cpdef void on_episode_end(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Call on episode end
  * 
  */
 
@@ -29991,18 +30197,18 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_episode_end", 0);
-  __Pyx_TraceCall("on_episode_end (wrapper)", __pyx_f[0], 1834, 0, __PYX_ERR(0, 1834, __pyx_L1_error));
+  __Pyx_TraceCall("on_episode_end (wrapper)", __pyx_f[0], 1851, 0, __PYX_ERR(0, 1851, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_on_episode_end(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1834, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1834, __pyx_L1_error)
+  __pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_on_episode_end(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1851, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1851, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -30012,15 +30218,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1849
+/* "cpprb/PyReplayBuffer.pyx":1866
  *         pass
  * 
  *     cpdef bool is_Nstep(self):             # <<<<<<<<<<<<<<
  *         r"""Get whether use Nstep or not
  * 
  */
 
@@ -30034,25 +30240,25 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   bool __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_Nstep", 0);
-  __Pyx_TraceCall("is_Nstep", __pyx_f[0], 1849, 0, __PYX_ERR(0, 1849, __pyx_L1_error));
+  __Pyx_TraceCall("is_Nstep", __pyx_f[0], 1866, 0, __PYX_ERR(0, 1866, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_is_Nstep); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1849, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_is_Nstep); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1866, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_14MPReplayBuffer_21is_Nstep)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -30060,18 +30266,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1849, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1866, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1849, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1866, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -30082,26 +30288,26 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1856
+  /* "cpprb/PyReplayBuffer.pyx":1873
  *         use_nstep : bool
  *         """
  *         return False             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1856,0,__PYX_ERR(0, 1856, __pyx_L1_error))
+  __Pyx_TraceLine(1873,0,__PYX_ERR(0, 1873, __pyx_L1_error))
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1849
+  /* "cpprb/PyReplayBuffer.pyx":1866
  *         pass
  * 
  *     cpdef bool is_Nstep(self):             # <<<<<<<<<<<<<<
  *         r"""Get whether use Nstep or not
  * 
  */
 
@@ -30138,17 +30344,17 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_Nstep", 0);
-  __Pyx_TraceCall("is_Nstep (wrapper)", __pyx_f[0], 1849, 0, __PYX_ERR(0, 1849, __pyx_L1_error));
+  __Pyx_TraceCall("is_Nstep (wrapper)", __pyx_f[0], 1866, 0, __PYX_ERR(0, 1866, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_is_Nstep(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1849, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_is_Nstep(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1866, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -30548,15 +30754,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1870
+/* "cpprb/PyReplayBuffer.pyx":1887
  *     cdef CppThreadSafePrioritizedSampler[float]* per
  * 
  *     def __init__(self,size,alpha,eps,max_p=None,             # <<<<<<<<<<<<<<
  *                  sum=None,sum_a=None,
  *                  min=None,min_a=None):
  */
 
@@ -30578,25 +30784,25 @@
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_size,&__pyx_n_s_alpha,&__pyx_n_s_eps,&__pyx_n_s_max_p,&__pyx_n_s_sum,&__pyx_n_s_sum_a,&__pyx_n_s_min,&__pyx_n_s_min_a,0};
     PyObject* values[8] = {0,0,0,0,0,0,0,0};
     values[3] = ((PyObject *)Py_None);
 
-    /* "cpprb/PyReplayBuffer.pyx":1871
+    /* "cpprb/PyReplayBuffer.pyx":1888
  * 
  *     def __init__(self,size,alpha,eps,max_p=None,
  *                  sum=None,sum_a=None,             # <<<<<<<<<<<<<<
  *                  min=None,min_a=None):
  *         self.size = size
  */
     values[4] = ((PyObject *)Py_None);
     values[5] = ((PyObject *)Py_None);
 
-    /* "cpprb/PyReplayBuffer.pyx":1872
+    /* "cpprb/PyReplayBuffer.pyx":1889
  *     def __init__(self,size,alpha,eps,max_p=None,
  *                  sum=None,sum_a=None,
  *                  min=None,min_a=None):             # <<<<<<<<<<<<<<
  *         self.size = size
  *         self.alpha = alpha
  */
     values[6] = ((PyObject *)Py_None);
@@ -30629,21 +30835,21 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_size)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_alpha)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 3, 8, 1); __PYX_ERR(0, 1870, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 3, 8, 1); __PYX_ERR(0, 1887, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_eps)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 3, 8, 2); __PYX_ERR(0, 1870, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 3, 8, 2); __PYX_ERR(0, 1887, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_max_p);
           if (value) { values[3] = value; kw_args--; }
         }
@@ -30669,15 +30875,15 @@
         case  7:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_min_a);
           if (value) { values[7] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1870, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1887, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
@@ -30701,23 +30907,23 @@
     __pyx_v_sum = values[4];
     __pyx_v_sum_a = values[5];
     __pyx_v_min = values[6];
     __pyx_v_min_a = values[7];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 3, 8, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1870, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 3, 8, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1887, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.ThreadSafePrioritizedSampler.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_28ThreadSafePrioritizedSampler___init__(((struct __pyx_obj_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler *)__pyx_v_self), __pyx_v_size, __pyx_v_alpha, __pyx_v_eps, __pyx_v_max_p, __pyx_v_sum, __pyx_v_sum_a, __pyx_v_min, __pyx_v_min_a);
 
-  /* "cpprb/PyReplayBuffer.pyx":1870
+  /* "cpprb/PyReplayBuffer.pyx":1887
  *     cdef CppThreadSafePrioritizedSampler[float]* per
  * 
  *     def __init__(self,size,alpha,eps,max_p=None,             # <<<<<<<<<<<<<<
  *                  sum=None,sum_a=None,
  *                  min=None,min_a=None):
  */
 
@@ -30758,69 +30964,69 @@
   Py_ssize_t __pyx_t_19;
   float __pyx_t_20;
   ymd::CppThreadSafePrioritizedSampler<float>  *__pyx_t_21;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
-  __Pyx_TraceCall("__init__", __pyx_f[0], 1870, 0, __PYX_ERR(0, 1870, __pyx_L1_error));
+  __Pyx_TraceCall("__init__", __pyx_f[0], 1887, 0, __PYX_ERR(0, 1887, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1873
+  /* "cpprb/PyReplayBuffer.pyx":1890
  *                  sum=None,sum_a=None,
  *                  min=None,min_a=None):
  *         self.size = size             # <<<<<<<<<<<<<<
  *         self.alpha = alpha
  *         self.eps = eps
  */
-  __Pyx_TraceLine(1873,0,__PYX_ERR(0, 1873, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_size); if (unlikely((__pyx_t_1 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1873, __pyx_L1_error)
+  __Pyx_TraceLine(1890,0,__PYX_ERR(0, 1890, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_size); if (unlikely((__pyx_t_1 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1890, __pyx_L1_error)
   __pyx_v_self->size = __pyx_t_1;
 
-  /* "cpprb/PyReplayBuffer.pyx":1874
+  /* "cpprb/PyReplayBuffer.pyx":1891
  *                  min=None,min_a=None):
  *         self.size = size
  *         self.alpha = alpha             # <<<<<<<<<<<<<<
  *         self.eps = eps
  * 
  */
-  __Pyx_TraceLine(1874,0,__PYX_ERR(0, 1874, __pyx_L1_error))
-  __pyx_t_2 = __pyx_PyFloat_AsFloat(__pyx_v_alpha); if (unlikely((__pyx_t_2 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1874, __pyx_L1_error)
+  __Pyx_TraceLine(1891,0,__PYX_ERR(0, 1891, __pyx_L1_error))
+  __pyx_t_2 = __pyx_PyFloat_AsFloat(__pyx_v_alpha); if (unlikely((__pyx_t_2 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1891, __pyx_L1_error)
   __pyx_v_self->alpha = __pyx_t_2;
 
-  /* "cpprb/PyReplayBuffer.pyx":1875
+  /* "cpprb/PyReplayBuffer.pyx":1892
  *         self.size = size
  *         self.alpha = alpha
  *         self.eps = eps             # <<<<<<<<<<<<<<
  * 
  *         self.max_p = max_p or RawArray(ctypes.c_float,1)
  */
-  __Pyx_TraceLine(1875,0,__PYX_ERR(0, 1875, __pyx_L1_error))
-  __pyx_t_2 = __pyx_PyFloat_AsFloat(__pyx_v_eps); if (unlikely((__pyx_t_2 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1875, __pyx_L1_error)
+  __Pyx_TraceLine(1892,0,__PYX_ERR(0, 1892, __pyx_L1_error))
+  __pyx_t_2 = __pyx_PyFloat_AsFloat(__pyx_v_eps); if (unlikely((__pyx_t_2 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1892, __pyx_L1_error)
   __pyx_v_self->eps = __pyx_t_2;
 
-  /* "cpprb/PyReplayBuffer.pyx":1877
+  /* "cpprb/PyReplayBuffer.pyx":1894
  *         self.eps = eps
  * 
  *         self.max_p = max_p or RawArray(ctypes.c_float,1)             # <<<<<<<<<<<<<<
  *         cdef float [:] view_max_p = self.max_p
  * 
  */
-  __Pyx_TraceLine(1877,0,__PYX_ERR(0, 1877, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_max_p); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 1877, __pyx_L1_error)
+  __Pyx_TraceLine(1894,0,__PYX_ERR(0, 1894, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_max_p); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 1894, __pyx_L1_error)
   if (!__pyx_t_4) {
   } else {
     __Pyx_INCREF(__pyx_v_max_p);
     __pyx_t_3 = __pyx_v_max_p;
     goto __pyx_L3_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_RawArray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1877, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_RawArray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1894, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1877, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1894, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_c_float); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1877, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_c_float); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1894, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
@@ -30830,130 +31036,130 @@
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_8, __pyx_int_1};
-    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1877, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1894, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_8, __pyx_int_1};
-    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1877, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1894, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   } else
   #endif
   {
-    __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1877, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1894, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_8);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_int_1);
     __pyx_t_8 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1877, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1894, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_INCREF(__pyx_t_5);
   __pyx_t_3 = __pyx_t_5;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_L3_bool_binop_done:;
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->max_p);
   __Pyx_DECREF(__pyx_v_self->max_p);
   __pyx_v_self->max_p = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1878
+  /* "cpprb/PyReplayBuffer.pyx":1895
  * 
  *         self.max_p = max_p or RawArray(ctypes.c_float,1)
  *         cdef float [:] view_max_p = self.max_p             # <<<<<<<<<<<<<<
  * 
  *         cdef size_t pow2size = 1
  */
-  __Pyx_TraceLine(1878,0,__PYX_ERR(0, 1878, __pyx_L1_error))
-  __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_self->max_p, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 1878, __pyx_L1_error)
+  __Pyx_TraceLine(1895,0,__PYX_ERR(0, 1895, __pyx_L1_error))
+  __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_self->max_p, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 1895, __pyx_L1_error)
   __pyx_v_view_max_p = __pyx_t_11;
   __pyx_t_11.memview = NULL;
   __pyx_t_11.data = NULL;
 
-  /* "cpprb/PyReplayBuffer.pyx":1880
+  /* "cpprb/PyReplayBuffer.pyx":1897
  *         cdef float [:] view_max_p = self.max_p
  * 
  *         cdef size_t pow2size = 1             # <<<<<<<<<<<<<<
  *         while pow2size < size:
  *             pow2size *= 2
  */
-  __Pyx_TraceLine(1880,0,__PYX_ERR(0, 1880, __pyx_L1_error))
+  __Pyx_TraceLine(1897,0,__PYX_ERR(0, 1897, __pyx_L1_error))
   __pyx_v_pow2size = 1;
 
-  /* "cpprb/PyReplayBuffer.pyx":1881
+  /* "cpprb/PyReplayBuffer.pyx":1898
  * 
  *         cdef size_t pow2size = 1
  *         while pow2size < size:             # <<<<<<<<<<<<<<
  *             pow2size *= 2
  * 
  */
-  __Pyx_TraceLine(1881,0,__PYX_ERR(0, 1881, __pyx_L1_error))
+  __Pyx_TraceLine(1898,0,__PYX_ERR(0, 1898, __pyx_L1_error))
   while (1) {
-    __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_pow2size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1881, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_pow2size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1898, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = PyObject_RichCompare(__pyx_t_3, __pyx_v_size, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1881, __pyx_L1_error)
+    __pyx_t_5 = PyObject_RichCompare(__pyx_t_3, __pyx_v_size, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1898, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 1881, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 1898, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (!__pyx_t_4) break;
 
-    /* "cpprb/PyReplayBuffer.pyx":1882
+    /* "cpprb/PyReplayBuffer.pyx":1899
  *         cdef size_t pow2size = 1
  *         while pow2size < size:
  *             pow2size *= 2             # <<<<<<<<<<<<<<
  * 
  *         self.sum   = sum   or RawArray(ctypes.c_float,2*pow2size-1)
  */
-    __Pyx_TraceLine(1882,0,__PYX_ERR(0, 1882, __pyx_L1_error))
+    __Pyx_TraceLine(1899,0,__PYX_ERR(0, 1899, __pyx_L1_error))
     __pyx_v_pow2size = (__pyx_v_pow2size * 2);
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1884
+  /* "cpprb/PyReplayBuffer.pyx":1901
  *             pow2size *= 2
  * 
  *         self.sum   = sum   or RawArray(ctypes.c_float,2*pow2size-1)             # <<<<<<<<<<<<<<
  *         self.sum_a = sum_a or RawArray(ctypes.c_bool ,1)
  *         self.min   = min   or RawArray(ctypes.c_float,2*pow2size-1)
  */
-  __Pyx_TraceLine(1884,0,__PYX_ERR(0, 1884, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_sum); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 1884, __pyx_L1_error)
+  __Pyx_TraceLine(1901,0,__PYX_ERR(0, 1901, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_sum); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 1901, __pyx_L1_error)
   if (!__pyx_t_4) {
   } else {
     __Pyx_INCREF(__pyx_v_sum);
     __pyx_t_5 = __pyx_v_sum;
     goto __pyx_L7_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_RawArray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1884, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_RawArray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1901, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1884, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1901, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_c_float); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1884, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_c_float); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1901, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_PyInt_FromSize_t(((2 * __pyx_v_pow2size) - 1)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1884, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_FromSize_t(((2 * __pyx_v_pow2size) - 1)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1901, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __pyx_t_7 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -30962,78 +31168,78 @@
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_8, __pyx_t_10};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1884, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1901, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_8, __pyx_t_10};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1884, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1901, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   } else
   #endif
   {
-    __pyx_t_12 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1884, __pyx_L1_error)
+    __pyx_t_12 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1901, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_9, __pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_10);
     PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_9, __pyx_t_10);
     __pyx_t_8 = 0;
     __pyx_t_10 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1884, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1901, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_INCREF(__pyx_t_3);
   __pyx_t_5 = __pyx_t_3;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_L7_bool_binop_done:;
   __Pyx_GIVEREF(__pyx_t_5);
   __Pyx_GOTREF(__pyx_v_self->sum);
   __Pyx_DECREF(__pyx_v_self->sum);
   __pyx_v_self->sum = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1885
+  /* "cpprb/PyReplayBuffer.pyx":1902
  * 
  *         self.sum   = sum   or RawArray(ctypes.c_float,2*pow2size-1)
  *         self.sum_a = sum_a or RawArray(ctypes.c_bool ,1)             # <<<<<<<<<<<<<<
  *         self.min   = min   or RawArray(ctypes.c_float,2*pow2size-1)
  *         self.min_a = min_a or RawArray(ctypes.c_bool ,1)
  */
-  __Pyx_TraceLine(1885,0,__PYX_ERR(0, 1885, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_sum_a); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 1885, __pyx_L1_error)
+  __Pyx_TraceLine(1902,0,__PYX_ERR(0, 1902, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_sum_a); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 1902, __pyx_L1_error)
   if (!__pyx_t_4) {
   } else {
     __Pyx_INCREF(__pyx_v_sum_a);
     __pyx_t_5 = __pyx_v_sum_a;
     goto __pyx_L9_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_RawArray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1885, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_RawArray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1902, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1885, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1902, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_c_bool); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1885, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_c_bool); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1902, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __pyx_t_12 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_12)) {
@@ -31043,79 +31249,79 @@
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_12, __pyx_t_10, __pyx_int_1};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1885, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1902, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_12, __pyx_t_10, __pyx_int_1};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1885, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1902, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1885, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1902, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_12) {
       __Pyx_GIVEREF(__pyx_t_12); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_12); __pyx_t_12 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_10);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_9, __pyx_t_10);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_9, __pyx_int_1);
     __pyx_t_10 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1885, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1902, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_INCREF(__pyx_t_3);
   __pyx_t_5 = __pyx_t_3;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_L9_bool_binop_done:;
   __Pyx_GIVEREF(__pyx_t_5);
   __Pyx_GOTREF(__pyx_v_self->sum_a);
   __Pyx_DECREF(__pyx_v_self->sum_a);
   __pyx_v_self->sum_a = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1886
+  /* "cpprb/PyReplayBuffer.pyx":1903
  *         self.sum   = sum   or RawArray(ctypes.c_float,2*pow2size-1)
  *         self.sum_a = sum_a or RawArray(ctypes.c_bool ,1)
  *         self.min   = min   or RawArray(ctypes.c_float,2*pow2size-1)             # <<<<<<<<<<<<<<
  *         self.min_a = min_a or RawArray(ctypes.c_bool ,1)
  * 
  */
-  __Pyx_TraceLine(1886,0,__PYX_ERR(0, 1886, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_min); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 1886, __pyx_L1_error)
+  __Pyx_TraceLine(1903,0,__PYX_ERR(0, 1903, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_min); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 1903, __pyx_L1_error)
   if (!__pyx_t_4) {
   } else {
     __Pyx_INCREF(__pyx_v_min);
     __pyx_t_5 = __pyx_v_min;
     goto __pyx_L11_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_RawArray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1886, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_RawArray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1903, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1886, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1903, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_c_float); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1886, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_c_float); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1903, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyInt_FromSize_t(((2 * __pyx_v_pow2size) - 1)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1886, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_FromSize_t(((2 * __pyx_v_pow2size) - 1)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1903, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_12 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_12)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -31124,78 +31330,78 @@
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_12, __pyx_t_10, __pyx_t_8};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1886, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1903, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_12, __pyx_t_10, __pyx_t_8};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1886, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1903, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1886, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1903, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_12) {
       __Pyx_GIVEREF(__pyx_t_12); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_12); __pyx_t_12 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_10);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_9, __pyx_t_10);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_9, __pyx_t_8);
     __pyx_t_10 = 0;
     __pyx_t_8 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1886, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1903, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_INCREF(__pyx_t_3);
   __pyx_t_5 = __pyx_t_3;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_L11_bool_binop_done:;
   __Pyx_GIVEREF(__pyx_t_5);
   __Pyx_GOTREF(__pyx_v_self->min);
   __Pyx_DECREF(__pyx_v_self->min);
   __pyx_v_self->min = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1887
+  /* "cpprb/PyReplayBuffer.pyx":1904
  *         self.sum_a = sum_a or RawArray(ctypes.c_bool ,1)
  *         self.min   = min   or RawArray(ctypes.c_float,2*pow2size-1)
  *         self.min_a = min_a or RawArray(ctypes.c_bool ,1)             # <<<<<<<<<<<<<<
  * 
  *         cdef float [:] view_sum   = self.sum
  */
-  __Pyx_TraceLine(1887,0,__PYX_ERR(0, 1887, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_min_a); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 1887, __pyx_L1_error)
+  __Pyx_TraceLine(1904,0,__PYX_ERR(0, 1904, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_min_a); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 1904, __pyx_L1_error)
   if (!__pyx_t_4) {
   } else {
     __Pyx_INCREF(__pyx_v_min_a);
     __pyx_t_5 = __pyx_v_min_a;
     goto __pyx_L13_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_RawArray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1887, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_RawArray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1904, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1887, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1904, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_c_bool); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1887, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_c_bool); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1904, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
@@ -31205,314 +31411,314 @@
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_8, __pyx_int_1};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1887, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1904, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_8, __pyx_int_1};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1887, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1904, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   } else
   #endif
   {
-    __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1887, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 1904, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_8);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_int_1);
     __pyx_t_8 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1887, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1904, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_INCREF(__pyx_t_3);
   __pyx_t_5 = __pyx_t_3;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_L13_bool_binop_done:;
   __Pyx_GIVEREF(__pyx_t_5);
   __Pyx_GOTREF(__pyx_v_self->min_a);
   __Pyx_DECREF(__pyx_v_self->min_a);
   __pyx_v_self->min_a = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1889
+  /* "cpprb/PyReplayBuffer.pyx":1906
  *         self.min_a = min_a or RawArray(ctypes.c_bool ,1)
  * 
  *         cdef float [:] view_sum   = self.sum             # <<<<<<<<<<<<<<
  *         cdef bool  [:] view_sum_a = self.sum_a
  *         cdef float [:] view_min   = self.min
  */
-  __Pyx_TraceLine(1889,0,__PYX_ERR(0, 1889, __pyx_L1_error))
-  __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_self->sum, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 1889, __pyx_L1_error)
+  __Pyx_TraceLine(1906,0,__PYX_ERR(0, 1906, __pyx_L1_error))
+  __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_self->sum, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 1906, __pyx_L1_error)
   __pyx_v_view_sum = __pyx_t_11;
   __pyx_t_11.memview = NULL;
   __pyx_t_11.data = NULL;
 
-  /* "cpprb/PyReplayBuffer.pyx":1890
+  /* "cpprb/PyReplayBuffer.pyx":1907
  * 
  *         cdef float [:] view_sum   = self.sum
  *         cdef bool  [:] view_sum_a = self.sum_a             # <<<<<<<<<<<<<<
  *         cdef float [:] view_min   = self.min
  *         cdef bool  [:] view_min_a = self.min_a
  */
-  __Pyx_TraceLine(1890,0,__PYX_ERR(0, 1890, __pyx_L1_error))
-  __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_bool(__pyx_v_self->sum_a, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 1890, __pyx_L1_error)
+  __Pyx_TraceLine(1907,0,__PYX_ERR(0, 1907, __pyx_L1_error))
+  __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_bool(__pyx_v_self->sum_a, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 1907, __pyx_L1_error)
   __pyx_v_view_sum_a = __pyx_t_13;
   __pyx_t_13.memview = NULL;
   __pyx_t_13.data = NULL;
 
-  /* "cpprb/PyReplayBuffer.pyx":1891
+  /* "cpprb/PyReplayBuffer.pyx":1908
  *         cdef float [:] view_sum   = self.sum
  *         cdef bool  [:] view_sum_a = self.sum_a
  *         cdef float [:] view_min   = self.min             # <<<<<<<<<<<<<<
  *         cdef bool  [:] view_min_a = self.min_a
  * 
  */
-  __Pyx_TraceLine(1891,0,__PYX_ERR(0, 1891, __pyx_L1_error))
-  __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_self->min, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 1891, __pyx_L1_error)
+  __Pyx_TraceLine(1908,0,__PYX_ERR(0, 1908, __pyx_L1_error))
+  __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_self->min, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 1908, __pyx_L1_error)
   __pyx_v_view_min = __pyx_t_11;
   __pyx_t_11.memview = NULL;
   __pyx_t_11.data = NULL;
 
-  /* "cpprb/PyReplayBuffer.pyx":1892
+  /* "cpprb/PyReplayBuffer.pyx":1909
  *         cdef bool  [:] view_sum_a = self.sum_a
  *         cdef float [:] view_min   = self.min
  *         cdef bool  [:] view_min_a = self.min_a             # <<<<<<<<<<<<<<
  * 
  *         cdef bool init = ((max_p is None) and
  */
-  __Pyx_TraceLine(1892,0,__PYX_ERR(0, 1892, __pyx_L1_error))
-  __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_bool(__pyx_v_self->min_a, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 1892, __pyx_L1_error)
+  __Pyx_TraceLine(1909,0,__PYX_ERR(0, 1909, __pyx_L1_error))
+  __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_bool(__pyx_v_self->min_a, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 1909, __pyx_L1_error)
   __pyx_v_view_min_a = __pyx_t_13;
   __pyx_t_13.memview = NULL;
   __pyx_t_13.data = NULL;
 
-  /* "cpprb/PyReplayBuffer.pyx":1894
+  /* "cpprb/PyReplayBuffer.pyx":1911
  *         cdef bool  [:] view_min_a = self.min_a
  * 
  *         cdef bool init = ((max_p is None) and             # <<<<<<<<<<<<<<
  *                           (sum   is None) and
  *                           (sum_a is None) and
  */
-  __Pyx_TraceLine(1894,0,__PYX_ERR(0, 1894, __pyx_L1_error))
+  __Pyx_TraceLine(1911,0,__PYX_ERR(0, 1911, __pyx_L1_error))
   __pyx_t_4 = (__pyx_v_max_p == Py_None);
   if (__pyx_t_4) {
   } else {
     __pyx_t_14 = __pyx_t_4;
     goto __pyx_L15_bool_binop_done;
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1895
+  /* "cpprb/PyReplayBuffer.pyx":1912
  * 
  *         cdef bool init = ((max_p is None) and
  *                           (sum   is None) and             # <<<<<<<<<<<<<<
  *                           (sum_a is None) and
  *                           (min   is None) and
  */
-  __Pyx_TraceLine(1895,0,__PYX_ERR(0, 1895, __pyx_L1_error))
+  __Pyx_TraceLine(1912,0,__PYX_ERR(0, 1912, __pyx_L1_error))
   __pyx_t_4 = (__pyx_v_sum == Py_None);
   if (__pyx_t_4) {
   } else {
     __pyx_t_14 = __pyx_t_4;
     goto __pyx_L15_bool_binop_done;
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1896
+  /* "cpprb/PyReplayBuffer.pyx":1913
  *         cdef bool init = ((max_p is None) and
  *                           (sum   is None) and
  *                           (sum_a is None) and             # <<<<<<<<<<<<<<
  *                           (min   is None) and
  *                           (min_a is None))
  */
-  __Pyx_TraceLine(1896,0,__PYX_ERR(0, 1896, __pyx_L1_error))
+  __Pyx_TraceLine(1913,0,__PYX_ERR(0, 1913, __pyx_L1_error))
   __pyx_t_4 = (__pyx_v_sum_a == Py_None);
   if (__pyx_t_4) {
   } else {
     __pyx_t_14 = __pyx_t_4;
     goto __pyx_L15_bool_binop_done;
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1897
+  /* "cpprb/PyReplayBuffer.pyx":1914
  *                           (sum   is None) and
  *                           (sum_a is None) and
  *                           (min   is None) and             # <<<<<<<<<<<<<<
  *                           (min_a is None))
  * 
  */
-  __Pyx_TraceLine(1897,0,__PYX_ERR(0, 1897, __pyx_L1_error))
+  __Pyx_TraceLine(1914,0,__PYX_ERR(0, 1914, __pyx_L1_error))
   __pyx_t_4 = (__pyx_v_min == Py_None);
   if (__pyx_t_4) {
   } else {
     __pyx_t_14 = __pyx_t_4;
     goto __pyx_L15_bool_binop_done;
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1898
+  /* "cpprb/PyReplayBuffer.pyx":1915
  *                           (sum_a is None) and
  *                           (min   is None) and
  *                           (min_a is None))             # <<<<<<<<<<<<<<
  * 
  *         self.per = new CppThreadSafePrioritizedSampler[float](size,alpha,
  */
-  __Pyx_TraceLine(1898,0,__PYX_ERR(0, 1898, __pyx_L1_error))
+  __Pyx_TraceLine(1915,0,__PYX_ERR(0, 1915, __pyx_L1_error))
   __pyx_t_4 = (__pyx_v_min_a == Py_None);
   __pyx_t_14 = __pyx_t_4;
   __pyx_L15_bool_binop_done:;
   __pyx_v_init = __pyx_t_14;
 
-  /* "cpprb/PyReplayBuffer.pyx":1900
+  /* "cpprb/PyReplayBuffer.pyx":1917
  *                           (min_a is None))
  * 
  *         self.per = new CppThreadSafePrioritizedSampler[float](size,alpha,             # <<<<<<<<<<<<<<
  *                                                               &view_max_p[0],
  *                                                               &view_sum[0],
  */
-  __Pyx_TraceLine(1900,0,__PYX_ERR(0, 1900, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_size); if (unlikely((__pyx_t_1 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1900, __pyx_L1_error)
-  __pyx_t_2 = __pyx_PyFloat_AsFloat(__pyx_v_alpha); if (unlikely((__pyx_t_2 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1900, __pyx_L1_error)
+  __Pyx_TraceLine(1917,0,__PYX_ERR(0, 1917, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_size); if (unlikely((__pyx_t_1 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1917, __pyx_L1_error)
+  __pyx_t_2 = __pyx_PyFloat_AsFloat(__pyx_v_alpha); if (unlikely((__pyx_t_2 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1917, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":1901
+  /* "cpprb/PyReplayBuffer.pyx":1918
  * 
  *         self.per = new CppThreadSafePrioritizedSampler[float](size,alpha,
  *                                                               &view_max_p[0],             # <<<<<<<<<<<<<<
  *                                                               &view_sum[0],
  *                                                               &view_sum_a[0],
  */
-  __Pyx_TraceLine(1901,0,__PYX_ERR(0, 1901, __pyx_L1_error))
+  __Pyx_TraceLine(1918,0,__PYX_ERR(0, 1918, __pyx_L1_error))
   __pyx_t_15 = 0;
   __pyx_t_9 = -1;
   if (__pyx_t_15 < 0) {
     __pyx_t_15 += __pyx_v_view_max_p.shape[0];
     if (unlikely(__pyx_t_15 < 0)) __pyx_t_9 = 0;
   } else if (unlikely(__pyx_t_15 >= __pyx_v_view_max_p.shape[0])) __pyx_t_9 = 0;
   if (unlikely(__pyx_t_9 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_9);
-    __PYX_ERR(0, 1901, __pyx_L1_error)
+    __PYX_ERR(0, 1918, __pyx_L1_error)
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1902
+  /* "cpprb/PyReplayBuffer.pyx":1919
  *         self.per = new CppThreadSafePrioritizedSampler[float](size,alpha,
  *                                                               &view_max_p[0],
  *                                                               &view_sum[0],             # <<<<<<<<<<<<<<
  *                                                               &view_sum_a[0],
  *                                                               &view_min[0],
  */
-  __Pyx_TraceLine(1902,0,__PYX_ERR(0, 1902, __pyx_L1_error))
+  __Pyx_TraceLine(1919,0,__PYX_ERR(0, 1919, __pyx_L1_error))
   __pyx_t_16 = 0;
   __pyx_t_9 = -1;
   if (__pyx_t_16 < 0) {
     __pyx_t_16 += __pyx_v_view_sum.shape[0];
     if (unlikely(__pyx_t_16 < 0)) __pyx_t_9 = 0;
   } else if (unlikely(__pyx_t_16 >= __pyx_v_view_sum.shape[0])) __pyx_t_9 = 0;
   if (unlikely(__pyx_t_9 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_9);
-    __PYX_ERR(0, 1902, __pyx_L1_error)
+    __PYX_ERR(0, 1919, __pyx_L1_error)
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1903
+  /* "cpprb/PyReplayBuffer.pyx":1920
  *                                                               &view_max_p[0],
  *                                                               &view_sum[0],
  *                                                               &view_sum_a[0],             # <<<<<<<<<<<<<<
  *                                                               &view_min[0],
  *                                                               &view_min_a[0],
  */
-  __Pyx_TraceLine(1903,0,__PYX_ERR(0, 1903, __pyx_L1_error))
+  __Pyx_TraceLine(1920,0,__PYX_ERR(0, 1920, __pyx_L1_error))
   __pyx_t_17 = 0;
   __pyx_t_9 = -1;
   if (__pyx_t_17 < 0) {
     __pyx_t_17 += __pyx_v_view_sum_a.shape[0];
     if (unlikely(__pyx_t_17 < 0)) __pyx_t_9 = 0;
   } else if (unlikely(__pyx_t_17 >= __pyx_v_view_sum_a.shape[0])) __pyx_t_9 = 0;
   if (unlikely(__pyx_t_9 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_9);
-    __PYX_ERR(0, 1903, __pyx_L1_error)
+    __PYX_ERR(0, 1920, __pyx_L1_error)
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1904
+  /* "cpprb/PyReplayBuffer.pyx":1921
  *                                                               &view_sum[0],
  *                                                               &view_sum_a[0],
  *                                                               &view_min[0],             # <<<<<<<<<<<<<<
  *                                                               &view_min_a[0],
  *                                                               init,
  */
-  __Pyx_TraceLine(1904,0,__PYX_ERR(0, 1904, __pyx_L1_error))
+  __Pyx_TraceLine(1921,0,__PYX_ERR(0, 1921, __pyx_L1_error))
   __pyx_t_18 = 0;
   __pyx_t_9 = -1;
   if (__pyx_t_18 < 0) {
     __pyx_t_18 += __pyx_v_view_min.shape[0];
     if (unlikely(__pyx_t_18 < 0)) __pyx_t_9 = 0;
   } else if (unlikely(__pyx_t_18 >= __pyx_v_view_min.shape[0])) __pyx_t_9 = 0;
   if (unlikely(__pyx_t_9 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_9);
-    __PYX_ERR(0, 1904, __pyx_L1_error)
+    __PYX_ERR(0, 1921, __pyx_L1_error)
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1905
+  /* "cpprb/PyReplayBuffer.pyx":1922
  *                                                               &view_sum_a[0],
  *                                                               &view_min[0],
  *                                                               &view_min_a[0],             # <<<<<<<<<<<<<<
  *                                                               init,
  *                                                               eps)
  */
-  __Pyx_TraceLine(1905,0,__PYX_ERR(0, 1905, __pyx_L1_error))
+  __Pyx_TraceLine(1922,0,__PYX_ERR(0, 1922, __pyx_L1_error))
   __pyx_t_19 = 0;
   __pyx_t_9 = -1;
   if (__pyx_t_19 < 0) {
     __pyx_t_19 += __pyx_v_view_min_a.shape[0];
     if (unlikely(__pyx_t_19 < 0)) __pyx_t_9 = 0;
   } else if (unlikely(__pyx_t_19 >= __pyx_v_view_min_a.shape[0])) __pyx_t_9 = 0;
   if (unlikely(__pyx_t_9 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_9);
-    __PYX_ERR(0, 1905, __pyx_L1_error)
+    __PYX_ERR(0, 1922, __pyx_L1_error)
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1907
+  /* "cpprb/PyReplayBuffer.pyx":1924
  *                                                               &view_min_a[0],
  *                                                               init,
  *                                                               eps)             # <<<<<<<<<<<<<<
  * 
  *     cdef CppThreadSafePrioritizedSampler[float]* ptr(self):
  */
-  __Pyx_TraceLine(1907,0,__PYX_ERR(0, 1907, __pyx_L1_error))
-  __pyx_t_20 = __pyx_PyFloat_AsFloat(__pyx_v_eps); if (unlikely((__pyx_t_20 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1907, __pyx_L1_error)
+  __Pyx_TraceLine(1924,0,__PYX_ERR(0, 1924, __pyx_L1_error))
+  __pyx_t_20 = __pyx_PyFloat_AsFloat(__pyx_v_eps); if (unlikely((__pyx_t_20 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 1924, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":1900
+  /* "cpprb/PyReplayBuffer.pyx":1917
  *                           (min_a is None))
  * 
  *         self.per = new CppThreadSafePrioritizedSampler[float](size,alpha,             # <<<<<<<<<<<<<<
  *                                                               &view_max_p[0],
  *                                                               &view_sum[0],
  */
-  __Pyx_TraceLine(1900,0,__PYX_ERR(0, 1900, __pyx_L1_error))
+  __Pyx_TraceLine(1917,0,__PYX_ERR(0, 1917, __pyx_L1_error))
   try {
     __pyx_t_21 = new ymd::CppThreadSafePrioritizedSampler<float> (__pyx_t_1, __pyx_t_2, (&(*((float *) ( /* dim=0 */ (__pyx_v_view_max_p.data + __pyx_t_15 * __pyx_v_view_max_p.strides[0]) )))), (&(*((float *) ( /* dim=0 */ (__pyx_v_view_sum.data + __pyx_t_16 * __pyx_v_view_sum.strides[0]) )))), (&(*((bool *) ( /* dim=0 */ (__pyx_v_view_sum_a.data + __pyx_t_17 * __pyx_v_view_sum_a.strides[0]) )))), (&(*((float *) ( /* dim=0 */ (__pyx_v_view_min.data + __pyx_t_18 * __pyx_v_view_min.strides[0]) )))), (&(*((bool *) ( /* dim=0 */ (__pyx_v_view_min_a.data + __pyx_t_19 * __pyx_v_view_min_a.strides[0]) )))), __pyx_v_init, __pyx_t_20);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 1900, __pyx_L1_error)
+    __PYX_ERR(0, 1917, __pyx_L1_error)
   }
   __pyx_v_self->per = __pyx_t_21;
 
-  /* "cpprb/PyReplayBuffer.pyx":1870
+  /* "cpprb/PyReplayBuffer.pyx":1887
  *     cdef CppThreadSafePrioritizedSampler[float]* per
  * 
  *     def __init__(self,size,alpha,eps,max_p=None,             # <<<<<<<<<<<<<<
  *                  sum=None,sum_a=None,
  *                  min=None,min_a=None):
  */
 
@@ -31538,15 +31744,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_view_min, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_view_min_a, 1);
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1909
+/* "cpprb/PyReplayBuffer.pyx":1926
  *                                                               eps)
  * 
  *     cdef CppThreadSafePrioritizedSampler[float]* ptr(self):             # <<<<<<<<<<<<<<
  *         return self.per
  * 
  */
 
@@ -31554,28 +31760,28 @@
   ymd::CppThreadSafePrioritizedSampler<float>  *__pyx_r;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("ptr", 0);
-  __Pyx_TraceCall("ptr", __pyx_f[0], 1909, 0, __PYX_ERR(0, 1909, __pyx_L1_error));
+  __Pyx_TraceCall("ptr", __pyx_f[0], 1926, 0, __PYX_ERR(0, 1926, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1910
+  /* "cpprb/PyReplayBuffer.pyx":1927
  * 
  *     cdef CppThreadSafePrioritizedSampler[float]* ptr(self):
  *         return self.per             # <<<<<<<<<<<<<<
  * 
  *     def __reduce__(self):
  */
-  __Pyx_TraceLine(1910,0,__PYX_ERR(0, 1910, __pyx_L1_error))
+  __Pyx_TraceLine(1927,0,__PYX_ERR(0, 1927, __pyx_L1_error))
   __pyx_r = __pyx_v_self->per;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1909
+  /* "cpprb/PyReplayBuffer.pyx":1926
  *                                                               eps)
  * 
  *     cdef CppThreadSafePrioritizedSampler[float]* ptr(self):             # <<<<<<<<<<<<<<
  *         return self.per
  * 
  */
 
@@ -31585,15 +31791,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1912
+/* "cpprb/PyReplayBuffer.pyx":1929
  *         return self.per
  * 
  *     def __reduce__(self):             # <<<<<<<<<<<<<<
  *         return (ThreadSafePrioritizedSampler,
  *                 (self.size,self.alpha,self.eps,self.max_p,
  */
 
@@ -31618,50 +31824,50 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce__", 0);
-  __Pyx_TraceCall("__reduce__", __pyx_f[0], 1912, 0, __PYX_ERR(0, 1912, __pyx_L1_error));
+  __Pyx_TraceCall("__reduce__", __pyx_f[0], 1929, 0, __PYX_ERR(0, 1929, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1913
+  /* "cpprb/PyReplayBuffer.pyx":1930
  * 
  *     def __reduce__(self):
  *         return (ThreadSafePrioritizedSampler,             # <<<<<<<<<<<<<<
  *                 (self.size,self.alpha,self.eps,self.max_p,
  *                  self.sum,self.sum_a,
  */
-  __Pyx_TraceLine(1913,0,__PYX_ERR(0, 1913, __pyx_L1_error))
+  __Pyx_TraceLine(1930,0,__PYX_ERR(0, 1930, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
 
-  /* "cpprb/PyReplayBuffer.pyx":1914
+  /* "cpprb/PyReplayBuffer.pyx":1931
  *     def __reduce__(self):
  *         return (ThreadSafePrioritizedSampler,
  *                 (self.size,self.alpha,self.eps,self.max_p,             # <<<<<<<<<<<<<<
  *                  self.sum,self.sum_a,
  *                  self.min,self.min_a))
  */
-  __Pyx_TraceLine(1914,0,__PYX_ERR(0, 1914, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_self->size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1914, __pyx_L1_error)
+  __Pyx_TraceLine(1931,0,__PYX_ERR(0, 1931, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_self->size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1931, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_self->alpha); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1914, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_self->alpha); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1931, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_self->eps); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1914, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_self->eps); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1931, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "cpprb/PyReplayBuffer.pyx":1916
+  /* "cpprb/PyReplayBuffer.pyx":1933
  *                 (self.size,self.alpha,self.eps,self.max_p,
  *                  self.sum,self.sum_a,
  *                  self.min,self.min_a))             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(1916,0,__PYX_ERR(0, 1916, __pyx_L1_error))
-  __pyx_t_4 = PyTuple_New(8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1914, __pyx_L1_error)
+  __Pyx_TraceLine(1933,0,__PYX_ERR(0, 1933, __pyx_L1_error))
+  __pyx_t_4 = PyTuple_New(8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1931, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
@@ -31680,35 +31886,35 @@
   __Pyx_INCREF(__pyx_v_self->min_a);
   __Pyx_GIVEREF(__pyx_v_self->min_a);
   PyTuple_SET_ITEM(__pyx_t_4, 7, __pyx_v_self->min_a);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1913
+  /* "cpprb/PyReplayBuffer.pyx":1930
  * 
  *     def __reduce__(self):
  *         return (ThreadSafePrioritizedSampler,             # <<<<<<<<<<<<<<
  *                 (self.size,self.alpha,self.eps,self.max_p,
  *                  self.sum,self.sum_a,
  */
-  __Pyx_TraceLine(1913,0,__PYX_ERR(0, 1913, __pyx_L1_error))
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1913, __pyx_L1_error)
+  __Pyx_TraceLine(1930,0,__PYX_ERR(0, 1930, __pyx_L1_error))
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1930, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler));
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4);
   __pyx_t_4 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1912
+  /* "cpprb/PyReplayBuffer.pyx":1929
  *         return self.per
  * 
  *     def __reduce__(self):             # <<<<<<<<<<<<<<
  *         return (ThreadSafePrioritizedSampler,
  *                 (self.size,self.alpha,self.eps,self.max_p,
  */
 
@@ -31723,15 +31929,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1944
+/* "cpprb/PyReplayBuffer.pyx":1961
  *     cdef vector[float] ps_vec
  * 
  *     def __init__(self,size,env_dict=None,*,alpha=0.6,eps=1e-4,**kwargs):             # <<<<<<<<<<<<<<
  *         r"""Initialize PrioritizedReplayBuffer
  * 
  */
 
@@ -31788,15 +31994,15 @@
         Py_ssize_t index;
         for (index = 2; index < 4 && kw_args > 0; index++) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1944, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1961, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -31806,15 +32012,15 @@
     __pyx_v_size = values[0];
     __pyx_v_env_dict = values[1];
     __pyx_v_alpha = values[2];
     __pyx_v_eps = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1944, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1961, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPPrioritizedReplayBuffer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer___init__(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self), __pyx_v_size, __pyx_v_env_dict, __pyx_v_alpha, __pyx_v_eps, __pyx_v_kwargs);
@@ -31841,133 +32047,133 @@
   int __pyx_t_9;
   std::vector<size_t>  __pyx_t_10;
   std::vector<float>  __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
-  __Pyx_TraceCall("__init__", __pyx_f[0], 1944, 0, __PYX_ERR(0, 1944, __pyx_L1_error));
+  __Pyx_TraceCall("__init__", __pyx_f[0], 1961, 0, __PYX_ERR(0, 1961, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1973
+  /* "cpprb/PyReplayBuffer.pyx":1990
  *         enable fast sampling.
  *         """
  *         super().__init__(size,env_dict,**kwargs)             # <<<<<<<<<<<<<<
  * 
  *         self.per = ThreadSafePrioritizedSampler(size,alpha,eps)
  */
-  __Pyx_TraceLine(1973,0,__PYX_ERR(0, 1973, __pyx_L1_error))
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1973, __pyx_L1_error)
+  __Pyx_TraceLine(1990,0,__PYX_ERR(0, 1990, __pyx_L1_error))
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer));
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)__pyx_v_self));
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1973, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_init); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1973, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_init); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1973, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_size);
   __Pyx_GIVEREF(__pyx_v_size);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_size);
   __Pyx_INCREF(__pyx_v_env_dict);
   __Pyx_GIVEREF(__pyx_v_env_dict);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_env_dict);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_v_kwargs); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1973, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_v_kwargs); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1975
+  /* "cpprb/PyReplayBuffer.pyx":1992
  *         super().__init__(size,env_dict,**kwargs)
  * 
  *         self.per = ThreadSafePrioritizedSampler(size,alpha,eps)             # <<<<<<<<<<<<<<
  * 
  *         self.weights = VectorFloat()
  */
-  __Pyx_TraceLine(1975,0,__PYX_ERR(0, 1975, __pyx_L1_error))
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1975, __pyx_L1_error)
+  __Pyx_TraceLine(1992,0,__PYX_ERR(0, 1992, __pyx_L1_error))
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1992, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_size);
   __Pyx_GIVEREF(__pyx_v_size);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_size);
   __Pyx_INCREF(__pyx_v_alpha);
   __Pyx_GIVEREF(__pyx_v_alpha);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_alpha);
   __Pyx_INCREF(__pyx_v_eps);
   __Pyx_GIVEREF(__pyx_v_eps);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_v_eps);
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1975, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1992, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->per);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->per));
   __pyx_v_self->per = ((struct __pyx_obj_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1977
+  /* "cpprb/PyReplayBuffer.pyx":1994
  *         self.per = ThreadSafePrioritizedSampler(size,alpha,eps)
  * 
  *         self.weights = VectorFloat()             # <<<<<<<<<<<<<<
  *         self.indexes = VectorSize_t()
  * 
  */
-  __Pyx_TraceLine(1977,0,__PYX_ERR(0, 1977, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_5cpprb_13VectorWrapper_VectorFloat)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1977, __pyx_L1_error)
+  __Pyx_TraceLine(1994,0,__PYX_ERR(0, 1994, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_5cpprb_13VectorWrapper_VectorFloat)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1994, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->weights);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->weights));
   __pyx_v_self->weights = ((struct __pyx_obj_5cpprb_13VectorWrapper_VectorFloat *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1978
+  /* "cpprb/PyReplayBuffer.pyx":1995
  * 
  *         self.weights = VectorFloat()
  *         self.indexes = VectorSize_t()             # <<<<<<<<<<<<<<
  * 
  *         shm = RawArray(np.ctypeslib.as_ctypes_type(np.bool_),
  */
-  __Pyx_TraceLine(1978,0,__PYX_ERR(0, 1978, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_5cpprb_13VectorWrapper_VectorSize_t)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1978, __pyx_L1_error)
+  __Pyx_TraceLine(1995,0,__PYX_ERR(0, 1995, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_5cpprb_13VectorWrapper_VectorSize_t)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1995, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->indexes);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->indexes));
   __pyx_v_self->indexes = ((struct __pyx_obj_5cpprb_13VectorWrapper_VectorSize_t *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1980
+  /* "cpprb/PyReplayBuffer.pyx":1997
  *         self.indexes = VectorSize_t()
  * 
  *         shm = RawArray(np.ctypeslib.as_ctypes_type(np.bool_),             # <<<<<<<<<<<<<<
  *                        int(np.array(size,copy=False,dtype='int').prod()))
  *         self.unchange_since_sample = np.ctypeslib.as_array(shm)
  */
-  __Pyx_TraceLine(1980,0,__PYX_ERR(0, 1980, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_RawArray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1980, __pyx_L1_error)
+  __Pyx_TraceLine(1997,0,__PYX_ERR(0, 1997, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_RawArray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1997, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1980, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1997, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ctypeslib); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1980, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ctypeslib); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1997, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_as_ctypes_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1980, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_as_ctypes_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1997, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1980, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1997, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_bool_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1980, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_bool_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1997, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -31975,64 +32181,64 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1980, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1997, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1981
+  /* "cpprb/PyReplayBuffer.pyx":1998
  * 
  *         shm = RawArray(np.ctypeslib.as_ctypes_type(np.bool_),
  *                        int(np.array(size,copy=False,dtype='int').prod()))             # <<<<<<<<<<<<<<
  *         self.unchange_since_sample = np.ctypeslib.as_array(shm)
  *         self.unchange_since_sample[:] = True
  */
-  __Pyx_TraceLine(1981,0,__PYX_ERR(0, 1981, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1981, __pyx_L1_error)
+  __Pyx_TraceLine(1998,0,__PYX_ERR(0, 1998, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1998, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_array); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1981, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_array); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1998, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1981, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1998, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_v_size);
   __Pyx_GIVEREF(__pyx_v_size);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_size);
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1981, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1998, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1981, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_n_u_int) < 0) __PYX_ERR(0, 1981, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1981, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 1998, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_n_u_int) < 0) __PYX_ERR(0, 1998, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1998, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_prod); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1981, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_prod); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1998, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1981, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1998, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyNumber_Int(__pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1981, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyNumber_Int(__pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1998, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -32042,125 +32248,125 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_1, __pyx_t_7};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1980, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1997, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_1, __pyx_t_7};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1980, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1997, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1980, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1997, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_9, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_9, __pyx_t_7);
     __pyx_t_1 = 0;
     __pyx_t_7 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1980, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1997, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_shm = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1982
+  /* "cpprb/PyReplayBuffer.pyx":1999
  *         shm = RawArray(np.ctypeslib.as_ctypes_type(np.bool_),
  *                        int(np.array(size,copy=False,dtype='int').prod()))
  *         self.unchange_since_sample = np.ctypeslib.as_array(shm)             # <<<<<<<<<<<<<<
  *         self.unchange_since_sample[:] = True
  * 
  */
-  __Pyx_TraceLine(1982,0,__PYX_ERR(0, 1982, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1982, __pyx_L1_error)
+  __Pyx_TraceLine(1999,0,__PYX_ERR(0, 1999, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1999, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ctypeslib); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1982, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ctypeslib); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1999, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_as_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1982, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_as_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1999, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_8, __pyx_v_shm) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_shm);
   __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1982, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1999, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->unchange_since_sample);
   __Pyx_DECREF(__pyx_v_self->unchange_since_sample);
   __pyx_v_self->unchange_since_sample = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1983
+  /* "cpprb/PyReplayBuffer.pyx":2000
  *                        int(np.array(size,copy=False,dtype='int').prod()))
  *         self.unchange_since_sample = np.ctypeslib.as_array(shm)
  *         self.unchange_since_sample[:] = True             # <<<<<<<<<<<<<<
  * 
  *         self.helper = None
  */
-  __Pyx_TraceLine(1983,0,__PYX_ERR(0, 1983, __pyx_L1_error))
-  if (__Pyx_PyObject_SetSlice(__pyx_v_self->unchange_since_sample, Py_True, 0, 0, NULL, NULL, &__pyx_slice__16, 0, 0, 1) < 0) __PYX_ERR(0, 1983, __pyx_L1_error)
+  __Pyx_TraceLine(2000,0,__PYX_ERR(0, 2000, __pyx_L1_error))
+  if (__Pyx_PyObject_SetSlice(__pyx_v_self->unchange_since_sample, Py_True, 0, 0, NULL, NULL, &__pyx_slice__16, 0, 0, 1) < 0) __PYX_ERR(0, 2000, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":1985
+  /* "cpprb/PyReplayBuffer.pyx":2002
  *         self.unchange_since_sample[:] = True
  * 
  *         self.helper = None             # <<<<<<<<<<<<<<
  *         self.terminate = Value(ctypes.c_bool)
  *         self.terminate.value = False
  */
-  __Pyx_TraceLine(1985,0,__PYX_ERR(0, 1985, __pyx_L1_error))
+  __Pyx_TraceLine(2002,0,__PYX_ERR(0, 2002, __pyx_L1_error))
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->helper);
   __Pyx_DECREF(__pyx_v_self->helper);
   __pyx_v_self->helper = Py_None;
 
-  /* "cpprb/PyReplayBuffer.pyx":1986
+  /* "cpprb/PyReplayBuffer.pyx":2003
  * 
  *         self.helper = None
  *         self.terminate = Value(ctypes.c_bool)             # <<<<<<<<<<<<<<
  *         self.terminate.value = False
  * 
  */
-  __Pyx_TraceLine(1986,0,__PYX_ERR(0, 1986, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1986, __pyx_L1_error)
+  __Pyx_TraceLine(2003,0,__PYX_ERR(0, 2003, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2003, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1986, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2003, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_c_bool); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1986, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_c_bool); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2003, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -32168,162 +32374,162 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_8, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1986, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2003, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->terminate);
   __Pyx_DECREF(__pyx_v_self->terminate);
   __pyx_v_self->terminate = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1987
+  /* "cpprb/PyReplayBuffer.pyx":2004
  *         self.helper = None
  *         self.terminate = Value(ctypes.c_bool)
  *         self.terminate.value = False             # <<<<<<<<<<<<<<
  * 
  *         self.learner_per_ready = Event()
  */
-  __Pyx_TraceLine(1987,0,__PYX_ERR(0, 1987, __pyx_L1_error))
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self->terminate, __pyx_n_s_value, Py_False) < 0) __PYX_ERR(0, 1987, __pyx_L1_error)
+  __Pyx_TraceLine(2004,0,__PYX_ERR(0, 2004, __pyx_L1_error))
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self->terminate, __pyx_n_s_value, Py_False) < 0) __PYX_ERR(0, 2004, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":1989
+  /* "cpprb/PyReplayBuffer.pyx":2006
  *         self.terminate.value = False
  * 
  *         self.learner_per_ready = Event()             # <<<<<<<<<<<<<<
  *         self.learner_per_ready.clear()
  *         self.explorer_per_ready = Event()
  */
-  __Pyx_TraceLine(1989,0,__PYX_ERR(0, 1989, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Event); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1989, __pyx_L1_error)
+  __Pyx_TraceLine(2006,0,__PYX_ERR(0, 2006, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Event); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2006, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1989, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2006, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->learner_per_ready);
   __Pyx_DECREF(__pyx_v_self->learner_per_ready);
   __pyx_v_self->learner_per_ready = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1990
+  /* "cpprb/PyReplayBuffer.pyx":2007
  * 
  *         self.learner_per_ready = Event()
  *         self.learner_per_ready.clear()             # <<<<<<<<<<<<<<
  *         self.explorer_per_ready = Event()
  *         self.explorer_per_ready.set()
  */
-  __Pyx_TraceLine(1990,0,__PYX_ERR(0, 1990, __pyx_L1_error))
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_per_ready, __pyx_n_s_clear); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1990, __pyx_L1_error)
+  __Pyx_TraceLine(2007,0,__PYX_ERR(0, 2007, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_per_ready, __pyx_n_s_clear); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2007, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1990, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2007, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1991
+  /* "cpprb/PyReplayBuffer.pyx":2008
  *         self.learner_per_ready = Event()
  *         self.learner_per_ready.clear()
  *         self.explorer_per_ready = Event()             # <<<<<<<<<<<<<<
  *         self.explorer_per_ready.set()
  *         self.explorer_per_count = Value(ctypes.c_size_t,0)
  */
-  __Pyx_TraceLine(1991,0,__PYX_ERR(0, 1991, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Event); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1991, __pyx_L1_error)
+  __Pyx_TraceLine(2008,0,__PYX_ERR(0, 2008, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Event); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2008, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1991, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2008, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->explorer_per_ready);
   __Pyx_DECREF(__pyx_v_self->explorer_per_ready);
   __pyx_v_self->explorer_per_ready = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1992
+  /* "cpprb/PyReplayBuffer.pyx":2009
  *         self.learner_per_ready.clear()
  *         self.explorer_per_ready = Event()
  *         self.explorer_per_ready.set()             # <<<<<<<<<<<<<<
  *         self.explorer_per_count = Value(ctypes.c_size_t,0)
  * 
  */
-  __Pyx_TraceLine(1992,0,__PYX_ERR(0, 1992, __pyx_L1_error))
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_ready, __pyx_n_s_set); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1992, __pyx_L1_error)
+  __Pyx_TraceLine(2009,0,__PYX_ERR(0, 2009, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_ready, __pyx_n_s_set); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2009, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1992, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2009, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1993
+  /* "cpprb/PyReplayBuffer.pyx":2010
  *         self.explorer_per_ready = Event()
  *         self.explorer_per_ready.set()
  *         self.explorer_per_count = Value(ctypes.c_size_t,0)             # <<<<<<<<<<<<<<
  * 
  *         self.idx_vec = vector[size_t]()
  */
-  __Pyx_TraceLine(1993,0,__PYX_ERR(0, 1993, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1993, __pyx_L1_error)
+  __Pyx_TraceLine(2010,0,__PYX_ERR(0, 2010, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2010, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1993, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_ctypes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2010, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_c_size_t); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1993, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_c_size_t); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2010, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_7)) {
@@ -32333,85 +32539,85 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_8, __pyx_int_0};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1993, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2010, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_8, __pyx_int_0};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1993, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2010, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   } else
   #endif
   {
-    __pyx_t_1 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1993, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2010, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_9, __pyx_t_8);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_9, __pyx_int_0);
     __pyx_t_8 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1993, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2010, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->explorer_per_count);
   __Pyx_DECREF(__pyx_v_self->explorer_per_count);
   __pyx_v_self->explorer_per_count = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":1995
+  /* "cpprb/PyReplayBuffer.pyx":2012
  *         self.explorer_per_count = Value(ctypes.c_size_t,0)
  * 
  *         self.idx_vec = vector[size_t]()             # <<<<<<<<<<<<<<
  *         self.ps_vec = vector[float]()
  * 
  */
-  __Pyx_TraceLine(1995,0,__PYX_ERR(0, 1995, __pyx_L1_error))
+  __Pyx_TraceLine(2012,0,__PYX_ERR(0, 2012, __pyx_L1_error))
   try {
     __pyx_t_10 = std::vector<size_t> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 1995, __pyx_L1_error)
+    __PYX_ERR(0, 2012, __pyx_L1_error)
   }
   __pyx_v_self->idx_vec = __pyx_t_10;
 
-  /* "cpprb/PyReplayBuffer.pyx":1996
+  /* "cpprb/PyReplayBuffer.pyx":2013
  * 
  *         self.idx_vec = vector[size_t]()
  *         self.ps_vec = vector[float]()             # <<<<<<<<<<<<<<
  * 
  *     cdef void _lock_explorer_per(self) except *:
  */
-  __Pyx_TraceLine(1996,0,__PYX_ERR(0, 1996, __pyx_L1_error))
+  __Pyx_TraceLine(2013,0,__PYX_ERR(0, 2013, __pyx_L1_error))
   try {
     __pyx_t_11 = std::vector<float> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 1996, __pyx_L1_error)
+    __PYX_ERR(0, 2013, __pyx_L1_error)
   }
   __pyx_v_self->ps_vec = __pyx_t_11;
 
-  /* "cpprb/PyReplayBuffer.pyx":1944
+  /* "cpprb/PyReplayBuffer.pyx":1961
  *     cdef vector[float] ps_vec
  * 
  *     def __init__(self,size,env_dict=None,*,alpha=0.6,eps=1e-4,**kwargs):             # <<<<<<<<<<<<<<
  *         r"""Initialize PrioritizedReplayBuffer
  * 
  */
 
@@ -32432,15 +32638,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_shm);
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":1998
+/* "cpprb/PyReplayBuffer.pyx":2015
  *         self.ps_vec = vector[float]()
  * 
  *     cdef void _lock_explorer_per(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_per_ready.wait() # Wait permission
  *         self.learner_per_ready.clear()  # Block learner
  */
 
@@ -32458,147 +32664,147 @@
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_lock_explorer_per", 0);
-  __Pyx_TraceCall("_lock_explorer_per", __pyx_f[0], 1998, 0, __PYX_ERR(0, 1998, __pyx_L1_error));
+  __Pyx_TraceCall("_lock_explorer_per", __pyx_f[0], 2015, 0, __PYX_ERR(0, 2015, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":1999
+  /* "cpprb/PyReplayBuffer.pyx":2016
  * 
  *     cdef void _lock_explorer_per(self) except *:
  *         self.explorer_per_ready.wait() # Wait permission             # <<<<<<<<<<<<<<
  *         self.learner_per_ready.clear()  # Block learner
  *         with self.explorer_per_count.get_lock():
  */
-  __Pyx_TraceLine(1999,0,__PYX_ERR(0, 1999, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_ready, __pyx_n_s_wait); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1999, __pyx_L1_error)
+  __Pyx_TraceLine(2016,0,__PYX_ERR(0, 2016, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_ready, __pyx_n_s_wait); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2016, __pyx_L1_error)
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1999, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2016, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2000
+  /* "cpprb/PyReplayBuffer.pyx":2017
  *     cdef void _lock_explorer_per(self) except *:
  *         self.explorer_per_ready.wait() # Wait permission
  *         self.learner_per_ready.clear()  # Block learner             # <<<<<<<<<<<<<<
  *         with self.explorer_per_count.get_lock():
  *             self.explorer_per_count.value += 1
  */
-  __Pyx_TraceLine(2000,0,__PYX_ERR(0, 2000, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_per_ready, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2000, __pyx_L1_error)
+  __Pyx_TraceLine(2017,0,__PYX_ERR(0, 2017, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_per_ready, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2017, __pyx_L1_error)
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2000, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2017, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2001
+  /* "cpprb/PyReplayBuffer.pyx":2018
  *         self.explorer_per_ready.wait() # Wait permission
  *         self.learner_per_ready.clear()  # Block learner
  *         with self.explorer_per_count.get_lock():             # <<<<<<<<<<<<<<
  *             self.explorer_per_count.value += 1
  * 
  */
-  __Pyx_TraceLine(2001,0,__PYX_ERR(0, 2001, __pyx_L1_error))
+  __Pyx_TraceLine(2018,0,__PYX_ERR(0, 2018, __pyx_L1_error))
   /*with:*/ {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_count, __pyx_n_s_get_lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2001, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_count, __pyx_n_s_get_lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2018, __pyx_L1_error)
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
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2001, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2018, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2001, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2018, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2001, __pyx_L3_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2018, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2001, __pyx_L3_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2018, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     /*try:*/ {
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
 
-          /* "cpprb/PyReplayBuffer.pyx":2002
+          /* "cpprb/PyReplayBuffer.pyx":2019
  *         self.learner_per_ready.clear()  # Block learner
  *         with self.explorer_per_count.get_lock():
  *             self.explorer_per_count.value += 1             # <<<<<<<<<<<<<<
  * 
  *     cdef void _unlock_explorer_per(self) except *:
  */
-          __Pyx_TraceLine(2002,0,__PYX_ERR(0, 2002, __pyx_L7_error))
+          __Pyx_TraceLine(2019,0,__PYX_ERR(0, 2019, __pyx_L7_error))
           __Pyx_INCREF(__pyx_v_self->explorer_per_count);
           __pyx_t_1 = __pyx_v_self->explorer_per_count;
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2002, __pyx_L7_error)
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2019, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2002, __pyx_L7_error)
+          __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2019, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_value, __pyx_t_3) < 0) __PYX_ERR(0, 2002, __pyx_L7_error)
+          if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_value, __pyx_t_3) < 0) __PYX_ERR(0, 2019, __pyx_L7_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-          /* "cpprb/PyReplayBuffer.pyx":2001
+          /* "cpprb/PyReplayBuffer.pyx":2018
  *         self.explorer_per_ready.wait() # Wait permission
  *         self.learner_per_ready.clear()  # Block learner
  *         with self.explorer_per_count.get_lock():             # <<<<<<<<<<<<<<
  *             self.explorer_per_count.value += 1
  * 
  */
         }
@@ -32609,36 +32815,36 @@
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPPrioritizedReplayBuffer._lock_explorer_per", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 2001, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 2018, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2001, __pyx_L9_except_error)
+          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2018, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2001, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2018, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_9);
           __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-          if (__pyx_t_10 < 0) __PYX_ERR(0, 2001, __pyx_L9_except_error)
+          if (__pyx_t_10 < 0) __PYX_ERR(0, 2018, __pyx_L9_except_error)
           __pyx_t_11 = ((!(__pyx_t_10 != 0)) != 0);
           if (__pyx_t_11) {
             __Pyx_GIVEREF(__pyx_t_1);
             __Pyx_GIVEREF(__pyx_t_3);
             __Pyx_XGIVEREF(__pyx_t_2);
             __Pyx_ErrRestoreWithState(__pyx_t_1, __pyx_t_3, __pyx_t_2);
             __pyx_t_1 = 0; __pyx_t_3 = 0; __pyx_t_2 = 0; 
-            __PYX_ERR(0, 2001, __pyx_L9_except_error)
+            __PYX_ERR(0, 2018, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -32656,30 +32862,30 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_4) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__21, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2001, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2018, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L16;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L1_error;
     __pyx_L16:;
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":1998
+  /* "cpprb/PyReplayBuffer.pyx":2015
  *         self.ps_vec = vector[float]()
  * 
  *     cdef void _lock_explorer_per(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_per_ready.wait() # Wait permission
  *         self.learner_per_ready.clear()  # Block learner
  */
 
@@ -32692,15 +32898,15 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPPrioritizedReplayBuffer._lock_explorer_per", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "cpprb/PyReplayBuffer.pyx":2004
+/* "cpprb/PyReplayBuffer.pyx":2021
  *             self.explorer_per_count.value += 1
  * 
  *     cdef void _unlock_explorer_per(self) except *:             # <<<<<<<<<<<<<<
  *         with self.explorer_per_count.get_lock():
  *             self.explorer_per_count.value -= 1
  */
 
@@ -32718,93 +32924,93 @@
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_unlock_explorer_per", 0);
-  __Pyx_TraceCall("_unlock_explorer_per", __pyx_f[0], 2004, 0, __PYX_ERR(0, 2004, __pyx_L1_error));
+  __Pyx_TraceCall("_unlock_explorer_per", __pyx_f[0], 2021, 0, __PYX_ERR(0, 2021, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":2005
+  /* "cpprb/PyReplayBuffer.pyx":2022
  * 
  *     cdef void _unlock_explorer_per(self) except *:
  *         with self.explorer_per_count.get_lock():             # <<<<<<<<<<<<<<
  *             self.explorer_per_count.value -= 1
  *         if self.explorer_per_count.value == 0:
  */
-  __Pyx_TraceLine(2005,0,__PYX_ERR(0, 2005, __pyx_L1_error))
+  __Pyx_TraceLine(2022,0,__PYX_ERR(0, 2022, __pyx_L1_error))
   /*with:*/ {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_count, __pyx_n_s_get_lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2005, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_count, __pyx_n_s_get_lock); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2022, __pyx_L1_error)
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
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2005, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2022, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2005, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2022, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2005, __pyx_L3_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2022, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2005, __pyx_L3_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2022, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     /*try:*/ {
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
 
-          /* "cpprb/PyReplayBuffer.pyx":2006
+          /* "cpprb/PyReplayBuffer.pyx":2023
  *     cdef void _unlock_explorer_per(self) except *:
  *         with self.explorer_per_count.get_lock():
  *             self.explorer_per_count.value -= 1             # <<<<<<<<<<<<<<
  *         if self.explorer_per_count.value == 0:
  *             self.learner_per_ready.set()
  */
-          __Pyx_TraceLine(2006,0,__PYX_ERR(0, 2006, __pyx_L7_error))
+          __Pyx_TraceLine(2023,0,__PYX_ERR(0, 2023, __pyx_L7_error))
           __Pyx_INCREF(__pyx_v_self->explorer_per_count);
           __pyx_t_1 = __pyx_v_self->explorer_per_count;
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2006, __pyx_L7_error)
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2023, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_t_2, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2006, __pyx_L7_error)
+          __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_t_2, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2023, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_value, __pyx_t_3) < 0) __PYX_ERR(0, 2006, __pyx_L7_error)
+          if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_value, __pyx_t_3) < 0) __PYX_ERR(0, 2023, __pyx_L7_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-          /* "cpprb/PyReplayBuffer.pyx":2005
+          /* "cpprb/PyReplayBuffer.pyx":2022
  * 
  *     cdef void _unlock_explorer_per(self) except *:
  *         with self.explorer_per_count.get_lock():             # <<<<<<<<<<<<<<
  *             self.explorer_per_count.value -= 1
  *         if self.explorer_per_count.value == 0:
  */
         }
@@ -32815,36 +33021,36 @@
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPPrioritizedReplayBuffer._unlock_explorer_per", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 2005, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 2022, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2005, __pyx_L9_except_error)
+          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2022, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2005, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2022, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_9);
           __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-          if (__pyx_t_10 < 0) __PYX_ERR(0, 2005, __pyx_L9_except_error)
+          if (__pyx_t_10 < 0) __PYX_ERR(0, 2022, __pyx_L9_except_error)
           __pyx_t_11 = ((!(__pyx_t_10 != 0)) != 0);
           if (__pyx_t_11) {
             __Pyx_GIVEREF(__pyx_t_1);
             __Pyx_GIVEREF(__pyx_t_3);
             __Pyx_XGIVEREF(__pyx_t_2);
             __Pyx_ErrRestoreWithState(__pyx_t_1, __pyx_t_3, __pyx_t_2);
             __pyx_t_1 = 0; __pyx_t_3 = 0; __pyx_t_2 = 0; 
-            __PYX_ERR(0, 2005, __pyx_L9_except_error)
+            __PYX_ERR(0, 2022, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -32862,83 +33068,83 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_4) {
           __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__21, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2005, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2022, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L16;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L1_error;
     __pyx_L16:;
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":2007
+  /* "cpprb/PyReplayBuffer.pyx":2024
  *         with self.explorer_per_count.get_lock():
  *             self.explorer_per_count.value -= 1
  *         if self.explorer_per_count.value == 0:             # <<<<<<<<<<<<<<
  *             self.learner_per_ready.set()
  * 
  */
-  __Pyx_TraceLine(2007,0,__PYX_ERR(0, 2007, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_count, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2007, __pyx_L1_error)
+  __Pyx_TraceLine(2024,0,__PYX_ERR(0, 2024, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_count, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2024, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_t_2, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2007, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_EqObjC(__pyx_t_2, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2024, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 2007, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 2024, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_11) {
 
-    /* "cpprb/PyReplayBuffer.pyx":2008
+    /* "cpprb/PyReplayBuffer.pyx":2025
  *             self.explorer_per_count.value -= 1
  *         if self.explorer_per_count.value == 0:
  *             self.learner_per_ready.set()             # <<<<<<<<<<<<<<
  * 
  *     cdef void _lock_learner_per(self) except *:
  */
-    __Pyx_TraceLine(2008,0,__PYX_ERR(0, 2008, __pyx_L1_error))
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_per_ready, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2008, __pyx_L1_error)
+    __Pyx_TraceLine(2025,0,__PYX_ERR(0, 2025, __pyx_L1_error))
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_per_ready, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2025, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2008, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2025, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":2007
+    /* "cpprb/PyReplayBuffer.pyx":2024
  *         with self.explorer_per_count.get_lock():
  *             self.explorer_per_count.value -= 1
  *         if self.explorer_per_count.value == 0:             # <<<<<<<<<<<<<<
  *             self.learner_per_ready.set()
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":2004
+  /* "cpprb/PyReplayBuffer.pyx":2021
  *             self.explorer_per_count.value += 1
  * 
  *     cdef void _unlock_explorer_per(self) except *:             # <<<<<<<<<<<<<<
  *         with self.explorer_per_count.get_lock():
  *             self.explorer_per_count.value -= 1
  */
 
@@ -32951,15 +33157,15 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPPrioritizedReplayBuffer._unlock_explorer_per", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "cpprb/PyReplayBuffer.pyx":2010
+/* "cpprb/PyReplayBuffer.pyx":2027
  *             self.learner_per_ready.set()
  * 
  *     cdef void _lock_learner_per(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_per_ready.clear()
  *         self.learner_per_ready.wait()
  */
 
@@ -32969,71 +33175,71 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_lock_learner_per", 0);
-  __Pyx_TraceCall("_lock_learner_per", __pyx_f[0], 2010, 0, __PYX_ERR(0, 2010, __pyx_L1_error));
+  __Pyx_TraceCall("_lock_learner_per", __pyx_f[0], 2027, 0, __PYX_ERR(0, 2027, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":2011
+  /* "cpprb/PyReplayBuffer.pyx":2028
  * 
  *     cdef void _lock_learner_per(self) except *:
  *         self.explorer_per_ready.clear()             # <<<<<<<<<<<<<<
  *         self.learner_per_ready.wait()
  * 
  */
-  __Pyx_TraceLine(2011,0,__PYX_ERR(0, 2011, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_ready, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2011, __pyx_L1_error)
+  __Pyx_TraceLine(2028,0,__PYX_ERR(0, 2028, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_ready, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2028, __pyx_L1_error)
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2011, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2028, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2012
+  /* "cpprb/PyReplayBuffer.pyx":2029
  *     cdef void _lock_learner_per(self) except *:
  *         self.explorer_per_ready.clear()
  *         self.learner_per_ready.wait()             # <<<<<<<<<<<<<<
  * 
  *     cdef void _unlock_learner_per(self) except *:
  */
-  __Pyx_TraceLine(2012,0,__PYX_ERR(0, 2012, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_per_ready, __pyx_n_s_wait); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2012, __pyx_L1_error)
+  __Pyx_TraceLine(2029,0,__PYX_ERR(0, 2029, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->learner_per_ready, __pyx_n_s_wait); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2029, __pyx_L1_error)
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2012, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2029, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2010
+  /* "cpprb/PyReplayBuffer.pyx":2027
  *             self.learner_per_ready.set()
  * 
  *     cdef void _lock_learner_per(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_per_ready.clear()
  *         self.learner_per_ready.wait()
  */
 
@@ -33045,15 +33251,15 @@
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPPrioritizedReplayBuffer._lock_learner_per", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "cpprb/PyReplayBuffer.pyx":2014
+/* "cpprb/PyReplayBuffer.pyx":2031
  *         self.learner_per_ready.wait()
  * 
  *     cdef void _unlock_learner_per(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_per_ready.set()
  * 
  */
 
@@ -33063,44 +33269,44 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_unlock_learner_per", 0);
-  __Pyx_TraceCall("_unlock_learner_per", __pyx_f[0], 2014, 0, __PYX_ERR(0, 2014, __pyx_L1_error));
+  __Pyx_TraceCall("_unlock_learner_per", __pyx_f[0], 2031, 0, __PYX_ERR(0, 2031, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":2015
+  /* "cpprb/PyReplayBuffer.pyx":2032
  * 
  *     cdef void _unlock_learner_per(self) except *:
  *         self.explorer_per_ready.set()             # <<<<<<<<<<<<<<
  * 
  *     cdef void _lock_learner_unlock_learner_per(self) except *:
  */
-  __Pyx_TraceLine(2015,0,__PYX_ERR(0, 2015, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_ready, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2015, __pyx_L1_error)
+  __Pyx_TraceLine(2032,0,__PYX_ERR(0, 2032, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_ready, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2032, __pyx_L1_error)
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2015, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2032, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2014
+  /* "cpprb/PyReplayBuffer.pyx":2031
  *         self.learner_per_ready.wait()
  * 
  *     cdef void _unlock_learner_per(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_per_ready.set()
  * 
  */
 
@@ -33112,15 +33318,15 @@
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPPrioritizedReplayBuffer._unlock_learner_per", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "cpprb/PyReplayBuffer.pyx":2017
+/* "cpprb/PyReplayBuffer.pyx":2034
  *         self.explorer_per_ready.set()
  * 
  *     cdef void _lock_learner_unlock_learner_per(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_ready.clear()
  *         self.explorer_per_ready.set()
  */
 
@@ -33130,98 +33336,98 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_lock_learner_unlock_learner_per", 0);
-  __Pyx_TraceCall("_lock_learner_unlock_learner_per", __pyx_f[0], 2017, 0, __PYX_ERR(0, 2017, __pyx_L1_error));
+  __Pyx_TraceCall("_lock_learner_unlock_learner_per", __pyx_f[0], 2034, 0, __PYX_ERR(0, 2034, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":2018
+  /* "cpprb/PyReplayBuffer.pyx":2035
  * 
  *     cdef void _lock_learner_unlock_learner_per(self) except *:
  *         self.explorer_ready.clear()             # <<<<<<<<<<<<<<
  *         self.explorer_per_ready.set()
  *         self.learner_ready.wait()
  */
-  __Pyx_TraceLine(2018,0,__PYX_ERR(0, 2018, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->__pyx_base.explorer_ready, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2018, __pyx_L1_error)
+  __Pyx_TraceLine(2035,0,__PYX_ERR(0, 2035, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->__pyx_base.explorer_ready, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2035, __pyx_L1_error)
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2018, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2035, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2019
+  /* "cpprb/PyReplayBuffer.pyx":2036
  *     cdef void _lock_learner_unlock_learner_per(self) except *:
  *         self.explorer_ready.clear()
  *         self.explorer_per_ready.set()             # <<<<<<<<<<<<<<
  *         self.learner_ready.wait()
  * 
  */
-  __Pyx_TraceLine(2019,0,__PYX_ERR(0, 2019, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_ready, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2019, __pyx_L1_error)
+  __Pyx_TraceLine(2036,0,__PYX_ERR(0, 2036, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->explorer_per_ready, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2036, __pyx_L1_error)
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2019, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2036, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2020
+  /* "cpprb/PyReplayBuffer.pyx":2037
  *         self.explorer_ready.clear()
  *         self.explorer_per_ready.set()
  *         self.learner_ready.wait()             # <<<<<<<<<<<<<<
  * 
  *     def add(self,*,priorities = None,**kwargs):
  */
-  __Pyx_TraceLine(2020,0,__PYX_ERR(0, 2020, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->__pyx_base.learner_ready, __pyx_n_s_wait); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2020, __pyx_L1_error)
+  __Pyx_TraceLine(2037,0,__PYX_ERR(0, 2037, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->__pyx_base.learner_ready, __pyx_n_s_wait); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2037, __pyx_L1_error)
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2020, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2037, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2017
+  /* "cpprb/PyReplayBuffer.pyx":2034
  *         self.explorer_per_ready.set()
  * 
  *     cdef void _lock_learner_unlock_learner_per(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_ready.clear()
  *         self.explorer_per_ready.set()
  */
 
@@ -33233,15 +33439,15 @@
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPPrioritizedReplayBuffer._lock_learner_unlock_learner_per", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "cpprb/PyReplayBuffer.pyx":2022
+/* "cpprb/PyReplayBuffer.pyx":2039
  *         self.learner_ready.wait()
  * 
  *     def add(self,*,priorities = None,**kwargs):             # <<<<<<<<<<<<<<
  *         r"""Add transition(s) into replay buffer.
  * 
  */
 
@@ -33273,25 +33479,25 @@
       kw_args = PyDict_Size(__pyx_kwds);
       if (kw_args == 1) {
         const Py_ssize_t index = 0;
         PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
         if (value) { values[index] = value; kw_args--; }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, 0, "add") < 0)) __PYX_ERR(0, 2022, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, 0, "add") < 0)) __PYX_ERR(0, 2039, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 0) {
       goto __pyx_L5_argtuple_error;
     } else {
     }
     __pyx_v_priorities = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("add", 1, 0, 0, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 2022, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("add", 1, 0, 0, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 2039, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPPrioritizedReplayBuffer.add", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_2add(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self), __pyx_v_priorities, __pyx_v_kwargs);
@@ -33329,93 +33535,93 @@
   Py_ssize_t __pyx_t_14;
   Py_ssize_t __pyx_t_15;
   int __pyx_t_16;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add", 0);
-  __Pyx_TraceCall("add", __pyx_f[0], 2022, 0, __PYX_ERR(0, 2022, __pyx_L1_error));
+  __Pyx_TraceCall("add", __pyx_f[0], 2039, 0, __PYX_ERR(0, 2039, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_priorities);
 
-  /* "cpprb/PyReplayBuffer.pyx":2053
+  /* "cpprb/PyReplayBuffer.pyx":2070
  *         It is user responsibility that all the values have the same step-size.
  *         """
  *         cdef size_t N = self.size_check.step_size(kwargs)             # <<<<<<<<<<<<<<
  *         cdef const float [:] ps
  * 
  */
-  __Pyx_TraceLine(2053,0,__PYX_ERR(0, 2053, __pyx_L1_error))
-  __pyx_t_1 = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_StepChecker *)__pyx_v_self->__pyx_base.size_check->__pyx_vtab)->step_size(__pyx_v_self->__pyx_base.size_check, __pyx_v_kwargs); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2053, __pyx_L1_error)
+  __Pyx_TraceLine(2070,0,__PYX_ERR(0, 2070, __pyx_L1_error))
+  __pyx_t_1 = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_StepChecker *)__pyx_v_self->__pyx_base.size_check->__pyx_vtab)->step_size(__pyx_v_self->__pyx_base.size_check, __pyx_v_kwargs); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2070, __pyx_L1_error)
   __pyx_v_N = __pyx_t_1;
 
-  /* "cpprb/PyReplayBuffer.pyx":2056
+  /* "cpprb/PyReplayBuffer.pyx":2073
  *         cdef const float [:] ps
  * 
  *         if priorities is not None:             # <<<<<<<<<<<<<<
  *             priorities = np.ravel(np.array(priorities,copy=False,
  *                                            ndmin=1,dtype=np.single))
  */
-  __Pyx_TraceLine(2056,0,__PYX_ERR(0, 2056, __pyx_L1_error))
+  __Pyx_TraceLine(2073,0,__PYX_ERR(0, 2073, __pyx_L1_error))
   __pyx_t_2 = (__pyx_v_priorities != Py_None);
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "cpprb/PyReplayBuffer.pyx":2057
+    /* "cpprb/PyReplayBuffer.pyx":2074
  * 
  *         if priorities is not None:
  *             priorities = np.ravel(np.array(priorities,copy=False,             # <<<<<<<<<<<<<<
  *                                            ndmin=1,dtype=np.single))
  *             if N != priorities.shape[0]:
  */
-    __Pyx_TraceLine(2057,0,__PYX_ERR(0, 2057, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2057, __pyx_L1_error)
+    __Pyx_TraceLine(2074,0,__PYX_ERR(0, 2074, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2074, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ravel); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2057, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ravel); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2074, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2057, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2074, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2057, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2074, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2057, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2074, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_v_priorities);
     __Pyx_GIVEREF(__pyx_v_priorities);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_priorities);
-    __pyx_t_8 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2057, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2074, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 2057, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_ndmin, __pyx_int_1) < 0) __PYX_ERR(0, 2057, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 2074, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_ndmin, __pyx_int_1) < 0) __PYX_ERR(0, 2074, __pyx_L1_error)
 
-    /* "cpprb/PyReplayBuffer.pyx":2058
+    /* "cpprb/PyReplayBuffer.pyx":2075
  *         if priorities is not None:
  *             priorities = np.ravel(np.array(priorities,copy=False,
  *                                            ndmin=1,dtype=np.single))             # <<<<<<<<<<<<<<
  *             if N != priorities.shape[0]:
  *                 raise ValueError("`priorities` shape is imcompatible")
  */
-    __Pyx_TraceLine(2058,0,__PYX_ERR(0, 2058, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2058, __pyx_L1_error)
+    __Pyx_TraceLine(2075,0,__PYX_ERR(0, 2075, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2075, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_single); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2058, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_single); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2075, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_10) < 0) __PYX_ERR(0, 2057, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_10) < 0) __PYX_ERR(0, 2074, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":2057
+    /* "cpprb/PyReplayBuffer.pyx":2074
  * 
  *         if priorities is not None:
  *             priorities = np.ravel(np.array(priorities,copy=False,             # <<<<<<<<<<<<<<
  *                                            ndmin=1,dtype=np.single))
  *             if N != priorities.shape[0]:
  */
-    __Pyx_TraceLine(2057,0,__PYX_ERR(0, 2057, __pyx_L1_error))
-    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_5, __pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2057, __pyx_L1_error)
+    __Pyx_TraceLine(2074,0,__PYX_ERR(0, 2074, __pyx_L1_error))
+    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_5, __pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2074, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
@@ -33425,110 +33631,110 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_8, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_10);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2057, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2074, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF_SET(__pyx_v_priorities, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":2059
+    /* "cpprb/PyReplayBuffer.pyx":2076
  *             priorities = np.ravel(np.array(priorities,copy=False,
  *                                            ndmin=1,dtype=np.single))
  *             if N != priorities.shape[0]:             # <<<<<<<<<<<<<<
  *                 raise ValueError("`priorities` shape is imcompatible")
  * 
  */
-    __Pyx_TraceLine(2059,0,__PYX_ERR(0, 2059, __pyx_L1_error))
-    __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2059, __pyx_L1_error)
+    __Pyx_TraceLine(2076,0,__PYX_ERR(0, 2076, __pyx_L1_error))
+    __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_N); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2076, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_priorities, __pyx_n_s_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2059, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_priorities, __pyx_n_s_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2076, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_10 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2059, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2076, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PyObject_RichCompare(__pyx_t_4, __pyx_t_10, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2059, __pyx_L1_error)
+    __pyx_t_6 = PyObject_RichCompare(__pyx_t_4, __pyx_t_10, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2076, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 2059, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 2076, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "cpprb/PyReplayBuffer.pyx":2060
+      /* "cpprb/PyReplayBuffer.pyx":2077
  *                                            ndmin=1,dtype=np.single))
  *             if N != priorities.shape[0]:
  *                 raise ValueError("`priorities` shape is imcompatible")             # <<<<<<<<<<<<<<
  * 
  *         cdef size_t index = self.index.fetch_add(N)
  */
-      __Pyx_TraceLine(2060,0,__PYX_ERR(0, 2060, __pyx_L1_error))
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2060, __pyx_L1_error)
+      __Pyx_TraceLine(2077,0,__PYX_ERR(0, 2077, __pyx_L1_error))
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2077, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 2060, __pyx_L1_error)
+      __PYX_ERR(0, 2077, __pyx_L1_error)
 
-      /* "cpprb/PyReplayBuffer.pyx":2059
+      /* "cpprb/PyReplayBuffer.pyx":2076
  *             priorities = np.ravel(np.array(priorities,copy=False,
  *                                            ndmin=1,dtype=np.single))
  *             if N != priorities.shape[0]:             # <<<<<<<<<<<<<<
  *                 raise ValueError("`priorities` shape is imcompatible")
  * 
  */
     }
 
-    /* "cpprb/PyReplayBuffer.pyx":2056
+    /* "cpprb/PyReplayBuffer.pyx":2073
  *         cdef const float [:] ps
  * 
  *         if priorities is not None:             # <<<<<<<<<<<<<<
  *             priorities = np.ravel(np.array(priorities,copy=False,
  *                                            ndmin=1,dtype=np.single))
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":2062
+  /* "cpprb/PyReplayBuffer.pyx":2079
  *                 raise ValueError("`priorities` shape is imcompatible")
  * 
  *         cdef size_t index = self.index.fetch_add(N)             # <<<<<<<<<<<<<<
  *         cdef size_t end = index + N
  *         cdef add_idx = np.arange(index,end)
  */
-  __Pyx_TraceLine(2062,0,__PYX_ERR(0, 2062, __pyx_L1_error))
+  __Pyx_TraceLine(2079,0,__PYX_ERR(0, 2079, __pyx_L1_error))
   __pyx_v_index = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ProcessSafeRingBufferIndex *)__pyx_v_self->__pyx_base.index->__pyx_base.__pyx_vtab)->__pyx_base.fetch_add(((struct __pyx_obj_5cpprb_14PyReplayBuffer_RingBufferIndex *)__pyx_v_self->__pyx_base.index), __pyx_v_N);
 
-  /* "cpprb/PyReplayBuffer.pyx":2063
+  /* "cpprb/PyReplayBuffer.pyx":2080
  * 
  *         cdef size_t index = self.index.fetch_add(N)
  *         cdef size_t end = index + N             # <<<<<<<<<<<<<<
  *         cdef add_idx = np.arange(index,end)
  * 
  */
-  __Pyx_TraceLine(2063,0,__PYX_ERR(0, 2063, __pyx_L1_error))
+  __Pyx_TraceLine(2080,0,__PYX_ERR(0, 2080, __pyx_L1_error))
   __pyx_v_end = (__pyx_v_index + __pyx_v_N);
 
-  /* "cpprb/PyReplayBuffer.pyx":2064
+  /* "cpprb/PyReplayBuffer.pyx":2081
  *         cdef size_t index = self.index.fetch_add(N)
  *         cdef size_t end = index + N
  *         cdef add_idx = np.arange(index,end)             # <<<<<<<<<<<<<<
  * 
  *         if end > self.buffer_size:
  */
-  __Pyx_TraceLine(2064,0,__PYX_ERR(0, 2064, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2064, __pyx_L1_error)
+  __Pyx_TraceLine(2081,0,__PYX_ERR(0, 2081, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2081, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_arange); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2064, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_arange); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2081, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_PyInt_FromSize_t(__pyx_v_index); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2064, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_FromSize_t(__pyx_v_index); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2081, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_8 = __Pyx_PyInt_FromSize_t(__pyx_v_end); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2064, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_FromSize_t(__pyx_v_end); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2081, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_5 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -33537,152 +33743,152 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_11 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_10, __pyx_t_8};
-    __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2064, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2081, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_10, __pyx_t_8};
-    __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2064, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2081, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2064, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2081, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_10);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_11, __pyx_t_10);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_11, __pyx_t_8);
     __pyx_t_10 = 0;
     __pyx_t_8 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2064, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2081, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_add_idx = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2066
+  /* "cpprb/PyReplayBuffer.pyx":2083
  *         cdef add_idx = np.arange(index,end)
  * 
  *         if end > self.buffer_size:             # <<<<<<<<<<<<<<
  *             add_idx[add_idx >= self.buffer_size] -= self.buffer_size
  * 
  */
-  __Pyx_TraceLine(2066,0,__PYX_ERR(0, 2066, __pyx_L1_error))
+  __Pyx_TraceLine(2083,0,__PYX_ERR(0, 2083, __pyx_L1_error))
   __pyx_t_3 = ((__pyx_v_end > __pyx_v_self->__pyx_base.buffer_size) != 0);
   if (__pyx_t_3) {
 
-    /* "cpprb/PyReplayBuffer.pyx":2067
+    /* "cpprb/PyReplayBuffer.pyx":2084
  * 
  *         if end > self.buffer_size:
  *             add_idx[add_idx >= self.buffer_size] -= self.buffer_size             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_TraceLine(2067,0,__PYX_ERR(0, 2067, __pyx_L1_error))
-    __pyx_t_6 = __Pyx_PyInt_FromSize_t(__pyx_v_self->__pyx_base.buffer_size); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2067, __pyx_L1_error)
+    __Pyx_TraceLine(2084,0,__PYX_ERR(0, 2084, __pyx_L1_error))
+    __pyx_t_6 = __Pyx_PyInt_FromSize_t(__pyx_v_self->__pyx_base.buffer_size); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2084, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = PyObject_RichCompare(__pyx_v_add_idx, __pyx_t_6, Py_GE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2067, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_v_add_idx, __pyx_t_6, Py_GE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2084, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_add_idx, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2067, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_add_idx, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2084, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyInt_FromSize_t(__pyx_v_self->__pyx_base.buffer_size); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2067, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_FromSize_t(__pyx_v_self->__pyx_base.buffer_size); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2084, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = PyNumber_InPlaceSubtract(__pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2067, __pyx_L1_error)
+    __pyx_t_8 = PyNumber_InPlaceSubtract(__pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2084, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(PyObject_SetItem(__pyx_v_add_idx, __pyx_t_4, __pyx_t_8) < 0)) __PYX_ERR(0, 2067, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_add_idx, __pyx_t_4, __pyx_t_8) < 0)) __PYX_ERR(0, 2084, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":2066
+    /* "cpprb/PyReplayBuffer.pyx":2083
  *         cdef add_idx = np.arange(index,end)
  * 
  *         if end > self.buffer_size:             # <<<<<<<<<<<<<<
  *             add_idx[add_idx >= self.buffer_size] -= self.buffer_size
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":2070
+  /* "cpprb/PyReplayBuffer.pyx":2087
  * 
  * 
  *         self._lock_explorer_per()             # <<<<<<<<<<<<<<
  * 
  *         if priorities is not None:
  */
-  __Pyx_TraceLine(2070,0,__PYX_ERR(0, 2070, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->_lock_explorer_per(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2070, __pyx_L1_error)
+  __Pyx_TraceLine(2087,0,__PYX_ERR(0, 2087, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->_lock_explorer_per(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2087, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2072
+  /* "cpprb/PyReplayBuffer.pyx":2089
  *         self._lock_explorer_per()
  * 
  *         if priorities is not None:             # <<<<<<<<<<<<<<
  *             ps = np.ravel(np.array(priorities,copy=False,ndmin=1,dtype=np.single))
  *             self.per.ptr().set_priorities(index,&ps[0],N,self.get_buffer_size())
  */
-  __Pyx_TraceLine(2072,0,__PYX_ERR(0, 2072, __pyx_L1_error))
+  __Pyx_TraceLine(2089,0,__PYX_ERR(0, 2089, __pyx_L1_error))
   __pyx_t_3 = (__pyx_v_priorities != Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
   if (__pyx_t_2) {
 
-    /* "cpprb/PyReplayBuffer.pyx":2073
+    /* "cpprb/PyReplayBuffer.pyx":2090
  * 
  *         if priorities is not None:
  *             ps = np.ravel(np.array(priorities,copy=False,ndmin=1,dtype=np.single))             # <<<<<<<<<<<<<<
  *             self.per.ptr().set_priorities(index,&ps[0],N,self.get_buffer_size())
  *         else:
  */
-    __Pyx_TraceLine(2073,0,__PYX_ERR(0, 2073, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2073, __pyx_L1_error)
+    __Pyx_TraceLine(2090,0,__PYX_ERR(0, 2090, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2090, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_ravel); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2073, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_ravel); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2090, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2073, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2090, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_array); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2073, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_array); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2090, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2073, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2090, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_INCREF(__pyx_v_priorities);
     __Pyx_GIVEREF(__pyx_v_priorities);
     PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_priorities);
-    __pyx_t_10 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2073, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2090, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 2073, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_ndmin, __pyx_int_1) < 0) __PYX_ERR(0, 2073, __pyx_L1_error)
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2073, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 2090, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_ndmin, __pyx_int_1) < 0) __PYX_ERR(0, 2090, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2090, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_single); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2073, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_single); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2090, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 2073, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 2090, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, __pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2073, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, __pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2090, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __pyx_t_10 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_7);
@@ -33692,215 +33898,215 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_10, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_9);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2073, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2090, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_ds_float__const__(__pyx_t_4, 0); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 2073, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_ds_float__const__(__pyx_t_4, 0); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 2090, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_ps = __pyx_t_12;
     __pyx_t_12.memview = NULL;
     __pyx_t_12.data = NULL;
 
-    /* "cpprb/PyReplayBuffer.pyx":2074
+    /* "cpprb/PyReplayBuffer.pyx":2091
  *         if priorities is not None:
  *             ps = np.ravel(np.array(priorities,copy=False,ndmin=1,dtype=np.single))
  *             self.per.ptr().set_priorities(index,&ps[0],N,self.get_buffer_size())             # <<<<<<<<<<<<<<
  *         else:
  *             self.per.ptr().set_priorities(index,N,self.get_buffer_size())
  */
-    __Pyx_TraceLine(2074,0,__PYX_ERR(0, 2074, __pyx_L1_error))
+    __Pyx_TraceLine(2091,0,__PYX_ERR(0, 2091, __pyx_L1_error))
     __pyx_t_13 = 0;
     __pyx_t_11 = -1;
     if (__pyx_t_13 < 0) {
       __pyx_t_13 += __pyx_v_ps.shape[0];
       if (unlikely(__pyx_t_13 < 0)) __pyx_t_11 = 0;
     } else if (unlikely(__pyx_t_13 >= __pyx_v_ps.shape[0])) __pyx_t_11 = 0;
     if (unlikely(__pyx_t_11 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_11);
-      __PYX_ERR(0, 2074, __pyx_L1_error)
+      __PYX_ERR(0, 2091, __pyx_L1_error)
     }
     ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler *)__pyx_v_self->per->__pyx_vtab)->ptr(__pyx_v_self->per)->set_priorities(__pyx_v_index, (&(*((float const  *) ( /* dim=0 */ (__pyx_v_ps.data + __pyx_t_13 * __pyx_v_ps.strides[0]) )))), __pyx_v_N, ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_buffer_size(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self), 0));
 
-    /* "cpprb/PyReplayBuffer.pyx":2072
+    /* "cpprb/PyReplayBuffer.pyx":2089
  *         self._lock_explorer_per()
  * 
  *         if priorities is not None:             # <<<<<<<<<<<<<<
  *             ps = np.ravel(np.array(priorities,copy=False,ndmin=1,dtype=np.single))
  *             self.per.ptr().set_priorities(index,&ps[0],N,self.get_buffer_size())
  */
     goto __pyx_L6;
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":2076
+  /* "cpprb/PyReplayBuffer.pyx":2093
  *             self.per.ptr().set_priorities(index,&ps[0],N,self.get_buffer_size())
  *         else:
  *             self.per.ptr().set_priorities(index,N,self.get_buffer_size())             # <<<<<<<<<<<<<<
  * 
  *         if index+N <= self.buffer_size:
  */
-  __Pyx_TraceLine(2076,0,__PYX_ERR(0, 2076, __pyx_L1_error))
+  __Pyx_TraceLine(2093,0,__PYX_ERR(0, 2093, __pyx_L1_error))
   /*else*/ {
     ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler *)__pyx_v_self->per->__pyx_vtab)->ptr(__pyx_v_self->per)->set_priorities(__pyx_v_index, __pyx_v_N, ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_buffer_size(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self), 0));
   }
   __pyx_L6:;
 
-  /* "cpprb/PyReplayBuffer.pyx":2078
+  /* "cpprb/PyReplayBuffer.pyx":2095
  *             self.per.ptr().set_priorities(index,N,self.get_buffer_size())
  * 
  *         if index+N <= self.buffer_size:             # <<<<<<<<<<<<<<
  *             self.unchange_since_sample[index:index+N] = False
  *         else:
  */
-  __Pyx_TraceLine(2078,0,__PYX_ERR(0, 2078, __pyx_L1_error))
+  __Pyx_TraceLine(2095,0,__PYX_ERR(0, 2095, __pyx_L1_error))
   __pyx_t_2 = (((__pyx_v_index + __pyx_v_N) <= __pyx_v_self->__pyx_base.buffer_size) != 0);
   if (__pyx_t_2) {
 
-    /* "cpprb/PyReplayBuffer.pyx":2079
+    /* "cpprb/PyReplayBuffer.pyx":2096
  * 
  *         if index+N <= self.buffer_size:
  *             self.unchange_since_sample[index:index+N] = False             # <<<<<<<<<<<<<<
  *         else:
  *             self.unchange_since_sample[index:] = False
  */
-    __Pyx_TraceLine(2079,0,__PYX_ERR(0, 2079, __pyx_L1_error))
-    if (__Pyx_PyObject_SetSlice(__pyx_v_self->unchange_since_sample, Py_False, __pyx_v_index, (__pyx_v_index + __pyx_v_N), NULL, NULL, NULL, 1, 1, 1) < 0) __PYX_ERR(0, 2079, __pyx_L1_error)
+    __Pyx_TraceLine(2096,0,__PYX_ERR(0, 2096, __pyx_L1_error))
+    if (__Pyx_PyObject_SetSlice(__pyx_v_self->unchange_since_sample, Py_False, __pyx_v_index, (__pyx_v_index + __pyx_v_N), NULL, NULL, NULL, 1, 1, 1) < 0) __PYX_ERR(0, 2096, __pyx_L1_error)
 
-    /* "cpprb/PyReplayBuffer.pyx":2078
+    /* "cpprb/PyReplayBuffer.pyx":2095
  *             self.per.ptr().set_priorities(index,N,self.get_buffer_size())
  * 
  *         if index+N <= self.buffer_size:             # <<<<<<<<<<<<<<
  *             self.unchange_since_sample[index:index+N] = False
  *         else:
  */
     goto __pyx_L7;
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":2081
+  /* "cpprb/PyReplayBuffer.pyx":2098
  *             self.unchange_since_sample[index:index+N] = False
  *         else:
  *             self.unchange_since_sample[index:] = False             # <<<<<<<<<<<<<<
  *             self.unchange_since_sample[:index+N-self.buffer_size] = False
  * 
  */
-  __Pyx_TraceLine(2081,0,__PYX_ERR(0, 2081, __pyx_L1_error))
+  __Pyx_TraceLine(2098,0,__PYX_ERR(0, 2098, __pyx_L1_error))
   /*else*/ {
-    if (__Pyx_PyObject_SetSlice(__pyx_v_self->unchange_since_sample, Py_False, __pyx_v_index, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 2081, __pyx_L1_error)
+    if (__Pyx_PyObject_SetSlice(__pyx_v_self->unchange_since_sample, Py_False, __pyx_v_index, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 2098, __pyx_L1_error)
 
-    /* "cpprb/PyReplayBuffer.pyx":2082
+    /* "cpprb/PyReplayBuffer.pyx":2099
  *         else:
  *             self.unchange_since_sample[index:] = False
  *             self.unchange_since_sample[:index+N-self.buffer_size] = False             # <<<<<<<<<<<<<<
  * 
  *         self._lock_explorer()
  */
-    __Pyx_TraceLine(2082,0,__PYX_ERR(0, 2082, __pyx_L1_error))
-    if (__Pyx_PyObject_SetSlice(__pyx_v_self->unchange_since_sample, Py_False, 0, ((__pyx_v_index + __pyx_v_N) - __pyx_v_self->__pyx_base.buffer_size), NULL, NULL, NULL, 0, 1, 1) < 0) __PYX_ERR(0, 2082, __pyx_L1_error)
+    __Pyx_TraceLine(2099,0,__PYX_ERR(0, 2099, __pyx_L1_error))
+    if (__Pyx_PyObject_SetSlice(__pyx_v_self->unchange_since_sample, Py_False, 0, ((__pyx_v_index + __pyx_v_N) - __pyx_v_self->__pyx_base.buffer_size), NULL, NULL, NULL, 0, 1, 1) < 0) __PYX_ERR(0, 2099, __pyx_L1_error)
   }
   __pyx_L7:;
 
-  /* "cpprb/PyReplayBuffer.pyx":2084
+  /* "cpprb/PyReplayBuffer.pyx":2101
  *             self.unchange_since_sample[:index+N-self.buffer_size] = False
  * 
  *         self._lock_explorer()             # <<<<<<<<<<<<<<
  *         self._unlock_explorer_per()
  * 
  */
-  __Pyx_TraceLine(2084,0,__PYX_ERR(0, 2084, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base._lock_explorer(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2084, __pyx_L1_error)
+  __Pyx_TraceLine(2101,0,__PYX_ERR(0, 2101, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base._lock_explorer(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2101, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2085
+  /* "cpprb/PyReplayBuffer.pyx":2102
  * 
  *         self._lock_explorer()
  *         self._unlock_explorer_per()             # <<<<<<<<<<<<<<
  * 
  *         for name, b in self.buffer.items():
  */
-  __Pyx_TraceLine(2085,0,__PYX_ERR(0, 2085, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->_unlock_explorer_per(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2085, __pyx_L1_error)
+  __Pyx_TraceLine(2102,0,__PYX_ERR(0, 2102, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->_unlock_explorer_per(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2102, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2087
+  /* "cpprb/PyReplayBuffer.pyx":2104
  *         self._unlock_explorer_per()
  * 
  *         for name, b in self.buffer.items():             # <<<<<<<<<<<<<<
  *             b[add_idx] = np.reshape(np.array(kwargs[name],copy=False,ndmin=2),
  *                                     self.env_dict[name]["add_shape"])
  */
-  __Pyx_TraceLine(2087,0,__PYX_ERR(0, 2087, __pyx_L1_error))
+  __Pyx_TraceLine(2104,0,__PYX_ERR(0, 2104, __pyx_L1_error))
   __pyx_t_14 = 0;
   if (unlikely(__pyx_v_self->__pyx_base.buffer == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-    __PYX_ERR(0, 2087, __pyx_L1_error)
+    __PYX_ERR(0, 2104, __pyx_L1_error)
   }
-  __pyx_t_7 = __Pyx_dict_iterator(__pyx_v_self->__pyx_base.buffer, 0, __pyx_n_s_items, (&__pyx_t_15), (&__pyx_t_11)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2087, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_dict_iterator(__pyx_v_self->__pyx_base.buffer, 0, __pyx_n_s_items, (&__pyx_t_15), (&__pyx_t_11)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_4);
   __pyx_t_4 = __pyx_t_7;
   __pyx_t_7 = 0;
   while (1) {
     __pyx_t_16 = __Pyx_dict_iter_next(__pyx_t_4, __pyx_t_15, &__pyx_t_14, &__pyx_t_7, &__pyx_t_9, NULL, __pyx_t_11);
     if (unlikely(__pyx_t_16 == 0)) break;
-    if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 2087, __pyx_L1_error)
+    if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 2104, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_XDECREF_SET(__pyx_v_b, __pyx_t_9);
     __pyx_t_9 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":2088
+    /* "cpprb/PyReplayBuffer.pyx":2105
  * 
  *         for name, b in self.buffer.items():
  *             b[add_idx] = np.reshape(np.array(kwargs[name],copy=False,ndmin=2),             # <<<<<<<<<<<<<<
  *                                     self.env_dict[name]["add_shape"])
  * 
  */
-    __Pyx_TraceLine(2088,0,__PYX_ERR(0, 2088, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2088, __pyx_L1_error)
+    __Pyx_TraceLine(2105,0,__PYX_ERR(0, 2105, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_reshape); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2088, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_reshape); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 2105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2088, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_array); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2088, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_array); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2088, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2088, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7);
     __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2088, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 2088, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_ndmin, __pyx_int_2) < 0) __PYX_ERR(0, 2088, __pyx_L1_error)
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2088, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_copy, Py_False) < 0) __PYX_ERR(0, 2105, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_ndmin, __pyx_int_2) < 0) __PYX_ERR(0, 2105, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":2089
+    /* "cpprb/PyReplayBuffer.pyx":2106
  *         for name, b in self.buffer.items():
  *             b[add_idx] = np.reshape(np.array(kwargs[name],copy=False,ndmin=2),
  *                                     self.env_dict[name]["add_shape"])             # <<<<<<<<<<<<<<
  * 
  *         self._unlock_explorer()
  */
-    __Pyx_TraceLine(2089,0,__PYX_ERR(0, 2089, __pyx_L1_error))
-    __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_self->__pyx_base.env_dict, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2089, __pyx_L1_error)
+    __Pyx_TraceLine(2106,0,__PYX_ERR(0, 2106, __pyx_L1_error))
+    __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_self->__pyx_base.env_dict, __pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 2106, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_add_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2089, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_add_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 2106, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = NULL;
     __pyx_t_16 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_10);
       if (likely(__pyx_t_7)) {
@@ -33910,88 +34116,88 @@
         __Pyx_DECREF_SET(__pyx_t_10, function);
         __pyx_t_16 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_10)) {
       PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_5, __pyx_t_6};
-      __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2088, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2105, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
       PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_5, __pyx_t_6};
-      __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2088, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2105, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_8 = PyTuple_New(2+__pyx_t_16); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2088, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(2+__pyx_t_16); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 2105, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_7) {
         __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7); __pyx_t_7 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_16, __pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_16, __pyx_t_6);
       __pyx_t_5 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_8, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2088, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_8, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 2105, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":2088
+    /* "cpprb/PyReplayBuffer.pyx":2105
  * 
  *         for name, b in self.buffer.items():
  *             b[add_idx] = np.reshape(np.array(kwargs[name],copy=False,ndmin=2),             # <<<<<<<<<<<<<<
  *                                     self.env_dict[name]["add_shape"])
  * 
  */
-    __Pyx_TraceLine(2088,0,__PYX_ERR(0, 2088, __pyx_L1_error))
-    if (unlikely(PyObject_SetItem(__pyx_v_b, __pyx_v_add_idx, __pyx_t_9) < 0)) __PYX_ERR(0, 2088, __pyx_L1_error)
+    __Pyx_TraceLine(2105,0,__PYX_ERR(0, 2105, __pyx_L1_error))
+    if (unlikely(PyObject_SetItem(__pyx_v_b, __pyx_v_add_idx, __pyx_t_9) < 0)) __PYX_ERR(0, 2105, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2091
+  /* "cpprb/PyReplayBuffer.pyx":2108
  *                                     self.env_dict[name]["add_shape"])
  * 
  *         self._unlock_explorer()             # <<<<<<<<<<<<<<
  *         return index
  * 
  */
-  __Pyx_TraceLine(2091,0,__PYX_ERR(0, 2091, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base._unlock_explorer(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2091, __pyx_L1_error)
+  __Pyx_TraceLine(2108,0,__PYX_ERR(0, 2108, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base._unlock_explorer(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2108, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2092
+  /* "cpprb/PyReplayBuffer.pyx":2109
  * 
  *         self._unlock_explorer()
  *         return index             # <<<<<<<<<<<<<<
  * 
  *     def sample(self,batch_size,beta = 0.4):
  */
-  __Pyx_TraceLine(2092,0,__PYX_ERR(0, 2092, __pyx_L1_error))
+  __Pyx_TraceLine(2109,0,__PYX_ERR(0, 2109, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2092, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2022
+  /* "cpprb/PyReplayBuffer.pyx":2039
  *         self.learner_ready.wait()
  * 
  *     def add(self,*,priorities = None,**kwargs):             # <<<<<<<<<<<<<<
  *         r"""Add transition(s) into replay buffer.
  * 
  */
 
@@ -34015,15 +34221,15 @@
   __Pyx_XDECREF(__pyx_v_priorities);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":2094
+/* "cpprb/PyReplayBuffer.pyx":2111
  *         return index
  * 
  *     def sample(self,batch_size,beta = 0.4):             # <<<<<<<<<<<<<<
  *         r"""Sample the stored transitions.
  * 
  */
 
@@ -34063,15 +34269,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_beta);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "sample") < 0)) __PYX_ERR(0, 2094, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "sample") < 0)) __PYX_ERR(0, 2111, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -34079,15 +34285,15 @@
       }
     }
     __pyx_v_batch_size = values[0];
     __pyx_v_beta = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("sample", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 2094, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("sample", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 2111, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPPrioritizedReplayBuffer.sample", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_4sample(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self), __pyx_v_batch_size, __pyx_v_beta);
 
@@ -34107,185 +34313,185 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sample", 0);
-  __Pyx_TraceCall("sample", __pyx_f[0], 2094, 0, __PYX_ERR(0, 2094, __pyx_L1_error));
+  __Pyx_TraceCall("sample", __pyx_f[0], 2111, 0, __PYX_ERR(0, 2111, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":2120
+  /* "cpprb/PyReplayBuffer.pyx":2137
  *         (:math:`= w_{i}/\max_{j}(w_{j})`), which ensure the weights :math:`\leq` 1.
  *         """
  *         self._lock_learner_per()             # <<<<<<<<<<<<<<
  *         self.per.ptr().sample(batch_size,beta,
  *                               self.weights.vec,self.indexes.vec,
  */
-  __Pyx_TraceLine(2120,0,__PYX_ERR(0, 2120, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->_lock_learner_per(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2120, __pyx_L1_error)
+  __Pyx_TraceLine(2137,0,__PYX_ERR(0, 2137, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->_lock_learner_per(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2137, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2121
+  /* "cpprb/PyReplayBuffer.pyx":2138
  *         """
  *         self._lock_learner_per()
  *         self.per.ptr().sample(batch_size,beta,             # <<<<<<<<<<<<<<
  *                               self.weights.vec,self.indexes.vec,
  *                               self.get_stored_size())
  */
-  __Pyx_TraceLine(2121,0,__PYX_ERR(0, 2121, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_batch_size); if (unlikely((__pyx_t_1 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 2121, __pyx_L1_error)
-  __pyx_t_2 = __pyx_PyFloat_AsFloat(__pyx_v_beta); if (unlikely((__pyx_t_2 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 2121, __pyx_L1_error)
+  __Pyx_TraceLine(2138,0,__PYX_ERR(0, 2138, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_batch_size); if (unlikely((__pyx_t_1 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 2138, __pyx_L1_error)
+  __pyx_t_2 = __pyx_PyFloat_AsFloat(__pyx_v_beta); if (unlikely((__pyx_t_2 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 2138, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2123
+  /* "cpprb/PyReplayBuffer.pyx":2140
  *         self.per.ptr().sample(batch_size,beta,
  *                               self.weights.vec,self.indexes.vec,
  *                               self.get_stored_size())             # <<<<<<<<<<<<<<
  *         cdef idx = self.indexes.as_numpy()
  * 
  */
-  __Pyx_TraceLine(2123,0,__PYX_ERR(0, 2123, __pyx_L1_error))
+  __Pyx_TraceLine(2140,0,__PYX_ERR(0, 2140, __pyx_L1_error))
   ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler *)__pyx_v_self->per->__pyx_vtab)->ptr(__pyx_v_self->per)->sample(__pyx_t_1, __pyx_t_2, __pyx_v_self->weights->vec, __pyx_v_self->indexes->vec, ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_stored_size(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self), 0));
 
-  /* "cpprb/PyReplayBuffer.pyx":2124
+  /* "cpprb/PyReplayBuffer.pyx":2141
  *                               self.weights.vec,self.indexes.vec,
  *                               self.get_stored_size())
  *         cdef idx = self.indexes.as_numpy()             # <<<<<<<<<<<<<<
  * 
  *         self._lock_learner_unlock_learner_per()
  */
-  __Pyx_TraceLine(2124,0,__PYX_ERR(0, 2124, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->indexes), __pyx_n_s_as_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2124, __pyx_L1_error)
+  __Pyx_TraceLine(2141,0,__PYX_ERR(0, 2141, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->indexes), __pyx_n_s_as_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2124, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_idx = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2126
+  /* "cpprb/PyReplayBuffer.pyx":2143
  *         cdef idx = self.indexes.as_numpy()
  * 
  *         self._lock_learner_unlock_learner_per()             # <<<<<<<<<<<<<<
  * 
  *         samples = self._encode_sample(idx)
  */
-  __Pyx_TraceLine(2126,0,__PYX_ERR(0, 2126, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->_lock_learner_unlock_learner_per(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2126, __pyx_L1_error)
+  __Pyx_TraceLine(2143,0,__PYX_ERR(0, 2143, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->_lock_learner_unlock_learner_per(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2143, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2128
+  /* "cpprb/PyReplayBuffer.pyx":2145
  *         self._lock_learner_unlock_learner_per()
  * 
  *         samples = self._encode_sample(idx)             # <<<<<<<<<<<<<<
  *         self.unchange_since_sample[:] = True
  *         self._unlock_learner()
  */
-  __Pyx_TraceLine(2128,0,__PYX_ERR(0, 2128, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_encode_sample); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2128, __pyx_L1_error)
+  __Pyx_TraceLine(2145,0,__PYX_ERR(0, 2145, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_encode_sample); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_idx) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_idx);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2128, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_samples = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2129
+  /* "cpprb/PyReplayBuffer.pyx":2146
  * 
  *         samples = self._encode_sample(idx)
  *         self.unchange_since_sample[:] = True             # <<<<<<<<<<<<<<
  *         self._unlock_learner()
  * 
  */
-  __Pyx_TraceLine(2129,0,__PYX_ERR(0, 2129, __pyx_L1_error))
-  if (__Pyx_PyObject_SetSlice(__pyx_v_self->unchange_since_sample, Py_True, 0, 0, NULL, NULL, &__pyx_slice__16, 0, 0, 1) < 0) __PYX_ERR(0, 2129, __pyx_L1_error)
+  __Pyx_TraceLine(2146,0,__PYX_ERR(0, 2146, __pyx_L1_error))
+  if (__Pyx_PyObject_SetSlice(__pyx_v_self->unchange_since_sample, Py_True, 0, 0, NULL, NULL, &__pyx_slice__16, 0, 0, 1) < 0) __PYX_ERR(0, 2146, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2130
+  /* "cpprb/PyReplayBuffer.pyx":2147
  *         samples = self._encode_sample(idx)
  *         self.unchange_since_sample[:] = True
  *         self._unlock_learner()             # <<<<<<<<<<<<<<
  * 
  *         samples['weights'] = self.weights.as_numpy()
  */
-  __Pyx_TraceLine(2130,0,__PYX_ERR(0, 2130, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base._unlock_learner(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2130, __pyx_L1_error)
+  __Pyx_TraceLine(2147,0,__PYX_ERR(0, 2147, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base._unlock_learner(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2147, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2132
+  /* "cpprb/PyReplayBuffer.pyx":2149
  *         self._unlock_learner()
  * 
  *         samples['weights'] = self.weights.as_numpy()             # <<<<<<<<<<<<<<
  *         samples['indexes'] = idx
  * 
  */
-  __Pyx_TraceLine(2132,0,__PYX_ERR(0, 2132, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->weights), __pyx_n_s_as_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2132, __pyx_L1_error)
+  __Pyx_TraceLine(2149,0,__PYX_ERR(0, 2149, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->weights), __pyx_n_s_as_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2132, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_samples, __pyx_n_u_weights, __pyx_t_3) < 0)) __PYX_ERR(0, 2132, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_v_samples, __pyx_n_u_weights, __pyx_t_3) < 0)) __PYX_ERR(0, 2149, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2133
+  /* "cpprb/PyReplayBuffer.pyx":2150
  * 
  *         samples['weights'] = self.weights.as_numpy()
  *         samples['indexes'] = idx             # <<<<<<<<<<<<<<
  * 
  *         return samples
  */
-  __Pyx_TraceLine(2133,0,__PYX_ERR(0, 2133, __pyx_L1_error))
-  if (unlikely(PyObject_SetItem(__pyx_v_samples, __pyx_n_u_indexes, __pyx_v_idx) < 0)) __PYX_ERR(0, 2133, __pyx_L1_error)
+  __Pyx_TraceLine(2150,0,__PYX_ERR(0, 2150, __pyx_L1_error))
+  if (unlikely(PyObject_SetItem(__pyx_v_samples, __pyx_n_u_indexes, __pyx_v_idx) < 0)) __PYX_ERR(0, 2150, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2135
+  /* "cpprb/PyReplayBuffer.pyx":2152
  *         samples['indexes'] = idx
  * 
  *         return samples             # <<<<<<<<<<<<<<
  * 
  *     def update_priorities(self,indexes,priorities):
  */
-  __Pyx_TraceLine(2135,0,__PYX_ERR(0, 2135, __pyx_L1_error))
+  __Pyx_TraceLine(2152,0,__PYX_ERR(0, 2152, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_samples);
   __pyx_r = __pyx_v_samples;
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2094
+  /* "cpprb/PyReplayBuffer.pyx":2111
  *         return index
  * 
  *     def sample(self,batch_size,beta = 0.4):             # <<<<<<<<<<<<<<
  *         r"""Sample the stored transitions.
  * 
  */
 
@@ -34301,15 +34507,15 @@
   __Pyx_XDECREF(__pyx_v_samples);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":2137
+/* "cpprb/PyReplayBuffer.pyx":2154
  *         return samples
  * 
  *     def update_priorities(self,indexes,priorities):             # <<<<<<<<<<<<<<
  *         r"""Update priorities
  * 
  */
 
@@ -34344,32 +34550,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indexes)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_priorities)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("update_priorities", 1, 2, 2, 1); __PYX_ERR(0, 2137, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("update_priorities", 1, 2, 2, 1); __PYX_ERR(0, 2154, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "update_priorities") < 0)) __PYX_ERR(0, 2137, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "update_priorities") < 0)) __PYX_ERR(0, 2154, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_indexes = values[0];
     __pyx_v_priorities = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("update_priorities", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 2137, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("update_priorities", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 2154, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPPrioritizedReplayBuffer.update_priorities", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_6update_priorities(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self), __pyx_v_indexes, __pyx_v_priorities);
 
@@ -34398,167 +34604,167 @@
   Py_ssize_t __pyx_t_9;
   int __pyx_t_10;
   size_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("update_priorities", 0);
-  __Pyx_TraceCall("update_priorities", __pyx_f[0], 2137, 0, __PYX_ERR(0, 2137, __pyx_L1_error));
+  __Pyx_TraceCall("update_priorities", __pyx_f[0], 2154, 0, __PYX_ERR(0, 2154, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":2156
+  /* "cpprb/PyReplayBuffer.pyx":2173
  *         """
  * 
  *         if priorities is None:             # <<<<<<<<<<<<<<
  *             raise TypeError("`properties` must not be `None`")
  * 
  */
-  __Pyx_TraceLine(2156,0,__PYX_ERR(0, 2156, __pyx_L1_error))
+  __Pyx_TraceLine(2173,0,__PYX_ERR(0, 2173, __pyx_L1_error))
   __pyx_t_1 = (__pyx_v_priorities == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "cpprb/PyReplayBuffer.pyx":2157
+    /* "cpprb/PyReplayBuffer.pyx":2174
  * 
  *         if priorities is None:
  *             raise TypeError("`properties` must not be `None`")             # <<<<<<<<<<<<<<
  * 
  *         cdef const size_t [:] idx = Csize(indexes)
  */
-    __Pyx_TraceLine(2157,0,__PYX_ERR(0, 2157, __pyx_L1_error))
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2157, __pyx_L1_error)
+    __Pyx_TraceLine(2174,0,__PYX_ERR(0, 2174, __pyx_L1_error))
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2174, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 2157, __pyx_L1_error)
+    __PYX_ERR(0, 2174, __pyx_L1_error)
 
-    /* "cpprb/PyReplayBuffer.pyx":2156
+    /* "cpprb/PyReplayBuffer.pyx":2173
  *         """
  * 
  *         if priorities is None:             # <<<<<<<<<<<<<<
  *             raise TypeError("`properties` must not be `None`")
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":2159
+  /* "cpprb/PyReplayBuffer.pyx":2176
  *             raise TypeError("`properties` must not be `None`")
  * 
  *         cdef const size_t [:] idx = Csize(indexes)             # <<<<<<<<<<<<<<
  *         cdef const float [:] ps = Cfloat(priorities)
  * 
  */
-  __Pyx_TraceLine(2159,0,__PYX_ERR(0, 2159, __pyx_L1_error))
-  __pyx_t_4 = __pyx_f_5cpprb_14PyReplayBuffer_Csize(__pyx_v_indexes); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 2159, __pyx_L1_error)
+  __Pyx_TraceLine(2176,0,__PYX_ERR(0, 2176, __pyx_L1_error))
+  __pyx_t_4 = __pyx_f_5cpprb_14PyReplayBuffer_Csize(__pyx_v_indexes); if (unlikely(!__pyx_t_4.memview)) __PYX_ERR(0, 2176, __pyx_L1_error)
   __pyx_v_idx = __pyx_t_4;
   __pyx_t_4.memview = NULL;
   __pyx_t_4.data = NULL;
 
-  /* "cpprb/PyReplayBuffer.pyx":2160
+  /* "cpprb/PyReplayBuffer.pyx":2177
  * 
  *         cdef const size_t [:] idx = Csize(indexes)
  *         cdef const float [:] ps = Cfloat(priorities)             # <<<<<<<<<<<<<<
  * 
  *         self.idx_vec.clear()
  */
-  __Pyx_TraceLine(2160,0,__PYX_ERR(0, 2160, __pyx_L1_error))
-  __pyx_t_5 = __pyx_f_5cpprb_14PyReplayBuffer_Cfloat(__pyx_v_priorities); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 2160, __pyx_L1_error)
+  __Pyx_TraceLine(2177,0,__PYX_ERR(0, 2177, __pyx_L1_error))
+  __pyx_t_5 = __pyx_f_5cpprb_14PyReplayBuffer_Cfloat(__pyx_v_priorities); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 2177, __pyx_L1_error)
   __pyx_v_ps = __pyx_t_5;
   __pyx_t_5.memview = NULL;
   __pyx_t_5.data = NULL;
 
-  /* "cpprb/PyReplayBuffer.pyx":2162
+  /* "cpprb/PyReplayBuffer.pyx":2179
  *         cdef const float [:] ps = Cfloat(priorities)
  * 
  *         self.idx_vec.clear()             # <<<<<<<<<<<<<<
  *         self.idx_vec.reserve(idx.shape[0])
  * 
  */
-  __Pyx_TraceLine(2162,0,__PYX_ERR(0, 2162, __pyx_L1_error))
+  __Pyx_TraceLine(2179,0,__PYX_ERR(0, 2179, __pyx_L1_error))
   __pyx_v_self->idx_vec.clear();
 
-  /* "cpprb/PyReplayBuffer.pyx":2163
+  /* "cpprb/PyReplayBuffer.pyx":2180
  * 
  *         self.idx_vec.clear()
  *         self.idx_vec.reserve(idx.shape[0])             # <<<<<<<<<<<<<<
  * 
  *         self.ps_vec.clear()
  */
-  __Pyx_TraceLine(2163,0,__PYX_ERR(0, 2163, __pyx_L1_error))
+  __Pyx_TraceLine(2180,0,__PYX_ERR(0, 2180, __pyx_L1_error))
   __pyx_v_self->idx_vec.reserve((__pyx_v_idx.shape[0]));
 
-  /* "cpprb/PyReplayBuffer.pyx":2165
+  /* "cpprb/PyReplayBuffer.pyx":2182
  *         self.idx_vec.reserve(idx.shape[0])
  * 
  *         self.ps_vec.clear()             # <<<<<<<<<<<<<<
  *         self.ps_vec.reserve(ps.shape[0])
  * 
  */
-  __Pyx_TraceLine(2165,0,__PYX_ERR(0, 2165, __pyx_L1_error))
+  __Pyx_TraceLine(2182,0,__PYX_ERR(0, 2182, __pyx_L1_error))
   __pyx_v_self->ps_vec.clear();
 
-  /* "cpprb/PyReplayBuffer.pyx":2166
+  /* "cpprb/PyReplayBuffer.pyx":2183
  * 
  *         self.ps_vec.clear()
  *         self.ps_vec.reserve(ps.shape[0])             # <<<<<<<<<<<<<<
  * 
  *         self._lock_learner_per()
  */
-  __Pyx_TraceLine(2166,0,__PYX_ERR(0, 2166, __pyx_L1_error))
+  __Pyx_TraceLine(2183,0,__PYX_ERR(0, 2183, __pyx_L1_error))
   __pyx_v_self->ps_vec.reserve((__pyx_v_ps.shape[0]));
 
-  /* "cpprb/PyReplayBuffer.pyx":2168
+  /* "cpprb/PyReplayBuffer.pyx":2185
  *         self.ps_vec.reserve(ps.shape[0])
  * 
  *         self._lock_learner_per()             # <<<<<<<<<<<<<<
  *         cdef size_t stored_size = self.get_stored_size()
  *         for _i in range(idx.shape[0]):
  */
-  __Pyx_TraceLine(2168,0,__PYX_ERR(0, 2168, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->_lock_learner_per(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2168, __pyx_L1_error)
+  __Pyx_TraceLine(2185,0,__PYX_ERR(0, 2185, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->_lock_learner_per(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2185, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2169
+  /* "cpprb/PyReplayBuffer.pyx":2186
  * 
  *         self._lock_learner_per()
  *         cdef size_t stored_size = self.get_stored_size()             # <<<<<<<<<<<<<<
  *         for _i in range(idx.shape[0]):
  *             if idx[_i] < stored_size and self.unchange_since_sample[idx[_i]]:
  */
-  __Pyx_TraceLine(2169,0,__PYX_ERR(0, 2169, __pyx_L1_error))
+  __Pyx_TraceLine(2186,0,__PYX_ERR(0, 2186, __pyx_L1_error))
   __pyx_v_stored_size = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_stored_size(((struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *)__pyx_v_self), 0);
 
-  /* "cpprb/PyReplayBuffer.pyx":2170
+  /* "cpprb/PyReplayBuffer.pyx":2187
  *         self._lock_learner_per()
  *         cdef size_t stored_size = self.get_stored_size()
  *         for _i in range(idx.shape[0]):             # <<<<<<<<<<<<<<
  *             if idx[_i] < stored_size and self.unchange_since_sample[idx[_i]]:
  *                 self.idx_vec.push_back(idx[_i])
  */
-  __Pyx_TraceLine(2170,0,__PYX_ERR(0, 2170, __pyx_L1_error))
+  __Pyx_TraceLine(2187,0,__PYX_ERR(0, 2187, __pyx_L1_error))
   __pyx_t_6 = (__pyx_v_idx.shape[0]);
   __pyx_t_7 = __pyx_t_6;
   for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
     __pyx_v__i = __pyx_t_8;
 
-    /* "cpprb/PyReplayBuffer.pyx":2171
+    /* "cpprb/PyReplayBuffer.pyx":2188
  *         cdef size_t stored_size = self.get_stored_size()
  *         for _i in range(idx.shape[0]):
  *             if idx[_i] < stored_size and self.unchange_since_sample[idx[_i]]:             # <<<<<<<<<<<<<<
  *                 self.idx_vec.push_back(idx[_i])
  *                 self.ps_vec.push_back(ps[_i])
  */
-    __Pyx_TraceLine(2171,0,__PYX_ERR(0, 2171, __pyx_L1_error))
+    __Pyx_TraceLine(2188,0,__PYX_ERR(0, 2188, __pyx_L1_error))
     __pyx_t_9 = __pyx_v__i;
     __pyx_t_10 = -1;
     if (__pyx_t_9 < 0) {
       __pyx_t_9 += __pyx_v_idx.shape[0];
       if (unlikely(__pyx_t_9 < 0)) __pyx_t_10 = 0;
     } else if (unlikely(__pyx_t_9 >= __pyx_v_idx.shape[0])) __pyx_t_10 = 0;
     if (unlikely(__pyx_t_10 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_10);
-      __PYX_ERR(0, 2171, __pyx_L1_error)
+      __PYX_ERR(0, 2188, __pyx_L1_error)
     }
     __pyx_t_1 = (((*((size_t const  *) ( /* dim=0 */ (__pyx_v_idx.data + __pyx_t_9 * __pyx_v_idx.strides[0]) ))) < __pyx_v_stored_size) != 0);
     if (__pyx_t_1) {
     } else {
       __pyx_t_2 = __pyx_t_1;
       goto __pyx_L7_bool_binop_done;
     }
@@ -34566,142 +34772,142 @@
     __pyx_t_10 = -1;
     if (__pyx_t_9 < 0) {
       __pyx_t_9 += __pyx_v_idx.shape[0];
       if (unlikely(__pyx_t_9 < 0)) __pyx_t_10 = 0;
     } else if (unlikely(__pyx_t_9 >= __pyx_v_idx.shape[0])) __pyx_t_10 = 0;
     if (unlikely(__pyx_t_10 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_10);
-      __PYX_ERR(0, 2171, __pyx_L1_error)
+      __PYX_ERR(0, 2188, __pyx_L1_error)
     }
     __pyx_t_11 = (*((size_t const  *) ( /* dim=0 */ (__pyx_v_idx.data + __pyx_t_9 * __pyx_v_idx.strides[0]) )));
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_self->unchange_since_sample, __pyx_t_11, size_t const , 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2171, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_self->unchange_since_sample, __pyx_t_11, size_t const , 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2188, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 2171, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 2188, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_2 = __pyx_t_1;
     __pyx_L7_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "cpprb/PyReplayBuffer.pyx":2172
+      /* "cpprb/PyReplayBuffer.pyx":2189
  *         for _i in range(idx.shape[0]):
  *             if idx[_i] < stored_size and self.unchange_since_sample[idx[_i]]:
  *                 self.idx_vec.push_back(idx[_i])             # <<<<<<<<<<<<<<
  *                 self.ps_vec.push_back(ps[_i])
  * 
  */
-      __Pyx_TraceLine(2172,0,__PYX_ERR(0, 2172, __pyx_L1_error))
+      __Pyx_TraceLine(2189,0,__PYX_ERR(0, 2189, __pyx_L1_error))
       __pyx_t_9 = __pyx_v__i;
       __pyx_t_10 = -1;
       if (__pyx_t_9 < 0) {
         __pyx_t_9 += __pyx_v_idx.shape[0];
         if (unlikely(__pyx_t_9 < 0)) __pyx_t_10 = 0;
       } else if (unlikely(__pyx_t_9 >= __pyx_v_idx.shape[0])) __pyx_t_10 = 0;
       if (unlikely(__pyx_t_10 != -1)) {
         __Pyx_RaiseBufferIndexError(__pyx_t_10);
-        __PYX_ERR(0, 2172, __pyx_L1_error)
+        __PYX_ERR(0, 2189, __pyx_L1_error)
       }
       try {
         __pyx_v_self->idx_vec.push_back((*((size_t const  *) ( /* dim=0 */ (__pyx_v_idx.data + __pyx_t_9 * __pyx_v_idx.strides[0]) ))));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 2172, __pyx_L1_error)
+        __PYX_ERR(0, 2189, __pyx_L1_error)
       }
 
-      /* "cpprb/PyReplayBuffer.pyx":2173
+      /* "cpprb/PyReplayBuffer.pyx":2190
  *             if idx[_i] < stored_size and self.unchange_since_sample[idx[_i]]:
  *                 self.idx_vec.push_back(idx[_i])
  *                 self.ps_vec.push_back(ps[_i])             # <<<<<<<<<<<<<<
  * 
  *         cdef N = self.idx_vec.size()
  */
-      __Pyx_TraceLine(2173,0,__PYX_ERR(0, 2173, __pyx_L1_error))
+      __Pyx_TraceLine(2190,0,__PYX_ERR(0, 2190, __pyx_L1_error))
       __pyx_t_9 = __pyx_v__i;
       __pyx_t_10 = -1;
       if (__pyx_t_9 < 0) {
         __pyx_t_9 += __pyx_v_ps.shape[0];
         if (unlikely(__pyx_t_9 < 0)) __pyx_t_10 = 0;
       } else if (unlikely(__pyx_t_9 >= __pyx_v_ps.shape[0])) __pyx_t_10 = 0;
       if (unlikely(__pyx_t_10 != -1)) {
         __Pyx_RaiseBufferIndexError(__pyx_t_10);
-        __PYX_ERR(0, 2173, __pyx_L1_error)
+        __PYX_ERR(0, 2190, __pyx_L1_error)
       }
       try {
         __pyx_v_self->ps_vec.push_back((*((float const  *) ( /* dim=0 */ (__pyx_v_ps.data + __pyx_t_9 * __pyx_v_ps.strides[0]) ))));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 2173, __pyx_L1_error)
+        __PYX_ERR(0, 2190, __pyx_L1_error)
       }
 
-      /* "cpprb/PyReplayBuffer.pyx":2171
+      /* "cpprb/PyReplayBuffer.pyx":2188
  *         cdef size_t stored_size = self.get_stored_size()
  *         for _i in range(idx.shape[0]):
  *             if idx[_i] < stored_size and self.unchange_since_sample[idx[_i]]:             # <<<<<<<<<<<<<<
  *                 self.idx_vec.push_back(idx[_i])
  *                 self.ps_vec.push_back(ps[_i])
  */
     }
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":2175
+  /* "cpprb/PyReplayBuffer.pyx":2192
  *                 self.ps_vec.push_back(ps[_i])
  * 
  *         cdef N = self.idx_vec.size()             # <<<<<<<<<<<<<<
  *         if N > 0:
  *             self.per.ptr().update_priorities(self.idx_vec.data(),self.ps_vec.data(),N)
  */
-  __Pyx_TraceLine(2175,0,__PYX_ERR(0, 2175, __pyx_L1_error))
-  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_self->idx_vec.size()); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2175, __pyx_L1_error)
+  __Pyx_TraceLine(2192,0,__PYX_ERR(0, 2192, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_self->idx_vec.size()); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_N = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2176
+  /* "cpprb/PyReplayBuffer.pyx":2193
  * 
  *         cdef N = self.idx_vec.size()
  *         if N > 0:             # <<<<<<<<<<<<<<
  *             self.per.ptr().update_priorities(self.idx_vec.data(),self.ps_vec.data(),N)
  *         self._unlock_learner_per()
  */
-  __Pyx_TraceLine(2176,0,__PYX_ERR(0, 2176, __pyx_L1_error))
-  __pyx_t_3 = PyObject_RichCompare(__pyx_v_N, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2176, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 2176, __pyx_L1_error)
+  __Pyx_TraceLine(2193,0,__PYX_ERR(0, 2193, __pyx_L1_error))
+  __pyx_t_3 = PyObject_RichCompare(__pyx_v_N, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2193, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 2193, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_2) {
 
-    /* "cpprb/PyReplayBuffer.pyx":2177
+    /* "cpprb/PyReplayBuffer.pyx":2194
  *         cdef N = self.idx_vec.size()
  *         if N > 0:
  *             self.per.ptr().update_priorities(self.idx_vec.data(),self.ps_vec.data(),N)             # <<<<<<<<<<<<<<
  *         self._unlock_learner_per()
  * 
  */
-    __Pyx_TraceLine(2177,0,__PYX_ERR(0, 2177, __pyx_L1_error))
-    __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_v_N); if (unlikely((__pyx_t_11 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 2177, __pyx_L1_error)
+    __Pyx_TraceLine(2194,0,__PYX_ERR(0, 2194, __pyx_L1_error))
+    __pyx_t_11 = __Pyx_PyInt_As_size_t(__pyx_v_N); if (unlikely((__pyx_t_11 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 2194, __pyx_L1_error)
     ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler *)__pyx_v_self->per->__pyx_vtab)->ptr(__pyx_v_self->per)->update_priorities(__pyx_v_self->idx_vec.data(), __pyx_v_self->ps_vec.data(), __pyx_t_11);
 
-    /* "cpprb/PyReplayBuffer.pyx":2176
+    /* "cpprb/PyReplayBuffer.pyx":2193
  * 
  *         cdef N = self.idx_vec.size()
  *         if N > 0:             # <<<<<<<<<<<<<<
  *             self.per.ptr().update_priorities(self.idx_vec.data(),self.ps_vec.data(),N)
  *         self._unlock_learner_per()
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":2178
+  /* "cpprb/PyReplayBuffer.pyx":2195
  *         if N > 0:
  *             self.per.ptr().update_priorities(self.idx_vec.data(),self.ps_vec.data(),N)
  *         self._unlock_learner_per()             # <<<<<<<<<<<<<<
  * 
  *     cpdef void clear(self) except *:
  */
-  __Pyx_TraceLine(2178,0,__PYX_ERR(0, 2178, __pyx_L1_error))
-  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->_unlock_learner_per(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2178, __pyx_L1_error)
+  __Pyx_TraceLine(2195,0,__PYX_ERR(0, 2195, __pyx_L1_error))
+  ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *)__pyx_v_self->__pyx_base.__pyx_vtab)->_unlock_learner_per(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2195, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2137
+  /* "cpprb/PyReplayBuffer.pyx":2154
  *         return samples
  * 
  *     def update_priorities(self,indexes,priorities):             # <<<<<<<<<<<<<<
  *         r"""Update priorities
  * 
  */
 
@@ -34720,15 +34926,15 @@
   __Pyx_XDECREF(__pyx_v_N);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":2180
+/* "cpprb/PyReplayBuffer.pyx":2197
  *         self._unlock_learner_per()
  * 
  *     cpdef void clear(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Clear replay buffer
  *         """
  */
 
@@ -34740,25 +34946,25 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear", 0);
-  __Pyx_TraceCall("clear", __pyx_f[0], 2180, 0, __PYX_ERR(0, 2180, __pyx_L1_error));
+  __Pyx_TraceCall("clear", __pyx_f[0], 2197, 0, __PYX_ERR(0, 2197, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2180, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clear); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2197, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_9clear)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -34766,15 +34972,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2180, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2197, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
@@ -34786,64 +34992,64 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":2183
+  /* "cpprb/PyReplayBuffer.pyx":2200
  *         r"""Clear replay buffer
  *         """
  *         super(MPPrioritizedReplayBuffer,self).clear()             # <<<<<<<<<<<<<<
  *         clear(self.per.ptr())
  * 
  */
-  __Pyx_TraceLine(2183,0,__PYX_ERR(0, 2183, __pyx_L1_error))
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2183, __pyx_L1_error)
+  __Pyx_TraceLine(2200,0,__PYX_ERR(0, 2200, __pyx_L1_error))
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer));
   PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer));
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)__pyx_v_self));
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2183, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2183, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_clear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
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
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2183, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2184
+  /* "cpprb/PyReplayBuffer.pyx":2201
  *         """
  *         super(MPPrioritizedReplayBuffer,self).clear()
  *         clear(self.per.ptr())             # <<<<<<<<<<<<<<
  * 
  *     cpdef float get_max_priority(self):
  */
-  __Pyx_TraceLine(2184,0,__PYX_ERR(0, 2184, __pyx_L1_error))
+  __Pyx_TraceLine(2201,0,__PYX_ERR(0, 2201, __pyx_L1_error))
   ymd::clear<ymd::CppThreadSafePrioritizedSampler<float> >(((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler *)__pyx_v_self->per->__pyx_vtab)->ptr(__pyx_v_self->per));
 
-  /* "cpprb/PyReplayBuffer.pyx":2180
+  /* "cpprb/PyReplayBuffer.pyx":2197
  *         self._unlock_learner_per()
  * 
  *     cpdef void clear(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Clear replay buffer
  *         """
  */
 
@@ -34879,18 +35085,18 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear", 0);
-  __Pyx_TraceCall("clear (wrapper)", __pyx_f[0], 2180, 0, __PYX_ERR(0, 2180, __pyx_L1_error));
+  __Pyx_TraceCall("clear (wrapper)", __pyx_f[0], 2197, 0, __PYX_ERR(0, 2197, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_f_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_clear(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2180, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2180, __pyx_L1_error)
+  __pyx_f_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_clear(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2197, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -34900,15 +35106,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":2186
+/* "cpprb/PyReplayBuffer.pyx":2203
  *         clear(self.per.ptr())
  * 
  *     cpdef float get_max_priority(self):             # <<<<<<<<<<<<<<
  *         r"""Get the max priority of stored priorities
  * 
  */
 
@@ -34922,25 +35128,25 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   float __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_max_priority", 0);
-  __Pyx_TraceCall("get_max_priority", __pyx_f[0], 2186, 0, __PYX_ERR(0, 2186, __pyx_L1_error));
+  __Pyx_TraceCall("get_max_priority", __pyx_f[0], 2203, 0, __PYX_ERR(0, 2203, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_max_priority); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2186, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_max_priority); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2203, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_11get_max_priority)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -34948,18 +35154,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2186, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2203, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __pyx_PyFloat_AsFloat(__pyx_t_2); if (unlikely((__pyx_t_5 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 2186, __pyx_L1_error)
+        __pyx_t_5 = __pyx_PyFloat_AsFloat(__pyx_t_2); if (unlikely((__pyx_t_5 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 2203, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -34970,26 +35176,26 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":2194
+  /* "cpprb/PyReplayBuffer.pyx":2211
  *             the max priority of stored priorities
  *         """
  *         return self.per.ptr().get_max_priority()             # <<<<<<<<<<<<<<
  * 
  *     cpdef void on_episode_end(self) except *:
  */
-  __Pyx_TraceLine(2194,0,__PYX_ERR(0, 2194, __pyx_L1_error))
+  __Pyx_TraceLine(2211,0,__PYX_ERR(0, 2211, __pyx_L1_error))
   __pyx_r = ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler *)__pyx_v_self->per->__pyx_vtab)->ptr(__pyx_v_self->per)->get_max_priority();
   goto __pyx_L0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2186
+  /* "cpprb/PyReplayBuffer.pyx":2203
  *         clear(self.per.ptr())
  * 
  *     cpdef float get_max_priority(self):             # <<<<<<<<<<<<<<
  *         r"""Get the max priority of stored priorities
  * 
  */
 
@@ -35026,17 +35232,17 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_max_priority", 0);
-  __Pyx_TraceCall("get_max_priority (wrapper)", __pyx_f[0], 2186, 0, __PYX_ERR(0, 2186, __pyx_L1_error));
+  __Pyx_TraceCall("get_max_priority (wrapper)", __pyx_f[0], 2203, 0, __PYX_ERR(0, 2203, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_get_max_priority(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2186, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_get_max_priority(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -35046,15 +35252,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":2196
+/* "cpprb/PyReplayBuffer.pyx":2213
  *         return self.per.ptr().get_max_priority()
  * 
  *     cpdef void on_episode_end(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Call on episode end
  * 
  */
 
@@ -35066,25 +35272,25 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_episode_end", 0);
-  __Pyx_TraceCall("on_episode_end", __pyx_f[0], 2196, 0, __PYX_ERR(0, 2196, __pyx_L1_error));
+  __Pyx_TraceCall("on_episode_end", __pyx_f[0], 2213, 0, __PYX_ERR(0, 2213, __pyx_L1_error));
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_episode_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2196, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_on_episode_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2213, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_13on_episode_end)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -35092,15 +35298,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2196, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2213, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
@@ -35112,37 +35318,37 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":2197
+  /* "cpprb/PyReplayBuffer.pyx":2214
  * 
  *     cpdef void on_episode_end(self) except *:
  *         r"""Call on episode end             # <<<<<<<<<<<<<<
  * 
  *         Notes
  */
-  __Pyx_TraceLine(2197,0,__PYX_ERR(0, 2197, __pyx_L1_error))
+  __Pyx_TraceLine(2214,0,__PYX_ERR(0, 2214, __pyx_L1_error))
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.MPPrioritizedReplayBuffer.on_episode_end", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "cpprb/PyReplayBuffer.pyx":2196
+/* "cpprb/PyReplayBuffer.pyx":2213
  *         return self.per.ptr().get_max_priority()
  * 
  *     cpdef void on_episode_end(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Call on episode end
  * 
  */
 
@@ -35165,18 +35371,18 @@
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("on_episode_end", 0);
-  __Pyx_TraceCall("on_episode_end (wrapper)", __pyx_f[0], 2196, 0, __PYX_ERR(0, 2196, __pyx_L1_error));
+  __Pyx_TraceCall("on_episode_end (wrapper)", __pyx_f[0], 2213, 0, __PYX_ERR(0, 2213, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_f_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_on_episode_end(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2196, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2196, __pyx_L1_error)
+  __pyx_f_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_on_episode_end(__pyx_v_self, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2213, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -35678,15 +35884,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":2209
+/* "cpprb/PyReplayBuffer.pyx":2226
  * 
  * @cython.embedsignature(True)
  * def create_buffer(size,env_dict=None,*,prioritized = False,**kwargs):             # <<<<<<<<<<<<<<
  *     r"""Create specified version of replay buffer
  * 
  */
 
@@ -35737,15 +35943,15 @@
       }
       if (kw_args == 1) {
         const Py_ssize_t index = 2;
         PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
         if (value) { values[index] = value; kw_args--; }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "create_buffer") < 0)) __PYX_ERR(0, 2209, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "create_buffer") < 0)) __PYX_ERR(0, 2226, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -35754,15 +35960,15 @@
     }
     __pyx_v_size = values[0];
     __pyx_v_env_dict = values[1];
     __pyx_v_prioritized = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("create_buffer", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 2209, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("create_buffer", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 2226, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.create_buffer", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_6create_buffer(__pyx_self, __pyx_v_size, __pyx_v_env_dict, __pyx_v_prioritized, __pyx_v_kwargs);
@@ -35785,150 +35991,150 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__28)
   __Pyx_RefNannySetupContext("create_buffer", 0);
-  __Pyx_TraceCall("create_buffer", __pyx_f[0], 2209, 0, __PYX_ERR(0, 2209, __pyx_L1_error));
+  __Pyx_TraceCall("create_buffer", __pyx_f[0], 2226, 0, __PYX_ERR(0, 2226, __pyx_L1_error));
 
-  /* "cpprb/PyReplayBuffer.pyx":2236
+  /* "cpprb/PyReplayBuffer.pyx":2253
  *     Any other keyword arguments are passed to replay buffer constructor.
  *     """
  *     per = "Prioritized" if prioritized else ""             # <<<<<<<<<<<<<<
  * 
  *     buffer_name = f"{per}ReplayBuffer"
  */
-  __Pyx_TraceLine(2236,0,__PYX_ERR(0, 2236, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_prioritized); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 2236, __pyx_L1_error)
+  __Pyx_TraceLine(2253,0,__PYX_ERR(0, 2253, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_prioritized); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 2253, __pyx_L1_error)
   if (__pyx_t_2) {
     __Pyx_INCREF(__pyx_n_u_Prioritized);
     __pyx_t_1 = __pyx_n_u_Prioritized;
   } else {
     __Pyx_INCREF(__pyx_kp_u__29);
     __pyx_t_1 = __pyx_kp_u__29;
   }
   __pyx_v_per = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2238
+  /* "cpprb/PyReplayBuffer.pyx":2255
  *     per = "Prioritized" if prioritized else ""
  * 
  *     buffer_name = f"{per}ReplayBuffer"             # <<<<<<<<<<<<<<
  * 
  *     cls={"ReplayBuffer": ReplayBuffer,
  */
-  __Pyx_TraceLine(2238,0,__PYX_ERR(0, 2238, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyUnicode_Unicode(__pyx_v_per); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2238, __pyx_L1_error)
+  __Pyx_TraceLine(2255,0,__PYX_ERR(0, 2255, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyUnicode_Unicode(__pyx_v_per); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_t_1, __pyx_n_u_ReplayBuffer); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2238, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_t_1, __pyx_n_u_ReplayBuffer); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_buffer_name = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2240
+  /* "cpprb/PyReplayBuffer.pyx":2257
  *     buffer_name = f"{per}ReplayBuffer"
  * 
  *     cls={"ReplayBuffer": ReplayBuffer,             # <<<<<<<<<<<<<<
  *          "PrioritizedReplayBuffer": PrioritizedReplayBuffer}
  * 
  */
-  __Pyx_TraceLine(2240,0,__PYX_ERR(0, 2240, __pyx_L1_error))
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2240, __pyx_L1_error)
+  __Pyx_TraceLine(2257,0,__PYX_ERR(0, 2257, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_ReplayBuffer, ((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_ReplayBuffer)) < 0) __PYX_ERR(0, 2240, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_ReplayBuffer, ((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_ReplayBuffer)) < 0) __PYX_ERR(0, 2257, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2241
+  /* "cpprb/PyReplayBuffer.pyx":2258
  * 
  *     cls={"ReplayBuffer": ReplayBuffer,
  *          "PrioritizedReplayBuffer": PrioritizedReplayBuffer}             # <<<<<<<<<<<<<<
  * 
  *     buffer = cls.get(f"{buffer_name}",None)
  */
-  __Pyx_TraceLine(2241,0,__PYX_ERR(0, 2241, __pyx_L1_error))
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_PrioritizedReplayBuffer, ((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer)) < 0) __PYX_ERR(0, 2240, __pyx_L1_error)
+  __Pyx_TraceLine(2258,0,__PYX_ERR(0, 2258, __pyx_L1_error))
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_PrioritizedReplayBuffer, ((PyObject *)__pyx_ptype_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer)) < 0) __PYX_ERR(0, 2257, __pyx_L1_error)
   __pyx_v_cls = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2243
+  /* "cpprb/PyReplayBuffer.pyx":2260
  *          "PrioritizedReplayBuffer": PrioritizedReplayBuffer}
  * 
  *     buffer = cls.get(f"{buffer_name}",None)             # <<<<<<<<<<<<<<
  * 
  *     if buffer:
  */
-  __Pyx_TraceLine(2243,0,__PYX_ERR(0, 2243, __pyx_L1_error))
-  __pyx_t_3 = __Pyx_PyDict_GetItemDefault(__pyx_v_cls, __pyx_v_buffer_name, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2243, __pyx_L1_error)
+  __Pyx_TraceLine(2260,0,__PYX_ERR(0, 2260, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyDict_GetItemDefault(__pyx_v_cls, __pyx_v_buffer_name, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_buffer = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2245
+  /* "cpprb/PyReplayBuffer.pyx":2262
  *     buffer = cls.get(f"{buffer_name}",None)
  * 
  *     if buffer:             # <<<<<<<<<<<<<<
  *         return buffer(size,env_dict,**kwargs)
  * 
  */
-  __Pyx_TraceLine(2245,0,__PYX_ERR(0, 2245, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_buffer); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 2245, __pyx_L1_error)
+  __Pyx_TraceLine(2262,0,__PYX_ERR(0, 2262, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_buffer); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 2262, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "cpprb/PyReplayBuffer.pyx":2246
+    /* "cpprb/PyReplayBuffer.pyx":2263
  * 
  *     if buffer:
  *         return buffer(size,env_dict,**kwargs)             # <<<<<<<<<<<<<<
  * 
  *     raise NotImplementedError(f"{buffer_name} is not Implemented")
  */
-    __Pyx_TraceLine(2246,0,__PYX_ERR(0, 2246, __pyx_L1_error))
+    __Pyx_TraceLine(2263,0,__PYX_ERR(0, 2263, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2246, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_size);
     __Pyx_GIVEREF(__pyx_v_size);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_size);
     __Pyx_INCREF(__pyx_v_env_dict);
     __Pyx_GIVEREF(__pyx_v_env_dict);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_env_dict);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_v_buffer, __pyx_t_3, __pyx_v_kwargs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2246, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_v_buffer, __pyx_t_3, __pyx_v_kwargs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "cpprb/PyReplayBuffer.pyx":2245
+    /* "cpprb/PyReplayBuffer.pyx":2262
  *     buffer = cls.get(f"{buffer_name}",None)
  * 
  *     if buffer:             # <<<<<<<<<<<<<<
  *         return buffer(size,env_dict,**kwargs)
  * 
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":2248
+  /* "cpprb/PyReplayBuffer.pyx":2265
  *         return buffer(size,env_dict,**kwargs)
  * 
  *     raise NotImplementedError(f"{buffer_name} is not Implemented")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(2248,0,__PYX_ERR(0, 2248, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_v_buffer_name, __pyx_kp_u_is_not_Implemented); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2248, __pyx_L1_error)
+  __Pyx_TraceLine(2265,0,__PYX_ERR(0, 2265, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_v_buffer_name, __pyx_kp_u_is_not_Implemented); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2248, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_Raise(__pyx_t_3, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 2248, __pyx_L1_error)
+  __PYX_ERR(0, 2265, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2209
+  /* "cpprb/PyReplayBuffer.pyx":2226
  * 
  * @cython.embedsignature(True)
  * def create_buffer(size,env_dict=None,*,prioritized = False,**kwargs):             # <<<<<<<<<<<<<<
  *     r"""Create specified version of replay buffer
  * 
  */
 
@@ -35945,15 +36151,15 @@
   __Pyx_XDECREF(__pyx_v_buffer);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cpprb/PyReplayBuffer.pyx":2252
+/* "cpprb/PyReplayBuffer.pyx":2269
  * 
  * @cython.embedsignature(True)
  * def train(buffer: ReplayBuffer,             # <<<<<<<<<<<<<<
  *           env,
  *           get_action: Callable,
  */
 
@@ -35983,71 +36189,71 @@
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("train (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_buffer,&__pyx_n_s_env,&__pyx_n_s_get_action,&__pyx_n_s_update_policy,&__pyx_n_s_max_steps,&__pyx_n_s_max_episodes,&__pyx_n_s_batch_size,&__pyx_n_s_n_warmups,&__pyx_n_s_after_step,&__pyx_n_s_done_check,&__pyx_n_s_obs_update,&__pyx_n_s_rew_sum,&__pyx_n_s_episode_callback,&__pyx_n_s_logger,0};
     PyObject* values[14] = {0,0,0,0,0,0,0,0,0,0,0,0,0,0};
     values[4] = __pyx_k__30;
 
-    /* "cpprb/PyReplayBuffer.pyx":2257
+    /* "cpprb/PyReplayBuffer.pyx":2274
  *           update_policy: Callable,*,
  *           max_steps: int=int(1e6),
  *           max_episodes: Optional[int] = None,             # <<<<<<<<<<<<<<
  *           batch_size: int = 64,
  *           n_warmups: int = 0,
  */
     values[5] = ((PyObject *)Py_None);
     values[6] = ((PyObject *)__pyx_int_64);
     values[7] = ((PyObject *)__pyx_int_0);
 
-    /* "cpprb/PyReplayBuffer.pyx":2260
+    /* "cpprb/PyReplayBuffer.pyx":2277
  *           batch_size: int = 64,
  *           n_warmups: int = 0,
  *           after_step: Optional[Callable] = None,             # <<<<<<<<<<<<<<
  *           done_check: Optional[Callable] = None,
  *           obs_update: Optional[Callable] = None,
  */
     values[8] = ((PyObject *)Py_None);
 
-    /* "cpprb/PyReplayBuffer.pyx":2261
+    /* "cpprb/PyReplayBuffer.pyx":2278
  *           n_warmups: int = 0,
  *           after_step: Optional[Callable] = None,
  *           done_check: Optional[Callable] = None,             # <<<<<<<<<<<<<<
  *           obs_update: Optional[Callable] = None,
  *           rew_sum: Optional[Callable[[float, Any], float]] = None,
  */
     values[9] = ((PyObject *)Py_None);
 
-    /* "cpprb/PyReplayBuffer.pyx":2262
+    /* "cpprb/PyReplayBuffer.pyx":2279
  *           after_step: Optional[Callable] = None,
  *           done_check: Optional[Callable] = None,
  *           obs_update: Optional[Callable] = None,             # <<<<<<<<<<<<<<
  *           rew_sum: Optional[Callable[[float, Any], float]] = None,
  *           episode_callback: Optional[Callable[[int,int,float],Any]] = None,
  */
     values[10] = ((PyObject *)Py_None);
 
-    /* "cpprb/PyReplayBuffer.pyx":2263
+    /* "cpprb/PyReplayBuffer.pyx":2280
  *           done_check: Optional[Callable] = None,
  *           obs_update: Optional[Callable] = None,
  *           rew_sum: Optional[Callable[[float, Any], float]] = None,             # <<<<<<<<<<<<<<
  *           episode_callback: Optional[Callable[[int,int,float],Any]] = None,
  *           logger = None):
  */
     values[11] = ((PyObject *)Py_None);
 
-    /* "cpprb/PyReplayBuffer.pyx":2264
+    /* "cpprb/PyReplayBuffer.pyx":2281
  *           obs_update: Optional[Callable] = None,
  *           rew_sum: Optional[Callable[[float, Any], float]] = None,
  *           episode_callback: Optional[Callable[[int,int,float],Any]] = None,             # <<<<<<<<<<<<<<
  *           logger = None):
  *     r"""
  */
     values[12] = ((PyObject *)Py_None);
 
-    /* "cpprb/PyReplayBuffer.pyx":2265
+    /* "cpprb/PyReplayBuffer.pyx":2282
  *           rew_sum: Optional[Callable[[float, Any], float]] = None,
  *           episode_callback: Optional[Callable[[int,int,float],Any]] = None,
  *           logger = None):             # <<<<<<<<<<<<<<
  *     r"""
  *     Train RL policy (model)
  */
     values[13] = ((PyObject *)Py_None);
@@ -36071,38 +36277,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_buffer)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_env)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("train", 1, 4, 4, 1); __PYX_ERR(0, 2252, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("train", 1, 4, 4, 1); __PYX_ERR(0, 2269, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_get_action)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("train", 1, 4, 4, 2); __PYX_ERR(0, 2252, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("train", 1, 4, 4, 2); __PYX_ERR(0, 2269, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_update_policy)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("train", 1, 4, 4, 3); __PYX_ERR(0, 2252, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("train", 1, 4, 4, 3); __PYX_ERR(0, 2269, __pyx_L3_error)
         }
       }
       if (kw_args > 0 && likely(kw_args <= 10)) {
         Py_ssize_t index;
         for (index = 4; index < 14 && kw_args > 0; index++) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "train") < 0)) __PYX_ERR(0, 2252, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "train") < 0)) __PYX_ERR(0, 2269, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -36121,24 +36327,24 @@
     __pyx_v_obs_update = values[10];
     __pyx_v_rew_sum = values[11];
     __pyx_v_episode_callback = values[12];
     __pyx_v_logger = values[13];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("train", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 2252, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("train", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 2269, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("cpprb.PyReplayBuffer.train", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_buffer), __pyx_ptype_5cpprb_14PyReplayBuffer_ReplayBuffer, 1, "buffer", 0))) __PYX_ERR(0, 2252, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_buffer), __pyx_ptype_5cpprb_14PyReplayBuffer_ReplayBuffer, 1, "buffer", 0))) __PYX_ERR(0, 2269, __pyx_L1_error)
   __pyx_r = __pyx_pf_5cpprb_14PyReplayBuffer_8train(__pyx_self, __pyx_v_buffer, __pyx_v_env, __pyx_v_get_action, __pyx_v_update_policy, __pyx_v_max_steps, __pyx_v_max_episodes, __pyx_v_batch_size, __pyx_v_n_warmups, __pyx_v_after_step, __pyx_v_done_check, __pyx_v_obs_update, __pyx_v_rew_sum, __pyx_v_episode_callback, __pyx_v_logger);
 
-  /* "cpprb/PyReplayBuffer.pyx":2252
+  /* "cpprb/PyReplayBuffer.pyx":2269
  * 
  * @cython.embedsignature(True)
  * def train(buffer: ReplayBuffer,             # <<<<<<<<<<<<<<
  *           env,
  *           get_action: Callable,
  */
 
@@ -36207,553 +36413,553 @@
   double __pyx_t_23;
   double __pyx_t_24;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__31)
   __Pyx_RefNannySetupContext("train", 0);
-  __Pyx_TraceCall("train", __pyx_f[0], 2252, 0, __PYX_ERR(0, 2252, __pyx_L1_error));
+  __Pyx_TraceCall("train", __pyx_f[0], 2269, 0, __PYX_ERR(0, 2269, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_logger);
 
-  /* "cpprb/PyReplayBuffer.pyx":2310
+  /* "cpprb/PyReplayBuffer.pyx":2327
  *     `cpprb.train` is still beta release. API can be changed.
  *     """
  *     warnings.warn("`cpprb.train` is still beta release. API can be changed.")             # <<<<<<<<<<<<<<
  * 
  *     logger = logger or default_logger()
  */
-  __Pyx_TraceLine(2310,0,__PYX_ERR(0, 2310, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_warnings); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2310, __pyx_L1_error)
+  __Pyx_TraceLine(2327,0,__PYX_ERR(0, 2327, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_warnings); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2310, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_warn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_u_cpprb_train_is_still_beta_relea) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_cpprb_train_is_still_beta_relea);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2310, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2312
+  /* "cpprb/PyReplayBuffer.pyx":2329
  *     warnings.warn("`cpprb.train` is still beta release. API can be changed.")
  * 
  *     logger = logger or default_logger()             # <<<<<<<<<<<<<<
  * 
  *     cdef size_t size_t_limit = -1
  */
-  __Pyx_TraceLine(2312,0,__PYX_ERR(0, 2312, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_logger); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2312, __pyx_L1_error)
+  __Pyx_TraceLine(2329,0,__PYX_ERR(0, 2329, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_logger); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2329, __pyx_L1_error)
   if (!__pyx_t_4) {
   } else {
     __Pyx_INCREF(__pyx_v_logger);
     __pyx_t_1 = __pyx_v_logger;
     goto __pyx_L3_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_default_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2312, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_default_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2329, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2312, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2329, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_INCREF(__pyx_t_3);
   __pyx_t_1 = __pyx_t_3;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_L3_bool_binop_done:;
   __Pyx_DECREF_SET(__pyx_v_logger, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2314
+  /* "cpprb/PyReplayBuffer.pyx":2331
  *     logger = logger or default_logger()
  * 
  *     cdef size_t size_t_limit = -1             # <<<<<<<<<<<<<<
  *     if max_steps >= int(size_t_limit):
  *         raise ValueError(f"max_steps ({max_steps}) is too big. " +
  */
-  __Pyx_TraceLine(2314,0,__PYX_ERR(0, 2314, __pyx_L1_error))
+  __Pyx_TraceLine(2331,0,__PYX_ERR(0, 2331, __pyx_L1_error))
   __pyx_v_size_t_limit = -1L;
 
-  /* "cpprb/PyReplayBuffer.pyx":2315
+  /* "cpprb/PyReplayBuffer.pyx":2332
  * 
  *     cdef size_t size_t_limit = -1
  *     if max_steps >= int(size_t_limit):             # <<<<<<<<<<<<<<
  *         raise ValueError(f"max_steps ({max_steps}) is too big. " +
  *                          f"max_steps < {size_t_limit}")
  */
-  __Pyx_TraceLine(2315,0,__PYX_ERR(0, 2315, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_size_t_limit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2315, __pyx_L1_error)
+  __Pyx_TraceLine(2332,0,__PYX_ERR(0, 2332, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_size_t_limit); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2332, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2315, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2332, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_max_steps, __pyx_t_3, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2315, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_max_steps, __pyx_t_3, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2332, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2315, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2332, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_4)) {
 
-    /* "cpprb/PyReplayBuffer.pyx":2316
+    /* "cpprb/PyReplayBuffer.pyx":2333
  *     cdef size_t size_t_limit = -1
  *     if max_steps >= int(size_t_limit):
  *         raise ValueError(f"max_steps ({max_steps}) is too big. " +             # <<<<<<<<<<<<<<
  *                          f"max_steps < {size_t_limit}")
  * 
  */
-    __Pyx_TraceLine(2316,0,__PYX_ERR(0, 2316, __pyx_L1_error))
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2316, __pyx_L1_error)
+    __Pyx_TraceLine(2333,0,__PYX_ERR(0, 2333, __pyx_L1_error))
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = 0;
     __pyx_t_7 = 127;
     __Pyx_INCREF(__pyx_kp_u_max_steps_2);
     __pyx_t_6 += 11;
     __Pyx_GIVEREF(__pyx_kp_u_max_steps_2);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_max_steps_2);
-    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_v_max_steps, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2316, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_v_max_steps, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) : __pyx_t_7;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
     __pyx_t_3 = 0;
     __Pyx_INCREF(__pyx_kp_u_is_too_big);
     __pyx_t_6 += 14;
     __Pyx_GIVEREF(__pyx_kp_u_is_too_big);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_is_too_big);
-    __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2316, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":2317
+    /* "cpprb/PyReplayBuffer.pyx":2334
  *     if max_steps >= int(size_t_limit):
  *         raise ValueError(f"max_steps ({max_steps}) is too big. " +
  *                          f"max_steps < {size_t_limit}")             # <<<<<<<<<<<<<<
  * 
  *     cdef bool use_per = isinstance(buffer,PrioritizedReplayBuffer)
  */
-    __Pyx_TraceLine(2317,0,__PYX_ERR(0, 2317, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_PyUnicode_From_size_t(__pyx_v_size_t_limit, 0, ' ', 'd'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2317, __pyx_L1_error)
+    __Pyx_TraceLine(2334,0,__PYX_ERR(0, 2334, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_PyUnicode_From_size_t(__pyx_v_size_t_limit, 0, ' ', 'd'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_max_steps_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2317, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_max_steps_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":2316
+    /* "cpprb/PyReplayBuffer.pyx":2333
  *     cdef size_t size_t_limit = -1
  *     if max_steps >= int(size_t_limit):
  *         raise ValueError(f"max_steps ({max_steps}) is too big. " +             # <<<<<<<<<<<<<<
  *                          f"max_steps < {size_t_limit}")
  * 
  */
-    __Pyx_TraceLine(2316,0,__PYX_ERR(0, 2316, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2316, __pyx_L1_error)
+    __Pyx_TraceLine(2333,0,__PYX_ERR(0, 2333, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2316, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 2316, __pyx_L1_error)
+    __PYX_ERR(0, 2333, __pyx_L1_error)
 
-    /* "cpprb/PyReplayBuffer.pyx":2315
+    /* "cpprb/PyReplayBuffer.pyx":2332
  * 
  *     cdef size_t size_t_limit = -1
  *     if max_steps >= int(size_t_limit):             # <<<<<<<<<<<<<<
  *         raise ValueError(f"max_steps ({max_steps}) is too big. " +
  *                          f"max_steps < {size_t_limit}")
  */
   }
 
-  /* "cpprb/PyReplayBuffer.pyx":2319
+  /* "cpprb/PyReplayBuffer.pyx":2336
  *                          f"max_steps < {size_t_limit}")
  * 
  *     cdef bool use_per = isinstance(buffer,PrioritizedReplayBuffer)             # <<<<<<<<<<<<<<
  *     cdef bool has_after_step = after_step
  *     cdef bool has_check = done_check
  */
-  __Pyx_TraceLine(2319,0,__PYX_ERR(0, 2319, __pyx_L1_error))
+  __Pyx_TraceLine(2336,0,__PYX_ERR(0, 2336, __pyx_L1_error))
   __pyx_t_4 = __Pyx_TypeCheck(((PyObject *)__pyx_v_buffer), __pyx_ptype_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer); 
   __pyx_v_use_per = __pyx_t_4;
 
-  /* "cpprb/PyReplayBuffer.pyx":2320
+  /* "cpprb/PyReplayBuffer.pyx":2337
  * 
  *     cdef bool use_per = isinstance(buffer,PrioritizedReplayBuffer)
  *     cdef bool has_after_step = after_step             # <<<<<<<<<<<<<<
  *     cdef bool has_check = done_check
  *     cdef bool has_obs_update = obs_update
  */
-  __Pyx_TraceLine(2320,0,__PYX_ERR(0, 2320, __pyx_L1_error))
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_after_step); if (unlikely((__pyx_t_8 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 2320, __pyx_L1_error)
+  __Pyx_TraceLine(2337,0,__PYX_ERR(0, 2337, __pyx_L1_error))
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_after_step); if (unlikely((__pyx_t_8 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 2337, __pyx_L1_error)
   __pyx_v_has_after_step = __pyx_t_8;
 
-  /* "cpprb/PyReplayBuffer.pyx":2321
+  /* "cpprb/PyReplayBuffer.pyx":2338
  *     cdef bool use_per = isinstance(buffer,PrioritizedReplayBuffer)
  *     cdef bool has_after_step = after_step
  *     cdef bool has_check = done_check             # <<<<<<<<<<<<<<
  *     cdef bool has_obs_update = obs_update
  *     cdef bool has_rew_sum = rew_sum
  */
-  __Pyx_TraceLine(2321,0,__PYX_ERR(0, 2321, __pyx_L1_error))
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_done_check); if (unlikely((__pyx_t_8 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 2321, __pyx_L1_error)
+  __Pyx_TraceLine(2338,0,__PYX_ERR(0, 2338, __pyx_L1_error))
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_done_check); if (unlikely((__pyx_t_8 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 2338, __pyx_L1_error)
   __pyx_v_has_check = __pyx_t_8;
 
-  /* "cpprb/PyReplayBuffer.pyx":2322
+  /* "cpprb/PyReplayBuffer.pyx":2339
  *     cdef bool has_after_step = after_step
  *     cdef bool has_check = done_check
  *     cdef bool has_obs_update = obs_update             # <<<<<<<<<<<<<<
  *     cdef bool has_rew_sum = rew_sum
  *     cdef bool has_episode_callback = episode_callback
  */
-  __Pyx_TraceLine(2322,0,__PYX_ERR(0, 2322, __pyx_L1_error))
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_obs_update); if (unlikely((__pyx_t_8 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 2322, __pyx_L1_error)
+  __Pyx_TraceLine(2339,0,__PYX_ERR(0, 2339, __pyx_L1_error))
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_obs_update); if (unlikely((__pyx_t_8 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 2339, __pyx_L1_error)
   __pyx_v_has_obs_update = __pyx_t_8;
 
-  /* "cpprb/PyReplayBuffer.pyx":2323
+  /* "cpprb/PyReplayBuffer.pyx":2340
  *     cdef bool has_check = done_check
  *     cdef bool has_obs_update = obs_update
  *     cdef bool has_rew_sum = rew_sum             # <<<<<<<<<<<<<<
  *     cdef bool has_episode_callback = episode_callback
  * 
  */
-  __Pyx_TraceLine(2323,0,__PYX_ERR(0, 2323, __pyx_L1_error))
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_rew_sum); if (unlikely((__pyx_t_8 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 2323, __pyx_L1_error)
+  __Pyx_TraceLine(2340,0,__PYX_ERR(0, 2340, __pyx_L1_error))
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_rew_sum); if (unlikely((__pyx_t_8 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 2340, __pyx_L1_error)
   __pyx_v_has_rew_sum = __pyx_t_8;
 
-  /* "cpprb/PyReplayBuffer.pyx":2324
+  /* "cpprb/PyReplayBuffer.pyx":2341
  *     cdef bool has_obs_update = obs_update
  *     cdef bool has_rew_sum = rew_sum
  *     cdef bool has_episode_callback = episode_callback             # <<<<<<<<<<<<<<
  * 
  *     cdef size_t _max_steps = max(max_steps,0)
  */
-  __Pyx_TraceLine(2324,0,__PYX_ERR(0, 2324, __pyx_L1_error))
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_episode_callback); if (unlikely((__pyx_t_8 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 2324, __pyx_L1_error)
+  __Pyx_TraceLine(2341,0,__PYX_ERR(0, 2341, __pyx_L1_error))
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_episode_callback); if (unlikely((__pyx_t_8 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 2341, __pyx_L1_error)
   __pyx_v_has_episode_callback = __pyx_t_8;
 
-  /* "cpprb/PyReplayBuffer.pyx":2326
+  /* "cpprb/PyReplayBuffer.pyx":2343
  *     cdef bool has_episode_callback = episode_callback
  * 
  *     cdef size_t _max_steps = max(max_steps,0)             # <<<<<<<<<<<<<<
  *     cdef size_t _max_episodes = min(max(max_episodes or size_t_limit, 0),size_t_limit)
  *     cdef size_t _n_warmup = min(max(0,n_warmups),size_t_limit)
  */
-  __Pyx_TraceLine(2326,0,__PYX_ERR(0, 2326, __pyx_L1_error))
+  __Pyx_TraceLine(2343,0,__PYX_ERR(0, 2343, __pyx_L1_error))
   __pyx_t_9 = 0;
   __Pyx_INCREF(__pyx_v_max_steps);
   __pyx_t_2 = __pyx_v_max_steps;
-  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2326, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_GT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2326, __pyx_L1_error)
+  __pyx_t_5 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_GT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2343, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2326, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2343, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__pyx_t_4) {
-    __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2326, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2343, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_1 = __pyx_t_5;
     __pyx_t_5 = 0;
   } else {
     __Pyx_INCREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_10 = __Pyx_PyInt_As_size_t(__pyx_t_1); if (unlikely((__pyx_t_10 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 2326, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_size_t(__pyx_t_1); if (unlikely((__pyx_t_10 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 2343, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v__max_steps = __pyx_t_10;
 
-  /* "cpprb/PyReplayBuffer.pyx":2327
+  /* "cpprb/PyReplayBuffer.pyx":2344
  * 
  *     cdef size_t _max_steps = max(max_steps,0)
  *     cdef size_t _max_episodes = min(max(max_episodes or size_t_limit, 0),size_t_limit)             # <<<<<<<<<<<<<<
  *     cdef size_t _n_warmup = min(max(0,n_warmups),size_t_limit)
  * 
  */
-  __Pyx_TraceLine(2327,0,__PYX_ERR(0, 2327, __pyx_L1_error))
+  __Pyx_TraceLine(2344,0,__PYX_ERR(0, 2344, __pyx_L1_error))
   __pyx_t_10 = __pyx_v_size_t_limit;
   __pyx_t_9 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_max_episodes); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2327, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_max_episodes); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2344, __pyx_L1_error)
   if (!__pyx_t_4) {
   } else {
     __Pyx_INCREF(__pyx_v_max_episodes);
     __pyx_t_1 = __pyx_v_max_episodes;
     goto __pyx_L6_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_size_t_limit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2327, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_size_t_limit); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2344, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_L6_bool_binop_done:;
-  __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2327, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2344, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_5, __pyx_t_1, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2327, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_5, __pyx_t_1, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2344, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2327, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2344, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
-    __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2327, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2344, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_2 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
     __Pyx_INCREF(__pyx_t_1);
     __pyx_t_2 = __pyx_t_1;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_t_1 = __pyx_t_2;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2327, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2344, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyObject_RichCompare(__pyx_t_3, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2327, __pyx_L1_error)
+  __pyx_t_5 = PyObject_RichCompare(__pyx_t_3, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2344, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2327, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2344, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__pyx_t_4) {
-    __pyx_t_5 = __Pyx_PyInt_FromSize_t(__pyx_t_10); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2327, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_FromSize_t(__pyx_t_10); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2344, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_2 = __pyx_t_5;
     __pyx_t_5 = 0;
   } else {
     __Pyx_INCREF(__pyx_t_1);
     __pyx_t_2 = __pyx_t_1;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_10 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_10 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 2327, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_10 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 2344, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v__max_episodes = __pyx_t_10;
 
-  /* "cpprb/PyReplayBuffer.pyx":2328
+  /* "cpprb/PyReplayBuffer.pyx":2345
  *     cdef size_t _max_steps = max(max_steps,0)
  *     cdef size_t _max_episodes = min(max(max_episodes or size_t_limit, 0),size_t_limit)
  *     cdef size_t _n_warmup = min(max(0,n_warmups),size_t_limit)             # <<<<<<<<<<<<<<
  * 
  *     cdef size_t step = 0
  */
-  __Pyx_TraceLine(2328,0,__PYX_ERR(0, 2328, __pyx_L1_error))
+  __Pyx_TraceLine(2345,0,__PYX_ERR(0, 2345, __pyx_L1_error))
   __pyx_t_10 = __pyx_v_size_t_limit;
   __Pyx_INCREF(__pyx_v_n_warmups);
   __pyx_t_2 = __pyx_v_n_warmups;
   __pyx_t_9 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2328, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_5, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2328, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_5, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2345, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2328, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2345, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
     __Pyx_INCREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
   } else {
-    __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2328, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2345, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_t_2 = __pyx_t_1;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2328, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2328, __pyx_L1_error)
+  __pyx_t_5 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2345, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2328, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2345, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__pyx_t_4) {
-    __pyx_t_5 = __Pyx_PyInt_FromSize_t(__pyx_t_10); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2328, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_FromSize_t(__pyx_t_10); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2345, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_1 = __pyx_t_5;
     __pyx_t_5 = 0;
   } else {
     __Pyx_INCREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_10 = __Pyx_PyInt_As_size_t(__pyx_t_1); if (unlikely((__pyx_t_10 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 2328, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_size_t(__pyx_t_1); if (unlikely((__pyx_t_10 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 2345, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v__n_warmup = __pyx_t_10;
 
-  /* "cpprb/PyReplayBuffer.pyx":2330
+  /* "cpprb/PyReplayBuffer.pyx":2347
  *     cdef size_t _n_warmup = min(max(0,n_warmups),size_t_limit)
  * 
  *     cdef size_t step = 0             # <<<<<<<<<<<<<<
  *     cdef size_t episode = 0
  *     cdef size_t episode_step = 0
  */
-  __Pyx_TraceLine(2330,0,__PYX_ERR(0, 2330, __pyx_L1_error))
+  __Pyx_TraceLine(2347,0,__PYX_ERR(0, 2347, __pyx_L1_error))
   __pyx_v_step = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2331
+  /* "cpprb/PyReplayBuffer.pyx":2348
  * 
  *     cdef size_t step = 0
  *     cdef size_t episode = 0             # <<<<<<<<<<<<<<
  *     cdef size_t episode_step = 0
  *     cdef float episode_reward = 0.0
  */
-  __Pyx_TraceLine(2331,0,__PYX_ERR(0, 2331, __pyx_L1_error))
+  __Pyx_TraceLine(2348,0,__PYX_ERR(0, 2348, __pyx_L1_error))
   __pyx_v_episode = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2332
+  /* "cpprb/PyReplayBuffer.pyx":2349
  *     cdef size_t step = 0
  *     cdef size_t episode = 0
  *     cdef size_t episode_step = 0             # <<<<<<<<<<<<<<
  *     cdef float episode_reward = 0.0
  *     cdef bool is_warmup = True
  */
-  __Pyx_TraceLine(2332,0,__PYX_ERR(0, 2332, __pyx_L1_error))
+  __Pyx_TraceLine(2349,0,__PYX_ERR(0, 2349, __pyx_L1_error))
   __pyx_v_episode_step = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2333
+  /* "cpprb/PyReplayBuffer.pyx":2350
  *     cdef size_t episode = 0
  *     cdef size_t episode_step = 0
  *     cdef float episode_reward = 0.0             # <<<<<<<<<<<<<<
  *     cdef bool is_warmup = True
  * 
  */
-  __Pyx_TraceLine(2333,0,__PYX_ERR(0, 2333, __pyx_L1_error))
+  __Pyx_TraceLine(2350,0,__PYX_ERR(0, 2350, __pyx_L1_error))
   __pyx_v_episode_reward = 0.0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2334
+  /* "cpprb/PyReplayBuffer.pyx":2351
  *     cdef size_t episode_step = 0
  *     cdef float episode_reward = 0.0
  *     cdef bool is_warmup = True             # <<<<<<<<<<<<<<
  * 
  *     obs = env.reset()
  */
-  __Pyx_TraceLine(2334,0,__PYX_ERR(0, 2334, __pyx_L1_error))
+  __Pyx_TraceLine(2351,0,__PYX_ERR(0, 2351, __pyx_L1_error))
   __pyx_v_is_warmup = 1;
 
-  /* "cpprb/PyReplayBuffer.pyx":2336
+  /* "cpprb/PyReplayBuffer.pyx":2353
  *     cdef bool is_warmup = True
  * 
  *     obs = env.reset()             # <<<<<<<<<<<<<<
  *     cdef double episode_start_time = time.perf_counter()
  *     cdef double episode_end_time = 0.0
  */
-  __Pyx_TraceLine(2336,0,__PYX_ERR(0, 2336, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_env, __pyx_n_s_reset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2336, __pyx_L1_error)
+  __Pyx_TraceLine(2353,0,__PYX_ERR(0, 2353, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_env, __pyx_n_s_reset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2353, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2336, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2353, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_obs = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2337
+  /* "cpprb/PyReplayBuffer.pyx":2354
  * 
  *     obs = env.reset()
  *     cdef double episode_start_time = time.perf_counter()             # <<<<<<<<<<<<<<
  *     cdef double episode_end_time = 0.0
  *     for step in range(_max_steps):
  */
-  __Pyx_TraceLine(2337,0,__PYX_ERR(0, 2337, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2337, __pyx_L1_error)
+  __Pyx_TraceLine(2354,0,__PYX_ERR(0, 2354, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2354, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_perf_counter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2337, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_perf_counter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2354, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2337, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2354, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_11 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_11 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 2337, __pyx_L1_error)
+  __pyx_t_11 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_11 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 2354, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_episode_start_time = __pyx_t_11;
 
-  /* "cpprb/PyReplayBuffer.pyx":2338
+  /* "cpprb/PyReplayBuffer.pyx":2355
  *     obs = env.reset()
  *     cdef double episode_start_time = time.perf_counter()
  *     cdef double episode_end_time = 0.0             # <<<<<<<<<<<<<<
  *     for step in range(_max_steps):
  *         is_warmup = (step < _n_warmup)
  */
-  __Pyx_TraceLine(2338,0,__PYX_ERR(0, 2338, __pyx_L1_error))
+  __Pyx_TraceLine(2355,0,__PYX_ERR(0, 2355, __pyx_L1_error))
   __pyx_v_episode_end_time = 0.0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2339
+  /* "cpprb/PyReplayBuffer.pyx":2356
  *     cdef double episode_start_time = time.perf_counter()
  *     cdef double episode_end_time = 0.0
  *     for step in range(_max_steps):             # <<<<<<<<<<<<<<
  *         is_warmup = (step < _n_warmup)
  * 
  */
-  __Pyx_TraceLine(2339,0,__PYX_ERR(0, 2339, __pyx_L1_error))
+  __Pyx_TraceLine(2356,0,__PYX_ERR(0, 2356, __pyx_L1_error))
   __pyx_t_10 = __pyx_v__max_steps;
   __pyx_t_12 = __pyx_t_10;
   for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
     __pyx_v_step = __pyx_t_13;
 
-    /* "cpprb/PyReplayBuffer.pyx":2340
+    /* "cpprb/PyReplayBuffer.pyx":2357
  *     cdef double episode_end_time = 0.0
  *     for step in range(_max_steps):
  *         is_warmup = (step < _n_warmup)             # <<<<<<<<<<<<<<
  * 
  *         # Get action
  */
-    __Pyx_TraceLine(2340,0,__PYX_ERR(0, 2340, __pyx_L1_error))
+    __Pyx_TraceLine(2357,0,__PYX_ERR(0, 2357, __pyx_L1_error))
     __pyx_v_is_warmup = (__pyx_v_step < __pyx_v__n_warmup);
 
-    /* "cpprb/PyReplayBuffer.pyx":2343
+    /* "cpprb/PyReplayBuffer.pyx":2360
  * 
  *         # Get action
  *         action = get_action(obs,step,episode,is_warmup)             # <<<<<<<<<<<<<<
  * 
  *         # Step environment
  */
-    __Pyx_TraceLine(2343,0,__PYX_ERR(0, 2343, __pyx_L1_error))
-    __pyx_t_5 = __Pyx_PyInt_FromSize_t(__pyx_v_step); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2343, __pyx_L1_error)
+    __Pyx_TraceLine(2360,0,__PYX_ERR(0, 2360, __pyx_L1_error))
+    __pyx_t_5 = __Pyx_PyInt_FromSize_t(__pyx_v_step); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_episode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2343, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_episode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_v_is_warmup); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2343, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_v_is_warmup); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_get_action);
     __pyx_t_14 = __pyx_v_get_action; __pyx_t_15 = NULL;
     __pyx_t_16 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
       __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_14);
       if (likely(__pyx_t_15)) {
@@ -36763,35 +36969,35 @@
         __Pyx_DECREF_SET(__pyx_t_14, function);
         __pyx_t_16 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_14)) {
       PyObject *__pyx_temp[5] = {__pyx_t_15, __pyx_v_obs, __pyx_t_5, __pyx_t_2, __pyx_t_3};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_14, __pyx_temp+1-__pyx_t_16, 4+__pyx_t_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2343, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_14, __pyx_temp+1-__pyx_t_16, 4+__pyx_t_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2360, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_14)) {
       PyObject *__pyx_temp[5] = {__pyx_t_15, __pyx_v_obs, __pyx_t_5, __pyx_t_2, __pyx_t_3};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_14, __pyx_temp+1-__pyx_t_16, 4+__pyx_t_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2343, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_14, __pyx_temp+1-__pyx_t_16, 4+__pyx_t_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2360, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else
     #endif
     {
-      __pyx_t_17 = PyTuple_New(4+__pyx_t_16); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2343, __pyx_L1_error)
+      __pyx_t_17 = PyTuple_New(4+__pyx_t_16); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2360, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_17);
       if (__pyx_t_15) {
         __Pyx_GIVEREF(__pyx_t_15); PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_t_15); __pyx_t_15 = NULL;
       }
       __Pyx_INCREF(__pyx_v_obs);
       __Pyx_GIVEREF(__pyx_v_obs);
       PyTuple_SET_ITEM(__pyx_t_17, 0+__pyx_t_16, __pyx_v_obs);
@@ -36800,61 +37006,61 @@
       __Pyx_GIVEREF(__pyx_t_2);
       PyTuple_SET_ITEM(__pyx_t_17, 2+__pyx_t_16, __pyx_t_2);
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_17, 3+__pyx_t_16, __pyx_t_3);
       __pyx_t_5 = 0;
       __pyx_t_2 = 0;
       __pyx_t_3 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_14, __pyx_t_17, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2343, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_14, __pyx_t_17, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2360, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
     }
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
     __Pyx_XDECREF_SET(__pyx_v_action, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":2346
+    /* "cpprb/PyReplayBuffer.pyx":2363
  * 
  *         # Step environment
  *         if has_after_step:             # <<<<<<<<<<<<<<
  *             transition = after_step(obs,action,env.step(action),step,episode)
  *         else:
  */
-    __Pyx_TraceLine(2346,0,__PYX_ERR(0, 2346, __pyx_L1_error))
+    __Pyx_TraceLine(2363,0,__PYX_ERR(0, 2363, __pyx_L1_error))
     __pyx_t_4 = (__pyx_v_has_after_step != 0);
     if (__pyx_t_4) {
 
-      /* "cpprb/PyReplayBuffer.pyx":2347
+      /* "cpprb/PyReplayBuffer.pyx":2364
  *         # Step environment
  *         if has_after_step:
  *             transition = after_step(obs,action,env.step(action),step,episode)             # <<<<<<<<<<<<<<
  *         else:
  *             next_obs, reward, done, _ = env.step(action)
  */
-      __Pyx_TraceLine(2347,0,__PYX_ERR(0, 2347, __pyx_L1_error))
-      __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_v_env, __pyx_n_s_step); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2347, __pyx_L1_error)
+      __Pyx_TraceLine(2364,0,__PYX_ERR(0, 2364, __pyx_L1_error))
+      __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_v_env, __pyx_n_s_step); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2364, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_17);
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_17))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_17);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_17);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_17, function);
         }
       }
       __pyx_t_14 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_17, __pyx_t_3, __pyx_v_action) : __Pyx_PyObject_CallOneArg(__pyx_t_17, __pyx_v_action);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2347, __pyx_L1_error)
+      if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2364, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-      __pyx_t_17 = __Pyx_PyInt_FromSize_t(__pyx_v_step); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2347, __pyx_L1_error)
+      __pyx_t_17 = __Pyx_PyInt_FromSize_t(__pyx_v_step); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2364, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_17);
-      __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_episode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2347, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_episode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2364, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_INCREF(__pyx_v_after_step);
       __pyx_t_2 = __pyx_v_after_step; __pyx_t_5 = NULL;
       __pyx_t_16 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_5)) {
@@ -36864,35 +37070,35 @@
           __Pyx_DECREF_SET(__pyx_t_2, function);
           __pyx_t_16 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_2)) {
         PyObject *__pyx_temp[6] = {__pyx_t_5, __pyx_v_obs, __pyx_v_action, __pyx_t_14, __pyx_t_17, __pyx_t_3};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_16, 5+__pyx_t_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2347, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_16, 5+__pyx_t_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2364, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
         PyObject *__pyx_temp[6] = {__pyx_t_5, __pyx_v_obs, __pyx_v_action, __pyx_t_14, __pyx_t_17, __pyx_t_3};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_16, 5+__pyx_t_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2347, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_16, 5+__pyx_t_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2364, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       } else
       #endif
       {
-        __pyx_t_15 = PyTuple_New(5+__pyx_t_16); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2347, __pyx_L1_error)
+        __pyx_t_15 = PyTuple_New(5+__pyx_t_16); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2364, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         if (__pyx_t_5) {
           __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_5); __pyx_t_5 = NULL;
         }
         __Pyx_INCREF(__pyx_v_obs);
         __Pyx_GIVEREF(__pyx_v_obs);
         PyTuple_SET_ITEM(__pyx_t_15, 0+__pyx_t_16, __pyx_v_obs);
@@ -36904,65 +37110,65 @@
         __Pyx_GIVEREF(__pyx_t_17);
         PyTuple_SET_ITEM(__pyx_t_15, 3+__pyx_t_16, __pyx_t_17);
         __Pyx_GIVEREF(__pyx_t_3);
         PyTuple_SET_ITEM(__pyx_t_15, 4+__pyx_t_16, __pyx_t_3);
         __pyx_t_14 = 0;
         __pyx_t_17 = 0;
         __pyx_t_3 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_15, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2347, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_15, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2364, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
       }
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF_SET(__pyx_v_transition, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2346
+      /* "cpprb/PyReplayBuffer.pyx":2363
  * 
  *         # Step environment
  *         if has_after_step:             # <<<<<<<<<<<<<<
  *             transition = after_step(obs,action,env.step(action),step,episode)
  *         else:
  */
       goto __pyx_L10;
     }
 
-    /* "cpprb/PyReplayBuffer.pyx":2349
+    /* "cpprb/PyReplayBuffer.pyx":2366
  *             transition = after_step(obs,action,env.step(action),step,episode)
  *         else:
  *             next_obs, reward, done, _ = env.step(action)             # <<<<<<<<<<<<<<
  *             transition = {"obs": obs,
  *                           "act": action,
  */
-    __Pyx_TraceLine(2349,0,__PYX_ERR(0, 2349, __pyx_L1_error))
+    __Pyx_TraceLine(2366,0,__PYX_ERR(0, 2366, __pyx_L1_error))
     /*else*/ {
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_env, __pyx_n_s_step); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2349, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_env, __pyx_n_s_step); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2366, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_15 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_15)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_15);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_15, __pyx_v_action) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_action);
       __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2349, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2366, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
         PyObject* sequence = __pyx_t_1;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 4)) {
           if (size > 4) __Pyx_RaiseTooManyValuesError(4);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 2349, __pyx_L1_error)
+          __PYX_ERR(0, 2366, __pyx_L1_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_15 = PyTuple_GET_ITEM(sequence, 1); 
           __pyx_t_3 = PyTuple_GET_ITEM(sequence, 2); 
           __pyx_t_17 = PyTuple_GET_ITEM(sequence, 3); 
@@ -36977,194 +37183,194 @@
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_17);
         #else
         {
           Py_ssize_t i;
           PyObject** temps[4] = {&__pyx_t_2,&__pyx_t_15,&__pyx_t_3,&__pyx_t_17};
           for (i=0; i < 4; i++) {
-            PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 2349, __pyx_L1_error)
+            PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 2366, __pyx_L1_error)
             __Pyx_GOTREF(item);
             *(temps[i]) = item;
           }
         }
         #endif
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       } else {
         Py_ssize_t index = -1;
         PyObject** temps[4] = {&__pyx_t_2,&__pyx_t_15,&__pyx_t_3,&__pyx_t_17};
-        __pyx_t_14 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2349, __pyx_L1_error)
+        __pyx_t_14 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2366, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_14);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_t_18 = Py_TYPE(__pyx_t_14)->tp_iternext;
         for (index=0; index < 4; index++) {
           PyObject* item = __pyx_t_18(__pyx_t_14); if (unlikely(!item)) goto __pyx_L11_unpacking_failed;
           __Pyx_GOTREF(item);
           *(temps[index]) = item;
         }
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_18(__pyx_t_14), 4) < 0) __PYX_ERR(0, 2349, __pyx_L1_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_18(__pyx_t_14), 4) < 0) __PYX_ERR(0, 2366, __pyx_L1_error)
         __pyx_t_18 = NULL;
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         goto __pyx_L12_unpacking_done;
         __pyx_L11_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __pyx_t_18 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 2349, __pyx_L1_error)
+        __PYX_ERR(0, 2366, __pyx_L1_error)
         __pyx_L12_unpacking_done:;
       }
       __Pyx_XDECREF_SET(__pyx_v_next_obs, __pyx_t_2);
       __pyx_t_2 = 0;
       __Pyx_XDECREF_SET(__pyx_v_reward, __pyx_t_15);
       __pyx_t_15 = 0;
       __Pyx_XDECREF_SET(__pyx_v_done, __pyx_t_3);
       __pyx_t_3 = 0;
       __Pyx_XDECREF_SET(__pyx_v__, __pyx_t_17);
       __pyx_t_17 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2350
+      /* "cpprb/PyReplayBuffer.pyx":2367
  *         else:
  *             next_obs, reward, done, _ = env.step(action)
  *             transition = {"obs": obs,             # <<<<<<<<<<<<<<
  *                           "act": action,
  *                           "rew": reward,
  */
-      __Pyx_TraceLine(2350,0,__PYX_ERR(0, 2350, __pyx_L1_error))
-      __pyx_t_1 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2350, __pyx_L1_error)
+      __Pyx_TraceLine(2367,0,__PYX_ERR(0, 2367, __pyx_L1_error))
+      __pyx_t_1 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2367, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_obs, __pyx_v_obs) < 0) __PYX_ERR(0, 2350, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_obs, __pyx_v_obs) < 0) __PYX_ERR(0, 2367, __pyx_L1_error)
 
-      /* "cpprb/PyReplayBuffer.pyx":2351
+      /* "cpprb/PyReplayBuffer.pyx":2368
  *             next_obs, reward, done, _ = env.step(action)
  *             transition = {"obs": obs,
  *                           "act": action,             # <<<<<<<<<<<<<<
  *                           "rew": reward,
  *                           "next_obs": next_obs,
  */
-      __Pyx_TraceLine(2351,0,__PYX_ERR(0, 2351, __pyx_L1_error))
-      if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_act, __pyx_v_action) < 0) __PYX_ERR(0, 2350, __pyx_L1_error)
+      __Pyx_TraceLine(2368,0,__PYX_ERR(0, 2368, __pyx_L1_error))
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_act, __pyx_v_action) < 0) __PYX_ERR(0, 2367, __pyx_L1_error)
 
-      /* "cpprb/PyReplayBuffer.pyx":2352
+      /* "cpprb/PyReplayBuffer.pyx":2369
  *             transition = {"obs": obs,
  *                           "act": action,
  *                           "rew": reward,             # <<<<<<<<<<<<<<
  *                           "next_obs": next_obs,
  *                           "done": done}
  */
-      __Pyx_TraceLine(2352,0,__PYX_ERR(0, 2352, __pyx_L1_error))
-      if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_rew, __pyx_v_reward) < 0) __PYX_ERR(0, 2350, __pyx_L1_error)
+      __Pyx_TraceLine(2369,0,__PYX_ERR(0, 2369, __pyx_L1_error))
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_rew, __pyx_v_reward) < 0) __PYX_ERR(0, 2367, __pyx_L1_error)
 
-      /* "cpprb/PyReplayBuffer.pyx":2353
+      /* "cpprb/PyReplayBuffer.pyx":2370
  *                           "act": action,
  *                           "rew": reward,
  *                           "next_obs": next_obs,             # <<<<<<<<<<<<<<
  *                           "done": done}
  * 
  */
-      __Pyx_TraceLine(2353,0,__PYX_ERR(0, 2353, __pyx_L1_error))
-      if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_next_obs, __pyx_v_next_obs) < 0) __PYX_ERR(0, 2350, __pyx_L1_error)
+      __Pyx_TraceLine(2370,0,__PYX_ERR(0, 2370, __pyx_L1_error))
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_next_obs, __pyx_v_next_obs) < 0) __PYX_ERR(0, 2367, __pyx_L1_error)
 
-      /* "cpprb/PyReplayBuffer.pyx":2354
+      /* "cpprb/PyReplayBuffer.pyx":2371
  *                           "rew": reward,
  *                           "next_obs": next_obs,
  *                           "done": done}             # <<<<<<<<<<<<<<
  * 
  *         # Add to buffer
  */
-      __Pyx_TraceLine(2354,0,__PYX_ERR(0, 2354, __pyx_L1_error))
-      if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_done, __pyx_v_done) < 0) __PYX_ERR(0, 2350, __pyx_L1_error)
+      __Pyx_TraceLine(2371,0,__PYX_ERR(0, 2371, __pyx_L1_error))
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_done, __pyx_v_done) < 0) __PYX_ERR(0, 2367, __pyx_L1_error)
       __Pyx_XDECREF_SET(__pyx_v_transition, __pyx_t_1);
       __pyx_t_1 = 0;
     }
     __pyx_L10:;
 
-    /* "cpprb/PyReplayBuffer.pyx":2357
+    /* "cpprb/PyReplayBuffer.pyx":2374
  * 
  *         # Add to buffer
  *         buffer.add(**transition)             # <<<<<<<<<<<<<<
  * 
  *         # For Nstep, ReplayBuffer can be empty after `add(**transition)` method
  */
-    __Pyx_TraceLine(2357,0,__PYX_ERR(0, 2357, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_buffer), __pyx_n_s_add); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2357, __pyx_L1_error)
+    __Pyx_TraceLine(2374,0,__PYX_ERR(0, 2374, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_buffer), __pyx_n_s_add); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2374, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (unlikely(__pyx_v_transition == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-      __PYX_ERR(0, 2357, __pyx_L1_error)
+      __PYX_ERR(0, 2374, __pyx_L1_error)
     }
     if (likely(PyDict_CheckExact(__pyx_v_transition))) {
-      __pyx_t_17 = PyDict_Copy(__pyx_v_transition); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2357, __pyx_L1_error)
+      __pyx_t_17 = PyDict_Copy(__pyx_v_transition); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2374, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_17);
     } else {
-      __pyx_t_17 = PyObject_CallFunctionObjArgs((PyObject*)&PyDict_Type, __pyx_v_transition, NULL); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2357, __pyx_L1_error)
+      __pyx_t_17 = PyObject_CallFunctionObjArgs((PyObject*)&PyDict_Type, __pyx_v_transition, NULL); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2374, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_17);
     }
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_17); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2357, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_17); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2374, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "cpprb/PyReplayBuffer.pyx":2360
+    /* "cpprb/PyReplayBuffer.pyx":2377
  * 
  *         # For Nstep, ReplayBuffer can be empty after `add(**transition)` method
  *         if (buffer.get_stored_size() > 0) and (not is_warmup):             # <<<<<<<<<<<<<<
  *             # Sample
  *             sample = buffer.sample(batch_size)
  */
-    __Pyx_TraceLine(2360,0,__PYX_ERR(0, 2360, __pyx_L1_error))
+    __Pyx_TraceLine(2377,0,__PYX_ERR(0, 2377, __pyx_L1_error))
     __pyx_t_19 = ((((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_buffer->__pyx_vtab)->get_stored_size(__pyx_v_buffer, 0) > 0) != 0);
     if (__pyx_t_19) {
     } else {
       __pyx_t_4 = __pyx_t_19;
       goto __pyx_L14_bool_binop_done;
     }
     __pyx_t_19 = ((!(__pyx_v_is_warmup != 0)) != 0);
     __pyx_t_4 = __pyx_t_19;
     __pyx_L14_bool_binop_done:;
     if (__pyx_t_4) {
 
-      /* "cpprb/PyReplayBuffer.pyx":2362
+      /* "cpprb/PyReplayBuffer.pyx":2379
  *         if (buffer.get_stored_size() > 0) and (not is_warmup):
  *             # Sample
  *             sample = buffer.sample(batch_size)             # <<<<<<<<<<<<<<
  *             absTD = update_policy(sample,step,episode)
  * 
  */
-      __Pyx_TraceLine(2362,0,__PYX_ERR(0, 2362, __pyx_L1_error))
-      __pyx_t_17 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_buffer), __pyx_n_s_sample); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2362, __pyx_L1_error)
+      __Pyx_TraceLine(2379,0,__PYX_ERR(0, 2379, __pyx_L1_error))
+      __pyx_t_17 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_buffer), __pyx_n_s_sample); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2379, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_17);
       __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_17))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_17);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_17);
           __Pyx_INCREF(__pyx_t_1);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_17, function);
         }
       }
       __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_17, __pyx_t_1, __pyx_v_batch_size) : __Pyx_PyObject_CallOneArg(__pyx_t_17, __pyx_v_batch_size);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2362, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2379, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
       __Pyx_XDECREF_SET(__pyx_v_sample, __pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2363
+      /* "cpprb/PyReplayBuffer.pyx":2380
  *             # Sample
  *             sample = buffer.sample(batch_size)
  *             absTD = update_policy(sample,step,episode)             # <<<<<<<<<<<<<<
  * 
  *             if use_per:
  */
-      __Pyx_TraceLine(2363,0,__PYX_ERR(0, 2363, __pyx_L1_error))
-      __pyx_t_17 = __Pyx_PyInt_FromSize_t(__pyx_v_step); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2363, __pyx_L1_error)
+      __Pyx_TraceLine(2380,0,__PYX_ERR(0, 2380, __pyx_L1_error))
+      __pyx_t_17 = __Pyx_PyInt_FromSize_t(__pyx_v_step); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2380, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_17);
-      __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_episode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2363, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_episode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2380, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_v_update_policy);
       __pyx_t_15 = __pyx_v_update_policy; __pyx_t_2 = NULL;
       __pyx_t_16 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_15);
         if (likely(__pyx_t_2)) {
@@ -37174,76 +37380,76 @@
           __Pyx_DECREF_SET(__pyx_t_15, function);
           __pyx_t_16 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_15)) {
         PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_v_sample, __pyx_t_17, __pyx_t_1};
-        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_15, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2363, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_15, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2380, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_15)) {
         PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_v_sample, __pyx_t_17, __pyx_t_1};
-        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_15, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2363, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_15, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2380, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       } else
       #endif
       {
-        __pyx_t_14 = PyTuple_New(3+__pyx_t_16); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2363, __pyx_L1_error)
+        __pyx_t_14 = PyTuple_New(3+__pyx_t_16); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2380, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_14);
         if (__pyx_t_2) {
           __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_2); __pyx_t_2 = NULL;
         }
         __Pyx_INCREF(__pyx_v_sample);
         __Pyx_GIVEREF(__pyx_v_sample);
         PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_16, __pyx_v_sample);
         __Pyx_GIVEREF(__pyx_t_17);
         PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_16, __pyx_t_17);
         __Pyx_GIVEREF(__pyx_t_1);
         PyTuple_SET_ITEM(__pyx_t_14, 2+__pyx_t_16, __pyx_t_1);
         __pyx_t_17 = 0;
         __pyx_t_1 = 0;
-        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_15, __pyx_t_14, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2363, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_15, __pyx_t_14, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2380, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       }
       __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
       __Pyx_XDECREF_SET(__pyx_v_absTD, __pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2365
+      /* "cpprb/PyReplayBuffer.pyx":2382
  *             absTD = update_policy(sample,step,episode)
  * 
  *             if use_per:             # <<<<<<<<<<<<<<
  *                 buffer.update_priorities(sample["indexes"],absTD)
  * 
  */
-      __Pyx_TraceLine(2365,0,__PYX_ERR(0, 2365, __pyx_L1_error))
+      __Pyx_TraceLine(2382,0,__PYX_ERR(0, 2382, __pyx_L1_error))
       __pyx_t_4 = (__pyx_v_use_per != 0);
       if (__pyx_t_4) {
 
-        /* "cpprb/PyReplayBuffer.pyx":2366
+        /* "cpprb/PyReplayBuffer.pyx":2383
  * 
  *             if use_per:
  *                 buffer.update_priorities(sample["indexes"],absTD)             # <<<<<<<<<<<<<<
  * 
  *         # Summarize reward
  */
-        __Pyx_TraceLine(2366,0,__PYX_ERR(0, 2366, __pyx_L1_error))
-        __pyx_t_15 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_buffer), __pyx_n_s_update_priorities); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2366, __pyx_L1_error)
+        __Pyx_TraceLine(2383,0,__PYX_ERR(0, 2383, __pyx_L1_error))
+        __pyx_t_15 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_buffer), __pyx_n_s_update_priorities); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2383, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
-        __pyx_t_14 = __Pyx_PyObject_Dict_GetItem(__pyx_v_sample, __pyx_n_u_indexes); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2366, __pyx_L1_error)
+        __pyx_t_14 = __Pyx_PyObject_Dict_GetItem(__pyx_v_sample, __pyx_n_u_indexes); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2383, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_14);
         __pyx_t_1 = NULL;
         __pyx_t_16 = 0;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_15))) {
           __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_15);
           if (likely(__pyx_t_1)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
@@ -37252,76 +37458,76 @@
             __Pyx_DECREF_SET(__pyx_t_15, function);
             __pyx_t_16 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_15)) {
           PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_t_14, __pyx_v_absTD};
-          __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_15, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2366, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_15, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2383, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_15)) {
           PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_t_14, __pyx_v_absTD};
-          __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_15, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2366, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_15, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2383, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         } else
         #endif
         {
-          __pyx_t_17 = PyTuple_New(2+__pyx_t_16); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2366, __pyx_L1_error)
+          __pyx_t_17 = PyTuple_New(2+__pyx_t_16); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2383, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_17);
           if (__pyx_t_1) {
             __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_t_1); __pyx_t_1 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_14);
           PyTuple_SET_ITEM(__pyx_t_17, 0+__pyx_t_16, __pyx_t_14);
           __Pyx_INCREF(__pyx_v_absTD);
           __Pyx_GIVEREF(__pyx_v_absTD);
           PyTuple_SET_ITEM(__pyx_t_17, 1+__pyx_t_16, __pyx_v_absTD);
           __pyx_t_14 = 0;
-          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_15, __pyx_t_17, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2366, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_15, __pyx_t_17, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2383, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
         }
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "cpprb/PyReplayBuffer.pyx":2365
+        /* "cpprb/PyReplayBuffer.pyx":2382
  *             absTD = update_policy(sample,step,episode)
  * 
  *             if use_per:             # <<<<<<<<<<<<<<
  *                 buffer.update_priorities(sample["indexes"],absTD)
  * 
  */
       }
 
-      /* "cpprb/PyReplayBuffer.pyx":2360
+      /* "cpprb/PyReplayBuffer.pyx":2377
  * 
  *         # For Nstep, ReplayBuffer can be empty after `add(**transition)` method
  *         if (buffer.get_stored_size() > 0) and (not is_warmup):             # <<<<<<<<<<<<<<
  *             # Sample
  *             sample = buffer.sample(batch_size)
  */
     }
 
-    /* "cpprb/PyReplayBuffer.pyx":2369
+    /* "cpprb/PyReplayBuffer.pyx":2386
  * 
  *         # Summarize reward
  *         episode_reward = (rew_sum(episode_reward,transition) if has_rew_sum             # <<<<<<<<<<<<<<
  *                           else transition["rew"])
  * 
  */
-    __Pyx_TraceLine(2369,0,__PYX_ERR(0, 2369, __pyx_L1_error))
+    __Pyx_TraceLine(2386,0,__PYX_ERR(0, 2386, __pyx_L1_error))
     if ((__pyx_v_has_rew_sum != 0)) {
-      __pyx_t_15 = PyFloat_FromDouble(__pyx_v_episode_reward); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2369, __pyx_L1_error)
+      __pyx_t_15 = PyFloat_FromDouble(__pyx_v_episode_reward); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2386, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_v_rew_sum);
       __pyx_t_17 = __pyx_v_rew_sum; __pyx_t_14 = NULL;
       __pyx_t_16 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_17))) {
         __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_17);
         if (likely(__pyx_t_14)) {
@@ -37331,311 +37537,311 @@
           __Pyx_DECREF_SET(__pyx_t_17, function);
           __pyx_t_16 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_17)) {
         PyObject *__pyx_temp[3] = {__pyx_t_14, __pyx_t_15, __pyx_v_transition};
-        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_17, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2369, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_17, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2386, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_17)) {
         PyObject *__pyx_temp[3] = {__pyx_t_14, __pyx_t_15, __pyx_v_transition};
-        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_17, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2369, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_17, __pyx_temp+1-__pyx_t_16, 2+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2386, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
       } else
       #endif
       {
-        __pyx_t_1 = PyTuple_New(2+__pyx_t_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2369, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_New(2+__pyx_t_16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2386, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         if (__pyx_t_14) {
           __Pyx_GIVEREF(__pyx_t_14); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_14); __pyx_t_14 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_15);
         PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_16, __pyx_t_15);
         __Pyx_INCREF(__pyx_v_transition);
         __Pyx_GIVEREF(__pyx_v_transition);
         PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_16, __pyx_v_transition);
         __pyx_t_15 = 0;
-        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_17, __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2369, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_17, __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2386, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
       __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-      __pyx_t_21 = __pyx_PyFloat_AsFloat(__pyx_t_3); if (unlikely((__pyx_t_21 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 2369, __pyx_L1_error)
+      __pyx_t_21 = __pyx_PyFloat_AsFloat(__pyx_t_3); if (unlikely((__pyx_t_21 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 2386, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_20 = __pyx_t_21;
     } else {
 
-      /* "cpprb/PyReplayBuffer.pyx":2370
+      /* "cpprb/PyReplayBuffer.pyx":2387
  *         # Summarize reward
  *         episode_reward = (rew_sum(episode_reward,transition) if has_rew_sum
  *                           else transition["rew"])             # <<<<<<<<<<<<<<
  * 
  *         # Prepare the next step
  */
-      __Pyx_TraceLine(2370,0,__PYX_ERR(0, 2370, __pyx_L1_error))
-      __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_transition, __pyx_n_u_rew); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2370, __pyx_L1_error)
+      __Pyx_TraceLine(2387,0,__PYX_ERR(0, 2387, __pyx_L1_error))
+      __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_transition, __pyx_n_u_rew); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2387, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_21 = __pyx_PyFloat_AsFloat(__pyx_t_3); if (unlikely((__pyx_t_21 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 2370, __pyx_L1_error)
+      __pyx_t_21 = __pyx_PyFloat_AsFloat(__pyx_t_3); if (unlikely((__pyx_t_21 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 2387, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_20 = __pyx_t_21;
     }
     __pyx_v_episode_reward = __pyx_t_20;
 
-    /* "cpprb/PyReplayBuffer.pyx":2373
+    /* "cpprb/PyReplayBuffer.pyx":2390
  * 
  *         # Prepare the next step
  *         if done_check(transition) if has_check else transition["done"]:             # <<<<<<<<<<<<<<
  *             episode_end_time = time.perf_counter()
  * 
  */
-    __Pyx_TraceLine(2373,0,__PYX_ERR(0, 2373, __pyx_L1_error))
+    __Pyx_TraceLine(2390,0,__PYX_ERR(0, 2390, __pyx_L1_error))
     if ((__pyx_v_has_check != 0)) {
       __Pyx_INCREF(__pyx_v_done_check);
       __pyx_t_1 = __pyx_v_done_check; __pyx_t_15 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_15)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
           __Pyx_INCREF(__pyx_t_15);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
         }
       }
       __pyx_t_17 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_15, __pyx_v_transition) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_transition);
       __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-      if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2373, __pyx_L1_error)
+      if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2390, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_17);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_3 = __pyx_t_17;
       __pyx_t_17 = 0;
     } else {
-      __pyx_t_17 = __Pyx_PyObject_Dict_GetItem(__pyx_v_transition, __pyx_n_u_done); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2373, __pyx_L1_error)
+      __pyx_t_17 = __Pyx_PyObject_Dict_GetItem(__pyx_v_transition, __pyx_n_u_done); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2390, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_17);
       __pyx_t_3 = __pyx_t_17;
       __pyx_t_17 = 0;
     }
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2373, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 2390, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (__pyx_t_4) {
 
-      /* "cpprb/PyReplayBuffer.pyx":2374
+      /* "cpprb/PyReplayBuffer.pyx":2391
  *         # Prepare the next step
  *         if done_check(transition) if has_check else transition["done"]:
  *             episode_end_time = time.perf_counter()             # <<<<<<<<<<<<<<
  * 
  *             # step/episode_step are index.
  */
-      __Pyx_TraceLine(2374,0,__PYX_ERR(0, 2374, __pyx_L1_error))
-      __Pyx_GetModuleGlobalName(__pyx_t_17, __pyx_n_s_time); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2374, __pyx_L1_error)
+      __Pyx_TraceLine(2391,0,__PYX_ERR(0, 2391, __pyx_L1_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_17, __pyx_n_s_time); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2391, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_17);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_17, __pyx_n_s_perf_counter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2374, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_17, __pyx_n_s_perf_counter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2391, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
       __pyx_t_17 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_17)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
           __Pyx_INCREF(__pyx_t_17);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
         }
       }
       __pyx_t_3 = (__pyx_t_17) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_17) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
       __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2374, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2391, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_11 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_11 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 2374, __pyx_L1_error)
+      __pyx_t_11 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_11 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 2391, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_v_episode_end_time = __pyx_t_11;
 
-      /* "cpprb/PyReplayBuffer.pyx":2378
+      /* "cpprb/PyReplayBuffer.pyx":2395
  *             # step/episode_step are index.
  *             # Total Steps/Episode Steps are counts.
  *             SPS = (episode_step+1) / max(episode_end_time-episode_start_time,1e-9)             # <<<<<<<<<<<<<<
  *             logger.info(f"{episode: 6}th Episode: " +
  *                         f"{episode_step+1: 5} Steps " +
  */
-      __Pyx_TraceLine(2378,0,__PYX_ERR(0, 2378, __pyx_L1_error))
+      __Pyx_TraceLine(2395,0,__PYX_ERR(0, 2395, __pyx_L1_error))
       __pyx_t_22 = (__pyx_v_episode_step + 1);
       __pyx_t_11 = 1e-9;
       __pyx_t_23 = (__pyx_v_episode_end_time - __pyx_v_episode_start_time);
       if (((__pyx_t_11 > __pyx_t_23) != 0)) {
         __pyx_t_24 = __pyx_t_11;
       } else {
         __pyx_t_24 = __pyx_t_23;
       }
       __pyx_t_11 = __pyx_t_24;
       if (unlikely(__pyx_t_11 == 0)) {
         PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-        __PYX_ERR(0, 2378, __pyx_L1_error)
+        __PYX_ERR(0, 2395, __pyx_L1_error)
       }
       __pyx_v_SPS = (((double)__pyx_t_22) / __pyx_t_11);
 
-      /* "cpprb/PyReplayBuffer.pyx":2379
+      /* "cpprb/PyReplayBuffer.pyx":2396
  *             # Total Steps/Episode Steps are counts.
  *             SPS = (episode_step+1) / max(episode_end_time-episode_start_time,1e-9)
  *             logger.info(f"{episode: 6}th Episode: " +             # <<<<<<<<<<<<<<
  *                         f"{episode_step+1: 5} Steps " +
  *                         f"({step+1: 7} Total Steps), " +
  */
-      __Pyx_TraceLine(2379,0,__PYX_ERR(0, 2379, __pyx_L1_error))
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_logger, __pyx_n_s_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2379, __pyx_L1_error)
+      __Pyx_TraceLine(2396,0,__PYX_ERR(0, 2396, __pyx_L1_error))
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_logger, __pyx_n_s_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2396, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_17 = __Pyx_PyInt_FromSize_t(__pyx_v_episode); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2379, __pyx_L1_error)
+      __pyx_t_17 = __Pyx_PyInt_FromSize_t(__pyx_v_episode); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2396, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_17);
-      __pyx_t_15 = __Pyx_PyObject_Format(__pyx_t_17, __pyx_kp_u_6); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2379, __pyx_L1_error)
+      __pyx_t_15 = __Pyx_PyObject_Format(__pyx_t_17, __pyx_kp_u_6); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2396, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
       __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-      __pyx_t_17 = __Pyx_PyUnicode_Concat(__pyx_t_15, __pyx_kp_u_th_Episode); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2379, __pyx_L1_error)
+      __pyx_t_17 = __Pyx_PyUnicode_Concat(__pyx_t_15, __pyx_kp_u_th_Episode); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2396, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_17);
       __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2380
+      /* "cpprb/PyReplayBuffer.pyx":2397
  *             SPS = (episode_step+1) / max(episode_end_time-episode_start_time,1e-9)
  *             logger.info(f"{episode: 6}th Episode: " +
  *                         f"{episode_step+1: 5} Steps " +             # <<<<<<<<<<<<<<
  *                         f"({step+1: 7} Total Steps), " +
  *                         f"{episode_reward: =+7.2f} Reward, " +
  */
-      __Pyx_TraceLine(2380,0,__PYX_ERR(0, 2380, __pyx_L1_error))
-      __pyx_t_15 = __Pyx_PyInt_FromSize_t((__pyx_v_episode_step + 1)); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2380, __pyx_L1_error)
+      __Pyx_TraceLine(2397,0,__PYX_ERR(0, 2397, __pyx_L1_error))
+      __pyx_t_15 = __Pyx_PyInt_FromSize_t((__pyx_v_episode_step + 1)); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2397, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
-      __pyx_t_14 = __Pyx_PyObject_Format(__pyx_t_15, __pyx_kp_u_5); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2380, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyObject_Format(__pyx_t_15, __pyx_kp_u_5); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2397, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-      __pyx_t_15 = __Pyx_PyUnicode_Concat(__pyx_t_14, __pyx_kp_u_Steps); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2380, __pyx_L1_error)
+      __pyx_t_15 = __Pyx_PyUnicode_Concat(__pyx_t_14, __pyx_kp_u_Steps); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2397, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2379
+      /* "cpprb/PyReplayBuffer.pyx":2396
  *             # Total Steps/Episode Steps are counts.
  *             SPS = (episode_step+1) / max(episode_end_time-episode_start_time,1e-9)
  *             logger.info(f"{episode: 6}th Episode: " +             # <<<<<<<<<<<<<<
  *                         f"{episode_step+1: 5} Steps " +
  *                         f"({step+1: 7} Total Steps), " +
  */
-      __Pyx_TraceLine(2379,0,__PYX_ERR(0, 2379, __pyx_L1_error))
-      __pyx_t_14 = __Pyx_PyUnicode_Concat(__pyx_t_17, __pyx_t_15); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2379, __pyx_L1_error)
+      __Pyx_TraceLine(2396,0,__PYX_ERR(0, 2396, __pyx_L1_error))
+      __pyx_t_14 = __Pyx_PyUnicode_Concat(__pyx_t_17, __pyx_t_15); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2396, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
       __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2381
+      /* "cpprb/PyReplayBuffer.pyx":2398
  *             logger.info(f"{episode: 6}th Episode: " +
  *                         f"{episode_step+1: 5} Steps " +
  *                         f"({step+1: 7} Total Steps), " +             # <<<<<<<<<<<<<<
  *                         f"{episode_reward: =+7.2f} Reward, " +
  *                         f"{SPS: =+5.2f} Steps/s")
  */
-      __Pyx_TraceLine(2381,0,__PYX_ERR(0, 2381, __pyx_L1_error))
-      __pyx_t_15 = PyTuple_New(3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2381, __pyx_L1_error)
+      __Pyx_TraceLine(2398,0,__PYX_ERR(0, 2398, __pyx_L1_error))
+      __pyx_t_15 = PyTuple_New(3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2398, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
       __pyx_t_6 = 0;
       __pyx_t_7 = 127;
       __Pyx_INCREF(__pyx_kp_u__32);
       __pyx_t_6 += 1;
       __Pyx_GIVEREF(__pyx_kp_u__32);
       PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_kp_u__32);
-      __pyx_t_17 = __Pyx_PyInt_FromSize_t((__pyx_v_step + 1)); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2381, __pyx_L1_error)
+      __pyx_t_17 = __Pyx_PyInt_FromSize_t((__pyx_v_step + 1)); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 2398, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_17);
-      __pyx_t_2 = __Pyx_PyObject_Format(__pyx_t_17, __pyx_kp_u_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2381, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Format(__pyx_t_17, __pyx_kp_u_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2398, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
       __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_7;
       __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
       __Pyx_GIVEREF(__pyx_t_2);
       PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_t_2);
       __pyx_t_2 = 0;
       __Pyx_INCREF(__pyx_kp_u_Total_Steps);
       __pyx_t_6 += 15;
       __Pyx_GIVEREF(__pyx_kp_u_Total_Steps);
       PyTuple_SET_ITEM(__pyx_t_15, 2, __pyx_kp_u_Total_Steps);
-      __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_15, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2381, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_15, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2398, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2380
+      /* "cpprb/PyReplayBuffer.pyx":2397
  *             SPS = (episode_step+1) / max(episode_end_time-episode_start_time,1e-9)
  *             logger.info(f"{episode: 6}th Episode: " +
  *                         f"{episode_step+1: 5} Steps " +             # <<<<<<<<<<<<<<
  *                         f"({step+1: 7} Total Steps), " +
  *                         f"{episode_reward: =+7.2f} Reward, " +
  */
-      __Pyx_TraceLine(2380,0,__PYX_ERR(0, 2380, __pyx_L1_error))
-      __pyx_t_15 = __Pyx_PyUnicode_Concat(__pyx_t_14, __pyx_t_2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2380, __pyx_L1_error)
+      __Pyx_TraceLine(2397,0,__PYX_ERR(0, 2397, __pyx_L1_error))
+      __pyx_t_15 = __Pyx_PyUnicode_Concat(__pyx_t_14, __pyx_t_2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2397, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2382
+      /* "cpprb/PyReplayBuffer.pyx":2399
  *                         f"{episode_step+1: 5} Steps " +
  *                         f"({step+1: 7} Total Steps), " +
  *                         f"{episode_reward: =+7.2f} Reward, " +             # <<<<<<<<<<<<<<
  *                         f"{SPS: =+5.2f} Steps/s")
  * 
  */
-      __Pyx_TraceLine(2382,0,__PYX_ERR(0, 2382, __pyx_L1_error))
-      __pyx_t_2 = PyFloat_FromDouble(__pyx_v_episode_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2382, __pyx_L1_error)
+      __Pyx_TraceLine(2399,0,__PYX_ERR(0, 2399, __pyx_L1_error))
+      __pyx_t_2 = PyFloat_FromDouble(__pyx_v_episode_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2399, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_14 = __Pyx_PyObject_Format(__pyx_t_2, __pyx_kp_u_7_2f); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2382, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyObject_Format(__pyx_t_2, __pyx_kp_u_7_2f); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2399, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_14, __pyx_kp_u_Reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2382, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_14, __pyx_kp_u_Reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2399, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2381
+      /* "cpprb/PyReplayBuffer.pyx":2398
  *             logger.info(f"{episode: 6}th Episode: " +
  *                         f"{episode_step+1: 5} Steps " +
  *                         f"({step+1: 7} Total Steps), " +             # <<<<<<<<<<<<<<
  *                         f"{episode_reward: =+7.2f} Reward, " +
  *                         f"{SPS: =+5.2f} Steps/s")
  */
-      __Pyx_TraceLine(2381,0,__PYX_ERR(0, 2381, __pyx_L1_error))
-      __pyx_t_14 = __Pyx_PyUnicode_Concat(__pyx_t_15, __pyx_t_2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2381, __pyx_L1_error)
+      __Pyx_TraceLine(2398,0,__PYX_ERR(0, 2398, __pyx_L1_error))
+      __pyx_t_14 = __Pyx_PyUnicode_Concat(__pyx_t_15, __pyx_t_2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2398, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2383
+      /* "cpprb/PyReplayBuffer.pyx":2400
  *                         f"({step+1: 7} Total Steps), " +
  *                         f"{episode_reward: =+7.2f} Reward, " +
  *                         f"{SPS: =+5.2f} Steps/s")             # <<<<<<<<<<<<<<
  * 
  *             # Summary
  */
-      __Pyx_TraceLine(2383,0,__PYX_ERR(0, 2383, __pyx_L1_error))
-      __pyx_t_2 = PyFloat_FromDouble(__pyx_v_SPS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2383, __pyx_L1_error)
+      __Pyx_TraceLine(2400,0,__PYX_ERR(0, 2400, __pyx_L1_error))
+      __pyx_t_2 = PyFloat_FromDouble(__pyx_v_SPS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_15 = __Pyx_PyObject_Format(__pyx_t_2, __pyx_kp_u_5_2f); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2383, __pyx_L1_error)
+      __pyx_t_15 = __Pyx_PyObject_Format(__pyx_t_2, __pyx_kp_u_5_2f); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_15, __pyx_kp_u_Steps_s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2383, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_t_15, __pyx_kp_u_Steps_s); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2382
+      /* "cpprb/PyReplayBuffer.pyx":2399
  *                         f"{episode_step+1: 5} Steps " +
  *                         f"({step+1: 7} Total Steps), " +
  *                         f"{episode_reward: =+7.2f} Reward, " +             # <<<<<<<<<<<<<<
  *                         f"{SPS: =+5.2f} Steps/s")
  * 
  */
-      __Pyx_TraceLine(2382,0,__PYX_ERR(0, 2382, __pyx_L1_error))
-      __pyx_t_15 = __Pyx_PyUnicode_Concat(__pyx_t_14, __pyx_t_2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2382, __pyx_L1_error)
+      __Pyx_TraceLine(2399,0,__PYX_ERR(0, 2399, __pyx_L1_error))
+      __pyx_t_15 = __Pyx_PyUnicode_Concat(__pyx_t_14, __pyx_t_2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2399, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_2 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_2)) {
@@ -37644,43 +37850,43 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
         }
       }
       __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_t_15) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_15);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2379, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2396, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2386
+      /* "cpprb/PyReplayBuffer.pyx":2403
  * 
  *             # Summary
  *             if has_episode_callback:             # <<<<<<<<<<<<<<
  *                 episode_callback(episode,episode_step,episode_reward)
  * 
  */
-      __Pyx_TraceLine(2386,0,__PYX_ERR(0, 2386, __pyx_L1_error))
+      __Pyx_TraceLine(2403,0,__PYX_ERR(0, 2403, __pyx_L1_error))
       __pyx_t_4 = (__pyx_v_has_episode_callback != 0);
       if (__pyx_t_4) {
 
-        /* "cpprb/PyReplayBuffer.pyx":2387
+        /* "cpprb/PyReplayBuffer.pyx":2404
  *             # Summary
  *             if has_episode_callback:
  *                 episode_callback(episode,episode_step,episode_reward)             # <<<<<<<<<<<<<<
  * 
  *             # Reset
  */
-        __Pyx_TraceLine(2387,0,__PYX_ERR(0, 2387, __pyx_L1_error))
-        __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_episode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2387, __pyx_L1_error)
+        __Pyx_TraceLine(2404,0,__PYX_ERR(0, 2404, __pyx_L1_error))
+        __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_episode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2404, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_15 = __Pyx_PyInt_FromSize_t(__pyx_v_episode_step); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2387, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyInt_FromSize_t(__pyx_v_episode_step); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 2404, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
-        __pyx_t_2 = PyFloat_FromDouble(__pyx_v_episode_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2387, __pyx_L1_error)
+        __pyx_t_2 = PyFloat_FromDouble(__pyx_v_episode_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2404, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_INCREF(__pyx_v_episode_callback);
         __pyx_t_14 = __pyx_v_episode_callback; __pyx_t_17 = NULL;
         __pyx_t_16 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
           __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_14);
           if (likely(__pyx_t_17)) {
@@ -37690,211 +37896,211 @@
             __Pyx_DECREF_SET(__pyx_t_14, function);
             __pyx_t_16 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_14)) {
           PyObject *__pyx_temp[4] = {__pyx_t_17, __pyx_t_1, __pyx_t_15, __pyx_t_2};
-          __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_14, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2387, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_14, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2404, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_14)) {
           PyObject *__pyx_temp[4] = {__pyx_t_17, __pyx_t_1, __pyx_t_15, __pyx_t_2};
-          __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_14, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2387, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_14, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2404, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         } else
         #endif
         {
-          __pyx_t_5 = PyTuple_New(3+__pyx_t_16); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2387, __pyx_L1_error)
+          __pyx_t_5 = PyTuple_New(3+__pyx_t_16); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2404, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           if (__pyx_t_17) {
             __Pyx_GIVEREF(__pyx_t_17); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_17); __pyx_t_17 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_1);
           PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_16, __pyx_t_1);
           __Pyx_GIVEREF(__pyx_t_15);
           PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_16, __pyx_t_15);
           __Pyx_GIVEREF(__pyx_t_2);
           PyTuple_SET_ITEM(__pyx_t_5, 2+__pyx_t_16, __pyx_t_2);
           __pyx_t_1 = 0;
           __pyx_t_15 = 0;
           __pyx_t_2 = 0;
-          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_14, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2387, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_14, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2404, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         }
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "cpprb/PyReplayBuffer.pyx":2386
+        /* "cpprb/PyReplayBuffer.pyx":2403
  * 
  *             # Summary
  *             if has_episode_callback:             # <<<<<<<<<<<<<<
  *                 episode_callback(episode,episode_step,episode_reward)
  * 
  */
       }
 
-      /* "cpprb/PyReplayBuffer.pyx":2390
+      /* "cpprb/PyReplayBuffer.pyx":2407
  * 
  *             # Reset
  *             obs = env.reset()             # <<<<<<<<<<<<<<
  *             buffer.on_episode_end()
  *             episode_reward = 0.0
  */
-      __Pyx_TraceLine(2390,0,__PYX_ERR(0, 2390, __pyx_L1_error))
-      __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_v_env, __pyx_n_s_reset); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2390, __pyx_L1_error)
+      __Pyx_TraceLine(2407,0,__PYX_ERR(0, 2407, __pyx_L1_error))
+      __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_v_env, __pyx_n_s_reset); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2407, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_14))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_14);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_14, function);
         }
       }
       __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_14);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2390, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2407, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_DECREF_SET(__pyx_v_obs, __pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2391
+      /* "cpprb/PyReplayBuffer.pyx":2408
  *             # Reset
  *             obs = env.reset()
  *             buffer.on_episode_end()             # <<<<<<<<<<<<<<
  *             episode_reward = 0.0
  *             episode_step = 0
  */
-      __Pyx_TraceLine(2391,0,__PYX_ERR(0, 2391, __pyx_L1_error))
-      ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_buffer->__pyx_vtab)->on_episode_end(__pyx_v_buffer, 0); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2391, __pyx_L1_error)
+      __Pyx_TraceLine(2408,0,__PYX_ERR(0, 2408, __pyx_L1_error))
+      ((struct __pyx_vtabstruct_5cpprb_14PyReplayBuffer_ReplayBuffer *)__pyx_v_buffer->__pyx_vtab)->on_episode_end(__pyx_v_buffer, 0); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 2408, __pyx_L1_error)
 
-      /* "cpprb/PyReplayBuffer.pyx":2392
+      /* "cpprb/PyReplayBuffer.pyx":2409
  *             obs = env.reset()
  *             buffer.on_episode_end()
  *             episode_reward = 0.0             # <<<<<<<<<<<<<<
  *             episode_step = 0
  * 
  */
-      __Pyx_TraceLine(2392,0,__PYX_ERR(0, 2392, __pyx_L1_error))
+      __Pyx_TraceLine(2409,0,__PYX_ERR(0, 2409, __pyx_L1_error))
       __pyx_v_episode_reward = 0.0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2393
+      /* "cpprb/PyReplayBuffer.pyx":2410
  *             buffer.on_episode_end()
  *             episode_reward = 0.0
  *             episode_step = 0             # <<<<<<<<<<<<<<
  * 
  *             # Update episode count
  */
-      __Pyx_TraceLine(2393,0,__PYX_ERR(0, 2393, __pyx_L1_error))
+      __Pyx_TraceLine(2410,0,__PYX_ERR(0, 2410, __pyx_L1_error))
       __pyx_v_episode_step = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2396
+      /* "cpprb/PyReplayBuffer.pyx":2413
  * 
  *             # Update episode count
  *             episode += 1             # <<<<<<<<<<<<<<
  *             if episode >= _max_episodes:
  *                 break
  */
-      __Pyx_TraceLine(2396,0,__PYX_ERR(0, 2396, __pyx_L1_error))
+      __Pyx_TraceLine(2413,0,__PYX_ERR(0, 2413, __pyx_L1_error))
       __pyx_v_episode = (__pyx_v_episode + 1);
 
-      /* "cpprb/PyReplayBuffer.pyx":2397
+      /* "cpprb/PyReplayBuffer.pyx":2414
  *             # Update episode count
  *             episode += 1
  *             if episode >= _max_episodes:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
-      __Pyx_TraceLine(2397,0,__PYX_ERR(0, 2397, __pyx_L1_error))
+      __Pyx_TraceLine(2414,0,__PYX_ERR(0, 2414, __pyx_L1_error))
       __pyx_t_4 = ((__pyx_v_episode >= __pyx_v__max_episodes) != 0);
       if (__pyx_t_4) {
 
-        /* "cpprb/PyReplayBuffer.pyx":2398
+        /* "cpprb/PyReplayBuffer.pyx":2415
  *             episode += 1
  *             if episode >= _max_episodes:
  *                 break             # <<<<<<<<<<<<<<
  * 
  *             episode_start_time = time.perf_counter()
  */
-        __Pyx_TraceLine(2398,0,__PYX_ERR(0, 2398, __pyx_L1_error))
+        __Pyx_TraceLine(2415,0,__PYX_ERR(0, 2415, __pyx_L1_error))
         goto __pyx_L9_break;
 
-        /* "cpprb/PyReplayBuffer.pyx":2397
+        /* "cpprb/PyReplayBuffer.pyx":2414
  *             # Update episode count
  *             episode += 1
  *             if episode >= _max_episodes:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
       }
 
-      /* "cpprb/PyReplayBuffer.pyx":2400
+      /* "cpprb/PyReplayBuffer.pyx":2417
  *                 break
  * 
  *             episode_start_time = time.perf_counter()             # <<<<<<<<<<<<<<
  *         else:
  *             obs = obs_update(transition) if has_obs_update else transition["next_obs"]
  */
-      __Pyx_TraceLine(2400,0,__PYX_ERR(0, 2400, __pyx_L1_error))
-      __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_time); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2400, __pyx_L1_error)
+      __Pyx_TraceLine(2417,0,__PYX_ERR(0, 2417, __pyx_L1_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_time); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 2417, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_perf_counter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2400, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_perf_counter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2417, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __pyx_t_14 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_14)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_14);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_3 = (__pyx_t_14) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_14) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2400, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2417, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_11 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_11 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 2400, __pyx_L1_error)
+      __pyx_t_11 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_11 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 2417, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_v_episode_start_time = __pyx_t_11;
 
-      /* "cpprb/PyReplayBuffer.pyx":2373
+      /* "cpprb/PyReplayBuffer.pyx":2390
  * 
  *         # Prepare the next step
  *         if done_check(transition) if has_check else transition["done"]:             # <<<<<<<<<<<<<<
  *             episode_end_time = time.perf_counter()
  * 
  */
       goto __pyx_L17;
     }
 
-    /* "cpprb/PyReplayBuffer.pyx":2402
+    /* "cpprb/PyReplayBuffer.pyx":2419
  *             episode_start_time = time.perf_counter()
  *         else:
  *             obs = obs_update(transition) if has_obs_update else transition["next_obs"]             # <<<<<<<<<<<<<<
  *             episode_step += 1
  */
-    __Pyx_TraceLine(2402,0,__PYX_ERR(0, 2402, __pyx_L1_error))
+    __Pyx_TraceLine(2419,0,__PYX_ERR(0, 2419, __pyx_L1_error))
     /*else*/ {
       if ((__pyx_v_has_obs_update != 0)) {
         __Pyx_INCREF(__pyx_v_obs_update);
         __pyx_t_14 = __pyx_v_obs_update; __pyx_t_2 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_14))) {
           __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_14);
           if (likely(__pyx_t_2)) {
@@ -37902,41 +38108,41 @@
             __Pyx_INCREF(__pyx_t_2);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_14, function);
           }
         }
         __pyx_t_5 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_2, __pyx_v_transition) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_v_transition);
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2402, __pyx_L1_error)
+        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2419, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __pyx_t_3 = __pyx_t_5;
         __pyx_t_5 = 0;
       } else {
-        __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_transition, __pyx_n_u_next_obs); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2402, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_transition, __pyx_n_u_next_obs); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 2419, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __pyx_t_3 = __pyx_t_5;
         __pyx_t_5 = 0;
       }
       __Pyx_DECREF_SET(__pyx_v_obs, __pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "cpprb/PyReplayBuffer.pyx":2403
+      /* "cpprb/PyReplayBuffer.pyx":2420
  *         else:
  *             obs = obs_update(transition) if has_obs_update else transition["next_obs"]
  *             episode_step += 1             # <<<<<<<<<<<<<<
  */
-      __Pyx_TraceLine(2403,0,__PYX_ERR(0, 2403, __pyx_L1_error))
+      __Pyx_TraceLine(2420,0,__PYX_ERR(0, 2420, __pyx_L1_error))
       __pyx_v_episode_step = (__pyx_v_episode_step + 1);
     }
     __pyx_L17:;
   }
   __pyx_L9_break:;
 
-  /* "cpprb/PyReplayBuffer.pyx":2252
+  /* "cpprb/PyReplayBuffer.pyx":2269
  * 
  * @cython.embedsignature(True)
  * def train(buffer: ReplayBuffer,             # <<<<<<<<<<<<<<
  *           env,
  *           get_action: Callable,
  */
 
@@ -59441,15 +59647,15 @@
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
   {&__pyx_n_s_Lock, __pyx_k_Lock, sizeof(__pyx_k_Lock), 0, 0, 1, 1},
   {&__pyx_n_s_MPPrioritizedReplayBuffer, __pyx_k_MPPrioritizedReplayBuffer, sizeof(__pyx_k_MPPrioritizedReplayBuffer), 0, 0, 1, 1},
   {&__pyx_n_s_MPReplayBuffer, __pyx_k_MPReplayBuffer, sizeof(__pyx_k_MPReplayBuffer), 0, 0, 1, 1},
-  {&__pyx_kp_u_MPReplayBuffer_clear_line_1783, __pyx_k_MPReplayBuffer_clear_line_1783, sizeof(__pyx_k_MPReplayBuffer_clear_line_1783), 0, 1, 0, 0},
+  {&__pyx_kp_u_MPReplayBuffer_clear_line_1800, __pyx_k_MPReplayBuffer_clear_line_1800, sizeof(__pyx_k_MPReplayBuffer_clear_line_1800), 0, 1, 0, 0},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
   {&__pyx_n_s_Nepisodes, __pyx_k_Nepisodes, sizeof(__pyx_k_Nepisodes), 0, 0, 1, 1},
   {&__pyx_kp_u_Non_native_byte_order_not_suppor, __pyx_k_Non_native_byte_order_not_suppor, sizeof(__pyx_k_Non_native_byte_order_not_suppor), 0, 1, 0, 0},
   {&__pyx_kp_u_None, __pyx_k_None, sizeof(__pyx_k_None), 0, 1, 0, 0},
   {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
@@ -59465,15 +59671,15 @@
   {&__pyx_n_u_PrioritizedReplayBuffer, __pyx_k_PrioritizedReplayBuffer, sizeof(__pyx_k_PrioritizedReplayBuffer), 0, 1, 0, 1},
   {&__pyx_n_s_Process, __pyx_k_Process, sizeof(__pyx_k_Process), 0, 0, 1, 1},
   {&__pyx_n_s_ProcessSafeRingBufferIndex, __pyx_k_ProcessSafeRingBufferIndex, sizeof(__pyx_k_ProcessSafeRingBufferIndex), 0, 0, 1, 1},
   {&__pyx_n_s_RawArray, __pyx_k_RawArray, sizeof(__pyx_k_RawArray), 0, 0, 1, 1},
   {&__pyx_n_s_RawValue, __pyx_k_RawValue, sizeof(__pyx_k_RawValue), 0, 0, 1, 1},
   {&__pyx_n_s_ReplayBuffer, __pyx_k_ReplayBuffer, sizeof(__pyx_k_ReplayBuffer), 0, 0, 1, 1},
   {&__pyx_n_u_ReplayBuffer, __pyx_k_ReplayBuffer, sizeof(__pyx_k_ReplayBuffer), 0, 1, 0, 1},
-  {&__pyx_kp_u_ReplayBuffer_clear_line_1169, __pyx_k_ReplayBuffer_clear_line_1169, sizeof(__pyx_k_ReplayBuffer_clear_line_1169), 0, 1, 0, 0},
+  {&__pyx_kp_u_ReplayBuffer_clear_line_1177, __pyx_k_ReplayBuffer_clear_line_1177, sizeof(__pyx_k_ReplayBuffer_clear_line_1177), 0, 1, 0, 0},
   {&__pyx_kp_u_Reward, __pyx_k_Reward, sizeof(__pyx_k_Reward), 0, 1, 0, 0},
   {&__pyx_n_s_RingBufferIndex, __pyx_k_RingBufferIndex, sizeof(__pyx_k_RingBufferIndex), 0, 0, 1, 1},
   {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
   {&__pyx_n_s_SPS, __pyx_k_SPS, sizeof(__pyx_k_SPS), 0, 0, 1, 1},
   {&__pyx_n_s_SelectiveEnvironment, __pyx_k_SelectiveEnvironment, sizeof(__pyx_k_SelectiveEnvironment), 0, 0, 1, 1},
   {&__pyx_n_s_SelectiveReplayBuffer, __pyx_k_SelectiveReplayBuffer, sizeof(__pyx_k_SelectiveReplayBuffer), 0, 0, 1, 1},
   {&__pyx_n_s_SharedBuffer, __pyx_k_SharedBuffer, sizeof(__pyx_k_SharedBuffer), 0, 0, 1, 1},
@@ -59786,15 +59992,15 @@
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 120, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 371, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 695, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 1423, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 1440, __pyx_L1_error)
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(2, 777, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 959, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 148, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 151, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 404, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 613, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 832, __pyx_L1_error)
@@ -59976,33 +60182,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
 
-  /* "cpprb/PyReplayBuffer.pyx":1423
+  /* "cpprb/PyReplayBuffer.pyx":1440
  *                                            ndmin=1,dtype=np.single))
  *             if N != priorities.shape[0]:
  *                 raise ValueError("`priorities` shape is imcompatible")             # <<<<<<<<<<<<<<
  * 
  *         if self.use_nstep:
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_u_priorities_shape_is_imcompatibl); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 1423, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_u_priorities_shape_is_imcompatibl); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 1440, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
 
-  /* "cpprb/PyReplayBuffer.pyx":1518
+  /* "cpprb/PyReplayBuffer.pyx":1535
  * 
  *         if priorities is None:
  *             raise TypeError("`properties` must not be `None`")             # <<<<<<<<<<<<<<
  * 
  *         cdef const size_t [:] idx = Csize(indexes)
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_u_properties_must_not_be_None); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 1518, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_u_properties_must_not_be_None); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 1535, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -60289,37 +60495,37 @@
  * 
  */
   __pyx_tuple__63 = PyTuple_Pack(2, __pyx_n_s_dict, __pyx_n_s_key); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(0, 530, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__63);
   __Pyx_GIVEREF(__pyx_tuple__63);
   __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__63, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cpprb_PyReplayBuffer_pyx, __pyx_n_s_find_array, 530, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 530, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2209
+  /* "cpprb/PyReplayBuffer.pyx":2226
  * 
  * @cython.embedsignature(True)
  * def create_buffer(size,env_dict=None,*,prioritized = False,**kwargs):             # <<<<<<<<<<<<<<
  *     r"""Create specified version of replay buffer
  * 
  */
-  __pyx_tuple__64 = PyTuple_Pack(8, __pyx_n_s_size, __pyx_n_s_env_dict, __pyx_n_s_prioritized, __pyx_n_s_kwargs, __pyx_n_s_per, __pyx_n_s_buffer_name, __pyx_n_s_cls, __pyx_n_s_buffer); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 2209, __pyx_L1_error)
+  __pyx_tuple__64 = PyTuple_Pack(8, __pyx_n_s_size, __pyx_n_s_env_dict, __pyx_n_s_prioritized, __pyx_n_s_kwargs, __pyx_n_s_per, __pyx_n_s_buffer_name, __pyx_n_s_cls, __pyx_n_s_buffer); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 2226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__64);
   __Pyx_GIVEREF(__pyx_tuple__64);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(2, 1, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__64, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cpprb_PyReplayBuffer_pyx, __pyx_n_s_create_buffer, 2209, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 2209, __pyx_L1_error)
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(2, 1, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__64, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cpprb_PyReplayBuffer_pyx, __pyx_n_s_create_buffer, 2226, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 2226, __pyx_L1_error)
 
-  /* "cpprb/PyReplayBuffer.pyx":2252
+  /* "cpprb/PyReplayBuffer.pyx":2269
  * 
  * @cython.embedsignature(True)
  * def train(buffer: ReplayBuffer,             # <<<<<<<<<<<<<<
  *           env,
  *           get_action: Callable,
  */
-  __pyx_tuple__65 = PyTuple_Pack(41, __pyx_n_s_buffer, __pyx_n_s_env, __pyx_n_s_get_action, __pyx_n_s_update_policy, __pyx_n_s_max_steps, __pyx_n_s_max_episodes, __pyx_n_s_batch_size, __pyx_n_s_n_warmups, __pyx_n_s_after_step, __pyx_n_s_done_check, __pyx_n_s_obs_update, __pyx_n_s_rew_sum, __pyx_n_s_episode_callback, __pyx_n_s_logger, __pyx_n_s_size_t_limit, __pyx_n_s_use_per, __pyx_n_s_has_after_step, __pyx_n_s_has_check, __pyx_n_s_has_obs_update, __pyx_n_s_has_rew_sum, __pyx_n_s_has_episode_callback, __pyx_n_s_max_steps_4, __pyx_n_s_max_episodes_2, __pyx_n_s_n_warmup, __pyx_n_s_step, __pyx_n_s_episode, __pyx_n_s_episode_step, __pyx_n_s_episode_reward, __pyx_n_s_is_warmup, __pyx_n_s_obs, __pyx_n_s_episode_start_time, __pyx_n_s_episode_end_time, __pyx_n_s_action, __pyx_n_s_transition, __pyx_n_s_next_obs, __pyx_n_s_reward, __pyx_n_s_done, __pyx_n_s__11, __pyx_n_s_sample, __pyx_n_s_absTD, __pyx_n_s_SPS); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(0, 2252, __pyx_L1_error)
+  __pyx_tuple__65 = PyTuple_Pack(41, __pyx_n_s_buffer, __pyx_n_s_env, __pyx_n_s_get_action, __pyx_n_s_update_policy, __pyx_n_s_max_steps, __pyx_n_s_max_episodes, __pyx_n_s_batch_size, __pyx_n_s_n_warmups, __pyx_n_s_after_step, __pyx_n_s_done_check, __pyx_n_s_obs_update, __pyx_n_s_rew_sum, __pyx_n_s_episode_callback, __pyx_n_s_logger, __pyx_n_s_size_t_limit, __pyx_n_s_use_per, __pyx_n_s_has_after_step, __pyx_n_s_has_check, __pyx_n_s_has_obs_update, __pyx_n_s_has_rew_sum, __pyx_n_s_has_episode_callback, __pyx_n_s_max_steps_4, __pyx_n_s_max_episodes_2, __pyx_n_s_n_warmup, __pyx_n_s_step, __pyx_n_s_episode, __pyx_n_s_episode_step, __pyx_n_s_episode_reward, __pyx_n_s_is_warmup, __pyx_n_s_obs, __pyx_n_s_episode_start_time, __pyx_n_s_episode_end_time, __pyx_n_s_action, __pyx_n_s_transition, __pyx_n_s_next_obs, __pyx_n_s_reward, __pyx_n_s_done, __pyx_n_s__11, __pyx_n_s_sample, __pyx_n_s_absTD, __pyx_n_s_SPS); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(0, 2269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__65);
   __Pyx_GIVEREF(__pyx_tuple__65);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(4, 10, 41, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__65, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cpprb_PyReplayBuffer_pyx, __pyx_n_s_train, 2252, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 2252, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(4, 10, 41, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__65, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cpprb_PyReplayBuffer_pyx, __pyx_n_s_train, 2269, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 2269, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_StepChecker(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
   __pyx_tuple__66 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__66)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -60661,14 +60867,15 @@
   __pyx_ptype_5cpprb_14PyReplayBuffer_ProcessSafeRingBufferIndex = &__pyx_type_5cpprb_14PyReplayBuffer_ProcessSafeRingBufferIndex;
   __pyx_vtabptr_5cpprb_14PyReplayBuffer_ReplayBuffer = &__pyx_vtable_5cpprb_14PyReplayBuffer_ReplayBuffer;
   __pyx_vtable_5cpprb_14PyReplayBuffer_ReplayBuffer.clear = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_clear;
   __pyx_vtable_5cpprb_14PyReplayBuffer_ReplayBuffer.get_stored_size = (size_t (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_stored_size;
   __pyx_vtable_5cpprb_14PyReplayBuffer_ReplayBuffer.get_buffer_size = (size_t (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_buffer_size;
   __pyx_vtable_5cpprb_14PyReplayBuffer_ReplayBuffer.get_next_index = (size_t (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_next_index;
   __pyx_vtable_5cpprb_14PyReplayBuffer_ReplayBuffer.add_cache = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *))__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_add_cache;
+  __pyx_vtable_5cpprb_14PyReplayBuffer_ReplayBuffer.add_cache_i = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, size_t, size_t))__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_add_cache_i;
   __pyx_vtable_5cpprb_14PyReplayBuffer_ReplayBuffer.on_episode_end = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_on_episode_end;
   __pyx_vtable_5cpprb_14PyReplayBuffer_ReplayBuffer.get_current_episode_len = (size_t (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_get_current_episode_len;
   __pyx_vtable_5cpprb_14PyReplayBuffer_ReplayBuffer.is_Nstep = (bool (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_12ReplayBuffer_is_Nstep;
   if (PyType_Ready(&__pyx_type_5cpprb_14PyReplayBuffer_ReplayBuffer) < 0) __PYX_ERR(0, 905, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_5cpprb_14PyReplayBuffer_ReplayBuffer.tp_print = 0;
   #endif
@@ -60691,110 +60898,110 @@
   __pyx_ptype_5cpprb_14PyReplayBuffer_ReplayBuffer = &__pyx_type_5cpprb_14PyReplayBuffer_ReplayBuffer;
   __pyx_vtabptr_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer = &__pyx_vtable_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer;
   __pyx_vtable_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer.__pyx_base = *__pyx_vtabptr_5cpprb_14PyReplayBuffer_ReplayBuffer;
   __pyx_vtable_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer.__pyx_base.clear = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_clear;
   __pyx_vtable_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer.__pyx_base.on_episode_end = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_on_episode_end;
   __pyx_vtable_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer.get_max_priority = (float (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_get_max_priority;
   __pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer.tp_base = __pyx_ptype_5cpprb_14PyReplayBuffer_ReplayBuffer;
-  if (PyType_Ready(&__pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1313, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1330, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer.tp_dictoffset && __pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #if CYTHON_COMPILING_IN_CPYTHON
   {
-    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 1313, __pyx_L1_error)
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 1330, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_2__init__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_2__init__.doc = __pyx_doc_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_2__init__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_5cpprb_14PyReplayBuffer_23PrioritizedReplayBuffer_2__init__;
     }
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer.tp_dict, __pyx_vtabptr_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1313, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_PrioritizedReplayBuffer, (PyObject *)&__pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1313, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1313, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer.tp_dict, __pyx_vtabptr_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1330, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_PrioritizedReplayBuffer, (PyObject *)&__pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1330, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1330, __pyx_L1_error)
   __pyx_ptype_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer = &__pyx_type_5cpprb_14PyReplayBuffer_PrioritizedReplayBuffer;
   __pyx_vtabptr_5cpprb_14PyReplayBuffer_MPReplayBuffer = &__pyx_vtable_5cpprb_14PyReplayBuffer_MPReplayBuffer;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPReplayBuffer._lock_explorer = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *))__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer__lock_explorer;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPReplayBuffer._unlock_explorer = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *))__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer__unlock_explorer;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPReplayBuffer._lock_learner = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *))__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer__lock_learner;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPReplayBuffer._unlock_learner = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *))__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer__unlock_learner;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPReplayBuffer.clear = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_clear;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPReplayBuffer.get_stored_size = (size_t (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_get_stored_size;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPReplayBuffer.get_buffer_size = (size_t (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_get_buffer_size;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPReplayBuffer.get_next_index = (size_t (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_get_next_index;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPReplayBuffer.on_episode_end = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_on_episode_end;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPReplayBuffer.is_Nstep = (bool (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_14MPReplayBuffer_is_Nstep;
-  if (PyType_Ready(&__pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer) < 0) __PYX_ERR(0, 1586, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer) < 0) __PYX_ERR(0, 1603, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer.tp_dictoffset && __pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #if CYTHON_COMPILING_IN_CPYTHON
   {
-    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 1586, __pyx_L1_error)
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 1603, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_5cpprb_14PyReplayBuffer_14MPReplayBuffer___init__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_5cpprb_14PyReplayBuffer_14MPReplayBuffer___init__.doc = __pyx_doc_5cpprb_14PyReplayBuffer_14MPReplayBuffer___init__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_5cpprb_14PyReplayBuffer_14MPReplayBuffer___init__;
     }
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer.tp_dict, __pyx_vtabptr_5cpprb_14PyReplayBuffer_MPReplayBuffer) < 0) __PYX_ERR(0, 1586, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MPReplayBuffer, (PyObject *)&__pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer) < 0) __PYX_ERR(0, 1586, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer) < 0) __PYX_ERR(0, 1586, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer.tp_dict, __pyx_vtabptr_5cpprb_14PyReplayBuffer_MPReplayBuffer) < 0) __PYX_ERR(0, 1603, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MPReplayBuffer, (PyObject *)&__pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer) < 0) __PYX_ERR(0, 1603, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer) < 0) __PYX_ERR(0, 1603, __pyx_L1_error)
   __pyx_ptype_5cpprb_14PyReplayBuffer_MPReplayBuffer = &__pyx_type_5cpprb_14PyReplayBuffer_MPReplayBuffer;
   __pyx_vtabptr_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler = &__pyx_vtable_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler;
   __pyx_vtable_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler.ptr = (ymd::CppThreadSafePrioritizedSampler<float>  *(*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler *))__pyx_f_5cpprb_14PyReplayBuffer_28ThreadSafePrioritizedSampler_ptr;
-  if (PyType_Ready(&__pyx_type_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler) < 0) __PYX_ERR(0, 1859, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler) < 0) __PYX_ERR(0, 1876, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler.tp_dictoffset && __pyx_type_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler.tp_dict, __pyx_vtabptr_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler) < 0) __PYX_ERR(0, 1859, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ThreadSafePrioritizedSampler, (PyObject *)&__pyx_type_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler) < 0) __PYX_ERR(0, 1859, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler.tp_dict, __pyx_vtabptr_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler) < 0) __PYX_ERR(0, 1876, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ThreadSafePrioritizedSampler, (PyObject *)&__pyx_type_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler) < 0) __PYX_ERR(0, 1876, __pyx_L1_error)
   __pyx_ptype_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler = &__pyx_type_5cpprb_14PyReplayBuffer_ThreadSafePrioritizedSampler;
   __pyx_vtabptr_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer = &__pyx_vtable_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer.__pyx_base = *__pyx_vtabptr_5cpprb_14PyReplayBuffer_MPReplayBuffer;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer.__pyx_base.clear = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_clear;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer.__pyx_base.on_episode_end = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_on_episode_end;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer._lock_explorer_per = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *))__pyx_f_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer__lock_explorer_per;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer._unlock_explorer_per = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *))__pyx_f_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer__unlock_explorer_per;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer._lock_learner_per = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *))__pyx_f_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer__lock_learner_per;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer._unlock_learner_per = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *))__pyx_f_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer__unlock_learner_per;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer._lock_learner_unlock_learner_per = (void (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *))__pyx_f_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer__lock_learner_unlock_learner_per;
   __pyx_vtable_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer.get_max_priority = (float (*)(struct __pyx_obj_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer *, int __pyx_skip_dispatch))__pyx_f_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer_get_max_priority;
   __pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer.tp_base = __pyx_ptype_5cpprb_14PyReplayBuffer_MPReplayBuffer;
-  if (PyType_Ready(&__pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1920, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1937, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer.tp_dictoffset && __pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #if CYTHON_COMPILING_IN_CPYTHON
   {
-    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 1920, __pyx_L1_error)
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 1937, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer___init__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer___init__.doc = __pyx_doc_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer___init__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_5cpprb_14PyReplayBuffer_25MPPrioritizedReplayBuffer___init__;
     }
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer.tp_dict, __pyx_vtabptr_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1920, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MPPrioritizedReplayBuffer, (PyObject *)&__pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1920, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1920, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer.tp_dict, __pyx_vtabptr_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1937, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MPPrioritizedReplayBuffer, (PyObject *)&__pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1937, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer) < 0) __PYX_ERR(0, 1937, __pyx_L1_error)
   __pyx_ptype_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer = &__pyx_type_5cpprb_14PyReplayBuffer_MPPrioritizedReplayBuffer;
   if (PyType_Ready(&__pyx_type_5cpprb_14PyReplayBuffer___pyx_scope_struct__dict2buffer) < 0) __PYX_ERR(0, 465, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_5cpprb_14PyReplayBuffer___pyx_scope_struct__dict2buffer.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5cpprb_14PyReplayBuffer___pyx_scope_struct__dict2buffer.tp_dictoffset && __pyx_type_5cpprb_14PyReplayBuffer___pyx_scope_struct__dict2buffer.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_5cpprb_14PyReplayBuffer___pyx_scope_struct__dict2buffer.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
@@ -61714,352 +61921,362 @@
  *     cdef size_t get_stored_size(self):             # <<<<<<<<<<<<<<
  *         with self.lock:
  *             return RingBufferIndex.get_stored_size(self)
  */
   __Pyx_TraceLine(899,0,__PYX_ERR(0, 899, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1169
+  /* "cpprb/PyReplayBuffer.pyx":1177
  *         return self._encode_sample(idx)
  * 
  *     cpdef void clear(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Clear replay buffer.
  * 
  */
-  __Pyx_TraceLine(1169,0,__PYX_ERR(0, 1169, __pyx_L1_error))
+  __Pyx_TraceLine(1177,0,__PYX_ERR(0, 1177, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1196
+  /* "cpprb/PyReplayBuffer.pyx":1204
  *             self.nstep.clear()
  * 
  *     cpdef size_t get_stored_size(self):             # <<<<<<<<<<<<<<
  *         r"""Get stored size
  * 
  */
-  __Pyx_TraceLine(1196,0,__PYX_ERR(0, 1196, __pyx_L1_error))
+  __Pyx_TraceLine(1204,0,__PYX_ERR(0, 1204, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1206
+  /* "cpprb/PyReplayBuffer.pyx":1214
  *         return self.index.get_stored_size()
  * 
  *     cpdef size_t get_buffer_size(self):             # <<<<<<<<<<<<<<
  *         r"""Get buffer size
  * 
  */
-  __Pyx_TraceLine(1206,0,__PYX_ERR(0, 1206, __pyx_L1_error))
+  __Pyx_TraceLine(1214,0,__PYX_ERR(0, 1214, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1216
+  /* "cpprb/PyReplayBuffer.pyx":1224
  *         return self.buffer_size
  * 
  *     cpdef size_t get_next_index(self):             # <<<<<<<<<<<<<<
  *         r"""Get the next index to store
  * 
  */
-  __Pyx_TraceLine(1216,0,__PYX_ERR(0, 1216, __pyx_L1_error))
+  __Pyx_TraceLine(1224,0,__PYX_ERR(0, 1224, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1226
+  /* "cpprb/PyReplayBuffer.pyx":1234
  *         return self.index.get_next_index()
  * 
  *     cdef void add_cache(self):             # <<<<<<<<<<<<<<
  *         r"""Add last items into cache
  * 
  */
-  __Pyx_TraceLine(1226,0,__PYX_ERR(0, 1226, __pyx_L1_error))
+  __Pyx_TraceLine(1234,0,__PYX_ERR(0, 1234, __pyx_L1_error))
+
+
+  /* "cpprb/PyReplayBuffer.pyx":1265
+ *             self.add_cache_i(key, key_end)
+ * 
+ *     cdef void add_cache_i(self, size_t key, size_t key_end):             # <<<<<<<<<<<<<<
+ *         # If key is already cached, don't do anything
+ *         if key in self.cache:
+ */
+  __Pyx_TraceLine(1265,0,__PYX_ERR(0, 1265, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1272
- *             self.cache[key] = cache_key
+  /* "cpprb/PyReplayBuffer.pyx":1289
+ * 
  * 
  *     cpdef void on_episode_end(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Call on episode end
  * 
  */
-  __Pyx_TraceLine(1272,0,__PYX_ERR(0, 1272, __pyx_L1_error))
+  __Pyx_TraceLine(1289,0,__PYX_ERR(0, 1289, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1294
+  /* "cpprb/PyReplayBuffer.pyx":1311
  *         self.episode_len = 0
  * 
  *     cpdef size_t get_current_episode_len(self):             # <<<<<<<<<<<<<<
  *         r"""Get current episode length
  * 
  */
-  __Pyx_TraceLine(1294,0,__PYX_ERR(0, 1294, __pyx_L1_error))
+  __Pyx_TraceLine(1311,0,__PYX_ERR(0, 1311, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1303
+  /* "cpprb/PyReplayBuffer.pyx":1320
  *         return self.episode_len
  * 
  *     cpdef bool is_Nstep(self):             # <<<<<<<<<<<<<<
  *         r"""Get whether use Nstep or not
  * 
  */
-  __Pyx_TraceLine(1303,0,__PYX_ERR(0, 1303, __pyx_L1_error))
+  __Pyx_TraceLine(1320,0,__PYX_ERR(0, 1320, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1543
+  /* "cpprb/PyReplayBuffer.pyx":1560
  *             self.per.update_priorities(self.idx_vec.data(),self.ps_vec.data(),N)
  * 
  *     cpdef void clear(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Clear replay buffer
  *         """
  */
-  __Pyx_TraceLine(1543,0,__PYX_ERR(0, 1543, __pyx_L1_error))
+  __Pyx_TraceLine(1560,0,__PYX_ERR(0, 1560, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1551
+  /* "cpprb/PyReplayBuffer.pyx":1568
  *             self.priorities_nstep.clear()
  * 
  *     cpdef float get_max_priority(self):             # <<<<<<<<<<<<<<
  *         r"""Get the max priority of stored priorities
  * 
  */
-  __Pyx_TraceLine(1551,0,__PYX_ERR(0, 1551, __pyx_L1_error))
+  __Pyx_TraceLine(1568,0,__PYX_ERR(0, 1568, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1561
+  /* "cpprb/PyReplayBuffer.pyx":1578
  *         return self.per.get_max_priority()
  * 
  *     cpdef void on_episode_end(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Call on episode end
  * 
  */
-  __Pyx_TraceLine(1561,0,__PYX_ERR(0, 1561, __pyx_L1_error))
+  __Pyx_TraceLine(1578,0,__PYX_ERR(0, 1578, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1658
+  /* "cpprb/PyReplayBuffer.pyx":1675
  *         self.explorer_count = Value(ctypes.c_size_t,0)
  * 
  *     cdef void _lock_explorer(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_ready.wait() # Wait permission
  *         self.learner_ready.clear()  # Block learner
  */
-  __Pyx_TraceLine(1658,0,__PYX_ERR(0, 1658, __pyx_L1_error))
+  __Pyx_TraceLine(1675,0,__PYX_ERR(0, 1675, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1664
+  /* "cpprb/PyReplayBuffer.pyx":1681
  *             self.explorer_count.value += 1
  * 
  *     cdef void _unlock_explorer(self) except *:             # <<<<<<<<<<<<<<
  *         with self.explorer_count.get_lock():
  *             self.explorer_count.value -= 1
  */
-  __Pyx_TraceLine(1664,0,__PYX_ERR(0, 1664, __pyx_L1_error))
+  __Pyx_TraceLine(1681,0,__PYX_ERR(0, 1681, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1670
+  /* "cpprb/PyReplayBuffer.pyx":1687
  *             self.learner_ready.set()
  * 
  *     cdef void _lock_learner(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_ready.clear() # New explorer cannot enter into critical section
  *         self.learner_ready.wait() # Wait until all explorer exit from critical section
  */
-  __Pyx_TraceLine(1670,0,__PYX_ERR(0, 1670, __pyx_L1_error))
+  __Pyx_TraceLine(1687,0,__PYX_ERR(0, 1687, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1674
+  /* "cpprb/PyReplayBuffer.pyx":1691
  *         self.learner_ready.wait() # Wait until all explorer exit from critical section
  * 
  *     cdef void _unlock_learner(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_ready.set() # Allow workers to enter into critical section
  * 
  */
-  __Pyx_TraceLine(1674,0,__PYX_ERR(0, 1674, __pyx_L1_error))
+  __Pyx_TraceLine(1691,0,__PYX_ERR(0, 1691, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1783
+  /* "cpprb/PyReplayBuffer.pyx":1800
  *         return ret
  * 
  *     cpdef void clear(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Clear replay buffer.
  * 
  */
-  __Pyx_TraceLine(1783,0,__PYX_ERR(0, 1783, __pyx_L1_error))
+  __Pyx_TraceLine(1800,0,__PYX_ERR(0, 1800, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1804
+  /* "cpprb/PyReplayBuffer.pyx":1821
  *         self.index.clear()
  * 
  *     cpdef size_t get_stored_size(self):             # <<<<<<<<<<<<<<
  *         r"""Get stored size
  * 
  */
-  __Pyx_TraceLine(1804,0,__PYX_ERR(0, 1804, __pyx_L1_error))
+  __Pyx_TraceLine(1821,0,__PYX_ERR(0, 1821, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1814
+  /* "cpprb/PyReplayBuffer.pyx":1831
  *         return self.index.get_stored_size()
  * 
  *     cpdef size_t get_buffer_size(self):             # <<<<<<<<<<<<<<
  *         r"""Get buffer size
  * 
  */
-  __Pyx_TraceLine(1814,0,__PYX_ERR(0, 1814, __pyx_L1_error))
+  __Pyx_TraceLine(1831,0,__PYX_ERR(0, 1831, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1824
+  /* "cpprb/PyReplayBuffer.pyx":1841
  *         return self.buffer_size
  * 
  *     cpdef size_t get_next_index(self):             # <<<<<<<<<<<<<<
  *         r"""Get the next index to store
  * 
  */
-  __Pyx_TraceLine(1824,0,__PYX_ERR(0, 1824, __pyx_L1_error))
+  __Pyx_TraceLine(1841,0,__PYX_ERR(0, 1841, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1834
+  /* "cpprb/PyReplayBuffer.pyx":1851
  *         return self.index.get_next_index()
  * 
  *     cpdef void on_episode_end(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Call on episode end
  * 
  */
-  __Pyx_TraceLine(1834,0,__PYX_ERR(0, 1834, __pyx_L1_error))
+  __Pyx_TraceLine(1851,0,__PYX_ERR(0, 1851, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1849
+  /* "cpprb/PyReplayBuffer.pyx":1866
  *         pass
  * 
  *     cpdef bool is_Nstep(self):             # <<<<<<<<<<<<<<
  *         r"""Get whether use Nstep or not
  * 
  */
-  __Pyx_TraceLine(1849,0,__PYX_ERR(0, 1849, __pyx_L1_error))
+  __Pyx_TraceLine(1866,0,__PYX_ERR(0, 1866, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1909
+  /* "cpprb/PyReplayBuffer.pyx":1926
  *                                                               eps)
  * 
  *     cdef CppThreadSafePrioritizedSampler[float]* ptr(self):             # <<<<<<<<<<<<<<
  *         return self.per
  * 
  */
-  __Pyx_TraceLine(1909,0,__PYX_ERR(0, 1909, __pyx_L1_error))
+  __Pyx_TraceLine(1926,0,__PYX_ERR(0, 1926, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":1998
+  /* "cpprb/PyReplayBuffer.pyx":2015
  *         self.ps_vec = vector[float]()
  * 
  *     cdef void _lock_explorer_per(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_per_ready.wait() # Wait permission
  *         self.learner_per_ready.clear()  # Block learner
  */
-  __Pyx_TraceLine(1998,0,__PYX_ERR(0, 1998, __pyx_L1_error))
+  __Pyx_TraceLine(2015,0,__PYX_ERR(0, 2015, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":2004
+  /* "cpprb/PyReplayBuffer.pyx":2021
  *             self.explorer_per_count.value += 1
  * 
  *     cdef void _unlock_explorer_per(self) except *:             # <<<<<<<<<<<<<<
  *         with self.explorer_per_count.get_lock():
  *             self.explorer_per_count.value -= 1
  */
-  __Pyx_TraceLine(2004,0,__PYX_ERR(0, 2004, __pyx_L1_error))
+  __Pyx_TraceLine(2021,0,__PYX_ERR(0, 2021, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":2010
+  /* "cpprb/PyReplayBuffer.pyx":2027
  *             self.learner_per_ready.set()
  * 
  *     cdef void _lock_learner_per(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_per_ready.clear()
  *         self.learner_per_ready.wait()
  */
-  __Pyx_TraceLine(2010,0,__PYX_ERR(0, 2010, __pyx_L1_error))
+  __Pyx_TraceLine(2027,0,__PYX_ERR(0, 2027, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":2014
+  /* "cpprb/PyReplayBuffer.pyx":2031
  *         self.learner_per_ready.wait()
  * 
  *     cdef void _unlock_learner_per(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_per_ready.set()
  * 
  */
-  __Pyx_TraceLine(2014,0,__PYX_ERR(0, 2014, __pyx_L1_error))
+  __Pyx_TraceLine(2031,0,__PYX_ERR(0, 2031, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":2017
+  /* "cpprb/PyReplayBuffer.pyx":2034
  *         self.explorer_per_ready.set()
  * 
  *     cdef void _lock_learner_unlock_learner_per(self) except *:             # <<<<<<<<<<<<<<
  *         self.explorer_ready.clear()
  *         self.explorer_per_ready.set()
  */
-  __Pyx_TraceLine(2017,0,__PYX_ERR(0, 2017, __pyx_L1_error))
+  __Pyx_TraceLine(2034,0,__PYX_ERR(0, 2034, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":2180
+  /* "cpprb/PyReplayBuffer.pyx":2197
  *         self._unlock_learner_per()
  * 
  *     cpdef void clear(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Clear replay buffer
  *         """
  */
-  __Pyx_TraceLine(2180,0,__PYX_ERR(0, 2180, __pyx_L1_error))
+  __Pyx_TraceLine(2197,0,__PYX_ERR(0, 2197, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":2186
+  /* "cpprb/PyReplayBuffer.pyx":2203
  *         clear(self.per.ptr())
  * 
  *     cpdef float get_max_priority(self):             # <<<<<<<<<<<<<<
  *         r"""Get the max priority of stored priorities
  * 
  */
-  __Pyx_TraceLine(2186,0,__PYX_ERR(0, 2186, __pyx_L1_error))
+  __Pyx_TraceLine(2203,0,__PYX_ERR(0, 2203, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":2196
+  /* "cpprb/PyReplayBuffer.pyx":2213
  *         return self.per.ptr().get_max_priority()
  * 
  *     cpdef void on_episode_end(self) except *:             # <<<<<<<<<<<<<<
  *         r"""Call on episode end
  * 
  */
-  __Pyx_TraceLine(2196,0,__PYX_ERR(0, 2196, __pyx_L1_error))
+  __Pyx_TraceLine(2213,0,__PYX_ERR(0, 2213, __pyx_L1_error))
 
 
-  /* "cpprb/PyReplayBuffer.pyx":2209
+  /* "cpprb/PyReplayBuffer.pyx":2226
  * 
  * @cython.embedsignature(True)
  * def create_buffer(size,env_dict=None,*,prioritized = False,**kwargs):             # <<<<<<<<<<<<<<
  *     r"""Create specified version of replay buffer
  * 
  */
-  __Pyx_TraceLine(2209,0,__PYX_ERR(0, 2209, __pyx_L1_error))
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5cpprb_14PyReplayBuffer_7create_buffer, NULL, __pyx_n_s_cpprb_PyReplayBuffer); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2209, __pyx_L1_error)
+  __Pyx_TraceLine(2226,0,__PYX_ERR(0, 2226, __pyx_L1_error))
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5cpprb_14PyReplayBuffer_7create_buffer, NULL, __pyx_n_s_cpprb_PyReplayBuffer); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_create_buffer, __pyx_t_2) < 0) __PYX_ERR(0, 2209, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_create_buffer, __pyx_t_2) < 0) __PYX_ERR(0, 2226, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2256
+  /* "cpprb/PyReplayBuffer.pyx":2273
  *           get_action: Callable,
  *           update_policy: Callable,*,
  *           max_steps: int=int(1e6),             # <<<<<<<<<<<<<<
  *           max_episodes: Optional[int] = None,
  *           batch_size: int = 64,
  */
-  __Pyx_TraceLine(2256,0,__PYX_ERR(0, 2256, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_float_1e6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2256, __pyx_L1_error)
+  __Pyx_TraceLine(2273,0,__PYX_ERR(0, 2273, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_float_1e6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_k__30 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "cpprb/PyReplayBuffer.pyx":2252
+  /* "cpprb/PyReplayBuffer.pyx":2269
  * 
  * @cython.embedsignature(True)
  * def train(buffer: ReplayBuffer,             # <<<<<<<<<<<<<<
  *           env,
  *           get_action: Callable,
  */
-  __Pyx_TraceLine(2252,0,__PYX_ERR(0, 2252, __pyx_L1_error))
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5cpprb_14PyReplayBuffer_9train, NULL, __pyx_n_s_cpprb_PyReplayBuffer); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2252, __pyx_L1_error)
+  __Pyx_TraceLine(2269,0,__PYX_ERR(0, 2269, __pyx_L1_error))
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5cpprb_14PyReplayBuffer_9train, NULL, __pyx_n_s_cpprb_PyReplayBuffer); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_train, __pyx_t_2) < 0) __PYX_ERR(0, 2252, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_train, __pyx_t_2) < 0) __PYX_ERR(0, 2269, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_StepChecker(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
@@ -62167,16 +62384,16 @@
  * # distutils: language = c++             # <<<<<<<<<<<<<<
  * # cython: linetrace=True
  * 
  */
   __Pyx_TraceLine(1,0,__PYX_ERR(0, 1, __pyx_L1_error))
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_ReplayBuffer_clear_line_1169, __pyx_kp_u_Clear_replay_buffer_Set_index_an) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_MPReplayBuffer_clear_line_1783, __pyx_kp_u_Clear_replay_buffer_Set_index_an) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_ReplayBuffer_clear_line_1177, __pyx_kp_u_Clear_replay_buffer_Set_index_an) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_MPReplayBuffer_clear_line_1800, __pyx_kp_u_Clear_replay_buffer_Set_index_an) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "../../../usr/local/lib/python3.7/site-packages/numpy/__init__.pxd":742
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
```

### Comparing `cpprb-9.4.5/cpprb/ReplayBuffer.hh` & `cpprb-9.4.6/cpprb/ReplayBuffer.hh`

 * *Files identical despite different names*

### Comparing `cpprb-9.4.5/cpprb/SegmentTree.hh` & `cpprb-9.4.6/cpprb/SegmentTree.hh`

 * *Files identical despite different names*

### Comparing `cpprb-9.4.5/cpprb/VectorWrapper.cpp` & `cpprb-9.4.6/cpprb/VectorWrapper.cpp`

 * *Files identical despite different names*

### Comparing `cpprb-9.4.5/cpprb/util.py` & `cpprb-9.4.6/cpprb/util.py`

 * *Files identical despite different names*

### Comparing `cpprb-9.4.5/cpprb.egg-info/PKG-INFO` & `cpprb-9.4.6/cpprb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpprb
-Version: 9.4.5
+Version: 9.4.6
 Summary: ReplayBuffer for Reinforcement Learning written by C++ and Cython
 Home-page: https://ymd_h.gitlab.io/cpprb/
 Author: Yamada Hiroyuki
 License: UNKNOWN
 Description: ![img](https://img.shields.io/gitlab/pipeline/ymd_h/cpprb.svg)
         ![img](https://img.shields.io/pypi/v/cpprb.svg)
         ![img](https://img.shields.io/pypi/l/cpprb.svg)
```

### Comparing `cpprb-9.4.5/setup.py` & `cpprb-9.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     warnings.warn("No README.md")
     long_description =  description
     long_description_content_type='text/plain'
 
 setup(name="cpprb",
       author="Yamada Hiroyuki",
       description=description,
-      version="9.4.5",
+      version="9.4.6",
       install_requires=requires,
       setup_requires=setup_requires,
       extras_require=extras,
       cmdclass={'build_ext': LazyImportBuildExtCommand},
       url="https://ymd_h.gitlab.io/cpprb/",
       ext_modules=ext_modules,
       include_dirs=["cpprb"],
```

