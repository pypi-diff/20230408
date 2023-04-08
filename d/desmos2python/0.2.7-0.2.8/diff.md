# Comparing `tmp/desmos2python-0.2.7.tar.gz` & `tmp/desmos2python-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desmos2python-0.2.7.tar", last modified: Fri Mar 10 23:53:34 2023, max compression
+gzip compressed data, was "desmos2python-0.2.8.tar", last modified: Sat Apr  8 21:30:45 2023, max compression
```

## Comparing `desmos2python-0.2.7.tar` & `desmos2python-0.2.8.tar`

### file list

```diff
@@ -1,616 +1,616 @@
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.390967 desmos2python-0.2.7/
--rw-r--r--   0 robertc   (1000) robertc   (1000)       38 2023-02-24 00:18:55.000000 desmos2python-0.2.7/.bumpversion.cfg
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.260967 desmos2python-0.2.7/.eggs/
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.260967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.270967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5143 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/__config__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    16174 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      331 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_distributor_init.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3885 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_globals.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.270967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1422 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/hook-numpy.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1143 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/pyinstaller-smoke.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1135 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/test_pyinstaller.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6668 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pytesttester.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.274300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7108 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3925 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_add_docstring.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4391 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_array_like.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5916 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_char_codes.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5628 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_dtype_like.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1111 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_extended_precision.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7479 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_generic_alias.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      345 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_nbit.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2701 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_nested_sequence.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      957 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_scalars.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      191 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_shape.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      337 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/setup.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      498 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_version.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.277633 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/
--rw-r--r--   0 robertc   (1000) robertc   (1000)    10221 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    43226 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_array_object.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)       66 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_constants.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    10050 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_creation_functions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4480 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_data_type_functions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3707 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_dtypes.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    24772 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_elementwise_functions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3008 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_manipulation_functions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1457 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_searching_functions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2948 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_set_functions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1754 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_sorting_functions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3378 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_statistical_functions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1376 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_typing.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      824 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_utility_functions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    17860 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/linalg.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      341 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/setup.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.280967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)      282 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    15771 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_array_object.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5023 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_creation_functions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      422 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_data_type_functions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3619 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_elementwise_functions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      546 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_set_functions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      602 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_sorting_functions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      676 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_validation.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.280967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/
--rw-r--r--   0 robertc   (1000) robertc   (1000)      432 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7447 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/_inspect.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    14069 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/_pep440.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3607 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/py3k.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      335 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/setup.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.280967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/tests/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      476 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/tests/test_compat.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4528 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/conftest.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.290967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5750 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   208966 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_add_newdocs.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    12081 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_add_newdocs_scalars.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4008 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_asarray.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    10495 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_dtype.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3673 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_dtype_ctypes.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     8615 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_exceptions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    28195 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_internal.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    11618 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_machar.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    11068 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_methods.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2855 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_string_helpers.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7534 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_type_aliases.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    13946 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_ufunc_config.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    62717 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/arrayprint.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      347 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/cversions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    73025 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/defchararray.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    51869 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/einsumfunc.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   125221 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/fromnumeric.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    19283 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/function_base.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7405 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/generate_numpy_api.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    24889 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/getlimits.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    11688 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/memmap.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    55987 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/multiarray.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    77644 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/numeric.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    17239 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/numerictypes.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     8306 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/overrides.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    37545 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/records.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    52357 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/setup.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    19519 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/setup_common.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    30487 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/shape_base.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.314300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2206 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/_locales.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.260967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/examples/
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.314300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/examples/cython/
--rw-r--r--   0 robertc   (1000) robertc   (1000)      496 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/examples/cython/setup.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.314300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/examples/limited_api/
--rw-r--r--   0 robertc   (1000) robertc   (1000)      435 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/examples/limited_api/setup.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2846 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test__exceptions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2220 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_abc.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    22434 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_api.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1977 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_argparse.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    32269 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_array_coercion.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7596 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_array_interface.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3570 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_arraymethod.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    37163 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_arrayprint.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5063 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_casting_floatingpoint_errors.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    34298 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_casting_unittests.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6559 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_conversion_utils.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1521 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_cpu_dispatcher.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7169 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_cpu_features.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7677 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_custom_dtypes.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3623 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_cython.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   115179 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_datetime.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    24607 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_defchararray.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    45494 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_deprecations.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3503 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_dlpack.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    72563 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_dtype.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    50176 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_einsum.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2219 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_errstate.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5643 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_extint128.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    14411 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_function_base.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5306 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_getlimits.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    24226 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_half.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1011 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_hashtable.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5130 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_indexerrors.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    54317 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_indexing.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3579 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_item_selection.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1172 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_limited_api.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    13042 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_longdouble.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1067 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_machar.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    29089 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_mem_overlap.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    15948 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_mem_policy.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7483 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_memmap.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   370512 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_multiarray.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   129553 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_nditer.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6460 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_nep50_promotions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   137666 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_numeric.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    21260 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_numerictypes.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    22084 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_overrides.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6737 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_print.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1168 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_protocols.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    20269 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_records.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    91243 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_regression.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6115 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalar_ctors.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7872 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalar_methods.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5588 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarbuffer.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2378 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarinherit.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    42813 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarmath.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    18694 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarprint.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    29661 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_shape_base.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    43624 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_simd.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3805 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_simd_module.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3835 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_strings.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   116424 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_ufunc.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   172489 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_umath.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3897 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_umath_accuracy.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    23243 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_umath_complex.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    12647 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_unicode.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2040 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/umath.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      389 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/umath_tests.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    17460 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ctypeslib.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.320967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5143 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/__config__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2074 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2613 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/_shell_utils.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      962 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/armccompiler.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    28126 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/ccompiler.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   100034 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/ccompiler_opt.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.324300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1032 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3718 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/autodist.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      709 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/bdist_rpm.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2613 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    19235 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_clib.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    32243 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_ext.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1144 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_py.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1665 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_scripts.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    31172 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_src.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    20670 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/config.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4369 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/config_compiler.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      575 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/develop.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      921 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/egg_info.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3078 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1399 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install_clib.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      848 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install_data.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      919 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install_headers.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      733 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/sdist.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     9536 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/conv_template.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     8173 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/core.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    22639 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/cpuinfo.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    10283 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/exec_command.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3568 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/extension.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.330967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/
--rw-r--r--   0 robertc   (1000) robertc   (1000)    40535 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5499 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/absoft.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2090 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/arm.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3903 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/compaq.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3080 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/environment.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1333 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/fujitsu.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1330 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/g95.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    20502 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/gnu.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1353 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/hpux.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3539 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/ibm.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6570 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/intel.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1327 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/lahey.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1714 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/mips.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2777 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/nag.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      758 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/none.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1560 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/nv.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1061 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/pathf95.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3568 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/pg.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1577 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/sun.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1667 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/vast.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7913 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/from_template.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4234 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/intelccompiler.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3630 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/lib2def.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2032 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/line_endings.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2879 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/log.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    22076 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/mingw32ccompiler.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    89369 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/misc_util.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2192 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/msvc9compiler.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2647 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/msvccompiler.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    12972 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/npy_pkg_config.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      634 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/numpy_distribution.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      713 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/pathccompiler.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      634 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/setup.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   111028 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/system_info.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.334300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2769 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_build_ext.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    28763 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_ccompiler_opt.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6347 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_ccompiler_opt_conf.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7395 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_exec_command.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1277 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2136 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler_gnu.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1058 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler_intel.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1102 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler_nagfor.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1103 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_from_template.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      868 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_log.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1609 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_mingw32ccompiler.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3218 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_misc_util.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2557 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_npy_pkg_config.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2114 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_shell_utils.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    11009 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_system_info.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5426 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/unixccompiler.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.334300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/doc/
--rw-r--r--   0 robertc   (1000) robertc   (1000)      508 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/doc/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     9155 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/doc/constants.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5357 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/doc/ufuncs.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2214 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/dual.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.340967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5227 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      130 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/__main__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)       34 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/__version__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    22703 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/auxfuncs.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    33017 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/capi_maps.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    25039 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/cb_rules.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    51359 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/cfuncs.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5089 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/common_rules.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   138893 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/crackfortran.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5230 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/diagnose.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    24626 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/f2py2e.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     9436 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/f90mod_rules.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     9454 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/func2subr.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    62755 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/rules.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2335 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/setup.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    53004 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/symbolic.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.344300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      832 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_abstract_interface.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    24049 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_array_from_pyobj.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1466 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_assumed_shape.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      564 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_block_docstring.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6152 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_callback.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    19756 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_character.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      584 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_common.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4186 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_compile_function.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    10650 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_crackfortran.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1662 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_docs.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      391 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_f2cmap.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    20848 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_f2py2e.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      847 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_kind.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      848 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_mixed.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      863 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_module_doc.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3941 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_parameter.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      454 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_quoted_character.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2157 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_regression.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1493 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_character.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2397 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_complex.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1850 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_integer.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2017 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_logical.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3353 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_real.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1635 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_semicolon_split.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1164 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_size.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2962 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_string.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    18341 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_symbolic.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      323 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_value_attrspec.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    10445 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/util.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3587 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/use_rules.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.347633 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     8175 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    52897 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/_pocketfft.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6154 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/helper.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      728 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/setup.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.347633 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/tests/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6148 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/tests/test_helper.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    12895 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/tests/test_pocketfft.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.354300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2253 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    22643 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/_datasource.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    30873 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/_iotools.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4855 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/_version.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    31362 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/arraypad.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    33655 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/arraysetops.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7063 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/arrayterator.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    34211 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/format.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   185141 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/function_base.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    37698 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/histograms.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    30944 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/index_tricks.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7052 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/mixins.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    65556 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/nanfunctions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    97431 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/npyio.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    44143 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/polynomial.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    56247 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/recfunctions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    15037 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/scimath.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      405 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/setup.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    39267 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/shape_base.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    17911 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/stride_tricks.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.360967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    10571 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test__datasource.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    13743 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test__iotools.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1999 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test__version.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    54259 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_arraypad.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    35912 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_arraysetops.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1291 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_arrayterator.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      247 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_financial_expired.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    40857 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_format.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   149343 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_function_base.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    32452 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_histograms.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    20256 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_index_tricks.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   106783 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_io.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    38314 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_loadtxt.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7030 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_mixins.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    46590 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_nanfunctions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    17546 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_packbits.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    11395 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_polynomial.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    41565 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_recfunctions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     8257 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_regression.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    26757 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_shape_base.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    22849 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_stride_tricks.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    18951 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_twodim_base.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    15119 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_type_check.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3278 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_ufunclike.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4636 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_utils.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    31355 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/twodim_base.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    19931 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/type_check.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     8031 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/ufunclike.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7721 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/user_array.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    36147 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/utils.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.360967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1813 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    89351 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/linalg.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3316 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/setup.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.364300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      640 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/test_deprecations.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    77576 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/test_linalg.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5597 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/test_regression.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.364300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1404 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4859 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/bench.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   271881 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/core.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    61910 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/extras.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    27232 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/mrecords.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      418 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/setup.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.364300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   209313 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_core.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2566 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_deprecations.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    72950 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_extras.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    19890 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_mrecords.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    32702 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_old_ma.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3078 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_regression.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    16570 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_subclassing.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    10239 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/testutils.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    15658 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/timer_comparison.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    10465 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matlib.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.367633 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/
--rw-r--r--   0 robertc   (1000) robertc   (1000)      242 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    30667 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/defmatrix.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      426 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/setup.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.367633 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    14982 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_defmatrix.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    11875 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_interaction.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     8932 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_masked_matrix.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2059 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_matrix_linalg.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      554 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_multiarray.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      441 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_numeric.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      927 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_regression.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.367633 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6781 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    38691 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/_polybase.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    62520 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/chebyshev.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    52238 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/hermite.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    52366 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/hermite_e.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    50582 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/laguerre.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    51274 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/legendre.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    48836 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/polynomial.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    23237 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/polyutils.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      373 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/setup.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.370967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    20522 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_chebyshev.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    18331 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_classes.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    18577 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_hermite.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    18911 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_hermite_e.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    17511 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_laguerre.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    18673 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_legendre.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    20529 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_polynomial.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3579 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_polyutils.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    20525 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_printing.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5371 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_symbol.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.370967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7506 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/__init__.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.264300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.370967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cffi/
--rw-r--r--   0 robertc   (1000) robertc   (1000)      880 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cffi/extending.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1829 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cffi/parse.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.370967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cython/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1401 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cython/setup.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.370967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/numba/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1957 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/numba/extending.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2034 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/numba/extending_distributions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2318 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_pickle.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6688 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/setup.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.374300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/__init__.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.374300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/data/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/data/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    16429 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_direct.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3676 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_extending.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)   114760 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_generator_mt19937.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5639 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_generator_mt19937_regressions.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    69969 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_random.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    84892 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_randomstate.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7917 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_randomstate_regression.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5439 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_regression.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3311 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_seed_sequence.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    28183 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_smoke.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1101 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/setup.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.374300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/
--rw-r--r--   0 robertc   (1000) robertc   (1000)      673 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/__init__.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.374300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    11401 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/decorators.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7816 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/extbuild.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    14516 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/noseclasses.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    19435 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/nosetester.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    16156 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/parameterized.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    87918 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/utils.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6180 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/print_coercion_tables.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      709 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/setup.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.374300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/tests/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1347 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/tests/test_doctesting.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    56820 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/tests/test_utils.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1255 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/utils.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.377633 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      221 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test__all__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    12290 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_ctypeslib.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1162 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_lazyloading.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1852 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_matlib.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1575 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_numpy_version.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    16138 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_public_api.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2354 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_reloading.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1645 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_scripts.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2280 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_warnings.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.377633 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5234 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6479 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/mypy_plugin.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      374 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/setup.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.377633 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/__init__.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.264300 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.380967 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7455 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/arithmetic.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2419 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/array_constructors.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      916 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/array_like.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      766 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/arrayprint.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      393 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/arrayterator.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      970 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/bitwise_ops.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2992 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/comparisons.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1073 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/dtype.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1370 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/einsumfunc.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      174 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/flatiter.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3742 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/fromnumeric.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1492 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/index_tricks.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      420 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/lib_utils.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      299 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/lib_version.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1331 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/literal.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1578 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/mod.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      595 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/modules.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1331 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/multiarray.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1626 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ndarray_conversion.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2715 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ndarray_misc.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      640 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ndarray_shape_manipulation.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1490 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/numeric.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      973 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/numerictypes.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    61881 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/random.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3479 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/scalars.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2684 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/simple.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)       96 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/simple_py3.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1120 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ufunc_config.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1039 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ufunclike.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      462 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ufuncs.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      150 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/warnings_and_errors.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7030 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_generic_alias.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      812 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_isfile.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3375 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_runtime.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    15312 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_typing.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      475 2023-02-24 13:11:47.000000 desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/version.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      111 2023-02-24 00:18:55.000000 desmos2python-0.2.7/.git_archival.txt
--rw-r--r--   0 robertc   (1000) robertc   (1000)       31 2023-02-24 00:18:55.000000 desmos2python-0.2.7/.gitattributes
--rw-r--r--   0 robertc   (1000) robertc   (1000)      170 2023-02-24 00:18:55.000000 desmos2python-0.2.7/AUTHORS.rst
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1069 2023-02-24 00:18:55.000000 desmos2python-0.2.7/LICENSE
--rw-r--r--   0 robertc   (1000) robertc   (1000)      747 2023-03-10 23:46:05.000000 desmos2python-0.2.7/MANIFEST.in
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1945 2023-03-10 23:46:05.000000 desmos2python-0.2.7/Makefile
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4000 2023-03-10 23:53:34.390967 desmos2python-0.2.7/PKG-INFO
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2831 2023-03-10 23:46:05.000000 desmos2python-0.2.7/README.md
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1725 2023-03-10 23:53:27.000000 desmos2python-0.2.7/README.rst
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.384300 desmos2python-0.2.7/desmos2python/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2278 2023-03-10 23:46:05.000000 desmos2python-0.2.7/desmos2python/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      908 2023-02-24 00:18:55.000000 desmos2python-0.2.7/desmos2python/_logger.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.384300 desmos2python-0.2.7/desmos2python/_setuptools_ext/
--rw-r--r--   0 robertc   (1000) robertc   (1000)       61 2023-02-24 14:34:27.000000 desmos2python-0.2.7/desmos2python/_setuptools_ext/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2532 2023-03-10 23:46:05.000000 desmos2python-0.2.7/desmos2python/_setuptools_ext/_setuptools_ext.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1050 2023-02-24 14:34:27.000000 desmos2python-0.2.7/desmos2python/api.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     9073 2023-02-24 14:34:27.000000 desmos2python-0.2.7/desmos2python/browser.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      953 2023-02-24 00:18:55.000000 desmos2python-0.2.7/desmos2python/consts.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    25995 2023-03-10 23:46:05.000000 desmos2python-0.2.7/desmos2python/latex.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2827 2023-03-10 23:46:05.000000 desmos2python-0.2.7/desmos2python/pdoc.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1865 2023-02-24 14:34:27.000000 desmos2python-0.2.7/desmos2python/render.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.384300 desmos2python-0.2.7/desmos2python/resources/
--rw-r--r--   0 robertc   (1000) robertc   (1000)      536 2023-03-10 23:46:05.000000 desmos2python-0.2.7/desmos2python/resources/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1065 2023-02-24 14:34:27.000000 desmos2python-0.2.7/desmos2python/resources/greek_alphabet.json
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5768 2023-03-10 23:46:05.000000 desmos2python-0.2.7/desmos2python/resources/greek_chars.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.387633 desmos2python-0.2.7/desmos2python/resources/javascript/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 00:18:55.000000 desmos2python-0.2.7/desmos2python/resources/javascript/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      791 2023-02-24 00:18:55.000000 desmos2python-0.2.7/desmos2python/resources/javascript/get_latex_desmos.js
--rw-r--r--   0 robertc   (1000) robertc   (1000)       86 2023-02-24 14:34:27.000000 desmos2python-0.2.7/desmos2python/resources/javascript/get_svg.js
--rw-r--r--   0 robertc   (1000) robertc   (1000)       69 2023-02-24 14:34:27.000000 desmos2python-0.2.7/desmos2python/resources/javascript/take_svg_screenshot.js
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.387633 desmos2python-0.2.7/desmos2python/resources/latex_json/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 00:18:55.000000 desmos2python-0.2.7/desmos2python/resources/latex_json/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      182 2023-02-24 00:18:55.000000 desmos2python-0.2.7/desmos2python/resources/latex_json/ex.json
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.387633 desmos2python-0.2.7/desmos2python/resources/screenshots/
--rw-r--r--   0 robertc   (1000) robertc   (1000)   519667 2023-02-24 14:34:27.000000 desmos2python-0.2.7/desmos2python/resources/screenshots/ex.svg
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.387633 desmos2python-0.2.7/desmos2python/resources/templates/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 00:18:55.000000 desmos2python-0.2.7/desmos2python/resources/templates/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2422 2023-02-24 14:34:27.000000 desmos2python-0.2.7/desmos2python/resources/templates/desmos_mock_graph.html.jinja2
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1559 2023-02-24 14:34:27.000000 desmos2python-0.2.7/desmos2python/resources/templates/desmos_model_ns.jinja2
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3492 2023-02-24 14:34:27.000000 desmos2python-0.2.7/desmos2python/svg.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1038 2023-03-10 23:46:05.000000 desmos2python-0.2.7/desmos2python/utils.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.384300 desmos2python-0.2.7/desmos2python.egg-info/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4000 2023-03-10 23:53:34.000000 desmos2python-0.2.7/desmos2python.egg-info/PKG-INFO
--rw-r--r--   0 robertc   (1000) robertc   (1000)    38084 2023-03-10 23:53:34.000000 desmos2python-0.2.7/desmos2python.egg-info/SOURCES.txt
--rw-r--r--   0 robertc   (1000) robertc   (1000)        1 2023-03-10 23:53:34.000000 desmos2python-0.2.7/desmos2python.egg-info/dependency_links.txt
--rw-r--r--   0 robertc   (1000) robertc   (1000)       91 2023-03-10 23:53:34.000000 desmos2python-0.2.7/desmos2python.egg-info/entry_points.txt
--rw-r--r--   0 robertc   (1000) robertc   (1000)        1 2023-03-10 23:53:28.000000 desmos2python-0.2.7/desmos2python.egg-info/not-zip-safe
--rw-r--r--   0 robertc   (1000) robertc   (1000)      326 2023-03-10 23:53:34.000000 desmos2python-0.2.7/desmos2python.egg-info/requires.txt
--rw-r--r--   0 robertc   (1000) robertc   (1000)       14 2023-03-10 23:53:34.000000 desmos2python-0.2.7/desmos2python.egg-info/top_level.txt
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.387633 desmos2python-0.2.7/doc-source/
--rw-r--r--   0 robertc   (1000) robertc   (1000)      215 2023-02-24 00:18:55.000000 desmos2python-0.2.7/doc-source/404.rst
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1358 2023-03-10 23:46:05.000000 desmos2python-0.2.7/doc-source/Source.rst
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.390967 desmos2python-0.2.7/doc-source/_static/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 00:18:55.000000 desmos2python-0.2.7/doc-source/_static/style.css
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.390967 desmos2python-0.2.7/doc-source/_templates/
--rw-r--r--   0 robertc   (1000) robertc   (1000)      228 2023-02-24 00:18:55.000000 desmos2python-0.2.7/doc-source/_templates/layout.html
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.390967 desmos2python-0.2.7/doc-source/api/
--rw-r--r--   0 robertc   (1000) robertc   (1000)       75 2023-02-24 00:18:55.000000 desmos2python-0.2.7/doc-source/api/desmos2python.rst
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1982 2023-02-24 00:18:55.000000 desmos2python-0.2.7/doc-source/conf.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      672 2023-03-10 23:46:05.000000 desmos2python-0.2.7/doc-source/contributing.rst
--rw-r--r--   0 robertc   (1000) robertc   (1000)       40 2023-02-24 00:18:55.000000 desmos2python-0.2.7/doc-source/docutils.conf
--rw-r--r--   0 robertc   (1000) robertc   (1000)    26814 2023-02-24 00:18:55.000000 desmos2python-0.2.7/doc-source/git_download.png
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3060 2023-02-24 00:18:55.000000 desmos2python-0.2.7/doc-source/index.rst
--rw-r--r--   0 robertc   (1000) robertc   (1000)      148 2023-02-24 00:18:55.000000 desmos2python-0.2.7/doc-source/license.rst
--rw-r--r--   0 robertc   (1000) robertc   (1000)    47775 2023-02-24 00:18:55.000000 desmos2python-0.2.7/doc-source/not-found.png
--rw-r--r--   0 robertc   (1000) robertc   (1000)      365 2023-02-24 00:18:55.000000 desmos2python-0.2.7/doc-source/requirements.txt
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.390967 desmos2python-0.2.7/docs/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 00:18:55.000000 desmos2python-0.2.7/docs/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      351 2023-03-10 23:46:05.000000 desmos2python-0.2.7/environment.yml
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1428 2023-02-24 14:34:27.000000 desmos2python-0.2.7/fix_readme.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      106 2023-02-24 00:18:55.000000 desmos2python-0.2.7/oryx-build-commands.txt
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4744 2023-03-10 23:46:05.000000 desmos2python-0.2.7/pyproject.toml
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.390967 desmos2python-0.2.7/requirements/
--rw-r--r--   0 robertc   (1000) robertc   (1000)       79 2023-03-10 23:46:05.000000 desmos2python-0.2.7/requirements/build-requirements.txt
--rw-r--r--   0 robertc   (1000) robertc   (1000)       85 2023-03-10 23:46:05.000000 desmos2python-0.2.7/requirements/dev-requirements.txt
--rw-r--r--   0 robertc   (1000) robertc   (1000)      159 2023-03-10 23:46:05.000000 desmos2python-0.2.7/requirements/requirements.txt
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1098 2023-03-10 23:53:34.390967 desmos2python-0.2.7/setup.cfg
--rw-r--r--   0 robertc   (1000) robertc   (1000)      688 2023-03-10 23:46:05.000000 desmos2python-0.2.7/setup.py
-drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-03-10 23:53:34.390967 desmos2python-0.2.7/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 00:18:55.000000 desmos2python-0.2.7/tests/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    11061 2023-02-24 00:18:55.000000 desmos2python-0.2.7/tests/ex.png
--rw-r--r--   0 robertc   (1000) robertc   (1000)    11061 2023-02-24 00:18:55.000000 desmos2python-0.2.7/tests/expected_ex.png
--rw-r--r--   0 robertc   (1000) robertc   (1000)      165 2023-02-24 00:18:55.000000 desmos2python-0.2.7/tests/requirements.txt
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2016 2023-02-24 14:34:27.000000 desmos2python-0.2.7/tests/run_tests.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.220634 desmos2python-0.2.8/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)       38 2023-02-24 00:18:55.000000 desmos2python-0.2.8/.bumpversion.cfg
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.147300 desmos2python-0.2.8/.eggs/
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.147300 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.153967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5143 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/__config__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    16174 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      331 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_distributor_init.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3885 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_globals.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.153967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1422 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/hook-numpy.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1143 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/pyinstaller-smoke.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1135 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/test_pyinstaller.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6668 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pytesttester.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.157300 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7108 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3925 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_add_docstring.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4391 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_array_like.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5916 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_char_codes.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5628 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_dtype_like.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1111 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_extended_precision.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7479 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_generic_alias.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      345 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_nbit.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2701 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_nested_sequence.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      957 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_scalars.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      191 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_shape.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      337 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/setup.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      498 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_version.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.157300 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    10221 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    43226 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_array_object.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)       66 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_constants.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    10050 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_creation_functions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4480 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_data_type_functions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3707 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_dtypes.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    24772 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_elementwise_functions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3008 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_manipulation_functions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1457 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_searching_functions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2948 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_set_functions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1754 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_sorting_functions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3378 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_statistical_functions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1376 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_typing.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      824 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_utility_functions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    17860 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/linalg.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      341 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/setup.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.160634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      282 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    15771 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_array_object.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5023 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_creation_functions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      422 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_data_type_functions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3619 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_elementwise_functions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      546 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_set_functions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      602 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_sorting_functions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      676 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_validation.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.160634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      432 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7447 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/_inspect.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    14069 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/_pep440.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3607 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/py3k.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      335 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/setup.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.160634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/tests/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      476 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/tests/test_compat.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4528 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/conftest.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.163967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5750 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   208966 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_add_newdocs.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    12081 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_add_newdocs_scalars.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4008 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_asarray.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    10495 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_dtype.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3673 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_dtype_ctypes.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     8615 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_exceptions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    28195 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_internal.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    11618 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_machar.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    11068 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_methods.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2855 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_string_helpers.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7534 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_type_aliases.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    13946 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_ufunc_config.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    62717 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/arrayprint.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      347 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/cversions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    73025 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/defchararray.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    51869 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/einsumfunc.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   125221 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/fromnumeric.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    19283 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/function_base.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7405 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/generate_numpy_api.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    24889 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/getlimits.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    11688 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/memmap.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    55987 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/multiarray.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    77644 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/numeric.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    17239 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/numerictypes.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     8306 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/overrides.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    37545 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/records.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    52357 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/setup.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    19519 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/setup_common.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    30487 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/shape_base.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.173967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2206 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/_locales.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.147300 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/examples/
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.173967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/examples/cython/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      496 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/examples/cython/setup.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.173967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/examples/limited_api/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      435 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/examples/limited_api/setup.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2846 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test__exceptions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2220 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_abc.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    22434 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_api.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1977 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_argparse.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    32269 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_array_coercion.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7596 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_array_interface.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3570 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_arraymethod.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    37163 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_arrayprint.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5063 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_casting_floatingpoint_errors.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    34298 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_casting_unittests.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6559 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_conversion_utils.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1521 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_cpu_dispatcher.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7169 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_cpu_features.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7677 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_custom_dtypes.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3623 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_cython.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   115179 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_datetime.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    24607 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_defchararray.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    45494 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_deprecations.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3503 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_dlpack.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    72563 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_dtype.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    50176 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_einsum.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2219 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_errstate.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5643 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_extint128.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    14411 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_function_base.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5306 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_getlimits.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    24226 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_half.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1011 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_hashtable.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5130 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_indexerrors.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    54317 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_indexing.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3579 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_item_selection.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1172 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_limited_api.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    13042 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_longdouble.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1067 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_machar.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    29089 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_mem_overlap.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    15948 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_mem_policy.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7483 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_memmap.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   370512 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_multiarray.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   129553 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_nditer.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6460 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_nep50_promotions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   137666 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_numeric.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    21260 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_numerictypes.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    22084 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_overrides.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6737 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_print.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1168 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_protocols.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    20269 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_records.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    91243 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_regression.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6115 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalar_ctors.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7872 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalar_methods.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5588 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarbuffer.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2378 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarinherit.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    42813 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarmath.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    18694 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarprint.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    29661 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_shape_base.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    43624 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_simd.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3805 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_simd_module.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3835 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_strings.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   116424 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_ufunc.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   172489 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_umath.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3897 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_umath_accuracy.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    23243 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_umath_complex.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    12647 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_unicode.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2040 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/umath.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      389 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/umath_tests.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    17460 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ctypeslib.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.177300 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5143 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/__config__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2074 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2613 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/_shell_utils.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      962 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/armccompiler.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    28126 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/ccompiler.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   100034 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/ccompiler_opt.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.177300 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1032 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3718 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/autodist.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      709 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/bdist_rpm.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2613 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    19235 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_clib.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    32243 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_ext.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1144 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_py.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1665 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_scripts.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    31172 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_src.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    20670 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/config.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4369 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/config_compiler.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      575 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/develop.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      921 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/egg_info.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3078 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1399 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install_clib.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      848 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install_data.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      919 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install_headers.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      733 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/sdist.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     9536 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/conv_template.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     8173 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/core.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    22639 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/cpuinfo.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    10283 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/exec_command.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3568 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/extension.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.180634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    40535 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5499 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/absoft.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2090 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/arm.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3903 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/compaq.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3080 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/environment.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1333 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/fujitsu.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1330 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/g95.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    20502 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/gnu.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1353 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/hpux.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3539 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/ibm.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6570 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/intel.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1327 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/lahey.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1714 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/mips.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2777 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/nag.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      758 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/none.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1560 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/nv.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1061 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/pathf95.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3568 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/pg.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1577 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/sun.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1667 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/vast.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7913 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/from_template.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4234 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/intelccompiler.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3630 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/lib2def.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2032 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/line_endings.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2879 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/log.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    22076 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/mingw32ccompiler.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    89369 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/misc_util.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2192 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/msvc9compiler.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2647 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/msvccompiler.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    12972 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/npy_pkg_config.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      634 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/numpy_distribution.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      713 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/pathccompiler.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      634 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/setup.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   111028 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/system_info.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.183967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2769 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_build_ext.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    28763 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_ccompiler_opt.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6347 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_ccompiler_opt_conf.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7395 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_exec_command.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1277 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2136 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler_gnu.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1058 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler_intel.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1102 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler_nagfor.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1103 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_from_template.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      868 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_log.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1609 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_mingw32ccompiler.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3218 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_misc_util.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2557 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_npy_pkg_config.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2114 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_shell_utils.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    11009 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_system_info.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5426 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/unixccompiler.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.183967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/doc/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      508 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/doc/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     9155 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/doc/constants.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5357 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/doc/ufuncs.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2214 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/dual.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.183967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5227 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      130 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/__main__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)       34 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/__version__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    22703 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/auxfuncs.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    33017 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/capi_maps.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    25039 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/cb_rules.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    51359 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/cfuncs.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5089 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/common_rules.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   138893 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/crackfortran.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5230 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/diagnose.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    24626 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/f2py2e.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     9436 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/f90mod_rules.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     9454 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/func2subr.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    62755 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/rules.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2335 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/setup.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    53004 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/symbolic.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.190634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      832 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_abstract_interface.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    24049 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_array_from_pyobj.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1466 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_assumed_shape.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      564 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_block_docstring.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6152 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_callback.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    19756 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_character.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      584 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_common.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4186 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_compile_function.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    10650 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_crackfortran.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1662 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_docs.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      391 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_f2cmap.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    20848 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_f2py2e.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      847 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_kind.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      848 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_mixed.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      863 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_module_doc.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3941 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_parameter.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      454 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_quoted_character.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2157 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_regression.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1493 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_character.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2397 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_complex.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1850 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_integer.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2017 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_logical.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3353 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_real.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1635 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_semicolon_split.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1164 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_size.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2962 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_string.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    18341 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_symbolic.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      323 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_value_attrspec.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    10445 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/util.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3587 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/use_rules.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.190634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     8175 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    52897 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/_pocketfft.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6154 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/helper.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      728 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/setup.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.190634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/tests/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6148 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/tests/test_helper.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    12895 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/tests/test_pocketfft.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.193967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2253 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    22643 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/_datasource.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    30873 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/_iotools.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4855 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/_version.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    31362 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/arraypad.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    33655 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/arraysetops.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7063 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/arrayterator.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    34211 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/format.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   185141 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/function_base.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    37698 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/histograms.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    30944 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/index_tricks.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7052 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/mixins.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    65556 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/nanfunctions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    97431 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/npyio.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    44143 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/polynomial.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    56247 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/recfunctions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    15037 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/scimath.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      405 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/setup.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    39267 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/shape_base.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    17911 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/stride_tricks.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.197300 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    10571 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test__datasource.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    13743 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test__iotools.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1999 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test__version.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    54259 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_arraypad.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    35912 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_arraysetops.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1291 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_arrayterator.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      247 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_financial_expired.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    40857 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_format.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   149343 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_function_base.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    32452 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_histograms.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    20256 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_index_tricks.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   106783 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_io.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    38314 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_loadtxt.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7030 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_mixins.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    46590 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_nanfunctions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    17546 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_packbits.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    11395 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_polynomial.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    41565 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_recfunctions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     8257 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_regression.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    26757 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_shape_base.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    22849 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_stride_tricks.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    18951 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_twodim_base.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    15119 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_type_check.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3278 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_ufunclike.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4636 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_utils.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    31355 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/twodim_base.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    19931 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/type_check.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     8031 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/ufunclike.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7721 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/user_array.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    36147 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/utils.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.197300 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1813 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    89351 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/linalg.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3316 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/setup.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.197300 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      640 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/test_deprecations.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    77576 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/test_linalg.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5597 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/test_regression.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.200634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1404 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4859 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/bench.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   271881 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/core.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    61910 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/extras.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    27232 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/mrecords.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      418 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/setup.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.200634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   209313 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_core.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2566 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_deprecations.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    72950 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_extras.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    19890 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_mrecords.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    32702 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_old_ma.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3078 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_regression.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    16570 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_subclassing.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    10239 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/testutils.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    15658 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/timer_comparison.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    10465 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matlib.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.200634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      242 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    30667 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/defmatrix.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      426 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/setup.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.200634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    14982 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_defmatrix.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    11875 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_interaction.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     8932 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_masked_matrix.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2059 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_matrix_linalg.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      554 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_multiarray.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      441 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_numeric.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      927 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_regression.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.203967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6781 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    38691 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/_polybase.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    62520 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/chebyshev.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    52238 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/hermite.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    52366 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/hermite_e.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    50582 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/laguerre.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    51274 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/legendre.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    48836 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/polynomial.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    23237 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/polyutils.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      373 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/setup.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.203967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    20522 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_chebyshev.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    18331 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_classes.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    18577 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_hermite.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    18911 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_hermite_e.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    17511 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_laguerre.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    18673 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_legendre.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    20529 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_polynomial.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3579 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_polyutils.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    20525 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_printing.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5371 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_symbol.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.203967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7506 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/__init__.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.150634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.203967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cffi/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      880 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cffi/extending.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1829 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cffi/parse.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.203967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cython/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1401 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cython/setup.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.203967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/numba/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1957 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/numba/extending.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2034 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/numba/extending_distributions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2318 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_pickle.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6688 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/setup.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.207300 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/__init__.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.207300 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/data/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/data/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    16429 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_direct.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3676 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_extending.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   114760 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_generator_mt19937.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5639 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_generator_mt19937_regressions.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    69969 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_random.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    84892 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_randomstate.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7917 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_randomstate_regression.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5439 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_regression.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3311 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_seed_sequence.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    28183 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_smoke.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1101 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/setup.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.207300 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      673 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/__init__.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.207300 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    11401 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/decorators.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7816 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/extbuild.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    14516 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/noseclasses.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    19435 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/nosetester.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    16156 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/parameterized.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    87918 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/utils.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6180 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/print_coercion_tables.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      709 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/setup.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.207300 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/tests/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1347 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/tests/test_doctesting.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    56820 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/tests/test_utils.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1255 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/utils.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.210634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      221 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test__all__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    12290 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_ctypeslib.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1162 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_lazyloading.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1852 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_matlib.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1575 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_numpy_version.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    16138 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_public_api.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2354 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_reloading.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1645 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_scripts.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2280 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_warnings.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.210634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5234 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6479 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/mypy_plugin.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      374 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/setup.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.210634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/__init__.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.150634 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.213967 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7455 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/arithmetic.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2419 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/array_constructors.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      916 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/array_like.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      766 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/arrayprint.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      393 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/arrayterator.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      970 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/bitwise_ops.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2992 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/comparisons.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1073 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/dtype.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1370 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/einsumfunc.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      174 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/flatiter.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3742 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/fromnumeric.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1492 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/index_tricks.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      420 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/lib_utils.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      299 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/lib_version.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1331 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/literal.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1578 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/mod.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      595 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/modules.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1331 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/multiarray.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1626 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ndarray_conversion.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2715 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ndarray_misc.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      640 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ndarray_shape_manipulation.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1490 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/numeric.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      973 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/numerictypes.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    61881 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/random.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3479 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/scalars.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2684 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/simple.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)       96 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/simple_py3.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1120 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ufunc_config.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1039 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ufunclike.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      462 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ufuncs.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      150 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/warnings_and_errors.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7030 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_generic_alias.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      812 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_isfile.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3375 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_runtime.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    15312 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_typing.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      475 2023-02-24 13:11:47.000000 desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/version.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      111 2023-02-24 00:18:55.000000 desmos2python-0.2.8/.git_archival.txt
+-rw-r--r--   0 robertc   (1000) robertc   (1000)       31 2023-02-24 00:18:55.000000 desmos2python-0.2.8/.gitattributes
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      170 2023-02-24 00:18:55.000000 desmos2python-0.2.8/AUTHORS.rst
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1069 2023-02-24 00:18:55.000000 desmos2python-0.2.8/LICENSE
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      747 2023-03-10 23:46:05.000000 desmos2python-0.2.8/MANIFEST.in
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1945 2023-03-10 23:46:05.000000 desmos2python-0.2.8/Makefile
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4000 2023-04-08 21:30:45.220634 desmos2python-0.2.8/PKG-INFO
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2831 2023-03-10 23:46:05.000000 desmos2python-0.2.8/README.md
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1725 2023-04-08 21:30:38.000000 desmos2python-0.2.8/README.rst
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.217300 desmos2python-0.2.8/desmos2python/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2278 2023-03-10 23:46:05.000000 desmos2python-0.2.8/desmos2python/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      908 2023-02-24 00:18:55.000000 desmos2python-0.2.8/desmos2python/_logger.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.217300 desmos2python-0.2.8/desmos2python/_setuptools_ext/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)       61 2023-02-24 14:34:27.000000 desmos2python-0.2.8/desmos2python/_setuptools_ext/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2546 2023-04-08 21:21:42.000000 desmos2python-0.2.8/desmos2python/_setuptools_ext/_setuptools_ext.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1050 2023-02-24 14:34:27.000000 desmos2python-0.2.8/desmos2python/api.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     9073 2023-02-24 14:34:27.000000 desmos2python-0.2.8/desmos2python/browser.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      953 2023-02-24 00:18:55.000000 desmos2python-0.2.8/desmos2python/consts.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    25995 2023-03-10 23:46:05.000000 desmos2python-0.2.8/desmos2python/latex.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2827 2023-03-10 23:46:05.000000 desmos2python-0.2.8/desmos2python/pdoc.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1865 2023-02-24 14:34:27.000000 desmos2python-0.2.8/desmos2python/render.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.217300 desmos2python-0.2.8/desmos2python/resources/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      536 2023-03-10 23:46:05.000000 desmos2python-0.2.8/desmos2python/resources/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1065 2023-02-24 14:34:27.000000 desmos2python-0.2.8/desmos2python/resources/greek_alphabet.json
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5768 2023-03-10 23:46:05.000000 desmos2python-0.2.8/desmos2python/resources/greek_chars.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.217300 desmos2python-0.2.8/desmos2python/resources/javascript/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 00:18:55.000000 desmos2python-0.2.8/desmos2python/resources/javascript/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      791 2023-02-24 00:18:55.000000 desmos2python-0.2.8/desmos2python/resources/javascript/get_latex_desmos.js
+-rw-r--r--   0 robertc   (1000) robertc   (1000)       86 2023-02-24 14:34:27.000000 desmos2python-0.2.8/desmos2python/resources/javascript/get_svg.js
+-rw-r--r--   0 robertc   (1000) robertc   (1000)       69 2023-02-24 14:34:27.000000 desmos2python-0.2.8/desmos2python/resources/javascript/take_svg_screenshot.js
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.217300 desmos2python-0.2.8/desmos2python/resources/latex_json/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 00:18:55.000000 desmos2python-0.2.8/desmos2python/resources/latex_json/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      182 2023-02-24 00:18:55.000000 desmos2python-0.2.8/desmos2python/resources/latex_json/ex.json
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.217300 desmos2python-0.2.8/desmos2python/resources/screenshots/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)   519667 2023-02-24 14:34:27.000000 desmos2python-0.2.8/desmos2python/resources/screenshots/ex.svg
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.217300 desmos2python-0.2.8/desmos2python/resources/templates/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 00:18:55.000000 desmos2python-0.2.8/desmos2python/resources/templates/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2422 2023-02-24 14:34:27.000000 desmos2python-0.2.8/desmos2python/resources/templates/desmos_mock_graph.html.jinja2
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1559 2023-02-24 14:34:27.000000 desmos2python-0.2.8/desmos2python/resources/templates/desmos_model_ns.jinja2
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3492 2023-02-24 14:34:27.000000 desmos2python-0.2.8/desmos2python/svg.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1038 2023-03-10 23:46:05.000000 desmos2python-0.2.8/desmos2python/utils.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.217300 desmos2python-0.2.8/desmos2python.egg-info/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4000 2023-04-08 21:30:44.000000 desmos2python-0.2.8/desmos2python.egg-info/PKG-INFO
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    38084 2023-04-08 21:30:45.000000 desmos2python-0.2.8/desmos2python.egg-info/SOURCES.txt
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        1 2023-04-08 21:30:44.000000 desmos2python-0.2.8/desmos2python.egg-info/dependency_links.txt
+-rw-r--r--   0 robertc   (1000) robertc   (1000)       91 2023-04-08 21:30:44.000000 desmos2python-0.2.8/desmos2python.egg-info/entry_points.txt
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        1 2023-04-08 21:30:39.000000 desmos2python-0.2.8/desmos2python.egg-info/not-zip-safe
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      326 2023-04-08 21:30:44.000000 desmos2python-0.2.8/desmos2python.egg-info/requires.txt
+-rw-r--r--   0 robertc   (1000) robertc   (1000)       14 2023-04-08 21:30:44.000000 desmos2python-0.2.8/desmos2python.egg-info/top_level.txt
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.220634 desmos2python-0.2.8/doc-source/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      215 2023-02-24 00:18:55.000000 desmos2python-0.2.8/doc-source/404.rst
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1358 2023-03-10 23:46:05.000000 desmos2python-0.2.8/doc-source/Source.rst
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.220634 desmos2python-0.2.8/doc-source/_static/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 00:18:55.000000 desmos2python-0.2.8/doc-source/_static/style.css
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.220634 desmos2python-0.2.8/doc-source/_templates/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      228 2023-02-24 00:18:55.000000 desmos2python-0.2.8/doc-source/_templates/layout.html
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.220634 desmos2python-0.2.8/doc-source/api/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)       75 2023-02-24 00:18:55.000000 desmos2python-0.2.8/doc-source/api/desmos2python.rst
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1982 2023-02-24 00:18:55.000000 desmos2python-0.2.8/doc-source/conf.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      672 2023-03-10 23:46:05.000000 desmos2python-0.2.8/doc-source/contributing.rst
+-rw-r--r--   0 robertc   (1000) robertc   (1000)       40 2023-02-24 00:18:55.000000 desmos2python-0.2.8/doc-source/docutils.conf
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    26814 2023-02-24 00:18:55.000000 desmos2python-0.2.8/doc-source/git_download.png
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3060 2023-02-24 00:18:55.000000 desmos2python-0.2.8/doc-source/index.rst
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      148 2023-02-24 00:18:55.000000 desmos2python-0.2.8/doc-source/license.rst
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    47775 2023-02-24 00:18:55.000000 desmos2python-0.2.8/doc-source/not-found.png
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      365 2023-02-24 00:18:55.000000 desmos2python-0.2.8/doc-source/requirements.txt
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.220634 desmos2python-0.2.8/docs/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 00:18:55.000000 desmos2python-0.2.8/docs/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      351 2023-03-10 23:46:05.000000 desmos2python-0.2.8/environment.yml
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1428 2023-02-24 14:34:27.000000 desmos2python-0.2.8/fix_readme.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      106 2023-02-24 00:18:55.000000 desmos2python-0.2.8/oryx-build-commands.txt
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4744 2023-03-10 23:46:05.000000 desmos2python-0.2.8/pyproject.toml
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.220634 desmos2python-0.2.8/requirements/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)       79 2023-03-10 23:46:05.000000 desmos2python-0.2.8/requirements/build-requirements.txt
+-rw-r--r--   0 robertc   (1000) robertc   (1000)       85 2023-03-10 23:46:05.000000 desmos2python-0.2.8/requirements/dev-requirements.txt
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      159 2023-03-10 23:46:05.000000 desmos2python-0.2.8/requirements/requirements.txt
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1098 2023-04-08 21:30:45.220634 desmos2python-0.2.8/setup.cfg
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      724 2023-04-08 21:23:14.000000 desmos2python-0.2.8/setup.py
+drwxr-xr-x   0 robertc   (1000) robertc   (1000)        0 2023-04-08 21:30:45.220634 desmos2python-0.2.8/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)        0 2023-02-24 00:18:55.000000 desmos2python-0.2.8/tests/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    11061 2023-02-24 00:18:55.000000 desmos2python-0.2.8/tests/ex.png
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    11061 2023-02-24 00:18:55.000000 desmos2python-0.2.8/tests/expected_ex.png
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      165 2023-02-24 00:18:55.000000 desmos2python-0.2.8/tests/requirements.txt
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2016 2023-02-24 14:34:27.000000 desmos2python-0.2.8/tests/run_tests.py
```

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/__config__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/__config__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_globals.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_globals.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/hook-numpy.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/hook-numpy.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/pyinstaller-smoke.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/pyinstaller-smoke.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/test_pyinstaller.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pyinstaller/test_pyinstaller.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pytesttester.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_pytesttester.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_add_docstring.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_add_docstring.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_array_like.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_array_like.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_char_codes.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_char_codes.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_dtype_like.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_dtype_like.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_extended_precision.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_extended_precision.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_generic_alias.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_generic_alias.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_nested_sequence.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_nested_sequence.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_scalars.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/_typing/_scalars.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_array_object.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_array_object.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_creation_functions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_creation_functions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_data_type_functions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_data_type_functions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_dtypes.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_dtypes.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_elementwise_functions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_elementwise_functions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_manipulation_functions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_manipulation_functions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_searching_functions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_searching_functions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_set_functions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_set_functions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_sorting_functions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_sorting_functions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_statistical_functions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_statistical_functions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_typing.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_typing.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_utility_functions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/_utility_functions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/linalg.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/linalg.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_array_object.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_array_object.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_creation_functions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_creation_functions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_elementwise_functions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_elementwise_functions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_set_functions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_set_functions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_sorting_functions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_sorting_functions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_validation.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/array_api/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/_inspect.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/_inspect.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/_pep440.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/_pep440.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/py3k.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/compat/py3k.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/conftest.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/conftest.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_add_newdocs.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_add_newdocs.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_add_newdocs_scalars.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_add_newdocs_scalars.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_asarray.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_asarray.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_dtype.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_dtype.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_dtype_ctypes.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_dtype_ctypes.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_exceptions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_exceptions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_internal.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_internal.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_machar.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_machar.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_methods.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_methods.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_string_helpers.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_string_helpers.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_type_aliases.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_type_aliases.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_ufunc_config.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/_ufunc_config.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/arrayprint.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/arrayprint.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/defchararray.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/defchararray.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/einsumfunc.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/einsumfunc.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/fromnumeric.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/fromnumeric.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/function_base.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/function_base.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/generate_numpy_api.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/generate_numpy_api.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/getlimits.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/getlimits.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/memmap.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/memmap.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/multiarray.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/multiarray.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/numeric.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/numeric.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/numerictypes.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/numerictypes.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/overrides.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/overrides.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/records.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/records.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/setup.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/setup.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/setup_common.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/setup_common.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/shape_base.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/shape_base.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/_locales.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/_locales.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test__exceptions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test__exceptions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_abc.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_api.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_argparse.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_argparse.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_array_coercion.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_array_coercion.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_array_interface.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_array_interface.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_arraymethod.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_arraymethod.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_arrayprint.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_arrayprint.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_casting_floatingpoint_errors.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_casting_floatingpoint_errors.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_casting_unittests.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_casting_unittests.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_conversion_utils.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_conversion_utils.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_cpu_dispatcher.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_cpu_dispatcher.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_cpu_features.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_cpu_features.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_custom_dtypes.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_custom_dtypes.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_cython.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_cython.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_datetime.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_defchararray.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_defchararray.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_deprecations.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_dlpack.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_dlpack.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_dtype.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_einsum.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_einsum.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_errstate.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_errstate.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_extint128.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_extint128.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_function_base.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_function_base.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_getlimits.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_getlimits.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_half.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_half.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_hashtable.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_hashtable.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_indexerrors.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_indexerrors.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_indexing.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_item_selection.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_item_selection.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_limited_api.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_limited_api.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_longdouble.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_longdouble.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_machar.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_machar.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_mem_overlap.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_mem_overlap.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_mem_policy.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_mem_policy.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_memmap.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_memmap.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_multiarray.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_multiarray.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_nditer.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_nditer.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_nep50_promotions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_nep50_promotions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_numeric.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_numeric.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_numerictypes.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_numerictypes.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_overrides.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_overrides.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_print.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_print.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_protocols.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_records.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_records.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_regression.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalar_ctors.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalar_ctors.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalar_methods.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalar_methods.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarbuffer.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarbuffer.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarinherit.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarinherit.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarmath.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarmath.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarprint.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_scalarprint.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_shape_base.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_shape_base.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_simd.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_simd.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_simd_module.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_simd_module.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_strings.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_ufunc.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_ufunc.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_umath.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_umath.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_umath_accuracy.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_umath_accuracy.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_umath_complex.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_umath_complex.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_unicode.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/umath.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/core/umath.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ctypeslib.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ctypeslib.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/__config__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/__config__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/_shell_utils.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/_shell_utils.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/armccompiler.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/armccompiler.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/ccompiler.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/ccompiler_opt.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/ccompiler_opt.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/autodist.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/autodist.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/bdist_rpm.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_clib.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_ext.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_py.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_scripts.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_src.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/build_src.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/config.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/config_compiler.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/config_compiler.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/develop.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/develop.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/egg_info.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install_clib.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install_clib.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install_data.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install_headers.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/sdist.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/conv_template.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/conv_template.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/core.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/core.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/cpuinfo.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/exec_command.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/exec_command.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/extension.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/extension.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/absoft.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/absoft.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/arm.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/arm.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/compaq.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/compaq.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/environment.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/environment.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/fujitsu.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/fujitsu.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/g95.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/g95.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/gnu.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/gnu.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/hpux.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/hpux.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/ibm.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/ibm.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/intel.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/intel.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/lahey.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/lahey.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/mips.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/mips.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/nag.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/nag.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/none.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/none.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/nv.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/nv.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/pathf95.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/pathf95.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/pg.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/pg.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/sun.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/sun.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/vast.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/fcompiler/vast.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/from_template.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/from_template.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/intelccompiler.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/intelccompiler.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/lib2def.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/lib2def.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/line_endings.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/line_endings.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/log.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/log.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/mingw32ccompiler.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/mingw32ccompiler.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/misc_util.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/misc_util.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/msvc9compiler.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/msvccompiler.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/npy_pkg_config.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/npy_pkg_config.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/numpy_distribution.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/numpy_distribution.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/pathccompiler.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/pathccompiler.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/setup.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/setup.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/system_info.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/system_info.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_build_ext.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_build_ext.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_ccompiler_opt.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_ccompiler_opt.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_ccompiler_opt_conf.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_ccompiler_opt_conf.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_exec_command.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_exec_command.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler_gnu.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler_gnu.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler_intel.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler_intel.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler_nagfor.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_fcompiler_nagfor.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_from_template.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_from_template.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_log.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_mingw32ccompiler.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_mingw32ccompiler.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_misc_util.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_misc_util.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_npy_pkg_config.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_npy_pkg_config.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_shell_utils.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_shell_utils.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_system_info.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/tests/test_system_info.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/unixccompiler.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/doc/constants.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/doc/constants.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/doc/ufuncs.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/doc/ufuncs.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/dual.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/dual.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/auxfuncs.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/auxfuncs.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/capi_maps.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/capi_maps.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/cb_rules.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/cb_rules.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/cfuncs.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/cfuncs.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/common_rules.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/common_rules.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/crackfortran.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/crackfortran.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/diagnose.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/diagnose.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/f2py2e.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/f2py2e.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/f90mod_rules.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/f90mod_rules.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/func2subr.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/func2subr.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/rules.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/rules.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/setup.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/setup.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/symbolic.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/symbolic.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_abstract_interface.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_abstract_interface.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_array_from_pyobj.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_array_from_pyobj.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_assumed_shape.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_assumed_shape.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_block_docstring.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_block_docstring.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_callback.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_character.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_character.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_common.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_compile_function.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_compile_function.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_crackfortran.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_crackfortran.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_docs.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_f2py2e.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_f2py2e.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_kind.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_kind.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_mixed.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_mixed.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_module_doc.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_module_doc.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_parameter.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_regression.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_character.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_character.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_complex.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_complex.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_integer.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_integer.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_logical.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_logical.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_real.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_return_real.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_semicolon_split.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_semicolon_split.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_size.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_size.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_string.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_symbolic.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/test_symbolic.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/util.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/tests/util.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/use_rules.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/f2py/use_rules.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/_pocketfft.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/_pocketfft.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/helper.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/helper.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/setup.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/setup.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/tests/test_helper.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/tests/test_pocketfft.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/fft/tests/test_pocketfft.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/_datasource.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/_datasource.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/_iotools.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/_iotools.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/_version.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/_version.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/arraypad.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/arraypad.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/arraysetops.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/arraysetops.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/arrayterator.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/arrayterator.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/format.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/format.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/function_base.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/function_base.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/histograms.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/histograms.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/index_tricks.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/index_tricks.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/mixins.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/mixins.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/nanfunctions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/nanfunctions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/npyio.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/npyio.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/polynomial.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/polynomial.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/recfunctions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/recfunctions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/scimath.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/scimath.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/shape_base.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/shape_base.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/stride_tricks.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/stride_tricks.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test__datasource.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test__datasource.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test__iotools.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test__iotools.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test__version.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test__version.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_arraypad.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_arraypad.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_arraysetops.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_arraysetops.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_arrayterator.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_arrayterator.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_format.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_function_base.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_function_base.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_histograms.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_histograms.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_index_tricks.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_index_tricks.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_io.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_loadtxt.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_loadtxt.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_mixins.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_nanfunctions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_nanfunctions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_packbits.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_packbits.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_polynomial.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_polynomial.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_recfunctions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_recfunctions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_regression.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_shape_base.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_shape_base.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_stride_tricks.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_stride_tricks.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_twodim_base.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_twodim_base.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_type_check.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_type_check.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_ufunclike.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_ufunclike.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_utils.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/twodim_base.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/twodim_base.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/type_check.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/type_check.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/ufunclike.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/ufunclike.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/user_array.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/user_array.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/utils.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/lib/utils.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/linalg.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/linalg.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/setup.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/setup.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/test_deprecations.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/test_linalg.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/test_regression.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/linalg/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/bench.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/bench.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/core.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/core.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/extras.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/extras.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/mrecords.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/mrecords.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_core.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_deprecations.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_extras.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_extras.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_mrecords.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_mrecords.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_old_ma.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_old_ma.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_regression.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_subclassing.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/tests/test_subclassing.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/testutils.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/testutils.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/timer_comparison.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/ma/timer_comparison.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matlib.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matlib.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/defmatrix.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/defmatrix.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_defmatrix.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_defmatrix.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_interaction.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_interaction.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_masked_matrix.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_masked_matrix.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_matrix_linalg.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_matrix_linalg.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_multiarray.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_multiarray.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_regression.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/matrixlib/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/_polybase.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/_polybase.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/chebyshev.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/chebyshev.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/hermite.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/hermite.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/hermite_e.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/hermite_e.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/laguerre.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/laguerre.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/legendre.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/legendre.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/polynomial.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/polynomial.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/polyutils.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/polyutils.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_chebyshev.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_chebyshev.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_classes.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_hermite.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_hermite.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_hermite_e.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_hermite_e.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_laguerre.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_laguerre.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_legendre.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_legendre.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_polynomial.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_polynomial.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_polyutils.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_polyutils.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_printing.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_symbol.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/polynomial/tests/test_symbol.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cffi/extending.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cffi/extending.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cffi/parse.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cffi/parse.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cython/setup.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/cython/setup.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/numba/extending.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/numba/extending.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/numba/extending_distributions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_examples/numba/extending_distributions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_pickle.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/_pickle.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/setup.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/setup.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_direct.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_direct.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_extending.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_extending.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_generator_mt19937.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_generator_mt19937.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_generator_mt19937_regressions.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_generator_mt19937_regressions.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_random.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_randomstate.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_randomstate.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_randomstate_regression.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_randomstate_regression.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_regression.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_seed_sequence.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_seed_sequence.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_smoke.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/random/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/setup.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/setup.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/decorators.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/decorators.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/extbuild.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/extbuild.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/noseclasses.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/noseclasses.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/nosetester.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/nosetester.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/parameterized.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/parameterized.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/utils.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/_private/utils.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/print_coercion_tables.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/print_coercion_tables.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/setup.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/setup.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/tests/test_doctesting.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/tests/test_doctesting.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/tests/test_utils.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/utils.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/testing/utils.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_ctypeslib.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_ctypeslib.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_lazyloading.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_lazyloading.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_matlib.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_matlib.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_numpy_version.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_numpy_version.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_public_api.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_public_api.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_reloading.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_reloading.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_scripts.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_warnings.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/__init__.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/mypy_plugin.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/arithmetic.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/arithmetic.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/array_constructors.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/array_constructors.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/array_like.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/array_like.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/arrayprint.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/arrayprint.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/bitwise_ops.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/bitwise_ops.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/comparisons.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/comparisons.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/dtype.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/dtype.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/einsumfunc.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/einsumfunc.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/fromnumeric.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/fromnumeric.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/index_tricks.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/index_tricks.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/literal.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/literal.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/mod.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/mod.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/modules.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/modules.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/multiarray.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/multiarray.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ndarray_conversion.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ndarray_conversion.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ndarray_misc.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ndarray_misc.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ndarray_shape_manipulation.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ndarray_shape_manipulation.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/numeric.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/numeric.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/numerictypes.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/numerictypes.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/random.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/random.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/scalars.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/scalars.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/simple.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/simple.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ufunc_config.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ufunc_config.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ufunclike.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/data/pass/ufunclike.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_generic_alias.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_generic_alias.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_isfile.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_isfile.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_runtime.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_typing.py` & `desmos2python-0.2.8/.eggs/numpy-1.24.2-py3.8-linux-x86_64.egg/numpy/typing/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/LICENSE` & `desmos2python-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/MANIFEST.in` & `desmos2python-0.2.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/Makefile` & `desmos2python-0.2.8/Makefile`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/PKG-INFO` & `desmos2python-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desmos2python
-Version: 0.2.7
+Version: 0.2.8
 Summary: seamless conversion between Desmos LaTeX equations and executable Python code.
 Home-page: https://github.com/rocapp/desmos2python
 Author: Robert Ahlroth Capps
 Author-email: rocapp@gmail.com
 License: MIT License
         
         Copyright (c) 2022 Robbie Capps
```

### Comparing `desmos2python-0.2.7/README.md` & `desmos2python-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/README.rst` & `desmos2python-0.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/__init__.py` & `desmos2python-0.2.8/desmos2python/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/_logger.py` & `desmos2python-0.2.8/desmos2python/_logger.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/_setuptools_ext/_setuptools_ext.py` & `desmos2python-0.2.8/desmos2python/_setuptools_ext/_setuptools_ext.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 """
 import json
 import tempfile
 import datetime
 import importlib
 import distutils.core
 from distutils.cmd import Command
-from setuptools.command.install import install
+from setuptools.command.install import install as _install
 
 __all__ = [
     'init_resources_d2p',
     'd2p_subdirs',
 ]
 
 
 #: sub-directories to be created
 d2p_subdirs = ['calcState_json',
                'latex_json', 'latex_tex',
                'templates', 'models', 'screenshots']
 
 
-class init_resources_d2p(install):
+class init_resources_d2p(_install):
     """custom setuptools command for initializing desmos2python resources.
 
     ref: https://github.com/pypa/setuptools/blob/1c3b501535a856838a077d50989a5c019d2db679/setuptools/_distutils/cmd.py#L17
     ref: https://stackoverflow.com/a/1321345/1871569
     """
     def __init__(self, dist):
         super().__init__(dist)
@@ -57,11 +57,11 @@
 
     def run(self):
         """initialize desmos2python package/user-local resources.
 
         - create the user resources directory if it doesn't exist.
         - symlink package resources to `$HOME/.local/share/desmos2python/` directory.
         """
-        install.run(self)
+        _install.run(self)
         self.D2P_Resources = importlib.import_module('desmos2python.utils').D2P_Resources
         self._init_user_resources()
         self._link_pkg_resources()
```

### Comparing `desmos2python-0.2.7/desmos2python/api.py` & `desmos2python-0.2.8/desmos2python/api.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/browser.py` & `desmos2python-0.2.8/desmos2python/browser.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/consts.py` & `desmos2python-0.2.8/desmos2python/consts.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/latex.py` & `desmos2python-0.2.8/desmos2python/latex.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/pdoc.py` & `desmos2python-0.2.8/desmos2python/pdoc.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/render.py` & `desmos2python-0.2.8/desmos2python/render.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/resources/__init__.py` & `desmos2python-0.2.8/desmos2python/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/resources/greek_alphabet.json` & `desmos2python-0.2.8/desmos2python/resources/greek_alphabet.json`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/resources/greek_chars.py` & `desmos2python-0.2.8/desmos2python/resources/greek_chars.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/resources/javascript/get_latex_desmos.js` & `desmos2python-0.2.8/desmos2python/resources/javascript/get_latex_desmos.js`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/resources/screenshots/ex.svg` & `desmos2python-0.2.8/desmos2python/resources/screenshots/ex.svg`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/resources/templates/desmos_mock_graph.html.jinja2` & `desmos2python-0.2.8/desmos2python/resources/templates/desmos_mock_graph.html.jinja2`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/resources/templates/desmos_model_ns.jinja2` & `desmos2python-0.2.8/desmos2python/resources/templates/desmos_model_ns.jinja2`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/svg.py` & `desmos2python-0.2.8/desmos2python/svg.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python/utils.py` & `desmos2python-0.2.8/desmos2python/utils.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/desmos2python.egg-info/PKG-INFO` & `desmos2python-0.2.8/desmos2python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desmos2python
-Version: 0.2.7
+Version: 0.2.8
 Summary: seamless conversion between Desmos LaTeX equations and executable Python code.
 Home-page: https://github.com/rocapp/desmos2python
 Author: Robert Ahlroth Capps
 Author-email: rocapp@gmail.com
 License: MIT License
         
         Copyright (c) 2022 Robbie Capps
```

### Comparing `desmos2python-0.2.7/desmos2python.egg-info/SOURCES.txt` & `desmos2python-0.2.8/desmos2python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/doc-source/Source.rst` & `desmos2python-0.2.8/doc-source/Source.rst`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/doc-source/conf.py` & `desmos2python-0.2.8/doc-source/conf.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/doc-source/contributing.rst` & `desmos2python-0.2.8/doc-source/contributing.rst`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/doc-source/git_download.png` & `desmos2python-0.2.8/doc-source/git_download.png`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/doc-source/index.rst` & `desmos2python-0.2.8/doc-source/index.rst`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/doc-source/not-found.png` & `desmos2python-0.2.8/doc-source/not-found.png`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/fix_readme.py` & `desmos2python-0.2.8/fix_readme.py`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/pyproject.toml` & `desmos2python-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/setup.cfg` & `desmos2python-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/setup.py` & `desmos2python-0.2.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,20 @@
 logger.setLevel(logging.ERROR)
 init_resources_d2p = \
     importlib \
     .import_module('._setuptools_ext', package='desmos2python') \
     .init_resources_d2p
 logger.setLevel(orig_lvl)
 
+
+class install(init_resources_d2p):
+    pass
+
+
 setup(
     name = "desmos2python",
     cmdclass = {
-        "install": init_resources_d2p,
+        "install": install,
         "init_resources_d2p": init_resources_d2p,
     },
     setup_requires = ['numpy', 'docutils',],
 )
```

### Comparing `desmos2python-0.2.7/tests/ex.png` & `desmos2python-0.2.8/tests/ex.png`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/tests/expected_ex.png` & `desmos2python-0.2.8/tests/expected_ex.png`

 * *Files identical despite different names*

### Comparing `desmos2python-0.2.7/tests/run_tests.py` & `desmos2python-0.2.8/tests/run_tests.py`

 * *Files identical despite different names*

