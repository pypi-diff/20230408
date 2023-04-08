# Comparing `tmp/last-asr-0.0.1.tar.gz` & `tmp/last-asr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "last-asr-0.0.1.tar", last modified: Wed Oct 19 20:49:34 2022, max compression
+gzip compressed data, was "last-asr-0.0.2.tar", last modified: Fri Apr  7 22:45:35 2023, max compression
```

## Comparing `last-asr-0.0.1.tar` & `last-asr-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,12 @@
--rw-r--r--   0        0        0     1334 2022-10-19 20:12:49.973327 last-asr-0.0.1/.github/workflows/pytest_and_autopublish.yml
--rw-r--r--   0        0        0      253 2022-10-19 20:12:49.973327 last-asr-0.0.1/.gitignore
--rw-r--r--   0        0        0    14783 2022-10-19 20:12:49.973327 last-asr-0.0.1/.pylintrc
--rw-r--r--   0        0        0      104 2022-10-19 20:12:49.973327 last-asr-0.0.1/.style.yapf
--rw-r--r--   0        0        0      780 2022-10-19 20:12:49.973327 last-asr-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0      296 2022-10-17 23:05:56.521482 last-asr-0.0.1/AUTHORS
--rw-r--r--   0        0        0     1103 2022-10-17 23:05:56.521482 last-asr-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2022-10-17 23:05:56.521482 last-asr-0.0.1/LICENSE
--rw-r--r--   0        0        0      605 2022-10-17 23:05:56.521482 last-asr-0.0.1/README.md
--rw-r--r--   0        0        0      723 2022-10-19 20:36:37.268847 last-asr-0.0.1/last/__init__.py
--rw-r--r--   0        0        0    10888 2022-10-19 20:12:49.973327 last-asr-0.0.1/last/semirings.py
--rw-r--r--   0        0        0     1127 2022-10-19 20:49:23.120406 last-asr-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      982 2022-10-19 20:12:49.973327 last-asr-0.0.1/tests/last_test.py
--rw-r--r--   0        0        0    12711 2022-10-19 20:12:49.973327 last-asr-0.0.1/tests/semirings_test.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 last-asr-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-07 22:44:59.937729 last-asr-0.0.2/LICENSE
+-rw-r--r--   0        0        0      682 2023-04-07 22:44:59.937729 last-asr-0.0.2/README.md
+-rw-r--r--   0        0        0      514 2023-04-07 22:44:59.937729 last-asr-0.0.2/last/.readthedocs.yaml
+-rw-r--r--   0        0        0      850 2023-04-07 22:44:59.937729 last-asr-0.0.2/last/__init__.py
+-rw-r--r--   0        0        0    18488 2023-04-07 22:44:59.937729 last-asr-0.0.2/last/alignments.py
+-rw-r--r--   0        0        0    12216 2023-04-07 22:44:59.937729 last-asr-0.0.2/last/contexts.py
+-rw-r--r--   0        0        0    34907 2023-04-07 22:44:59.937729 last-asr-0.0.2/last/lattices.py
+-rw-r--r--   0        0        0     4872 2023-04-07 22:44:59.937729 last-asr-0.0.2/last/scatter_reduce.py
+-rw-r--r--   0        0        0    15206 2023-04-07 22:44:59.941729 last-asr-0.0.2/last/semirings.py
+-rw-r--r--   0        0        0    11569 2023-04-07 22:44:59.941729 last-asr-0.0.2/last/weight_fns.py
+-rw-r--r--   0        0        0     1230 2023-04-07 22:44:59.941729 last-asr-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1632 1970-01-01 00:00:00.000000 last-asr-0.0.2/PKG-INFO
```

### Comparing `last-asr-0.0.1/LICENSE` & `last-asr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `last-asr-0.0.1/README.md` & `last-asr-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # LAttice-based Speech Transducer (LAST)
 
 [![Unittests](https://github.com/google-research/last/actions/workflows/pytest_and_autopublish.yml/badge.svg)](https://github.com/google-research/last/actions/workflows/pytest_and_autopublish.yml)
-[![PyPI version](https://badge.fury.io/py/last.svg)](https://badge.fury.io/py/last)
+[![PyPI version](https://badge.fury.io/py/last-asr.svg)](https://badge.fury.io/py/last-asr)
 
 *This is not an officially supported Google product.*
 
 The LAttice-based Speech Transducer (LAST) is a JAX library for building
 lattice-based speech transducer models, such as
 [GNAT](https://arxiv.org/abs/2205.13674).
 
-To start using LAST, simply run `pip install --upgrade last`.
+To start using LAST, simply run `pip install --upgrade last-asr`. For more
+information, check out https://last-asr.readthedocs.io.
```

### Comparing `last-asr-0.0.1/last/__init__.py` & `last-asr-0.0.2/last/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The LAST Authors.
+# Copyright 2023 The LAST Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,11 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """LAST API."""
 
+from last import alignments
+from last import contexts
 from last import semirings
+from last import weight_fns
+from last.lattices import RecognitionLattice
 
 # A new PyPI release will be pushed everytime `__version__` is increased.
-__version__ = '0.0.1'
+__version__ = '0.0.2'
```

### Comparing `last-asr-0.0.1/last/semirings.py` & `last-asr-0.0.2/last/semirings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The LAST Authors.
+# Copyright 2023 The LAST Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,44 +18,119 @@
 import dataclasses
 import functools
 from typing import Any, Callable, Generic, Optional, TypeVar
 
 import jax
 import jax.numpy as jnp
 
-# Types.
+# Types for documentation purposes.
 DType = Any
+PyTree = Any
+# Type variables for semiring values.
 T = TypeVar('T')
 S = TypeVar('S')
 
 
+def value_shape(x: PyTree) -> tuple[int, ...]:
+  """Obtains the shape of a semiring value.
+
+  A semiring value is a PyTree of one or more identically shaped ndarrays.
+  The shape of a semiring value is thus the common of shape of its leaves.
+
+  Args:
+    x: Some semiring value.
+
+  Returns:
+    The common shape of the leaves of x.
+
+  Raises:
+    ValueError: If the leaves of x do not have a common shape.
+  """
+  shapes = [i.shape for i in jax.tree_util.tree_leaves(x)]
+  if not shapes:
+    raise ValueError(
+        f'No common shape can be derived for an empty PyTree: {x!r}'
+    )
+  result = shapes[0]
+  for i in shapes[1:]:
+    if i != result:
+      raise ValueError(
+          'A semiring value must consist of ndarrays of a common shape. '
+          f'Got inconsistent shapes {result} vs {i} for PyTree: {x!r}'
+      )
+  return result
+
+
+def value_dtype(x: PyTree) -> DType:
+  """Obtains the dtypes of a semiring value.
+
+  Different leaves of a semiring value may have different dtypes. Methods
+  such as Semiring.{zeros,ones} can take a PyTree of dtypes in the same
+  structure as the corresponding semiring values. This function can be used
+  to extract such a dtype PyTree from a semiring value.
+
+  Args:
+    x: Some semiring value.
+
+  Returns:
+    dtypes in the same structure as x.
+  """
+  return jax.tree_util.tree_map(lambda x_: x_.dtype, x)
+
+
 class Semiring(Generic[T]):
   """Base Semiring interface.
 
   See https://en.wikipedia.org/wiki/Semiring for what a semiring is. A Semiring
   object holds methods that implement the semiring operations. To simplify
   non-semiring operations on the semiring values, the semiring values are not
   typed: for most basic semirings, each value is a single ndarray; for some more
-  complex semirings (e.g. Expectation), the values can be a tuple of ndarrays.
+  complex semirings (e.g. Expectation or Cartesian), the values can be a tuple
+  of ndarrays.
+
+  In general, a semiring value under some semiring is represented as a PyTree
+  of identically shaped ndarrays, with possibly different dtypes. The shape
+  and dtypes of a semiring value can be obtained with methods
+  `last.semirings.value_shape()` and `last.semirings.value_dtype()`.
 
   Semiring is not an abstract base class because we allow operations to be
-  unimplemented.
+  unimplemented (e.g. `prod`, is not commonly used).
 
-  Note: Reductions (prod & sum) can be tricky to implement right, here are two
-  important things to watch out for:
+  Note: Reductions (prod & sum) can be tricky to implement correctly, here are
+  two important things to watch out for:
   *   `axis` can be in the range [-rank, rank).
   *   The input can have 0-sized dimensions.
   """
 
   def zeros(self, shape: Sequence[int], dtype: Optional[DType] = None) -> T:
-    """Semiring zeros in the given shape and dtype."""
+    """Semiring zeros in the given shape and dtype.
+
+    Args:
+      shape: Desired output shape.
+      dtype: Optional PyTree of dtypes.
+
+    Returns:
+      If dtype is None, semiring zero values in the specified shape with
+      reasonable default dtypes. Otherwise, semiring zero values in the
+      specified shape with the specified dtypes.
+    """
     raise NotImplementedError
 
   def ones(self, shape: Sequence[int], dtype: Optional[DType] = None) -> T:
-    """Semiring ones in the given shape and dtype."""
+    """Semiring ones in the given shape and dtype.
+
+    Args:
+      shape: Desired output shape.
+      dtype: Optional PyTree of dtypes.
+
+    Returns:
+      If dtype is None, semiring one values in the specified shape with
+      reasonable default dtypes. Otherwise, semiring one values in the
+      specified shape with the specified dtypes.
+    """
     raise NotImplementedError
 
   def times(self, a: T, b: T) -> T:
     """Semiring multiplication between two values."""
     raise NotImplementedError
 
   def plus(self, a: T, b: T) -> T:
@@ -71,15 +146,17 @@
     raise NotImplementedError
 
 
 class _Real(Semiring[jnp.ndarray]):
   """Real semiring."""
 
   @staticmethod
-  def zeros(shape: Sequence[int], dtype: Optional[DType] = None) -> jnp.ndarray:
+  def zeros(
+      shape: Sequence[int], dtype: Optional[DType] = None
+  ) -> jnp.ndarray:
     return jnp.zeros(shape, dtype)
 
   @staticmethod
   def ones(shape: Sequence[int], dtype: Optional[DType] = None) -> jnp.ndarray:
     return jnp.ones(shape, dtype)
 
   @staticmethod
@@ -110,15 +187,17 @@
         f'Invalid reduction axis={axis!r} for input shape {a.shape}')
 
 
 class _Log(Semiring[jnp.ndarray]):
   """Log semiring."""
 
   @staticmethod
-  def zeros(shape: Sequence[int], dtype: Optional[DType] = None) -> jnp.ndarray:
+  def zeros(
+      shape: Sequence[int], dtype: Optional[DType] = None
+  ) -> jnp.ndarray:
     return jnp.full(shape, -jnp.inf, dtype)
 
   @staticmethod
   def ones(shape: Sequence[int], dtype: Optional[DType] = None) -> jnp.ndarray:
     return jnp.zeros(shape, dtype)
 
   @staticmethod
@@ -229,15 +308,17 @@
   """Max tropical semiring.
 
   The gradients of `plus` and `sum` is guaranteed to be non-zero on exactly 1
   input element, even in the event of a tie.
   """
 
   @staticmethod
-  def zeros(shape: Sequence[int], dtype: Optional[DType] = None) -> jnp.ndarray:
+  def zeros(
+      shape: Sequence[int], dtype: Optional[DType] = None
+  ) -> jnp.ndarray:
     return jnp.full(shape, -jnp.inf, dtype)
 
   @staticmethod
   def ones(shape: Sequence[int], dtype: Optional[DType] = None) -> jnp.ndarray:
     return jnp.zeros(shape, dtype)
 
   @staticmethod
@@ -331,25 +412,39 @@
     w_to_x: Function to convert a value from semiring `w` to semiring `x`.
   """
   w: Semiring[T]
   x: Semiring[S]
   w_to_x: Callable[[T], S]
 
   def weighted(self, w: T, v: S) -> tuple[T, S]:
-    return w, self.x.times(self.w_to_x(w), v)
-
-  def zeros(self,
-            shape: Sequence[int],
-            dtype: Optional[DType] = None) -> tuple[T, S]:
-    return self.w.zeros(shape, dtype), self.x.zeros(shape, dtype)
-
-  def ones(self,
-           shape: Sequence[int],
-           dtype: Optional[DType] = None) -> tuple[T, S]:
-    return self.w.ones(shape, dtype), self.x.zeros(shape, dtype)
+    # When w is zero in semiring self.w, self.w_to_x(w) is zero in semiring
+    # self.x. We stipulate that the weighted value should always be zero in
+    # semiring self.x. This is useful for avoiding NaNs when both semirings are
+    # Log and w is -inf and v is +inf (e.g. computing 0 log 0 under Log).
+    w_is_zero = w == self.w.zeros([], w.dtype)
+    safe_v = jnp.where(w_is_zero, 0, v)
+    return w, self.x.times(self.w_to_x(w), safe_v)
+
+  def zeros(
+      self, shape: Sequence[int], dtype: Optional[DType] = None
+  ) -> tuple[T, S]:
+    if dtype is None:
+      dtype_w = dtype_x = None
+    else:
+      dtype_w, dtype_x = dtype
+    return self.w.zeros(shape, dtype_w), self.x.zeros(shape, dtype_x)
+
+  def ones(
+      self, shape: Sequence[int], dtype: Optional[DType] = None
+  ) -> tuple[T, S]:
+    if dtype is None:
+      dtype_w = dtype_x = None
+    else:
+      dtype_w, dtype_x = dtype
+    return self.w.ones(shape, dtype_w), self.x.zeros(shape, dtype_x)
 
   def times(self, a: tuple[T, S], b: tuple[T, S]) -> tuple[T, S]:
     w_a, x_a = a
     w_b, x_b = b
     w = self.w.times(w_a, w_b)
     x = self.x.plus(
         self.x.times(self.w_to_x(w_a), x_b),
@@ -369,7 +464,56 @@
     x = self.x.sum(x, axis)
     return w, x
 
 
 # Expectation semiring with weight and weighted sum represented both using the
 # Log semiring. Therefore only summation on non-negative value is allowed.
 LogLogExpectation = Expectation(w=Log, x=Log, w_to_x=lambda x: x)
+
+
+@dataclasses.dataclass(frozen=True)
+class Cartesian(Generic[T, S], Semiring[tuple[T, S]]):
+  """Cartesian product of 2 semirings.
+
+  Attributes:
+    x: The first semiring.
+    y: The second semiring.
+  """
+
+  x: Semiring[T]
+  y: Semiring[S]
+
+  def zeros(
+      self, shape: Sequence[int], dtype: Optional[DType] = None
+  ) -> tuple[T, S]:
+    if dtype is None:
+      dtype_x = dtype_y = None
+    else:
+      dtype_x, dtype_y = dtype
+    return self.x.zeros(shape, dtype_x), self.y.zeros(shape, dtype_y)
+
+  def ones(
+      self, shape: Sequence[int], dtype: Optional[DType] = None
+  ) -> tuple[T, S]:
+    if dtype is None:
+      dtype_x = dtype_y = None
+    else:
+      dtype_x, dtype_y = dtype
+    return self.x.ones(shape, dtype_x), self.y.ones(shape, dtype_y)
+
+  def times(self, a: tuple[T, S], b: tuple[T, S]) -> tuple[T, S]:
+    a_x, a_y = a
+    b_x, b_y = b
+    return self.x.times(a_x, b_x), self.y.times(a_y, b_y)
+
+  def plus(self, a: tuple[T, S], b: tuple[T, S]) -> tuple[T, S]:
+    a_x, a_y = a
+    b_x, b_y = b
+    return self.x.plus(a_x, b_x), self.y.plus(a_y, b_y)
+
+  def sum(self, a: tuple[T, S], axis: int) -> tuple[T, S]:
+    a_x, a_y = a
+    return self.x.sum(a_x, axis), self.y.sum(a_y, axis)
+
+  def prod(self, a: tuple[T, S], axis: int) -> tuple[T, S]:
+    a_x, a_y = a
+    return self.x.prod(a_x, axis), self.y.prod(a_y, axis)
```

### Comparing `last-asr-0.0.1/pyproject.toml` & `last-asr-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 [project]
+# Unfortunately PyPI doesn't allow us to use "last" as the package name.
 name = "last-asr"
 description = "The LAttice-based Speech Transducer (LAST) library"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [{name = "LAST authors"}]
 classifiers = [
@@ -11,14 +12,15 @@
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Science/Research",
 ]
 keywords = ["speech", "jax"]
 
 # pip dependencies of the project
 dependencies = [
+  "einops>=0.5.0",
   "flax>=0.6.1",
   "jax>=0.3.21",
 ]
 
 # This is set automatically by flit using `last.__version__`
 dynamic = ["version"]
 
@@ -29,14 +31,15 @@
 
 [project.optional-dependencies]
 # Development deps (unittest, linting, formating,...)
 # Installed through `pip install .[dev]`
 dev = [
   "absl-py",
   "numpy",
+  "optax",
   "pytest",
   "pytest-xdist",
   "pylint>=2.6.0",
   "yapf",
 ]
 
 [build-system]
```

### Comparing `last-asr-0.0.1/PKG-INFO` & `last-asr-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: last-asr
-Version: 0.0.1
+Version: 0.0.2
 Summary: The LAttice-based Speech Transducer (LAST) library
 Keywords: speech,jax
 Author: LAST authors
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
+Requires-Dist: einops>=0.5.0
 Requires-Dist: flax>=0.6.1
 Requires-Dist: jax>=0.3.21
 Requires-Dist: absl-py ; extra == "dev"
 Requires-Dist: numpy ; extra == "dev"
+Requires-Dist: optax ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-xdist ; extra == "dev"
 Requires-Dist: pylint>=2.6.0 ; extra == "dev"
 Requires-Dist: yapf ; extra == "dev"
 Project-URL: homepage, https://github.com/google-research/last
 Project-URL: repository, https://github.com/google-research/last
 Provides-Extra: dev
 
 # LAttice-based Speech Transducer (LAST)
 
 [![Unittests](https://github.com/google-research/last/actions/workflows/pytest_and_autopublish.yml/badge.svg)](https://github.com/google-research/last/actions/workflows/pytest_and_autopublish.yml)
-[![PyPI version](https://badge.fury.io/py/last.svg)](https://badge.fury.io/py/last)
+[![PyPI version](https://badge.fury.io/py/last-asr.svg)](https://badge.fury.io/py/last-asr)
 
 *This is not an officially supported Google product.*
 
 The LAttice-based Speech Transducer (LAST) is a JAX library for building
 lattice-based speech transducer models, such as
 [GNAT](https://arxiv.org/abs/2205.13674).
 
-To start using LAST, simply run `pip install --upgrade last`.
+To start using LAST, simply run `pip install --upgrade last-asr`. For more
+information, check out https://last-asr.readthedocs.io.
```

