# Comparing `tmp/transfocate-0.5.5.tar.gz` & `tmp/transfocate-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transfocate-0.5.5.tar", last modified: Fri Jun  3 18:52:26 2022, max compression
+gzip compressed data, was "transfocate-0.5.7.tar", last modified: Tue Apr  4 19:57:03 2023, max compression
```

## Comparing `transfocate-0.5.5.tar` & `transfocate-0.5.7.tar`

### file list

```diff
@@ -1,34 +1,60 @@
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:26.000000 transfocate-0.5.5/
--rw-r--r--   0 klauer   (1318172782) 1704612529      127 2022-06-03 18:48:18.000000 transfocate-0.5.5/MANIFEST.in
--rw-r--r--   0 klauer   (1318172782) 1704612529      261 2022-06-03 18:52:26.000000 transfocate-0.5.5/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529     2550 2022-06-03 18:48:18.000000 transfocate-0.5.5/README.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529      181 2022-06-03 18:52:26.000000 transfocate-0.5.5/setup.cfg
--rw-r--r--   0 klauer   (1318172782) 1704612529      427 2022-06-03 18:48:18.000000 transfocate-0.5.5/setup.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:26.000000 transfocate-0.5.5/transfocate/
--rw-r--r--   0 klauer   (1318172782) 1704612529      297 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      497 2022-06-03 18:52:26.000000 transfocate-0.5.5/transfocate/_version.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     8493 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/automated_checkout.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4253 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/calculator.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    13166 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/checkout.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     6824 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/lens.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:26.000000 transfocate-0.5.5/transfocate/table/
--rw-r--r--   0 klauer   (1318172782) 1704612529   153490 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/table/MFX_EnergyLensInterlock_Tables_Transposed.xlsx
--rw-r--r--   0 klauer   (1318172782) 1704612529      311 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/table/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1970 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/table/info.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3540 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/table/ioc.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3362 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/table/plc_table.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5825 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/table/report.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:26.000000 transfocate-0.5.5/transfocate/tests/
--rw-r--r--   0 klauer   (1318172782) 1704612529      268 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/tests/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1271 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/tests/conftest.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2107 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/tests/test_calculator.py
--rw-r--r--   0 klauer   (1318172782) 1704612529       80 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/tests/test_import.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1555 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/tests/test_lens.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4396 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/tests/test_transfocate.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9335 2022-06-03 18:48:18.000000 transfocate-0.5.5/transfocate/transfocator.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:52:26.000000 transfocate-0.5.5/transfocate.egg-info/
--rw-r--r--   0 klauer   (1318172782) 1704612529      261 2022-06-03 18:52:26.000000 transfocate-0.5.5/transfocate.egg-info/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529      779 2022-06-03 18:52:26.000000 transfocate-0.5.5/transfocate.egg-info/SOURCES.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        1 2022-06-03 18:52:26.000000 transfocate-0.5.5/transfocate.egg-info/dependency_links.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       12 2022-06-03 18:52:26.000000 transfocate-0.5.5/transfocate.egg-info/top_level.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529    68549 2022-06-03 18:48:18.000000 transfocate-0.5.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:57:03.882167 transfocate-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-04-04 19:56:45.000000 transfocate-0.5.7/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-04-04 19:56:45.000000 transfocate-0.5.7/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-04 19:56:45.000000 transfocate-0.5.7/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-04 19:56:45.000000 transfocate-0.5.7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:57:03.874167 transfocate-0.5.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:57:03.878167 transfocate-0.5.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-04-04 19:56:45.000000 transfocate-0.5.7/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1163 2023-04-04 19:56:45.000000 transfocate-0.5.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-04-04 19:56:45.000000 transfocate-0.5.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-04 19:56:45.000000 transfocate-0.5.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3032 2023-04-04 19:56:45.000000 transfocate-0.5.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-04-04 19:56:45.000000 transfocate-0.5.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-04-04 19:56:45.000000 transfocate-0.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5785 2023-04-04 19:57:03.882167 transfocate-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-04 19:56:45.000000 transfocate-0.5.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:57:03.878167 transfocate-0.5.7/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-04-04 19:56:45.000000 transfocate-0.5.7/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-04 19:56:45.000000 transfocate-0.5.7/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:57:03.878167 transfocate-0.5.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-04-04 19:56:45.000000 transfocate-0.5.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:57:03.878167 transfocate-0.5.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-04 19:56:45.000000 transfocate-0.5.7/docs/source/calculator.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-04-04 19:56:45.000000 transfocate-0.5.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3305 2023-04-04 19:56:45.000000 transfocate-0.5.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-04 19:56:45.000000 transfocate-0.5.7/docs/source/lens.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-04-04 19:56:45.000000 transfocate-0.5.7/docs/source/transfocator.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-04 19:56:45.000000 transfocate-0.5.7/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-04-04 19:56:45.000000 transfocate-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-04 19:56:45.000000 transfocate-0.5.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-04 19:57:03.882167 transfocate-0.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:57:03.878167 transfocate-0.5.7/transfocate/
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-04 19:57:03.000000 transfocate-0.5.7/transfocate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8484 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/automated_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4245 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13100 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6718 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/lens.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:57:03.882167 transfocate-0.5.7/transfocate/table/
+-rw-r--r--   0 runner    (1001) docker     (122)   153490 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/table/MFX_EnergyLensInterlock_Tables_Transposed.xlsx
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/table/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3509 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/table/ioc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3332 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/table/plc_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5825 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/table/report.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:57:03.882167 transfocate-0.5.7/transfocate/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1085 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/tests/test_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/tests/test_lens.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4474 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/tests/test_transfocate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9363 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/transfocator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-04-04 19:56:45.000000 transfocate-0.5.7/transfocate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:57:03.882167 transfocate-0.5.7/transfocate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5785 2023-04-04 19:57:03.000000 transfocate-0.5.7/transfocate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-04-04 19:57:03.000000 transfocate-0.5.7/transfocate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-04 19:57:03.000000 transfocate-0.5.7/transfocate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-04-04 19:57:03.000000 transfocate-0.5.7/transfocate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-04 19:57:03.000000 transfocate-0.5.7/transfocate.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `transfocate-0.5.5/README.rst` & `transfocate-0.5.7/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -46,23 +46,23 @@
 -----------
 
 To perform a scan for a single XRT lens, use:
 
 .. code-block:: python
 
     >>> sweep_and_plot_xrt(xrt_lens, num_steps=100)
-    
+
 This will choose different combinations of TFS lenses to span the region, and
 scan energy in 100 discrete steps.
 To perform a scan for _all_ XRT lenses, use:
 
 .. code-block:: python
 
     >>> sweep_and_plot_xrt_all(num_steps=100)
-    
+
 Per-lens data and plots will be saved to Excel and PNG/PDF files, respectively.
 This can be combined into a full checkout report with the following:
 
 .. code-block:: python
 
     >>> generate_report()
```

### Comparing `transfocate-0.5.5/transfocate/automated_checkout.py` & `transfocate-0.5.7/transfocate/automated_checkout.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 import matplotlib.pyplot as plt
 from bluesky.callbacks import LiveTable
 
 import transfocate
 import transfocate.checkout
 
 from .table import generate_report
-from .table.info import MIN_ENERGY, MIN_RADIUS
+from .table.info import MIN_ENERGY
 from .table.info import data as spreadsheet_data
 
 DESCRIPTION = __doc__
 
 lens_to_spreadsheet_df = {
     0: spreadsheet_data["NO_LENS"],
     1: spreadsheet_data["LENS1_750"],
@@ -281,15 +281,15 @@
     except Exception as ex:
         print(
             """
 Sorry, trouble connecting to some devices. This happens occasionally at initialization.
 Please re-try running this script.
 """
         )
-        raise
+        raise ex
 
     print(DESCRIPTION)
     print("Run scans and generate report? ('yes' to continue)")
     if input().lower() == "yes":
         print("Number of data points? Default: 50")
         try:
             num_points = int(input().strip())
```

### Comparing `transfocate-0.5.5/transfocate/calculator.py` & `transfocate-0.5.7/transfocate/calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import itertools
 import logging
 
 import numpy as np
 
 from transfocate.lens import LensConnect
 
-
 logger = logging.getLogger(__name__)
 
 
 class Calculator:
     """
     Class for the transfocator beryllium lens calculator.
 
@@ -99,15 +98,15 @@
         # Loop through all possible tfs/xrt combinations
         for combo in self.combinations(include_prefocus=include_prefocus):
             # Check to see if the number of lenses is less than the limit
             if combo.nlens <= n:
                 try:
                     image = combo.image(z_obj)
                     diff = np.abs(image - target)
-                except Exception as exc:
+                except Exception:
                     logger.exception("Unable to calculate image position")
                     diff = np.inf
                 # See if we have found a better solution
                 if diff < solution_diff:
                     logger.debug("Found a combination with image %s, %s "
                                  "from target %s", image, diff, target)
                     solution = combo
```

### Comparing `transfocate-0.5.5/transfocate/checkout.py` & `transfocate-0.5.7/transfocate/checkout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-import time
 
-import bluesky
 import bluesky.plan_stubs as bps
 import bluesky.plans as bp
 import bluesky.preprocessors as bpp
-import databroker
-
 import ophyd
 from ophyd import Component as Cpt
 from ophyd import EpicsSignal, EpicsSignalRO
 
-import transfocate
-
 
 class LensCheckout(ophyd.Device):
     state = Cpt(EpicsSignal, ":STATE", kind="normal")  # , string=True)
     state_bypass = Cpt(
         EpicsSignal, ":BYP:INS", kind="normal",
         doc="Override state in bypass mode with this"
     )
```

### Comparing `transfocate-0.5.5/transfocate/lens.py` & `transfocate-0.5.7/transfocate/lens.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,27 @@
 """
 Basic Lens object handling
 """
-############
-# Standard #
-############
 import logging
 
-###############
-# Third Party #
-###############
 import numpy as np
 import prettytable
-from ophyd import EpicsSignalRO, EpicsSignal, Component as Cpt, Device
+from ophyd import Component as Cpt
+from ophyd import Device, EpicsSignal, EpicsSignalRO
 from pcdsdevices.inout import InOutPVStatePositioner
 
-##########
-# Module #
-##########
-
 logger = logging.getLogger(__name__)
 
 
 class LensTripLimits(Device):
     """Trip limits for a given pre-focus lens (or lack thereof)."""
     # _table_name = Cpt(EpicsSignalRO, ":STR", doc="Table name for trip information")
     low = Cpt(EpicsSignalRO, ":LOW", doc="Trip region low [um]", auto_monitor=False)
     high = Cpt(EpicsSignalRO, ":HIGH", doc="Trip region high [um]", auto_monitor=False)
-    
+
 
 class Lens(InOutPVStatePositioner):
     """
     Data structure for basic Lens object
 
     Parameters
     ----------
@@ -41,16 +32,18 @@
         Prefix for the PVs that contain focusing information
     """
     # StatePositioner information
     _inserted = Cpt(EpicsSignalRO, ':STATE')
     _removed = Cpt(EpicsSignalRO, ":OUT")
     _insert = Cpt(EpicsSignal, ':INSERT')
     _remove = Cpt(EpicsSignal, ':REMOVE')
-    _state_logic = {'_inserted': {0: 'defer',  1: 'IN'},
-                    '_removed': {0: 'defer', 1: 'OUT'}}
+    _state_logic = {
+        "_inserted": {0: "defer", 1: "IN"},
+        "_removed": {0: "defer", 1: "OUT"},
+    }
     # Signals related to optical configuration
     _sig_radius = Cpt(EpicsSignalRO, ":RADIUS", auto_monitor=True)
     _sig_z = Cpt(EpicsSignalRO, ":Z", auto_monitor=True)
     _sig_focus = Cpt(EpicsSignalRO, ":FOCUS", auto_monitor=True)
     # Default configuration attributes. Read attributes are set correctly by
     # InOutRecordPositioner
     _default_configuration_attrs = ['_sig_radius', '_sig_z']
@@ -133,15 +126,15 @@
             self._insert.put(1)
         elif state.name == 'OUT':
             self._remove.put(1)
         # We shouldn't ever get to this line as most calls will have gone
         # through check_value first. Just in case this is here to not fail
         # silently
         else:
-            raise ValueError("Invalid State {}".format(state))
+            raise ValueError(f"Invalid State {state}")
 
 
 class LensConnect:
     """
     Data structure for a basic system of lenses
 
     Parameters
@@ -167,15 +160,15 @@
         Returns
         -------
         float
             returns the effective radius of the lens array.
         """
         if not self.lenses:
             return 0.0
-        return 1/np.sum(np.reciprocal([float(l.radius) for l in self.lenses]))
+        return 1 / np.sum(np.reciprocal([float(lens.radius) for lens in self.lenses]))
 
     def image(self, z_obj):
         """
         Method recursively calculates the z location of the image of a system
         of lenses and returns it in meters (m)
 
         Parameters
```

### Comparing `transfocate-0.5.5/transfocate/table/MFX_EnergyLensInterlock_Tables_Transposed.xlsx` & `transfocate-0.5.7/transfocate/table/MFX_EnergyLensInterlock_Tables_Transposed.xlsx`

 * *Files identical despite different names*

### Comparing `transfocate-0.5.5/transfocate/table/info.py` & `transfocate-0.5.7/transfocate/table/info.py`

 * *Files identical despite different names*

### Comparing `transfocate-0.5.5/transfocate/table/ioc.py` & `transfocate-0.5.7/transfocate/table/ioc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """Generate IOC header files (in C) for the spreadsheet table."""
-import sys
 
-import numpy as np
 import pandas as pd
 
-
 from .info import data as spreadsheet_data
 
 # Header file output settings:
 ROW_FORMAT = "{{{energy:.6f}, {trip_min:.6f}, {trip_max:.6f}}}"
 HEADER = """
 /* WARNING: This file is auto-generated. Do not modify it. */
 #ifndef _H_MFX_RANGE_TABLE
```

### Comparing `transfocate-0.5.5/transfocate/table/plc_table.py` & `transfocate-0.5.7/transfocate/table/plc_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Create Beckhoff TwinCAT PLC source code for the spreadsheet."""
-import sys
 
-import numpy as np
 import pandas as pd
 
 from .info import data as spreadsheet_data
 
 # PLC file output settings:
 DECLARATION_FORMAT = "{table_name} : ARRAY[0..{row_count}] OF ST_TableRow;"
 ROW_FORMAT = (
```

### Comparing `transfocate-0.5.5/transfocate/table/report.py` & `transfocate-0.5.7/transfocate/table/report.py`

 * *Files identical despite different names*

### Comparing `transfocate-0.5.5/transfocate/tests/conftest.py` & `transfocate-0.5.7/transfocate/tests/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,14 @@
-###############
-# Third Party #
-###############
 import pytest
-##########
-# Module #
-##########
-from transfocate.lens import Lens, LensConnect
 from ophyd.sim import make_fake_device
 
-################
-# Mock Classes #
-################
-class FakeLens(object):
+from ..lens import Lens, LensConnect
+
+
+class FakeLens:
 
     image_from_obj = Lens.image_from_obj
 
     def __init__(self, radius, z, focus):
         self.radius = radius
         self.z = z
         self.focus = focus
@@ -25,17 +18,15 @@
         self.inserted = True
 
     def remove(self):
         self.inserted = False
 
 
 SynLens = make_fake_device(Lens)
-############
-# Fixtures #
-############
+
 
 @pytest.fixture(scope='module')
 def lens():
     lens = SynLens("TST:TFS:LENS:01:", name='Lens')
     lens._sig_radius.sim_put(500.0)
     lens._sig_z.sim_put(100.0)
     lens._sig_focus.sim_put(50.0)
```

### Comparing `transfocate-0.5.5/transfocate/tests/test_calculator.py` & `transfocate-0.5.7/transfocate/tests/test_calculator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,12 @@
-############
-# Standard #
-############
-
-###############
-# Third Party #
-###############
-import pytest
 import numpy as np
-##########
-# Module #
-##########
+import pytest
+
 from transfocate.calculator import Calculator
+
 from .conftest import FakeLens
 
 
 @pytest.fixture(scope='function')
 def calculator():
     # Prefocus lenses
     prefocus = [FakeLens(500., 100.0, 50.),
```

### Comparing `transfocate-0.5.5/transfocate/tests/test_lens.py` & `transfocate-0.5.7/transfocate/tests/test_lens.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,19 @@
-############
-# Standard #
-############
-
-###############
-# Third Party #
-###############
 import numpy as np
 
-##########
-# Module #
-##########
 
 def test_lens_properties(lens):
     assert np.isclose(500.0, lens.radius, atol=0.1)
-    assert np.isclose(100.0, lens.z,      atol=0.1)
-    assert np.isclose(50.0,  lens.focus,  atol=0.1)
+    assert np.isclose(100.0, lens.z, atol=0.1)
+    assert np.isclose(50.0, lens.focus, atol=0.1)
 
 
 def test_image_from_obj(lens):
     # Real image
-    assert np.isclose(lens.image_from_obj(0.0),  200.0, atol=0.1)
+    assert np.isclose(lens.image_from_obj(0.0), 200.0, atol=0.1)
     # Imaginary image
     assert np.isclose(lens.image_from_obj(75.0), 50.0, atol=0.1)
 
 
 def test_lens_state(lens):
     # Inserted Lens
     lens._removed.sim_put(0)
@@ -47,15 +37,15 @@
 
 
 def test_lens_connect_effective_radius(array):
     assert np.isclose(array.effective_radius, 250, atol=0.1)
 
 
 def test_lens_connect_image(array):
-    assert np.isclose(array.image(0.0),  312.5,   atol=0.1)
+    assert np.isclose(array.image(0.0), 312.5, atol=0.1)
     assert np.isclose(array.image(75.0), 303.125, atol=0.1)
     assert np.isclose(array.image(80.0), 303.409, atol=0.1)
     assert np.isclose(array.image(125.0), 304.6875, atol=0.1)
 
 
 def test_number_of_lenses(array):
     assert array.nlens == 2
```

### Comparing `transfocate-0.5.5/transfocate/tests/test_transfocate.py` & `transfocate-0.5.7/transfocate/tests/test_transfocate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 
-from ophyd.sim import make_fake_device
-import pytest
 import numpy as np
+import pytest
+from ophyd.sim import make_fake_device
 
-from transfocate.transfocator import Transfocator, constant_energy, TransfocatorEnergyInterrupt
+from transfocate.transfocator import (Transfocator,
+                                      TransfocatorEnergyInterrupt,
+                                      constant_energy)
 
 logger = logging.getLogger(__name__)
 
 
 # Utility functions for manipulating simulated lenses
 def insert(lens):
     lens._removed.sim_put(0)
```

### Comparing `transfocate-0.5.5/transfocate/transfocator.py` & `transfocate-0.5.7/transfocate/transfocator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import math
 import logging
+import math
+from functools import wraps
 
-from pcdsdevices.device_types import IMS
-from ophyd import Device, EpicsSignalRO, Component as Cpt, FormattedComponent, EpicsSignal
+from ophyd import Component as Cpt
+from ophyd import Device, EpicsSignal, EpicsSignalRO, FormattedComponent
 from ophyd.status import wait as status_wait
+from pcdsdevices.device_types import IMS
 
-from .lens import Lens, LensConnect, LensTripLimits
 from .calculator import Calculator
-from functools import wraps
+from .lens import Lens, LensConnect, LensTripLimits
 
 logger = logging.getLogger(__name__)
 
 
 class TransfocatorInterlock(Device):
     """
     Device containing signals pertinent to the interlock system.
@@ -32,57 +33,57 @@
         doc="Bypass in use?",
     )
     bypass_energy = Cpt(
         EpicsSignal, ":BYPASS:ENERGY",
         doc="Bypass energy",
     )
     ioc_alive = Cpt(
-        EpicsSignalRO, ":BEAM:ALIVE", # string=True,
+        EpicsSignalRO, ":BEAM:ALIVE",  # string=True,
         doc="IOC alive [active]"
     )
     faulted = Cpt(
-        EpicsSignalRO, ":BEAM:FAULTED", # string=True,
+        EpicsSignalRO, ":BEAM:FAULTED",  # string=True,
         doc="Fault currently active [active]"
     )
     state_fault = Cpt(
-        EpicsSignalRO, ":BEAM:UNKNOWN", # string=True,
+        EpicsSignalRO, ":BEAM:UNKNOWN",  # string=True,
         doc="Lens position unknown [active]"
     )
 
     violated_fault = Cpt(
-        EpicsSignalRO, ":BEAM:VIOLATED", # string=True,
+        EpicsSignalRO, ":BEAM:VIOLATED",  # string=True,
         doc="Summary fault due to energy/lens combination [active]"
     )
     min_fault = Cpt(
-        EpicsSignalRO, ":BEAM:MIN_FAULT", # string=True,
+        EpicsSignalRO, ":BEAM:MIN_FAULT",  # string=True,
         doc="Minimum required energy not met for lens combination [active]"
     )
     lens_required_fault = Cpt(
-        EpicsSignalRO, ":BEAM:REQ_TFS_FAULT", # string=True,
+        EpicsSignalRO, ":BEAM:REQ_TFS_FAULT",  # string=True,
         doc="Transfocator lens required for energy/lens combination [active]"
     )
     table_fault = Cpt(
-        EpicsSignalRO, ":BEAM:TAB_FAULT", # string=True,
+        EpicsSignalRO, ":BEAM:TAB_FAULT",  # string=True,
         doc="Effective radius in table-based disallowed area [active]"
     )
 
     violated_fault_latch = Cpt(
-        EpicsSignalRO, ":BEAM:VIOLATED_LT", # string=True,
+        EpicsSignalRO, ":BEAM:VIOLATED_LT",  # string=True,
         doc="Summary fault due to energy/lens combination [latched]"
     )
     min_fault_latch = Cpt(
-        EpicsSignalRO, ":BEAM:MIN_FAULT_LT", # string=True,
+        EpicsSignalRO, ":BEAM:MIN_FAULT_LT",  # string=True,
         doc="Minimum required energy not met for lens combination [latched]"
     )
     lens_required_fault_latch = Cpt(
-        EpicsSignalRO, ":BEAM:REQ_TFS_FAULT_LT", # string=True,
+        EpicsSignalRO, ":BEAM:REQ_TFS_FAULT_LT",  # string=True,
         doc="Transfocator lens required for energy/lens combination [latched]"
     )
     table_fault_latch = Cpt(
-        EpicsSignalRO, ":BEAM:TAB_FAULT_LT", # string=True,
+        EpicsSignalRO, ":BEAM:TAB_FAULT_LT",  # string=True,
         doc="Effective radius in table-based disallowed area [latched]"
     )
 
 
 class Transfocator(Device):
     """
     Class to represent the MFX Transfocator
```

