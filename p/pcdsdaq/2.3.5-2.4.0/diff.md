# Comparing `tmp/pcdsdaq-2.3.5.tar.gz` & `tmp/pcdsdaq-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pcdsdaq-2.3.5.tar", last modified: Fri Jun  3 18:52:04 2022, max compression
+gzip compressed data, was "pcdsdaq-2.4.0.tar", last modified: Tue Apr  4 19:29:30 2023, max compression
```

## Comparing `pcdsdaq-2.3.5.tar` & `pcdsdaq-2.4.0.tar`

### file list

```diff
@@ -1,26 +1,78 @@
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:04.000000 pcdsdaq-2.3.5/
--rw-r--r--   0 klauer   (1318172782) 1704612529       80 2022-06-03 18:47:54.000000 pcdsdaq-2.3.5/MANIFEST.in
--rw-r--r--   0 klauer   (1318172782) 1704612529      220 2022-06-03 18:52:04.000000 pcdsdaq-2.3.5/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529      561 2022-06-03 18:47:54.000000 pcdsdaq-2.3.5/README.rst
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:04.000000 pcdsdaq-2.3.5/bin/
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     1310 2022-06-03 18:47:54.000000 pcdsdaq-2.3.5/bin/pcdsdaq_lib_setup
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:04.000000 pcdsdaq-2.3.5/pcdsdaq/
--rw-r--r--   0 klauer   (1318172782) 1704612529       92 2022-06-03 18:47:54.000000 pcdsdaq-2.3.5/pcdsdaq/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      497 2022-06-03 18:52:04.000000 pcdsdaq-2.3.5/pcdsdaq/_version.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    19660 2022-06-03 18:47:54.000000 pcdsdaq-2.3.5/pcdsdaq/ami.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    42271 2022-06-03 18:47:54.000000 pcdsdaq-2.3.5/pcdsdaq/daq.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3102 2022-06-03 18:47:54.000000 pcdsdaq-2.3.5/pcdsdaq/ext_scripts.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2008 2022-06-03 18:47:54.000000 pcdsdaq-2.3.5/pcdsdaq/preprocessors.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    11562 2022-06-03 18:47:54.000000 pcdsdaq-2.3.5/pcdsdaq/scan_vars.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:04.000000 pcdsdaq-2.3.5/pcdsdaq/sim/
--rw-r--r--   0 klauer   (1318172782) 1704612529     1457 2022-06-03 18:47:54.000000 pcdsdaq-2.3.5/pcdsdaq/sim/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1355 2022-06-03 18:47:54.000000 pcdsdaq-2.3.5/pcdsdaq/sim/pyami.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     7425 2022-06-03 18:47:54.000000 pcdsdaq-2.3.5/pcdsdaq/sim/pydaq.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:04.000000 pcdsdaq-2.3.5/pcdsdaq.egg-info/
--rw-r--r--   0 klauer   (1318172782) 1704612529      220 2022-06-03 18:52:04.000000 pcdsdaq-2.3.5/pcdsdaq.egg-info/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529      406 2022-06-03 18:52:04.000000 pcdsdaq-2.3.5/pcdsdaq.egg-info/SOURCES.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        1 2022-06-03 18:52:04.000000 pcdsdaq-2.3.5/pcdsdaq.egg-info/dependency_links.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        8 2022-06-03 18:52:04.000000 pcdsdaq-2.3.5/pcdsdaq.egg-info/top_level.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      173 2022-06-03 18:52:04.000000 pcdsdaq-2.3.5/setup.cfg
--rw-r--r--   0 klauer   (1318172782) 1704612529      398 2022-06-03 18:47:54.000000 pcdsdaq-2.3.5/setup.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    68573 2022-06-03 18:47:54.000000 pcdsdaq-2.3.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.781514 pcdsdaq-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.773514 pcdsdaq-2.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.773514 pcdsdaq-2.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      748 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1230 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2996 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-04-04 19:29:30.781514 pcdsdaq-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.773514 pcdsdaq-2.4.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1310 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/bin/pcdsdaq_lib_setup
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.777514 pcdsdaq-2.4.0/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.777514 pcdsdaq-2.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.777514 pcdsdaq-2.4.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)      313 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/ami_api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/ami_basic.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8415 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/daq_api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5169 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/daq_basic.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/daq_config.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/env.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      512 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/plans_basic.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/preprocessors_api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6106 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/scan_pvs.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs/source/sim.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.777514 pcdsdaq-2.4.0/pcdsdaq/
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-04 19:29:30.000000 pcdsdaq-2.4.0/pcdsdaq/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19672 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/ami.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.781514 pcdsdaq-2.4.0/pcdsdaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27615 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/daq/interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34734 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/daq/lcls1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    76922 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/daq/lcls2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41884 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/daq/original.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/ext_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/plans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/scan_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.781514 pcdsdaq-2.4.0/pcdsdaq/sim/
+-rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/sim/pyami.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7425 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/sim/pydaq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pcdsdaq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.777514 pcdsdaq-2.4.0/pcdsdaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-04-04 19:29:30.000000 pcdsdaq-2.4.0/pcdsdaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-04-04 19:29:30.000000 pcdsdaq-2.4.0/pcdsdaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-04 19:29:30.000000 pcdsdaq-2.4.0/pcdsdaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-04 19:29:30.000000 pcdsdaq-2.4.0/pcdsdaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-04 19:29:30.000000 pcdsdaq-2.4.0/pcdsdaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-04 19:29:30.781514 pcdsdaq-2.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:30.781514 pcdsdaq-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5802 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/test_ami.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32178 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/test_daq_lcls2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14791 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/test_daq_original.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/test_ext_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/test_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6404 2023-04-04 19:29:14.000000 pcdsdaq-2.4.0/tests/test_scan_vars.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pcdsdaq-2.3.5/README.rst` & `pcdsdaq-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.3.5/bin/pcdsdaq_lib_setup` & `pcdsdaq-2.4.0/bin/pcdsdaq_lib_setup`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.3.5/pcdsdaq/ami.py` & `pcdsdaq-2.4.0/pcdsdaq/ami.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
 import time
 from importlib import import_module
 from threading import Thread
 
 import numpy as np
-from ophyd.device import Device, Component as Cpt, Staged
+from ophyd.device import Component as Cpt
+from ophyd.device import Device, Staged
 from ophyd.signal import Signal
 from ophyd.status import Status
 from ophyd.utils.errors import ReadOnlyError
 from toolz.itertoolz import partition
 
-from .ext_scripts import get_hutch_name, get_ami_proxy
+from .ext_scripts import get_ami_proxy, get_hutch_name
 
 logger = logging.getLogger(__name__)
 L3T_DEFAULT = '/reg/neh/operator/{}opr/l3t/amifil.l3t'
 
 # Set uninitialized globals for style-checker
 pyami = None
 pyami_connected = None
@@ -284,15 +285,15 @@
     upper: ``float``
         The upper bound for the value to pass
 
     Returns
     -------
     filter_string: ``str``
     """
-    return '{}<{}<{}'.format(lower, ami_name, upper)
+    return f'{lower}<{ami_name}<{upper}'
 
 
 def evr_filter(event_code):
     """
     Helper function that creates a filter for a certain event code.
 
     Parameters
```

### Comparing `pcdsdaq-2.3.5/pcdsdaq/daq.py` & `pcdsdaq-2.4.0/pcdsdaq/daq/original.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """
-This module defines a control interface for the LCLS1 DAQ.
+This is the previous LCLS1 DAQ control interface.
+
+This was a top-level daq.py file in versions prior to v3.0.0.
+It is preserved here because the v3.0.0 refactor changed many
+things and the old interface may still be needed for now.
 """
 import enum
 import functools
 import logging
 import os
-import time
 import threading
+import time
 from importlib import import_module
 
 from ophyd.status import Status
 from ophyd.utils import StatusTimeoutError, WaitTimeoutError
 
-from . import ext_scripts
-from .ami import set_ami_hutch, set_pyami_filter, set_monitor_det
+from .. import ext_scripts
+from ..ami import set_monitor_det, set_pyami_filter
+from .interface import register_daq
 
 logger = logging.getLogger(__name__)
 pydaq = None
 
 # Wait up to this many seconds for daq to be ready for a begin call
 BEGIN_TIMEOUT = 15
 # Do not allow begins within this many seconds of a stop
@@ -184,20 +189,21 @@
                     self._control.connect()
                     logger.info('Connected to DAQ')
                     conn = True
                     break
                 except Exception as exc:
                     if 'query' in str(exc):
                         err = True
-                        logger.error(('Failed to connect: DAQ is not '
-                                      'allocated!'))
+                        logger.error("Failed to connect: DAQ is not allocated!")
             if not (err or conn):
                 err = True
-                logger.error(('Failed to connect: DAQ is not running on this '
-                              'machine, and is not allocated!'))
+                logger.error(
+                    "Failed to connect: DAQ is not running on this "
+                    "machine, and is not allocated!"
+                )
             if err:
                 logger.debug('del Daq.control')
                 del self._control
                 self._control = None
         else:
             logger.info('Connect requested, but already connected to DAQ')
 
@@ -672,15 +678,15 @@
             at which they were configured, as specified by ``bluesky``.
         """
         logger.debug('Daq.configure(events=%s, duration=%s, record=%s, '
                      'use_l3t=%s, controls=%s, begin_sleep=%s)',
                      events, duration, record, use_l3t, controls, begin_sleep)
         state = self.state
         if state not in ('Connected', 'Configured'):
-            err = 'Cannot configure from state {}!'.format(state)
+            err = f'Cannot configure from state {state}!'
             raise StateTransitionError(err)
 
         self._check_duration(duration)
         old = self.read_configuration()
 
         self.preconfig(events=events, duration=duration, record=record,
                        use_l3t=use_l3t, controls=controls,
@@ -737,15 +743,15 @@
         """
         if config is None:
             config = self.config
 
         txt = []
         for key, value in config.items():
             if value is not None:
-                txt.append('{}={}'.format(key, value))
+                txt.append(f'{key}={value}')
         if header:
             header += ' '
         logger.info(header + ', '.join(txt))
 
     @property
     def record(self):
         """
@@ -1057,16 +1063,17 @@
         try:
             hutch_name = hutch_name or self.hutch_name
             if hutch_name is None:
                 hutch_name = ext_scripts.get_hutch_name()
             hutch_name = hutch_name.lower()
             if hutch_name not in ('amo', 'sxr', 'xpp', 'xcs', 'mfx', 'cxi',
                                   'mec', 'tst'):
-                raise ValueError(('{} is not a valid hutch, cannot determine '
-                                  'run number'.format(hutch_name)))
+                raise ValueError(
+                    f"{hutch_name} is not a valid hutch, cannot determine run number"
+                )
             if self.state in ('Open', 'Running') and self.config['record']:
                 return ext_scripts.get_run_number(hutch=hutch_name, live=True)
             else:
                 return ext_scripts.get_run_number(hutch=hutch_name, live=False)
         except FileNotFoundError:
             raise RuntimeError('No nfs access, cannot determine run number.')
 
@@ -1124,36 +1131,7 @@
     def set_monitor(self, det):
         return set_monitor_det(det)
     set_monitor.__doc__ = set_monitor_det.__doc__
 
 
 class StateTransitionError(Exception):
     pass
-
-
-_daq_instance = None
-
-
-def register_daq(daq):
-    """
-    Called by `Daq` at the end of ``__init__`` to save our one daq instance as
-    the real `Daq`. There will always only be one `Daq`.
-
-    Parameters
-    ----------
-    daq: `Daq`
-    """
-    global _daq_instance
-    _daq_instance = daq
-    if daq.hutch_name is not None:
-        set_ami_hutch(daq.hutch_name.lower())
-
-
-def get_daq():
-    """
-    Called by other modules to get the registered `Daq` instance.
-
-    Returns
-    -------
-    daq: `Daq`
-    """
-    return _daq_instance
```

### Comparing `pcdsdaq-2.3.5/pcdsdaq/ext_scripts.py` & `pcdsdaq-2.4.0/pcdsdaq/ext_scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import logging
 import re
 import socket
 import subprocess
 
-
 logger = logging.getLogger(__name__)
 CNF = '/reg/g/pcds/dist/pds/{0}/scripts/{0}.cnf'
 SCRIPTS = '/reg/g/pcds/engineering_tools/{}/scripts/{}'
 TOOLS = '/reg/g/pcds/dist/pds/tools/{}/{}'
 
 
 def call_script(args, timeout=None, ignore_return_code=False):
     logger.debug('Calling external script %s with timeout=%s,'
                  ' ignore_fail=%s', args, timeout, ignore_return_code)
     try:
-        return subprocess.check_output(args, universal_newlines=True,
+        return subprocess.check_output(args, text=True,
                                        timeout=timeout)
     except subprocess.CalledProcessError as exc:
         if ignore_return_code:
             return exc.output
         else:
             logger.debug('CalledProcessError from %s', args, exc_info=True)
             raise
```

### Comparing `pcdsdaq-2.3.5/pcdsdaq/preprocessors.py` & `pcdsdaq-2.4.0/pcdsdaq/preprocessors.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.3.5/pcdsdaq/scan_vars.py` & `pcdsdaq-2.4.0/pcdsdaq/scan_vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
-from typing import Any, Dict
+from typing import Any
 
 from bluesky.callbacks.core import CallbackBase
-from ophyd.device import Device, Component as Cpt
+from ophyd.device import Component as Cpt
+from ophyd.device import Device
 from ophyd.signal import EpicsSignal
 from toolz import partition
 
 from .daq import get_daq
 
 logger = logging.getLogger(__name__)
 
@@ -71,15 +72,15 @@
         """
         Disable automatic updating of PVs during a scan.
         """
         if self._cbid is not None:
             self._RE.unsubscribe(self._cbid)
             self._cbid = None
 
-    def start(self, doc: Dict[str, Any]):
+    def start(self, doc: dict[str, Any]):
         """
         Initialize the scan variables at the start of a run.
 
         This inspects the metadata dictionary and will set reasonable values if
         this metadata dictionary is well-formed as in ``bluesky`` built-ins
         like ``scan``. It also inspects the daq object.
         """
@@ -89,26 +90,25 @@
             self.i_step.put(self._i_start)
             self.is_scan.put(1)
             # inspect the doc
             # check for motor names
             try:
                 motors = doc['motors']
                 for i, name in enumerate(motors[:3]):
-                    sig = getattr(self, 'var{}'.format(i))
+                    sig = getattr(self, f'var{i}')
                     sig.put(name)
             except KeyError:
                 logger.debug('Skip var names, no "motors" in start doc')
 
             # check for a top level number of points, this is often present
             try:
                 num_points = doc['num_points']
             except KeyError:
                 logger.debug('No num_points, skip num from top-level key.')
                 has_top_level_num = False
-                pass
             else:
                 self.n_steps.put(num_points)
                 has_top_level_num = True
 
             # in this block we find the min/max and number of points
             # check the plan pattern, determines how we read the args
             # inner_product is mot, start, stop, (repeat), num
@@ -182,15 +182,15 @@
                 )
             return
         sig_max = getattr(self, f'var{index}_max')
         sig_min = getattr(self, f'var{index}_min')
         sig_max.put(max(start, stop))
         sig_min.put(min(start, stop))
 
-    def setup_inner_product(self, plan_pattern_args: Dict[str, Any]) -> None:
+    def setup_inner_product(self, plan_pattern_args: dict[str, Any]) -> None:
         """
         Handle max, min, number of steps for inner_product scans.
 
         These are the plans whose arguments are (mot, start, stop) repeat,
         then a num later, such as the normal scan.
         """
         # check for start/stop points
@@ -198,15 +198,15 @@
         for index, (_, start, stop) in enumerate(per_motor):
             self.update_min_max(start, stop, index)
 
         # check for number of steps
         num = plan_pattern_args['num']
         self.n_steps.put(num)
 
-    def setup_outer_product(self, plan_pattern_args: Dict[str, Any]) -> None:
+    def setup_outer_product(self, plan_pattern_args: dict[str, Any]) -> None:
         """
         Handle max, min, number of steps for outer_product scans.
 
         These are the plans whose arguments are (mot, start, stop, num)
         repeat, with snake directions intersperced starting after the second
         num (or not), such as grid_scan.
         """
@@ -232,15 +232,15 @@
             self.update_min_max(start, stop, index)
             # check for number of steps: a product of all the steps!
             product_num *= num
         self.n_steps.put(product_num)
 
     def setup_inner_list_product(
         self,
-        plan_pattern_args: Dict[str, Any],
+        plan_pattern_args: dict[str, Any],
     ) -> None:
         """
         Handle max, min, number of steps for inner_list_product scans.
 
         These are the plans whose arguments are (mot, list) repeat,
         where every list needs to have the same length because it's a 1D
         scan with multiple motors, such as list_scan.
@@ -251,15 +251,15 @@
             self.update_min_max(min(points), max(points), index)
             # On the first loop, cache the number of points
             if index == 0:
                 self.n_steps.put(len(points))
 
     def setup_outer_list_product(
         self,
-        plan_pattern_args: Dict[str, Any],
+        plan_pattern_args: dict[str, Any],
     ) -> None:
         """
         Handle max, min, number of steps for outer_list_product scans.
 
         These are the plans whose arguments are (mot, list) repeat,
         where the lists can be any length because it's a multi-dimensional
         mesh scan, like list_grid_scan.
```

### Comparing `pcdsdaq-2.3.5/pcdsdaq/sim/__init__.py` & `pcdsdaq-2.4.0/pcdsdaq/sim/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 This module provides a simulated pydaq module for offline testing and training.
 It does not assume that the real pydaq module is available.
 """
 import logging
 from importlib import import_module
 
 import pcdsdaq.ami as ami
-import pcdsdaq.daq as daq
+import pcdsdaq.daq.original as daq
 import pcdsdaq.ext_scripts as ext
-from . import pyami
-from . import pydaq
+
+from . import pyami, pydaq
 
 logger = logging.getLogger(__name__)
 
 
 def set_sim_mode(sim_mode):
     """
     Parameters
```

### Comparing `pcdsdaq-2.3.5/pcdsdaq/sim/pyami.py` & `pcdsdaq-2.4.0/pcdsdaq/sim/pyami.py`

 * *Files identical despite different names*

### Comparing `pcdsdaq-2.3.5/pcdsdaq/sim/pydaq.py` & `pcdsdaq-2.4.0/pcdsdaq/sim/pydaq.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import logging
 import numbers
-import time
 import threading
-import logging
+import time
 
 from pcdsdaq.daq import Daq
 from pcdsdaq.ext_scripts import get_hutch_name, get_run_number  # NOQA
 
 logger = logging.getLogger(__name__)
```

