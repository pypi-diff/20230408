# Comparing `tmp/path4gmns-0.9.2.tar.gz` & `tmp/path4gmns-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\path4gmns-0.9.2.tar", last modified: Tue Mar 14 23:16:45 2023, max compression
+gzip compressed data, was "dist\path4gmns-0.9.3.tar", last modified: Sat Apr  8 19:20:02 2023, max compression
```

## Comparing `path4gmns-0.9.2.tar` & `path4gmns-0.9.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 23:16:45.000000 path4gmns-0.9.2/
--rw-rw-rw-   0        0        0    13320 2023-03-14 23:16:45.000000 path4gmns-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0    11845 2023-03-14 23:13:53.000000 path4gmns-0.9.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-14 23:16:45.000000 path4gmns-0.9.2/path4gmns/
--rw-rw-rw-   0        0        0      255 2023-02-17 15:05:21.000000 path4gmns-0.9.2/path4gmns/__init__.py
--rw-rw-rw-   0        0        0    15232 2022-10-15 19:45:41.000000 path4gmns-0.9.2/path4gmns/accessibility.py
-drwxrwxrwx   0        0        0        0 2023-03-14 23:16:45.000000 path4gmns-0.9.2/path4gmns/bin/
--rw-rw-rw-   0        0        0   181248 2022-11-26 20:04:13.000000 path4gmns-0.9.2/path4gmns/bin/DTALite.dll
--rw-rw-rw-   0        0        0   225704 2022-11-26 20:04:13.000000 path4gmns-0.9.2/path4gmns/bin/DTALite.so
--rw-rw-rw-   0        0        0   250141 2022-11-26 20:04:13.000000 path4gmns-0.9.2/path4gmns/bin/DTALite_arm.dylib
--rw-rw-rw-   0        0        0   269200 2022-11-26 20:04:13.000000 path4gmns-0.9.2/path4gmns/bin/DTALite_x86.dylib
--rw-rw-rw-   0        0        0    11264 2023-03-06 00:36:00.000000 path4gmns-0.9.2/path4gmns/bin/path_engine.dll
--rw-rw-rw-   0        0        0    12208 2023-03-06 01:22:07.000000 path4gmns-0.9.2/path4gmns/bin/path_engine.so
--rw-rw-rw-   0        0        0    33553 2023-03-06 02:23:29.000000 path4gmns-0.9.2/path4gmns/bin/path_engine_arm.dylib
--rw-rw-rw-   0        0        0    49560 2023-03-06 00:33:22.000000 path4gmns-0.9.2/path4gmns/bin/path_engine_x86.dylib
--rw-rw-rw-   0        0        0    60618 2023-03-14 21:43:43.000000 path4gmns-0.9.2/path4gmns/classes.py
--rw-rw-rw-   0        0        0    11086 2023-03-14 21:43:56.000000 path4gmns-0.9.2/path4gmns/colgen.py
--rw-rw-rw-   0        0        0      467 2022-10-15 19:45:41.000000 path4gmns-0.9.2/path4gmns/consts.py
--rw-rw-rw-   0        0        0     3165 2022-11-26 20:04:13.000000 path4gmns-0.9.2/path4gmns/dtaapi.py
--rw-rw-rw-   0        0        0    14190 2023-03-06 00:33:22.000000 path4gmns-0.9.2/path4gmns/path.py
--rw-rw-rw-   0        0        0     4470 2023-03-06 00:33:22.000000 path4gmns-0.9.2/path4gmns/simulation.py
--rw-rw-rw-   0        0        0    48702 2023-03-13 01:50:02.000000 path4gmns-0.9.2/path4gmns/utils.py
--rw-rw-rw-   0        0        0     8768 2022-10-15 19:45:41.000000 path4gmns-0.9.2/path4gmns/zonesyn.py
-drwxrwxrwx   0        0        0        0 2023-03-14 23:16:45.000000 path4gmns-0.9.2/path4gmns.egg-info/
--rw-rw-rw-   0        0        0    13320 2023-03-14 23:16:45.000000 path4gmns-0.9.2/path4gmns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      608 2023-03-14 23:16:45.000000 path4gmns-0.9.2/path4gmns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 23:16:45.000000 path4gmns-0.9.2/path4gmns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-03-14 23:16:45.000000 path4gmns-0.9.2/path4gmns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-14 23:16:45.000000 path4gmns-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-02-17 15:05:21.000000 path4gmns-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 19:20:02.000000 path4gmns-0.9.3/
+-rw-rw-rw-   0        0        0    13503 2023-04-08 19:20:02.000000 path4gmns-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0    12012 2023-04-08 19:18:37.000000 path4gmns-0.9.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 19:20:02.000000 path4gmns-0.9.3/path4gmns/
+-rw-rw-rw-   0        0        0      255 2023-04-08 19:18:37.000000 path4gmns-0.9.3/path4gmns/__init__.py
+-rw-rw-rw-   0        0        0    15232 2022-10-15 19:45:41.000000 path4gmns-0.9.3/path4gmns/accessibility.py
+drwxrwxrwx   0        0        0        0 2023-04-08 19:20:02.000000 path4gmns-0.9.3/path4gmns/bin/
+-rw-rw-rw-   0        0        0   181248 2022-11-26 20:04:13.000000 path4gmns-0.9.3/path4gmns/bin/DTALite.dll
+-rw-rw-rw-   0        0        0   225704 2022-11-26 20:04:13.000000 path4gmns-0.9.3/path4gmns/bin/DTALite.so
+-rw-rw-rw-   0        0        0   250141 2022-11-26 20:04:13.000000 path4gmns-0.9.3/path4gmns/bin/DTALite_arm.dylib
+-rw-rw-rw-   0        0        0   269200 2022-11-26 20:04:13.000000 path4gmns-0.9.3/path4gmns/bin/DTALite_x86.dylib
+-rw-rw-rw-   0        0        0    11264 2023-03-14 23:21:22.000000 path4gmns-0.9.3/path4gmns/bin/path_engine.dll
+-rw-rw-rw-   0        0        0    12208 2023-03-14 23:21:22.000000 path4gmns-0.9.3/path4gmns/bin/path_engine.so
+-rw-rw-rw-   0        0        0    33553 2023-03-14 23:21:22.000000 path4gmns-0.9.3/path4gmns/bin/path_engine_arm.dylib
+-rw-rw-rw-   0        0        0    49560 2023-03-14 23:21:22.000000 path4gmns-0.9.3/path4gmns/bin/path_engine_x86.dylib
+-rw-rw-rw-   0        0        0    59885 2023-04-08 19:18:37.000000 path4gmns-0.9.3/path4gmns/classes.py
+-rw-rw-rw-   0        0        0    10672 2023-04-08 19:18:37.000000 path4gmns-0.9.3/path4gmns/colgen.py
+-rw-rw-rw-   0        0        0      467 2022-10-15 19:45:41.000000 path4gmns-0.9.3/path4gmns/consts.py
+-rw-rw-rw-   0        0        0     3165 2022-11-26 20:04:13.000000 path4gmns-0.9.3/path4gmns/dtaapi.py
+-rw-rw-rw-   0        0        0    14190 2023-03-14 23:21:22.000000 path4gmns-0.9.3/path4gmns/path.py
+-rw-rw-rw-   0        0        0     4470 2023-03-14 23:21:22.000000 path4gmns-0.9.3/path4gmns/simulation.py
+-rw-rw-rw-   0        0        0    49042 2023-04-08 19:18:37.000000 path4gmns-0.9.3/path4gmns/utils.py
+-rw-rw-rw-   0        0        0     8768 2022-10-15 19:45:41.000000 path4gmns-0.9.3/path4gmns/zonesyn.py
+drwxrwxrwx   0        0        0        0 2023-04-08 19:20:02.000000 path4gmns-0.9.3/path4gmns.egg-info/
+-rw-rw-rw-   0        0        0    13503 2023-04-08 19:20:02.000000 path4gmns-0.9.3/path4gmns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2023-04-08 19:20:02.000000 path4gmns-0.9.3/path4gmns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 19:20:02.000000 path4gmns-0.9.3/path4gmns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-08 19:20:02.000000 path4gmns-0.9.3/path4gmns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-08 19:20:02.000000 path4gmns-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-04-08 19:18:37.000000 path4gmns-0.9.3/setup.py
```

### Comparing `path4gmns-0.9.2/PKG-INFO` & `path4gmns-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 Metadata-Version: 2.1
 Name: path4gmns
-Version: 0.9.2
+Version: 0.9.3
 Summary: An open-source, cross-platform, lightweight, and fast Python                path engine for networks encoded in GMNS
 Home-page: https://github.com/jdlph/PATH4GMNS
 Author: Dr. Xuesong Zhou, Dr. Peiheng Li
 Author-email: xzhou74@asu.edu, jdlph@hotmail.com
 License: Apache License 2.0
 Description: # Path4GMNS
         [![platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-red)](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-red)
-         [![Downloads](https://pepy.tech/badge/path4gmns)](https://pepy.tech/project/path4gmns) [![GitHub release](https://img.shields.io/badge/release-v0.9.2-brightgreen)](https://img.shields.io/badge/release-v0.8.2-brightgreen) ![Read the Docs](https://img.shields.io/readthedocs/path4gmns)
+         [![Downloads](https://pepy.tech/badge/path4gmns)](https://pepy.tech/project/path4gmns) [![GitHub release](https://img.shields.io/badge/release-v0.9.3-brightgreen)](https://img.shields.io/badge/release-v0.8.2-brightgreen) ![Read the Docs](https://img.shields.io/readthedocs/path4gmns)
         
         Path4GMNS is an open-source, cross-platform, lightweight, and fast Python path engine for networks encoded in [GMNS](https://github.com/zephyr-data-specs/GMNS). Besides finding static shortest paths for simple analyses, its main functionality is to provide an efficient and flexible framework for column-based (path-based) modeling and applications in transportation (e.g., activity-based demand modeling). Path4GMNS supports, in short,
         
         1. finding (static) shortest path between two nodes,
-        2. constructing shortest paths for all individual agents,
-        3. performing path-based User-Equilibrium (UE) traffic assignment,
-        4. conducting dynamic traffic assignment (DTA) after UE.
-        5. evaluating multimodal accessibility and equity,
-        6. synthesizing zones and Origin-Destination (OD) demand for a given network.
+        2. performing path-based User-Equilibrium (UE) traffic assignment,
+        3. conducting dynamic traffic assignment (DTA) after UE.
+        4. evaluating multimodal accessibility and equity,
+        5. synthesizing zones and Origin-Destination (OD) demand for a given network.
         
         Path4GMNS also serves as an API to the C++-based [DTALite](https://github.com/jdlph/DTALite) to conduct various multimodal traffic assignments including,
            * Link-based UE,
            * Path-based UE,
            * UE + DTA,
            * OD Matrix Estimation (ODME).
         
         ![Architecture](/docs/source/imgs/architecture.png)
         
         ## Installation
-        Path4GMNS has been published on [PyPI](https://pypi.org/project/path4gmns/0.9.2/), and can be installed using
+        Path4GMNS has been published on [PyPI](https://pypi.org/project/path4gmns/0.9.3/), and can be installed using
         ```
         $ pip install path4gmns
         ```
-        If you need a specific version of Path4GMNS, say, 0.9.2,
+        If you need a specific version of Path4GMNS, say, 0.9.3,
         ```
-        $ pip install path4gmns==0.9.2
+        $ pip install path4gmns==0.9.3
         ```
         
-        v0.9.2 improves the performance with faster and better UE convergency along with bug fix on loading columns. Please **update to or install the latest version** and **discard all old versions**.
+        v0.9.3 fixes the bug on handling link capacity reduction in traffic assignment and remove dependency on read_demand() for loading columns. Please **update to or install the latest version** and **discard all old versions**.
         
         ### Dependency
         The Python modules are written in **Python 3.x**, which is the minimum requirement to explore the most of Path4GMNS. Some of its functions require further run-time support, which we will go through along with the corresponding **[Use Cases](https://path4gmns.readthedocs.io/en/latest/)**.
         
         ## Quick Start
         
          We highly recommend that you go through this **[Tutorial](https://github.com/jdlph/Path4GMNS/tree/dev/tests/tutorial.ipynb)** written in Jupyter notebook with step-by-step demonstration using the latest version, no matter you are one of the existing users or new to Path4GMNS. Its documentation is available on **[readthedocs](https://path4gmns.readthedocs.io/en/latest/)**.
@@ -95,28 +94,31 @@
         31. Introduce the simulation module along with a simple traffic simulator using the point queue model and shortest paths (v0.9.0)
         32. Fully optimize the C++ routing engine (v0.9.1)
         33. Use the UE result as routing decisions for simulation (v0.9.1)
         34. Optimize the column generation module with faster and better UE convergency (v0.9.2)
         35. Fix the bug on updating the total system travel time (v0.9.2)
         36. Resolve the potential issue on traversing the last through node in path engine (v0.9.2)
         37. Fix the bug on loading columns where link path and node paths are not in the proper order (v0.9.2)
+        38. FiX the bug on handling link capacity reduction in traffic assignment (v0.9.3)
+        39. Remove dependency on demand.csv for loading columns (v0.9.3)
+        40. Deprecate find_path_for_agents() (v0.9.3)
         
         Detailed update information can be found in [Releases](https://github.com/jdlph/Path4GMNS/releases).
         
         ## Please Contribute
         
         Any contributions are welcomed including advise new applications of Path4GMNS, enhance documentation (this guideline and [docstrings](https://docs.python-guide.org/writing/documentation/#writing-docstrings) in the source code), refactor and/or optimize the source code, report and/or resolve potential issues/bugs, suggest and/or add new functionalities, etc.
         
         Path4GMNS has a very simple workflow setup, i.e., **master for release (on both GitHub and PyPI)** and **dev for development**. If you would like to work directly on the source code (and probably the documentation), please make sure that **the destination branch of your pull request is dev**, i.e., all potential changes/updates shall go to the dev branch before merging into master for release.
         
         You are encouraged to join our [Discord Channel](https://discord.gg/JGFMta7kxZ) and [Gmail group](https://groups.google.com/g/path4gmns) to get the latest update and other information.
         
         ## How to Cite
         
-        Li, P. and Zhou, X. (2023, March 14). *Path4GMNS*. Retrieved from https://github.com/jdlph/Path4GMNS
+        Li, P. and Zhou, X. (2023, April 8). *Path4GMNS*. Retrieved from https://github.com/jdlph/Path4GMNS
         
         ## References
         Lu, C. C., Mahmassani, H. S., Zhou, X. (2009). Equivalent gap function-based reformulation and solution algorithm for the dynamic user equilibrium problem. Transportation Research Part B: Methodological, 43, 345-364.
         
         Jayakrishnan, R., Tsai, W. K., Prashker, J. N., Rajadyaksha, S. (1994). [A Faster Path-Based Algorithm for Traffic Assignment](https://escholarship.org/uc/item/2hf4541x) (Working Paper UCTC No. 191). The University of California Transportation Center.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `path4gmns-0.9.2/README.md` & `path4gmns-0.9.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # Path4GMNS
 [![platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-red)](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-red)
- [![Downloads](https://pepy.tech/badge/path4gmns)](https://pepy.tech/project/path4gmns) [![GitHub release](https://img.shields.io/badge/release-v0.9.2-brightgreen)](https://img.shields.io/badge/release-v0.8.2-brightgreen) ![Read the Docs](https://img.shields.io/readthedocs/path4gmns)
+ [![Downloads](https://pepy.tech/badge/path4gmns)](https://pepy.tech/project/path4gmns) [![GitHub release](https://img.shields.io/badge/release-v0.9.3-brightgreen)](https://img.shields.io/badge/release-v0.8.2-brightgreen) ![Read the Docs](https://img.shields.io/readthedocs/path4gmns)
 
 Path4GMNS is an open-source, cross-platform, lightweight, and fast Python path engine for networks encoded in [GMNS](https://github.com/zephyr-data-specs/GMNS). Besides finding static shortest paths for simple analyses, its main functionality is to provide an efficient and flexible framework for column-based (path-based) modeling and applications in transportation (e.g., activity-based demand modeling). Path4GMNS supports, in short,
 
 1. finding (static) shortest path between two nodes,
-2. constructing shortest paths for all individual agents,
-3. performing path-based User-Equilibrium (UE) traffic assignment,
-4. conducting dynamic traffic assignment (DTA) after UE.
-5. evaluating multimodal accessibility and equity,
-6. synthesizing zones and Origin-Destination (OD) demand for a given network.
+2. performing path-based User-Equilibrium (UE) traffic assignment,
+3. conducting dynamic traffic assignment (DTA) after UE.
+4. evaluating multimodal accessibility and equity,
+5. synthesizing zones and Origin-Destination (OD) demand for a given network.
 
 Path4GMNS also serves as an API to the C++-based [DTALite](https://github.com/jdlph/DTALite) to conduct various multimodal traffic assignments including,
    * Link-based UE,
    * Path-based UE,
    * UE + DTA,
    * OD Matrix Estimation (ODME).
 
 ![Architecture](/docs/source/imgs/architecture.png)
 
 ## Installation
-Path4GMNS has been published on [PyPI](https://pypi.org/project/path4gmns/0.9.2/), and can be installed using
+Path4GMNS has been published on [PyPI](https://pypi.org/project/path4gmns/0.9.3/), and can be installed using
 ```
 $ pip install path4gmns
 ```
-If you need a specific version of Path4GMNS, say, 0.9.2,
+If you need a specific version of Path4GMNS, say, 0.9.3,
 ```
-$ pip install path4gmns==0.9.2
+$ pip install path4gmns==0.9.3
 ```
 
-v0.9.2 improves the performance with faster and better UE convergency along with bug fix on loading columns. Please **update to or install the latest version** and **discard all old versions**.
+v0.9.3 fixes the bug on handling link capacity reduction in traffic assignment and remove dependency on read_demand() for loading columns. Please **update to or install the latest version** and **discard all old versions**.
 
 ### Dependency
 The Python modules are written in **Python 3.x**, which is the minimum requirement to explore the most of Path4GMNS. Some of its functions require further run-time support, which we will go through along with the corresponding **[Use Cases](https://path4gmns.readthedocs.io/en/latest/)**.
 
 ## Quick Start
 
  We highly recommend that you go through this **[Tutorial](https://github.com/jdlph/Path4GMNS/tree/dev/tests/tutorial.ipynb)** written in Jupyter notebook with step-by-step demonstration using the latest version, no matter you are one of the existing users or new to Path4GMNS. Its documentation is available on **[readthedocs](https://path4gmns.readthedocs.io/en/latest/)**.
@@ -87,26 +86,29 @@
 31. Introduce the simulation module along with a simple traffic simulator using the point queue model and shortest paths (v0.9.0)
 32. Fully optimize the C++ routing engine (v0.9.1)
 33. Use the UE result as routing decisions for simulation (v0.9.1)
 34. Optimize the column generation module with faster and better UE convergency (v0.9.2)
 35. Fix the bug on updating the total system travel time (v0.9.2)
 36. Resolve the potential issue on traversing the last through node in path engine (v0.9.2)
 37. Fix the bug on loading columns where link path and node paths are not in the proper order (v0.9.2)
+38. FiX the bug on handling link capacity reduction in traffic assignment (v0.9.3)
+39. Remove dependency on demand.csv for loading columns (v0.9.3)
+40. Deprecate find_path_for_agents() (v0.9.3)
 
 Detailed update information can be found in [Releases](https://github.com/jdlph/Path4GMNS/releases).
 
 ## Please Contribute
 
 Any contributions are welcomed including advise new applications of Path4GMNS, enhance documentation (this guideline and [docstrings](https://docs.python-guide.org/writing/documentation/#writing-docstrings) in the source code), refactor and/or optimize the source code, report and/or resolve potential issues/bugs, suggest and/or add new functionalities, etc.
 
 Path4GMNS has a very simple workflow setup, i.e., **master for release (on both GitHub and PyPI)** and **dev for development**. If you would like to work directly on the source code (and probably the documentation), please make sure that **the destination branch of your pull request is dev**, i.e., all potential changes/updates shall go to the dev branch before merging into master for release.
 
 You are encouraged to join our [Discord Channel](https://discord.gg/JGFMta7kxZ) and [Gmail group](https://groups.google.com/g/path4gmns) to get the latest update and other information.
 
 ## How to Cite
 
-Li, P. and Zhou, X. (2023, March 14). *Path4GMNS*. Retrieved from https://github.com/jdlph/Path4GMNS
+Li, P. and Zhou, X. (2023, April 8). *Path4GMNS*. Retrieved from https://github.com/jdlph/Path4GMNS
 
 ## References
 Lu, C. C., Mahmassani, H. S., Zhou, X. (2009). Equivalent gap function-based reformulation and solution algorithm for the dynamic user equilibrium problem. Transportation Research Part B: Methodological, 43, 345-364.
 
 Jayakrishnan, R., Tsai, W. K., Prashker, J. N., Rajadyaksha, S. (1994). [A Faster Path-Based Algorithm for Traffic Assignment](https://escholarship.org/uc/item/2hf4541x) (Working Paper UCTC No. 191). The University of California Transportation Center.
```

### Comparing `path4gmns-0.9.2/path4gmns/accessibility.py` & `path4gmns-0.9.3/path4gmns/accessibility.py`

 * *Files identical despite different names*

### Comparing `path4gmns-0.9.2/path4gmns/bin/DTALite.dll` & `path4gmns-0.9.3/path4gmns/bin/DTALite.dll`

 * *Files identical despite different names*

### Comparing `path4gmns-0.9.2/path4gmns/bin/DTALite.so` & `path4gmns-0.9.3/path4gmns/bin/DTALite.so`

 * *Files identical despite different names*

### Comparing `path4gmns-0.9.2/path4gmns/bin/DTALite_arm.dylib` & `path4gmns-0.9.3/path4gmns/bin/DTALite_arm.dylib`

 * *Files identical despite different names*

### Comparing `path4gmns-0.9.2/path4gmns/bin/DTALite_x86.dylib` & `path4gmns-0.9.3/path4gmns/bin/DTALite_x86.dylib`

 * *Files identical despite different names*

### Comparing `path4gmns-0.9.2/path4gmns/bin/path_engine.dll` & `path4gmns-0.9.3/path4gmns/bin/path_engine.dll`

 * *Files identical despite different names*

### Comparing `path4gmns-0.9.2/path4gmns/bin/path_engine.so` & `path4gmns-0.9.3/path4gmns/bin/path_engine.so`

 * *Files identical despite different names*

### Comparing `path4gmns-0.9.2/path4gmns/bin/path_engine_arm.dylib` & `path4gmns-0.9.3/path4gmns/bin/path_engine_arm.dylib`

 * *Files identical despite different names*

### Comparing `path4gmns-0.9.2/path4gmns/bin/path_engine_x86.dylib` & `path4gmns-0.9.3/path4gmns/bin/path_engine_x86.dylib`

 * *Files identical despite different names*

### Comparing `path4gmns-0.9.2/path4gmns/classes.py` & `path4gmns-0.9.3/path4gmns/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,41 +162,36 @@
     def get_generalized_cost(self, tau, value_of_time):
         return (
             self.travel_time_by_period[tau]
             + self.route_choice_cost
             + self.toll / max(SMALL_DIVISOR, value_of_time) * 60
         )
 
-    def reset_period_flow_vol(self, tau):
-        self.flow_vol_by_period[tau] = 0
+    def reset_period_flow_vol(self):
+        for tau in range(self.demand_period_size):
+            self.flow_vol_by_period[tau] = 0
 
     def increase_period_flow_vol(self, tau, fv):
         self.flow_vol_by_period[tau] += fv
 
-    def calculate_td_vdf(self, demand_periods=None, iter_num=-1):
-        if demand_periods is None:
-            for tau in range(self.demand_period_size):
-                self.travel_time_by_period[tau] = (
-                    self.vdfperiods[tau].run_bpr(self.flow_vol_by_period[tau])
-                )
-        else:
-            for dp in demand_periods:
-                tau = dp.get_id()
-                reduction_ratio = dp.get_reduction_ratio(self.id, iter_num)
-                self.travel_time_by_period[tau] = (
-                    self.vdfperiods[tau].run_bpr(self.flow_vol_by_period[tau],
-                                                 reduction_ratio)
-                )
+    def calculate_td_vdf(self):
+        for tau in range(self.demand_period_size):
+            self.travel_time_by_period[tau] = (
+                self.vdfperiods[tau].run_bpr(self.flow_vol_by_period[tau])
+            )
 
     def update_waiting_time(self, minute, wt):
         try:
             self.waiting_time[minute] += wt
         except IndexError:
             pass
 
+    def set_capacity_ratio(self, tau, rr):
+        self.vdfperiods[tau].capacity_ratio = rr
+
 
 class Agent:
     """ individual agent derived from aggregated demand between an OD pair
 
     id: integer starts from 1
     seq_no: internal agent index starting from 0 used for calculation
     """
@@ -922,25 +917,20 @@
     @staticmethod
     def get_legacy_name():
         return 'passenger'
 
 
 class SpecialEvent:
 
-    def __init__(self, name, beg_iteration, end_iteration) -> None:
+    def __init__(self, name) -> None:
         self.name = name
-        self.beg_iter = beg_iteration
-        self.end_iter = end_iteration
         self.affected_links = {}
 
-    def get_beg_iteration(self):
-        return self.beg_iter
-
-    def get_end_iteration(self):
-        return self.end_iter
+    def get_affected_links(self):
+        return self.affected_links.items()
 
 
 class DemandPeriod:
 
     def __init__(self, id=0, period='AM', time_period='0700_0800'):
         self.id = id
         self.period = period
@@ -965,32 +955,14 @@
 
     def get_id(self):
         return self.id
 
     def get_period(self):
         return self.period
 
-    def get_beg_iteration(self):
-        return self.special_event.get_beg_iteration()
-
-    def get_end_iteration(self):
-        return self.special_event.get_end_iteration()
-
-    def get_reduction_ratio(self, link_id, iter_num):
-        if self.special_event is None:
-            return 1
-
-        if iter_num < self.get_beg_iteration() - 1 or iter_num > self.get_end_iteration() - 1:
-            return 1
-
-        try:
-            return self.special_event.affected_links[link_id]
-        except KeyError:
-            return 1
-
     def get_duration(self):
         """ duration of demand period in minutes """
         return self.et - self.st
 
     def get_start_time(self):
         return self.st
 
@@ -1029,27 +1001,28 @@
         self.mu = mu
         # free flow travel time
         self.fftt = fftt
         self.capacity = cap
         self.phf = phf
         self.avg_travel_time = 0
         self.voc = 0
+        self.capacity_ratio = 1
 
     def get_avg_travel_time(self):
         return self.avg_travel_time
 
     def get_voc(self):
         return self.voc
 
     def get_fftt(self):
         return self.fftt
 
-    def run_bpr(self, vol, reduction_ratio=1):
+    def run_bpr(self, vol):
         vol = max(0, vol)
-        self.voc = vol / max(SMALL_DIVISOR, self.capacity * reduction_ratio)
+        self.voc = vol / max(SMALL_DIVISOR, self.capacity * self.capacity_ratio)
         self.avg_travel_time = (
             self.fftt
             + self.fftt
             * self.alpha
             * pow(self.voc, self.beta)
         )
 
@@ -1740,14 +1713,23 @@
 
     def set_simu_duration(self, dur):
         self.simu_dur = dur
 
     def set_simu_start_time(self, st):
         self.simu_st = st
 
+    def set_capacity_ratio(self, tau, link_id, r):
+        try:
+            link_no = self.get_link_seq_no(link_id)
+        except KeyError:
+            return
+
+        link = self.get_link(link_no)
+        link.set_capacity_ratio(tau, r)
+
 
 class UI:
     """ an abstract class only with user interfaces """
     def __init__(self, assignment):
         self._base_assignment = assignment
 
     def get_column_pool(self):
@@ -1777,15 +1759,18 @@
         """ return the sequence of link IDs along the agent path """
         return self._base_assignment.get_agent_link_path(agent_id)
 
     def get_ODMatrix(self):
         return self._base_assignment.network.ODMatrix
 
     def find_path_for_agents(self, mode='all'):
-        """ find and set up shortest path for each agent """
+        """ DEPRECATED
+
+        find and set up shortest path for each agent
+        """
         return self._base_assignment.find_path_for_agents(mode)
 
     def find_shortest_path(self, from_node_id, to_node_id,
                            mode='all', seq_type='node'):
         """ return shortest path between from_node_id and to_node_id
 
         Parameters
```

### Comparing `path4gmns-0.9.2/path4gmns/colgen.py` & `path4gmns-0.9.3/path4gmns/colgen.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,34 +19,31 @@
                 break
 
             sp.link_cost_array[link.get_seq_no()] = (
                 link.get_generalized_cost(tau, vot)
             )
 
 
-def _update_link_travel_time(links, demand_periods=None, iter_num=-1):
+def _update_link_travel_time(links):
     for link in links:
         if link.length == 0:
             break
 
-        link.calculate_td_vdf(demand_periods, iter_num)
+        link.calculate_td_vdf()
 
 
-def _update_link_and_column_volume(column_pool, links, demand_periods,
-                                   iter_num, reduce_path_vol = True):
+def _update_link_and_column_volume(column_pool, links, iter_num, reduce_path_vol = True):
     if iter_num == 0:
         return
 
     for link in links:
         if link.length == 0:
             break
 
-        for dp in demand_periods:
-            tau = dp.get_id()
-            link.reset_period_flow_vol(tau)
+        link.reset_period_flow_vol()
 
     for k, cv in column_pool.items():
         # k= (at, tau, oz_id, dz_id)
         tau = k[1]
 
         for col in cv.get_columns():
             path_vol = col.get_volume()
@@ -60,15 +57,15 @@
 
             if reduce_path_vol and not cv.is_route_fixed():
                 col.vol *= iter_num / (iter_num + 1)
 
 
 def _update_column_gradient_cost_and_flow(column_pool, links, agent_types, iter_num):
     total_gap = 0
-    total_travel_time = 0
+    total_sys_travel_time = 0
 
     for k, cv in column_pool.items():
         # k= (at, tau, oz_id, dz_id)
         vot = agent_types[k[0]].get_vot()
         tau = k[1]
 
         least_gradient_cost = MAX_LABEL_COST
@@ -90,15 +87,15 @@
             for col in cv.get_columns():
                 if col.get_id() == least_gradient_cost_path_id:
                     continue
 
                 col.update_gradient_cost_diffs(least_gradient_cost)
 
                 total_gap += col.get_gap()
-                total_travel_time += col.get_sys_travel_time()
+                total_sys_travel_time += col.get_sys_travel_time()
 
                 step_size = 1 / (iter_num + 2) * cv.get_od_volume()
                 previous_path_vol = col.get_volume()
 
                 vol = max(
                     0,
                     (previous_path_vol
@@ -109,54 +106,54 @@
                 col.set_volume(vol)
                 total_switched_out_path_vol += (
                     previous_path_vol - vol
                 )
 
         if least_gradient_cost_path_id != -1:
             col = cv.get_column(least_gradient_cost_path_id)
-            total_travel_time += col.get_sys_travel_time()
+            total_sys_travel_time += col.get_sys_travel_time()
             col.increase_volume(total_switched_out_path_vol)
 
-    rel_gap = total_gap / max(total_travel_time, SMALL_DIVISOR)
+    rel_gap = total_gap / max(total_sys_travel_time, SMALL_DIVISOR)
 
     print(f'current iteration number in column update: {iter_num}\n'
           f'total gap: {total_gap:.2f}; relative gap: {rel_gap:.4%}')
 
 
 def _backtrace_shortest_path_tree(centroid,
                                   centroids,
                                   links,
                                   node_preds,
                                   link_preds,
-                                  agent_type,
-                                  demand_period,
+                                  at_id,
+                                  dp_id,
                                   column_pool,
                                   iter_num):
 
     if not centroid.has_outgoing_links():
         return
 
     oz_id = centroid.get_zone_id()
     k_path_prob = 1 / (iter_num + 1)
 
     for c in centroids:
         dz_id = c.get_zone_id()
         if dz_id == oz_id:
             continue
 
-        if (agent_type, demand_period, oz_id, dz_id) not in column_pool.keys():
+        if (at_id, dp_id, oz_id, dz_id) not in column_pool.keys():
             continue
 
-        cv = column_pool[(agent_type, demand_period, oz_id, dz_id)]
+        cv = column_pool[(at_id, dp_id, oz_id, dz_id)]
         if cv.is_route_fixed():
             continue
 
         link_path = []
-
         dist = 0
+
         curr_node_seq_no = c.get_node_no()
         # retrieve the sequence backwards
         while curr_node_seq_no >= 0:
             curr_link_seq_no = link_preds[curr_node_seq_no]
             if curr_link_seq_no >= 0:
                 link_path.append(curr_link_seq_no)
                 dist += links[curr_link_seq_no].length
@@ -276,52 +273,48 @@
     # base assignment
     A = ui._base_assignment
     # set up SPNetwork
     A.setup_spnetwork()
 
     links = A.get_links()
     ats = A.get_agent_types()
-    dps = A.get_demand_periods()
     column_pool = A.get_column_pool()
 
     st = time()
 
     for i in range(column_gen_num):
         print(f'current iteration number in column generation: {i}')
 
-        _update_link_and_column_volume(column_pool, links, dps, i)
-        _update_link_travel_time(links, dps, i)
+        _update_link_and_column_volume(column_pool, links, i)
+        _update_link_travel_time(links)
         # update generalized link cost before assignment
         _update_link_cost_array(A.get_spnetworks())
         # loop through all centroids on the base network
         _generate_column_pool(A.get_spnetworks(), column_pool, i)
 
     print(f'\nprocessing time of generating columns: {time()-st:.2f} s\n')
 
     for i in range(column_update_num):
-        _update_link_and_column_volume(column_pool, links, dps, i, False)
-        _update_link_travel_time(links)
         _update_column_gradient_cost_and_flow(column_pool, links, ats, i)
+        _update_link_and_column_volume(column_pool, links, i + 1, False)
+        _update_link_travel_time(links)
 
     # postprocessing
-    _update_link_and_column_volume(column_pool, links, dps, column_gen_num, False)
-    _update_link_travel_time(links)
     _update_column_attributes(column_pool, links)
 
 
 def update_links_using_columns(network):
     """ a helper function for load_columns() """
     A = network._base_assignment
 
     column_pool = A.get_column_pool()
     links = A.get_links()
-    dps = A.get_demand_periods()
 
     # do not update column volume
-    _update_link_and_column_volume(column_pool, links, dps, 1, False)
+    _update_link_and_column_volume(column_pool, links, 1, False)
     _update_link_travel_time(links)
 
 
 def perform_network_assignment(assignment_mode, column_gen_num, column_update_num, ui):
     """DEPRECATED Column Generation API
 
     Keep it here as legacy support for existing users who already get used to it
```

### Comparing `path4gmns-0.9.2/path4gmns/dtaapi.py` & `path4gmns-0.9.3/path4gmns/dtaapi.py`

 * *Files identical despite different names*

### Comparing `path4gmns-0.9.2/path4gmns/path.py` & `path4gmns-0.9.3/path4gmns/path.py`

 * *Files identical despite different names*

### Comparing `path4gmns-0.9.2/path4gmns/simulation.py` & `path4gmns-0.9.3/path4gmns/simulation.py`

 * *Files identical despite different names*

### Comparing `path4gmns-0.9.2/path4gmns/utils.py` & `path4gmns-0.9.3/path4gmns/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -545,15 +545,15 @@
         print('read '+file)
 
         at = agent_type_id
         dp = demand_period_id
         column_pool.clear()
 
         reader = csv.DictReader(fp)
-        total_agents = 0
+        total_vol = 0
         for line in reader:
             # invalid origin zone id, discard it
             try:
                 oz_id = _convert_str_to_int(line['o_zone_id'])
             except InvalidRecord:
                 continue
 
@@ -584,19 +584,19 @@
                 continue
 
             # set up volume for ColumnVec
             if (at, dp, oz_id, dz_id) not in column_pool.keys():
                 column_pool[(at, dp, oz_id, dz_id)] = ColumnVec()
             column_pool[(at, dp, oz_id, dz_id)].increase_volume(volume)
 
-            total_agents += int(volume + 1)
+            total_vol += volume
 
-        print(f'the number of agents is {total_agents}')
+        print(f'the total demand is {total_vol:.2f}')
 
-        if total_agents == 0:
+        if total_vol == 0:
             raise Exception(
                 'NO VALID OD VOLUME!! Double check your demand.csv and '
                 'make sure there is zone info in node.csv'
             )
 
 
 def load_demand(ui,
@@ -826,22 +826,20 @@
                     s = d['special_event']
                     enable = s['enable']
                     # no need to set up a special event if it is off
                     if not enable:
                         raise KeyError
 
                     name = s['name']
-                    beg_iter = s['beg_iteration']
-                    end_iter = s['end_iteration']
-                    se = SpecialEvent(name, beg_iter, end_iter)
+                    se = SpecialEvent(name)
 
                     links = s['affected_links']
                     for link in links:
                         link_id = str(link['link_id'])
-                        ratio = link['reduction_ratio']
+                        ratio = link['capacity_ratio']
                         se.affected_links[link_id] = ratio
 
                     dp.special_event = se
                 except KeyError:
                     pass
 
                 assignment.update_demand_periods(dp)
@@ -950,25 +948,38 @@
                         at,
                         dp,
                         network.zones,
                         assignm.column_pool)
 
     network.update()
     assignm.network = network
+
+    if load_demand:
+        # set up capacity ratio of affected links from special event
+        for dp in assignm.demand_periods:
+            se = dp.special_event
+            if se is None:
+                continue
+
+            # k is link id and v is capacity ratio
+            for k, v in se.get_affected_links():
+                assignm.set_capacity_ratio(dp.get_id(), k, v)
+
     ui = UI(assignm)
 
     return ui
 
 
 def load_columns(ui, input_dir='.'):
     """ developer note: do we use agent.csv to set up network? """
     with open(input_dir+'/agent.csv', 'r') as f:
         print('read agent.csv')
 
         A = ui._base_assignment
+        cp = A.get_column_pool()
 
         reader = csv.DictReader(f)
 
         # just in case agent_id was not output
         last_agent_id = 0
         for line in reader:
             # critical info
@@ -1044,16 +1055,16 @@
                 dist = _convert_str_to_float(line['distance'])
             except InvalidRecord:
                 dist = 0
 
             # it could be empty
             geo = line['geometry']
 
-            if (at, dp, oz_id, dz_id) not in A.get_column_pool().keys():
-                continue
+            if (at, dp, oz_id, dz_id) not in cp.keys():
+                cp[(at, dp, oz_id, dz_id)] = ColumnVec()
 
             cv = A.get_column_vec(at, dp, oz_id, dz_id)
             path_id = cv.get_column_num()
             col = Column(path_id)
 
             try:
                 col.nodes = [A.get_node_no(int(x)) for x in reversed(node_seq.split(';')) if x]
@@ -1099,14 +1110,15 @@
                     col_.increase_volume(vol)
                     existing = True
                     break
 
             if not existing:
                 col.set_distance(dist)
                 cv.add_new_column(col)
+                cv.increase_volume(vol)
 
         update_links_using_columns(ui)
 
 
 def output_columns(ui, output_geometry=True, output_dir='.'):
     with open(output_dir+'/agent.csv', 'w',  newline='') as fp:
         base = ui._base_assignment
```

### Comparing `path4gmns-0.9.2/path4gmns/zonesyn.py` & `path4gmns-0.9.3/path4gmns/zonesyn.py`

 * *Files identical despite different names*

### Comparing `path4gmns-0.9.2/path4gmns.egg-info/PKG-INFO` & `path4gmns-0.9.3/path4gmns.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 Metadata-Version: 2.1
 Name: path4gmns
-Version: 0.9.2
+Version: 0.9.3
 Summary: An open-source, cross-platform, lightweight, and fast Python                path engine for networks encoded in GMNS
 Home-page: https://github.com/jdlph/PATH4GMNS
 Author: Dr. Xuesong Zhou, Dr. Peiheng Li
 Author-email: xzhou74@asu.edu, jdlph@hotmail.com
 License: Apache License 2.0
 Description: # Path4GMNS
         [![platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-red)](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-red)
-         [![Downloads](https://pepy.tech/badge/path4gmns)](https://pepy.tech/project/path4gmns) [![GitHub release](https://img.shields.io/badge/release-v0.9.2-brightgreen)](https://img.shields.io/badge/release-v0.8.2-brightgreen) ![Read the Docs](https://img.shields.io/readthedocs/path4gmns)
+         [![Downloads](https://pepy.tech/badge/path4gmns)](https://pepy.tech/project/path4gmns) [![GitHub release](https://img.shields.io/badge/release-v0.9.3-brightgreen)](https://img.shields.io/badge/release-v0.8.2-brightgreen) ![Read the Docs](https://img.shields.io/readthedocs/path4gmns)
         
         Path4GMNS is an open-source, cross-platform, lightweight, and fast Python path engine for networks encoded in [GMNS](https://github.com/zephyr-data-specs/GMNS). Besides finding static shortest paths for simple analyses, its main functionality is to provide an efficient and flexible framework for column-based (path-based) modeling and applications in transportation (e.g., activity-based demand modeling). Path4GMNS supports, in short,
         
         1. finding (static) shortest path between two nodes,
-        2. constructing shortest paths for all individual agents,
-        3. performing path-based User-Equilibrium (UE) traffic assignment,
-        4. conducting dynamic traffic assignment (DTA) after UE.
-        5. evaluating multimodal accessibility and equity,
-        6. synthesizing zones and Origin-Destination (OD) demand for a given network.
+        2. performing path-based User-Equilibrium (UE) traffic assignment,
+        3. conducting dynamic traffic assignment (DTA) after UE.
+        4. evaluating multimodal accessibility and equity,
+        5. synthesizing zones and Origin-Destination (OD) demand for a given network.
         
         Path4GMNS also serves as an API to the C++-based [DTALite](https://github.com/jdlph/DTALite) to conduct various multimodal traffic assignments including,
            * Link-based UE,
            * Path-based UE,
            * UE + DTA,
            * OD Matrix Estimation (ODME).
         
         ![Architecture](/docs/source/imgs/architecture.png)
         
         ## Installation
-        Path4GMNS has been published on [PyPI](https://pypi.org/project/path4gmns/0.9.2/), and can be installed using
+        Path4GMNS has been published on [PyPI](https://pypi.org/project/path4gmns/0.9.3/), and can be installed using
         ```
         $ pip install path4gmns
         ```
-        If you need a specific version of Path4GMNS, say, 0.9.2,
+        If you need a specific version of Path4GMNS, say, 0.9.3,
         ```
-        $ pip install path4gmns==0.9.2
+        $ pip install path4gmns==0.9.3
         ```
         
-        v0.9.2 improves the performance with faster and better UE convergency along with bug fix on loading columns. Please **update to or install the latest version** and **discard all old versions**.
+        v0.9.3 fixes the bug on handling link capacity reduction in traffic assignment and remove dependency on read_demand() for loading columns. Please **update to or install the latest version** and **discard all old versions**.
         
         ### Dependency
         The Python modules are written in **Python 3.x**, which is the minimum requirement to explore the most of Path4GMNS. Some of its functions require further run-time support, which we will go through along with the corresponding **[Use Cases](https://path4gmns.readthedocs.io/en/latest/)**.
         
         ## Quick Start
         
          We highly recommend that you go through this **[Tutorial](https://github.com/jdlph/Path4GMNS/tree/dev/tests/tutorial.ipynb)** written in Jupyter notebook with step-by-step demonstration using the latest version, no matter you are one of the existing users or new to Path4GMNS. Its documentation is available on **[readthedocs](https://path4gmns.readthedocs.io/en/latest/)**.
@@ -95,28 +94,31 @@
         31. Introduce the simulation module along with a simple traffic simulator using the point queue model and shortest paths (v0.9.0)
         32. Fully optimize the C++ routing engine (v0.9.1)
         33. Use the UE result as routing decisions for simulation (v0.9.1)
         34. Optimize the column generation module with faster and better UE convergency (v0.9.2)
         35. Fix the bug on updating the total system travel time (v0.9.2)
         36. Resolve the potential issue on traversing the last through node in path engine (v0.9.2)
         37. Fix the bug on loading columns where link path and node paths are not in the proper order (v0.9.2)
+        38. FiX the bug on handling link capacity reduction in traffic assignment (v0.9.3)
+        39. Remove dependency on demand.csv for loading columns (v0.9.3)
+        40. Deprecate find_path_for_agents() (v0.9.3)
         
         Detailed update information can be found in [Releases](https://github.com/jdlph/Path4GMNS/releases).
         
         ## Please Contribute
         
         Any contributions are welcomed including advise new applications of Path4GMNS, enhance documentation (this guideline and [docstrings](https://docs.python-guide.org/writing/documentation/#writing-docstrings) in the source code), refactor and/or optimize the source code, report and/or resolve potential issues/bugs, suggest and/or add new functionalities, etc.
         
         Path4GMNS has a very simple workflow setup, i.e., **master for release (on both GitHub and PyPI)** and **dev for development**. If you would like to work directly on the source code (and probably the documentation), please make sure that **the destination branch of your pull request is dev**, i.e., all potential changes/updates shall go to the dev branch before merging into master for release.
         
         You are encouraged to join our [Discord Channel](https://discord.gg/JGFMta7kxZ) and [Gmail group](https://groups.google.com/g/path4gmns) to get the latest update and other information.
         
         ## How to Cite
         
-        Li, P. and Zhou, X. (2023, March 14). *Path4GMNS*. Retrieved from https://github.com/jdlph/Path4GMNS
+        Li, P. and Zhou, X. (2023, April 8). *Path4GMNS*. Retrieved from https://github.com/jdlph/Path4GMNS
         
         ## References
         Lu, C. C., Mahmassani, H. S., Zhou, X. (2009). Equivalent gap function-based reformulation and solution algorithm for the dynamic user equilibrium problem. Transportation Research Part B: Methodological, 43, 345-364.
         
         Jayakrishnan, R., Tsai, W. K., Prashker, J. N., Rajadyaksha, S. (1994). [A Faster Path-Based Algorithm for Traffic Assignment](https://escholarship.org/uc/item/2hf4541x) (Working Paper UCTC No. 191). The University of California Transportation Center.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `path4gmns-0.9.2/path4gmns.egg-info/SOURCES.txt` & `path4gmns-0.9.3/path4gmns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `path4gmns-0.9.2/setup.py` & `path4gmns-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="path4gmns",
-    version="0.9.2",
+    version="0.9.3",
     author="Dr. Xuesong Zhou, Dr. Peiheng Li",
     author_email="xzhou74@asu.edu, jdlph@hotmail.com",
     description="An open-source, cross-platform, lightweight, and fast Python\
                 path engine for networks encoded in GMNS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jdlph/PATH4GMNS",
```

