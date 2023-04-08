# Comparing `tmp/qctrl_experiment_scheduler-0.1.2.tar.gz` & `tmp/qctrl_experiment_scheduler-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_experiment_scheduler-0.1.2.tar", max compression
+gzip compressed data, was "qctrl_experiment_scheduler-0.2.0.tar", max compression
```

## Comparing `qctrl_experiment_scheduler-0.1.2.tar` & `qctrl_experiment_scheduler-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    36653 2023-03-06 03:32:26.104410 qctrl_experiment_scheduler-0.1.2/LICENSE
--rw-r--r--   0        0        0      176 2023-03-06 03:32:26.104410 qctrl_experiment_scheduler-0.1.2/README.md
--rw-r--r--   0        0        0     2908 2023-03-06 03:32:40.224667 qctrl_experiment_scheduler-0.1.2/pyproject.toml
--rwxr-xr-x   0        0        0     1181 2023-03-06 03:32:40.232668 qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/__init__.py
--rwxr-xr-x   0        0        0    18594 2023-03-06 03:32:26.108410 qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/graph.py
--rw-r--r--   0        0        0     8557 2023-03-06 03:32:26.108410 qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/graph_traversal.py
--rw-r--r--   0        0        0    11004 2023-03-06 03:32:26.108410 qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/node.py
--rwxr-xr-x   0        0        0      990 2023-03-06 03:32:40.236668 qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/predefined/__init__.py
--rw-r--r--   0        0        0    20987 2023-03-06 03:32:26.108410 qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/predefined/amplitude_calibration.py
--rw-r--r--   0        0        0    16619 2023-03-06 03:32:26.108410 qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/predefined/simulation_backend.py
--rw-r--r--   0        0        0     7209 2023-03-06 03:32:26.108410 qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/variable.py
--rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 qctrl_experiment_scheduler-0.1.2/setup.py
--rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 qctrl_experiment_scheduler-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-04-07 23:09:17.455388 qctrl_experiment_scheduler-0.2.0/LICENSE
+-rw-r--r--   0        0        0      176 2023-04-07 23:09:17.455388 qctrl_experiment_scheduler-0.2.0/README.md
+-rw-r--r--   0        0        0     2674 2023-04-07 23:09:38.867300 qctrl_experiment_scheduler-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1181 2023-04-07 23:09:38.879299 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/__init__.py
+-rwxr-xr-x   0        0        0    18587 2023-04-07 23:09:17.459388 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/graph.py
+-rw-r--r--   0        0        0     8557 2023-04-07 23:09:17.459388 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/graph_traversal.py
+-rw-r--r--   0        0        0    11004 2023-04-07 23:09:17.459388 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/node.py
+-rwxr-xr-x   0        0        0      990 2023-04-07 23:09:38.875300 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/predefined/__init__.py
+-rw-r--r--   0        0        0    20987 2023-04-07 23:09:17.459388 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/predefined/amplitude_calibration.py
+-rw-r--r--   0        0        0    16619 2023-04-07 23:09:17.459388 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/predefined/simulation_backend.py
+-rw-r--r--   0        0        0     7209 2023-04-07 23:09:17.459388 qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/variable.py
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 qctrl_experiment_scheduler-0.2.0/setup.py
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 qctrl_experiment_scheduler-0.2.0/PKG-INFO
```

### Comparing `qctrl_experiment_scheduler-0.1.2/LICENSE` & `qctrl_experiment_scheduler-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_experiment_scheduler-0.1.2/pyproject.toml` & `qctrl_experiment_scheduler-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-experiment-scheduler"
-version = "0.1.2"
+version = "0.2.0"
 description = "Q-CTRL Experiment Scheduler"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
@@ -42,15 +42,14 @@
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Visualization",
@@ -65,39 +64,32 @@
 LinkedIn = "https://www.linkedin.com/company/q-ctrl/"
 Facebook = "https://www.facebook.com/qctrl"
 Twitter = "https://twitter.com/qctrlHQ"
 YouTube = "https://www.youtube.com/qctrl"
 GitHub = "https://github.com/qctrl"
 
 [tool.poetry.dependencies]
-python = ">=3.7.2, <3.12"
-numpy = [
-    {version = "^1.21.6", python = ">=3.7.2, <3.8"},
-    {version = "^1.23.5", python = ">=3.8, <3.12"}
-]
-networkx = [
-    {version = "~2.6", python = ">=3.7.2, <3.8"},
-    {version = "^3.0", python = ">=3.8"}
-]
-qctrl = "^21.0.0"
-qctrl-commons = "^17.9.1"
-qctrl-visualizer = "^4.5.0"
+python = ">=3.8, <3.12"
+numpy = "^1.23.5"
+networkx = "^2.7"
+qctrl = "^22.0.0"
+qctrl-commons = "^18.0.0"
+qctrl-visualizer = "^5.0.0"
 
 [tool.poetry.dev-dependencies]
-mypy = "^0.991"
-black = "^22.12.0"
-isort = "^5.7.0"
+black = "^23.1.0"
+isort = "^5.12.0"
+mypy = "^1.1.1"
 pre-commit = "^2.9.3"
-pytest = "^7.1.1"
+pylint = "^2.17.1"
+pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
-pylint = "^2.16.2"
-sphinx = "~5.1.0"
-sphinx-reredirects = "^0.0.1"
 qctrl-sphinx-theme = "~0.1.2"
-
+sphinx = "^5.0.0"
+sphinx-reredirects = "^0.0.1"
 
 [tool.black]
 exclude = '''
 (
   /(
     | \.github
     | docs
```

### Comparing `qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/__init__.py` & `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 """
 Q-CTRL Experiment Scheduler
 """
 
-__version__ = "0.1.2"
+__version__ = "0.2.0"
 __author__ = "Q-CTRL <support@q-ctrl.com>"
 
 from qctrlexperimentscheduler.graph import (
     CalibrationGraph,
     CalibrationProtocol,
 )
 from qctrlexperimentscheduler.graph_traversal import Verbosity
```

### Comparing `qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/graph.py` & `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,35 +341,35 @@
         )
 
         return self._variables[name]
 
     def execute(
         self,
         node: CalibrationNode,
-        protocol: CalibrationProtocol = CalibrationProtocol.OPTIMUS,
+        protocol: CalibrationProtocol = CalibrationProtocol.WAVE,
         verbosity: Verbosity = Verbosity.QUIET,
     ):
         """
         Execute calibrations in a graph in sequence, with the intention of
         keeping the selected node in a calibrated state.
 
         Parameters
         ----------
         node : CalibrationNode
             The node that you want to keep to calibrated.
         protocol : CalibrationProtocol, optional
             The algorithm used to traverse the calibration graph. By default,
-            this function uses a modified version of the Optimus algorithm [1]_.
+            this function uses a modified version of the Wave algorithm [1]_.
         verbosity : Verbosity, optional
             The verbosity level of this run. Defaults to QUIET.
 
         References
         ----------
-        .. [1] `J. Kelly, P. O'Malley, M. Neeley, H. Neven, J. M. Martinis,
-               arXiv:1803.03226. <https://arxiv.org/abs/1803.03226>`_
+        .. [1] `L. Riesebos, B. Bondurant, K. R. Brown. IEEE Micro 41, 57 (2021)
+               <https://ieeexplore.ieee.org/document/9477114>`_
         """
         check_argument(
             node.in_graph(self),
             "The node must belong to the calibration graph.",
             {"node": node},
         )
```

### Comparing `qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/graph_traversal.py` & `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/graph_traversal.py`

 * *Files identical despite different names*

### Comparing `qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/node.py` & `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/node.py`

 * *Files identical despite different names*

### Comparing `qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/predefined/__init__.py` & `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/predefined/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/predefined/amplitude_calibration.py` & `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/predefined/amplitude_calibration.py`

 * *Files identical despite different names*

### Comparing `qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/predefined/simulation_backend.py` & `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/predefined/simulation_backend.py`

 * *Files identical despite different names*

### Comparing `qctrl_experiment_scheduler-0.1.2/qctrlexperimentscheduler/variable.py` & `qctrl_experiment_scheduler-0.2.0/qctrlexperimentscheduler/variable.py`

 * *Files identical despite different names*

### Comparing `qctrl_experiment_scheduler-0.1.2/PKG-INFO` & `qctrl_experiment_scheduler-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: qctrl-experiment-scheduler
-Version: 0.1.2
+Version: 0.2.0
 Summary: Q-CTRL Experiment Scheduler
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
 Maintainer-email: support@q-ctrl.com
-Requires-Python: >=3.7.2,<3.12
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
@@ -21,29 +21,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
-Requires-Dist: networkx (>=2.6,<2.7); python_full_version >= "3.7.2" and python_version < "3.8"
-Requires-Dist: networkx (>=3.0,<4.0); python_version >= "3.8"
-Requires-Dist: numpy (>=1.21.6,<2.0.0); python_full_version >= "3.7.2" and python_version < "3.8"
-Requires-Dist: numpy (>=1.23.5,<2.0.0); python_version >= "3.8" and python_version < "3.12"
-Requires-Dist: qctrl (>=21.0.0,<22.0.0)
-Requires-Dist: qctrl-commons (>=17.9.1,<18.0.0)
-Requires-Dist: qctrl-visualizer (>=4.5.0,<5.0.0)
+Requires-Dist: networkx (>=2.7,<3.0)
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: qctrl (>=22.0.0,<23.0.0)
+Requires-Dist: qctrl-commons (>=18.0.0,<19.0.0)
+Requires-Dist: qctrl-visualizer (>=5.0.0,<6.0.0)
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Project-URL: YouTube, https://www.youtube.com/qctrl
 Description-Content-Type: text/markdown
```

