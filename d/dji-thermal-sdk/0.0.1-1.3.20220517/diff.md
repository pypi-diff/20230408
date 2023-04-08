# Comparing `tmp/dji_thermal_sdk-0.0.1.tar.gz` & `tmp/dji_thermal_sdk-1.3.20220517.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dji_thermal_sdk-0.0.1.tar", last modified: Fri Apr  7 22:27:54 2023, max compression
+gzip compressed data, was "dji_thermal_sdk-1.3.20220517.tar", last modified: Thu Jul  7 22:26:18 2022, max compression
```

## Comparing `dji_thermal_sdk-0.0.1.tar` & `dji_thermal_sdk-1.3.20220517.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 hxl170008  (1001) hxl170008  (1001)        0 2023-04-07 22:27:54.410297 dji_thermal_sdk-0.0.1/
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)    11357 2023-04-06 05:42:18.000000 dji_thermal_sdk-0.0.1/LICENSE
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)      111 2023-01-20 02:50:04.000000 dji_thermal_sdk-0.0.1/MANIFEST.in
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)    13366 2023-04-07 22:27:54.410297 dji_thermal_sdk-0.0.1/PKG-INFO
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)    12510 2023-04-07 22:22:12.000000 dji_thermal_sdk-0.0.1/README.md
-drwxrwxr-x   0 hxl170008  (1001) hxl170008  (1001)        0 2023-04-07 22:27:54.410297 dji_thermal_sdk-0.0.1/dji_thermal_sdk/
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)       22 2023-04-07 22:14:27.000000 dji_thermal_sdk-0.0.1/dji_thermal_sdk/__init__.py
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)    11695 2023-04-07 22:22:09.000000 dji_thermal_sdk-0.0.1/dji_thermal_sdk/_modidx.py
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)    17895 2023-04-07 22:14:27.000000 dji_thermal_sdk-0.0.1/dji_thermal_sdk/dji_sdk.py
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)     6187 2023-04-07 22:14:27.000000 dji_thermal_sdk-0.0.1/dji_thermal_sdk/utility.py
-drwxrwxr-x   0 hxl170008  (1001) hxl170008  (1001)        0 2023-04-07 22:27:54.410297 dji_thermal_sdk-0.0.1/dji_thermal_sdk.egg-info/
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)    13366 2023-04-07 22:27:54.000000 dji_thermal_sdk-0.0.1/dji_thermal_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)      434 2023-04-07 22:27:54.000000 dji_thermal_sdk-0.0.1/dji_thermal_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)        1 2023-04-07 22:27:54.000000 dji_thermal_sdk-0.0.1/dji_thermal_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)       52 2023-04-07 22:27:54.000000 dji_thermal_sdk-0.0.1/dji_thermal_sdk.egg-info/entry_points.txt
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)        1 2023-04-07 20:21:27.000000 dji_thermal_sdk-0.0.1/dji_thermal_sdk.egg-info/not-zip-safe
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)       29 2023-04-07 22:27:54.000000 dji_thermal_sdk-0.0.1/dji_thermal_sdk.egg-info/requires.txt
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)       16 2023-04-07 22:27:54.000000 dji_thermal_sdk-0.0.1/dji_thermal_sdk.egg-info/top_level.txt
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)     1041 2023-04-07 22:13:50.000000 dji_thermal_sdk-0.0.1/settings.ini
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)       38 2023-04-07 22:27:54.410297 dji_thermal_sdk-0.0.1/setup.cfg
--rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)     2560 2023-01-20 02:50:04.000000 dji_thermal_sdk-0.0.1/setup.py
+drwxrwxr-x   0 hxl170008  (1001) hxl170008  (1001)        0 2022-07-07 22:26:18.962633 dji_thermal_sdk-1.3.20220517/
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)     2348 2022-07-07 22:20:41.000000 dji_thermal_sdk-1.3.20220517/CONTRIBUTING.md
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)    11357 2022-07-07 22:20:41.000000 dji_thermal_sdk-1.3.20220517/LICENSE
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)      111 2022-07-07 22:20:41.000000 dji_thermal_sdk-1.3.20220517/MANIFEST.in
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)     8550 2022-07-07 22:26:18.962633 dji_thermal_sdk-1.3.20220517/PKG-INFO
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)     7659 2022-07-07 22:20:41.000000 dji_thermal_sdk-1.3.20220517/README.md
+drwxrwxr-x   0 hxl170008  (1001) hxl170008  (1001)        0 2022-07-07 22:26:18.962633 dji_thermal_sdk-1.3.20220517/dji_thermal_sdk/
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)       29 2022-07-07 22:20:41.000000 dji_thermal_sdk-1.3.20220517/dji_thermal_sdk/__init__.py
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)     4164 2022-07-07 22:20:41.000000 dji_thermal_sdk-1.3.20220517/dji_thermal_sdk/_nbdev.py
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)    17334 2022-07-07 22:20:41.000000 dji_thermal_sdk-1.3.20220517/dji_thermal_sdk/dji_sdk.py
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)     1001 2022-07-07 22:20:41.000000 dji_thermal_sdk-1.3.20220517/dji_thermal_sdk/utility.py
+drwxrwxr-x   0 hxl170008  (1001) hxl170008  (1001)        0 2022-07-07 22:26:18.962633 dji_thermal_sdk-1.3.20220517/dji_thermal_sdk.egg-info/
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)     8550 2022-07-07 22:26:18.000000 dji_thermal_sdk-1.3.20220517/dji_thermal_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)      449 2022-07-07 22:26:18.000000 dji_thermal_sdk-1.3.20220517/dji_thermal_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)        1 2022-07-07 22:26:18.000000 dji_thermal_sdk-1.3.20220517/dji_thermal_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)       20 2022-07-07 22:26:18.000000 dji_thermal_sdk-1.3.20220517/dji_thermal_sdk.egg-info/entry_points.txt
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)        1 2022-07-07 22:21:45.000000 dji_thermal_sdk-1.3.20220517/dji_thermal_sdk.egg-info/not-zip-safe
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)       21 2022-07-07 22:26:18.000000 dji_thermal_sdk-1.3.20220517/dji_thermal_sdk.egg-info/requires.txt
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)       16 2022-07-07 22:26:18.000000 dji_thermal_sdk-1.3.20220517/dji_thermal_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)     2455 2022-07-07 22:20:41.000000 dji_thermal_sdk-1.3.20220517/settings.ini
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)       38 2022-07-07 22:26:18.962633 dji_thermal_sdk-1.3.20220517/setup.cfg
+-rw-rw-r--   0 hxl170008  (1001) hxl170008  (1001)     3103 2022-07-07 22:20:41.000000 dji_thermal_sdk-1.3.20220517/setup.py
```

### Comparing `dji_thermal_sdk-0.0.1/LICENSE` & `dji_thermal_sdk-1.3.20220517/LICENSE`

 * *Files identical despite different names*

### Comparing `dji_thermal_sdk-0.0.1/dji_thermal_sdk/dji_sdk.py` & `dji_thermal_sdk-1.3.20220517/dji_thermal_sdk/dji_sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../00_core_dji.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: 00_core_dji.ipynb (unless otherwise specified).
 
-# %% auto 0
-__all__ = ['DIRP_PSEUDO_COLOR_WHITEHOT', 'DIRP_PSEUDO_COLOR_FULGURITE', 'DIRP_PSEUDO_COLOR_IRONRED', 'DIRP_PSEUDO_COLOR_HOTIRON',
-           'DIRP_PSEUDO_COLOR_MEDICAL', 'DIRP_PSEUDO_COLOR_ARCTIC', 'DIRP_PSEUDO_COLOR_RAINBOW1',
-           'DIRP_PSEUDO_COLOR_RAINBOW2', 'DIRP_PSEUDO_COLOR_TINT', 'DIRP_PSEUDO_COLOR_BLACKHOT',
-           'DIRP_PSEUDO_COLOR_NUM', 'DIRP_PSEUDO_COLOR_LUT_DEPTH', 'DIRP_SUCCESS', 'DIRP_ERROR_MALLOC',
-           'DIRP_ERROR_POINTER_NULL', 'DIRP_ERROR_INVALID_PARAMS', 'DIRP_ERROR_INVALID_RAW',
+__all__ = ['DIRP_PSEUDO_COLOR_WHITEHOT', 'DIRP_PSEUDO_COLOR_FULGURITE', 'DIRP_PSEUDO_COLOR_IRONRED',
+           'DIRP_PSEUDO_COLOR_HOTIRON', 'DIRP_PSEUDO_COLOR_MEDICAL', 'DIRP_PSEUDO_COLOR_ARCTIC',
+           'DIRP_PSEUDO_COLOR_RAINBOW1', 'DIRP_PSEUDO_COLOR_RAINBOW2', 'DIRP_PSEUDO_COLOR_TINT',
+           'DIRP_PSEUDO_COLOR_BLACKHOT', 'DIRP_PSEUDO_COLOR_NUM', 'DIRP_PSEUDO_COLOR_LUT_DEPTH', 'DIRP_SUCCESS',
+           'DIRP_ERROR_MALLOC', 'DIRP_ERROR_POINTER_NULL', 'DIRP_ERROR_INVALID_PARAMS', 'DIRP_ERROR_INVALID_RAW',
            'DIRP_ERROR_INVALID_HEADER', 'DIRP_ERROR_INVALID_CURVE', 'DIRP_ERROR_RJPEG_PARSE', 'DIRP_ERROR_SIZE',
            'DIRP_ERROR_INVALID_HANDLE', 'DIRP_ERROR_FORMAT_INPUT', 'DIRP_ERROR_FORMAT_OUTPUT',
            'DIRP_ERROR_UNSUPPORTED_FUNC', 'DIRP_ERROR_NOT_READY', 'DIRP_ERROR_ACTIVATION', 'DIRP_ERROR_INVALID_INI',
            'DIRP_ERROR_INVALID_SUB_DLL', 'DIRP_ERROR_ADVANCED', 'DIRP_HANDLE', 'dirp_api_version_t', 'dirp_color_bar_t',
            'dirp_enhancement_params_t', 'dirp_isotherm_t', 'dirp_isp_pseudo_color_lut_t',
            'dirp_measurement_params_range_t', 'dirp_measurement_params_t', 'dirp_resolution_t', 'dirp_rjpeg_version_t',
-           'set_dirp_dll', 'dji_init', 'dirp_create_from_rjpeg', 'dirp_destroy', 'dirp_get_api_version',
-           'dirp_get_color_bar', 'dirp_get_color_bar_adaptive_params', 'dirp_get_enhancement_params',
-           'dirp_get_isotherm', 'dirp_get_measurement_params', 'dirp_get_measurement_params_range',
-           'dirp_get_original_raw', 'dirp_get_pseudo_color', 'dirp_get_pseudo_color_lut', 'dirp_get_rjpeg_resolution',
-           'dirp_get_rjpeg_version', 'dirp_measure', 'dirp_measure_ex', 'dirp_process', 'dirp_process_strech',
-           'dirp_set_color_bar', 'dirp_set_enhancement_params', 'dirp_set_isotherm', 'dirp_set_logger_file',
-           'dirp_set_measurement_params', 'dirp_set_pseudo_color', 'dirp_set_verbose_level', 'get_pseudo_color']
+           'set_dirp_dll', 'dirp_create_from_rjpeg', 'dirp_destroy', 'dirp_get_api_version', 'dirp_get_color_bar',
+           'dirp_get_color_bar_adaptive_params', 'dirp_get_enhancement_params', 'dirp_get_isotherm',
+           'dirp_get_measurement_params', 'dirp_get_measurement_params_range', 'dirp_get_original_raw',
+           'dirp_get_pseudo_color', 'dirp_get_pseudo_color_lut', 'dirp_get_rjpeg_resolution', 'dirp_get_rjpeg_version',
+           'dirp_measure', 'dirp_measure_ex', 'dirp_process', 'dirp_process_strech', 'dirp_set_color_bar',
+           'dirp_set_enhancement_params', 'dirp_set_isotherm', 'dirp_set_logger_file', 'dirp_set_measurement_params',
+           'dirp_set_pseudo_color', 'dirp_set_verbose_level', 'get_pseudo_color']
 
-# %% ../00_core_dji.ipynb 3
-import os
+# Cell
 import ctypes as CT
 from ctypes import *
 
-# %% ../00_core_dji.ipynb 4
+# Cell
 _libdirp = ""
-
-# %% ../00_core_dji.ipynb 5
+# dirp_pseudo_color_e
 DIRP_PSEUDO_COLOR_WHITEHOT   = 0
 DIRP_PSEUDO_COLOR_FULGURITE  = 1
 DIRP_PSEUDO_COLOR_IRONRED    = 2
 DIRP_PSEUDO_COLOR_HOTIRON    = 3
 DIRP_PSEUDO_COLOR_MEDICAL    = 4
 DIRP_PSEUDO_COLOR_ARCTIC     = 5
 DIRP_PSEUDO_COLOR_RAINBOW1   = 6
@@ -40,15 +37,15 @@
 DIRP_PSEUDO_COLOR_TINT       = 8
 DIRP_PSEUDO_COLOR_BLACKHOT   = 9
 DIRP_PSEUDO_COLOR_NUM        = 10
 
 # palette look_up table
 DIRP_PSEUDO_COLOR_LUT_DEPTH = 256
 
-# %% ../00_core_dji.ipynb 6
+# dirp_ret_code_e
 DIRP_SUCCESS = 0
 DIRP_ERROR_MALLOC = -1
 DIRP_ERROR_POINTER_NULL = -2
 DIRP_ERROR_INVALID_PARAMS = -3,
 DIRP_ERROR_INVALID_RAW = -4
 DIRP_ERROR_INVALID_HEADER = -5
 DIRP_ERROR_INVALID_CURVE = -6
@@ -63,15 +60,15 @@
 DIRP_ERROR_INVALID_INI = -15
 DIRP_ERROR_INVALID_SUB_DLL = -16
 DIRP_ERROR_ADVANCED = -32
 
 # Initialize the handle of a r-jpeg image.
 DIRP_HANDLE = CT.c_void_p()
 
-# %% ../00_core_dji.ipynb 7
+# Cell
 class dirp_api_version_t(CT.Structure):
     '''
     API version structure definition
     '''
     _fields_ = [("api", CT.c_uint32), ("magic", CT.c_char * 8)]
 #
 class dirp_color_bar_t(Structure):
@@ -142,15 +139,19 @@
 class dirp_rjpeg_version_t (Structure):
     '''
     R-JPEG version structure definition
     '''
     _fields_ = [("rjpeg", CT.c_uint32),("header", CT.c_uint32),("curve", CT.c_uint32)]
     pass
 
-# %% ../00_core_dji.ipynb 8
+# Cell
+
+
+
+# Cell
 def set_dirp_dll(libdirp):
     global _libdirp
     _libdirp = libdirp
     pass
 
 def _getFunHandleFromDJIDll(dll_handle_str, fun_name_str):
     s = "{}.{}".format(dll_handle_str,fun_name_str)
@@ -159,34 +160,21 @@
         return fun
     except AttributeError as err:
         e = f"{dll_handle_str}.dll has no function '{fun_name_str}'"
         print(e)
         return -1
     pass
 
-# %% ../00_core_dji.ipynb 9
-def dji_init(dllpath:str=None):
-    if dllpath is None:
-        dllfp = os.path.join(os.getcwd(),"dji_thermal_sdk", "libdirp.dll")
-    else:
-        dllfp = dllpath
-    try:
-        libdirp = cdll.LoadLibrary(dllfp)
-        set_dirp_dll(libdirp)
-    except FileNotFoundError as err:
-        print(err)
-        print("https://www.dji.com/downloads/softwares/dji-thermal-sdk")
-
-# %% ../00_core_dji.ipynb 10
+# Cell
 def dirp_create_from_rjpeg(data, size, ph):
     '''
     Parameters:
         [in] data: R-JPEG binary data buffer pointer
         [in] size: R-JPEG binary data buffer size in bytes
-        [out]ph  : DIRP API handle pointer 
+        [out]ph  : DIRP API handle pointer
             - reminder: use two-level pointer to assign value to one-level pointer
     Return:
         int return code dirp_ret_code_e
     '''
     fun = _getFunHandleFromDJIDll("_libdirp","dirp_create_from_rjpeg")
     ret = fun(data, size, ph)
     return ret
@@ -227,19 +215,19 @@
     return ret
     pass
 #
 
 def dirp_get_color_bar_adaptive_params(h, color_bar):
     '''
     Get adaptive ISP color bar parameters in automatic mode.
-    In color bar automatic mode : manual_enable in dirp_color_bar_t is set as false. 
-    The inner ISP algorithm will calculate the best range values for color bar. 
-    Before calling this API you should call dirp_process once at least. 
-    And if any processing or measurement parameters had been changed, 
-    you should also call dirp_process again for getting new color bar adaptive parameters. 
+    In color bar automatic mode : manual_enable in dirp_color_bar_t is set as false.
+    The inner ISP algorithm will calculate the best range values for color bar.
+    Before calling this API you should call dirp_process once at least.
+    And if any processing or measurement parameters had been changed,
+    you should also call dirp_process again for getting new color bar adaptive parameters.
     In the above calling dirp_process, manual_enable in dirp_color_bar_t must be set as false.
 
     Parameters
         [in] h: DIRP API handle
         [out] color_bar: ISP color bar parameters pointer
 
     Return:
@@ -370,16 +358,16 @@
     fun = _getFunHandleFromDJIDll("_libdirp", "dirp_get_rjpeg_version")
     ret = fun(h, version)
     return ret
 #
 def dirp_measure(h, temp_image, size):
     '''
     Measure temperature of whole thermal image with RAW data in R-JPEG.
-    Each INT16 pixel value represents ten times the temperature value in Celsius. 
-    In other words, each LSB represents 0.1 degrees Celsius. 
+    Each INT16 pixel value represents ten times the temperature value in Celsius.
+    In other words, each LSB represents 0.1 degrees Celsius.
     The custom measurement parameters can be modifed by this API:dirp_set_measurement_params
     Parameters
         [in]h:DIRP API handle
         [out]temp_image:Temperature image data buffer pointer
         [in]size:Temperature image data buffer size in bytes
     Returns
         int return code dirp_ret_code_e
@@ -387,15 +375,15 @@
     fun = _getFunHandleFromDJIDll("_libdirp", "dirp_measure")
     ret = fun(h, temp_image, size)
     return ret
 #
 def dirp_measure_ex(h, temp_image, size):
     '''
     Measure temperature of whole thermal image with RAW data in R-JPEG.
-    Each FLOAT32 pixel value represents the real temperature in Celsius. 
+    Each FLOAT32 pixel value represents the real temperature in Celsius.
     The custom measurement parameters can be modifed by this API:
 
     dirp_set_measurement_params
     Parameters
         [in]h:DIRP API handle
         [out]temp_image:Temperature image data buffer pointer
         [in]size:Temperature image data buffer size in bytes
@@ -526,16 +514,16 @@
     Parameters
         [in]level:Log pring level dirp_verbose_level_e
 
     '''
     fun = _getFunHandleFromDJIDll("_libdirp", "dirp_set_verbose_level")
     ret = fun(level)
     return ret
-    
 
-# %% ../00_core_dji.ipynb 11
+
+# Cell
 def get_pseudo_color():
     "return the pseudo color dictionary."
     pseudo_color = {'white_hot':0, 'fulgurite':1, 'iron_red':2, 'hot_iron':3, 'medical':4,
                 'arctic': 5, 'rainbow1':6, 'rainbow2':7, 'Tint':8, 'black_hot':9
                }
-    return pseudo_color
+    return pseudo_color
```

### Comparing `dji_thermal_sdk-0.0.1/setup.py` & `dji_thermal_sdk-1.3.20220517/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,64 @@
 from pkg_resources import parse_version
 from configparser import ConfigParser
-import setuptools, shlex
+import setuptools,re,sys
 assert parse_version(setuptools.__version__)>=parse_version('36.2')
 
 # note: all settings are in settings.ini; edit there, not here
 config = ConfigParser(delimiters=['='])
 config.read('settings.ini')
 cfg = config['DEFAULT']
 
 cfg_keys = 'version description keywords author author_email'.split()
 expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
 for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
 setup_cfg = {o:cfg[o] for o in cfg_keys}
 
+if len(sys.argv)>1 and sys.argv[1]=='version':
+    print(setup_cfg['version'])
+    exit()
+
 licenses = {
     'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
     'mit': ('MIT License', 'OSI Approved :: MIT License'),
     'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
     'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
     'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
 }
 statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
     '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '3.6 3.7 3.8 3.9 3.10'.split()
+py_versions = '2.0 2.1 2.2 2.3 2.4 2.5 2.6 2.7 3.0 3.1 3.2 3.3 3.4 3.5 3.6 3.7 3.8 3.9 3.10'.split()
 
-requirements = shlex.split(cfg.get('requirements', ''))
-if cfg.get('pip_requirements'): requirements += shlex.split(cfg.get('pip_requirements', ''))
-min_python = cfg['min_python']
 lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
+min_python = cfg['min_python']
+
+requirements = ['pip', 'packaging']
+if cfg.get('requirements'): requirements += cfg.get('requirements','').split()
+if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
 dev_requirements = (cfg.get('dev_requirements') or '').split()
 
+long_description = open('README.md').read()
+# ![png](docs/images/output_13_0.png)
+for ext in ['png', 'svg']:
+    long_description = re.sub(r'!\['+ext+'\]\((.*)\)', '!['+ext+']('+'https://raw.githubusercontent.com/{}/{}'.format(cfg['user'],cfg['lib_name'])+'/'+cfg['branch']+'/\\1)', long_description)
+    long_description = re.sub(r'src=\"(.*)\.'+ext+'\"', 'src=\"https://raw.githubusercontent.com/{}/{}'.format(cfg['user'],cfg['lib_name'])+'/'+cfg['branch']+'/\\1.'+ext+'\"', long_description)
+
 setuptools.setup(
     name = cfg['lib_name'],
     license = lic[0],
     classifiers = [
         'Development Status :: ' + statuses[int(cfg['status'])],
         'Intended Audience :: ' + cfg['audience'].title(),
         'Natural Language :: ' + cfg['language'].title(),
     ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
     url = cfg['git_url'],
     packages = setuptools.find_packages(),
     include_package_data = True,
     install_requires = requirements,
     extras_require={ 'dev': dev_requirements },
-    dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md').read(),
+    long_description = long_description,
     long_description_content_type = 'text/markdown',
     zip_safe = False,
-    entry_points = {
-        'console_scripts': cfg.get('console_scripts','').split(),
-        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
-    },
+    entry_points = { 'console_scripts': cfg.get('console_scripts','').split() },
     **setup_cfg)
 
-
```

