# Comparing `tmp/napari-console-0.0.7.tar.gz` & `tmp/napari-console-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-console-0.0.7.tar", last modified: Tue Dec 13 08:55:41 2022, max compression
+gzip compressed data, was "napari-console-0.0.8.tar", last modified: Fri Apr  7 23:03:22 2023, max compression
```

## Comparing `napari-console-0.0.7.tar` & `napari-console-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 08:55:41.202093 napari-console-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 08:55:41.194093 napari-console-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 08:55:41.198093 napari-console-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2022-12-13 08:55:21.000000 napari-console-0.0.7/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      970 2022-12-13 08:55:21.000000 napari-console-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2022-12-13 08:55:21.000000 napari-console-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-13 08:55:21.000000 napari-console-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2022-12-13 08:55:41.202093 napari-console-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2022-12-13 08:55:21.000000 napari-console-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 08:55:41.198093 napari-console-0.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2022-12-13 08:55:21.000000 napari-console-0.0.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9448 2022-12-13 08:55:21.000000 napari-console-0.0.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2022-12-13 08:55:21.000000 napari-console-0.0.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2022-12-13 08:55:21.000000 napari-console-0.0.7/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 08:55:41.198093 napari-console-0.0.7/napari_console/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-13 08:55:21.000000 napari-console-0.0.7/napari_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2022-12-13 08:55:21.000000 napari-console-0.0.7/napari_console/_hookimpl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 08:55:41.202093 napari-console-0.0.7/napari_console/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 08:55:21.000000 napari-console-0.0.7/napari_console/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2022-12-13 08:55:21.000000 napari-console-0.0.7/napari_console/_tests/test_qt_console.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-13 08:55:41.000000 napari-console-0.0.7/napari_console/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2022-12-13 08:55:21.000000 napari-console-0.0.7/napari_console/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2022-12-13 08:55:21.000000 napari-console-0.0.7/napari_console/qt_console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 08:55:41.198093 napari-console-0.0.7/napari_console.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2022-12-13 08:55:41.000000 napari-console-0.0.7/napari_console.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2022-12-13 08:55:41.000000 napari-console-0.0.7/napari_console.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 08:55:41.000000 napari-console-0.0.7/napari_console.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-13 08:55:41.000000 napari-console-0.0.7/napari_console.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 08:55:40.000000 napari-console-0.0.7/napari_console.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-13 08:55:41.000000 napari-console-0.0.7/napari_console.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-13 08:55:41.000000 napari-console-0.0.7/napari_console.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2022-12-13 08:55:21.000000 napari-console-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-13 08:55:21.000000 napari-console-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2022-12-13 08:55:41.202093 napari-console-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2022-12-13 08:55:21.000000 napari-console-0.0.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:03:22.344079 napari-console-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:03:22.340079 napari-console-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:03:22.340079 napari-console-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-07 23:03:04.000000 napari-console-0.0.8/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-07 23:03:04.000000 napari-console-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-07 23:03:04.000000 napari-console-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-07 23:03:04.000000 napari-console-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-07 23:03:22.344079 napari-console-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-07 23:03:04.000000 napari-console-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:03:22.340079 napari-console-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-04-07 23:03:04.000000 napari-console-0.0.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-04-07 23:03:04.000000 napari-console-0.0.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-07 23:03:04.000000 napari-console-0.0.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-07 23:03:04.000000 napari-console-0.0.8/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:03:22.340079 napari-console-0.0.8/napari_console/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-07 23:03:04.000000 napari-console-0.0.8/napari_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-07 23:03:04.000000 napari-console-0.0.8/napari_console/_hookimpl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:03:22.344079 napari-console-0.0.8/napari_console/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:03:04.000000 napari-console-0.0.8/napari_console/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-07 23:03:04.000000 napari-console-0.0.8/napari_console/_tests/test_qt_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-07 23:03:22.000000 napari-console-0.0.8/napari_console/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-07 23:03:04.000000 napari-console-0.0.8/napari_console/qt_console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:03:22.344079 napari-console-0.0.8/napari_console.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-07 23:03:22.000000 napari-console-0.0.8/napari_console.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-07 23:03:22.000000 napari-console-0.0.8/napari_console.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:03:22.000000 napari-console-0.0.8/napari_console.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-07 23:03:22.000000 napari-console-0.0.8/napari_console.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:03:22.000000 napari-console-0.0.8/napari_console.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-07 23:03:22.000000 napari-console-0.0.8/napari_console.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-07 23:03:22.000000 napari-console-0.0.8/napari_console.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-07 23:03:04.000000 napari-console-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-07 23:03:04.000000 napari-console-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-07 23:03:22.344079 napari-console-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-07 23:03:04.000000 napari-console-0.0.8/tox.ini
```

### Comparing `napari-console-0.0.7/.github/workflows/test_and_deploy.yml` & `napari-console-0.0.8/.github/workflows/test_and_deploy.yml`

 * *Files 22% similar despite different names*

```diff
@@ -38,31 +38,27 @@
       - name: Install Windows OpenGL
         if: runner.os == 'Windows'
         run: |
           git clone --depth 1 https://github.com/pyvista/gl-ci-helpers.git
           powershell gl-ci-helpers/appveyor/install_opengl.ps1
           if (Test-Path -Path "C:\Windows\system32\opengl32.dll" -PathType Leaf) {Exit 0} else {Exit 1}
 
-      # run a minimal wm for linux tests that depend on UI events (e.g. setFocus)
-      # see https://github.com/pytest-dev/pytest-qt/issues/206
-      - name: Install WM on Linux
-        if: runner.os == 'Linux'
-        run: sudo apt-get update && sudo apt-get install -y herbstluftwm
-
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install setuptools tox tox-gh-actions
 
       - name: Install tox-conda
         if: runner.os == 'macOS' && matrix.python-version == '3.9'
-        run: pip install tox-conda
+        #  we are explicit about tox-gh-action or pip resolver will downgrade
+        #  tox, which will be incompatible with tox-gh-action
+        run: pip install tox-conda tox-gh-actions
 
       - name: Test with tox
-        uses: GabrielBB/xvfb-action@v1
+        uses: aganders3/headless-gui@v1
         with:
           run: python -m tox -vv
         env:
           PLATFORM: ${{ matrix.platform }}
           PYVISTA_OFF_SCREEN: True
 
       - name: Coverage
```

### Comparing `napari-console-0.0.7/.gitignore` & `napari-console-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-console-0.0.7/LICENSE` & `napari-console-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-console-0.0.7/PKG-INFO` & `napari-console-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: napari-console
-Version: 0.0.7
+Version: 0.0.8
 Summary: A plugin that adds a console to napari
 Home-page: https://github.com/napari/napari-console
 Author: Nicholas Sofroniew
 Author-email: sofroniewn@gmail.com
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # napari-console (WIP, under active development)
 
 [![License](https://img.shields.io/pypi/l/napari-console.svg?color=green)](https://github.com/napari/napari-console/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-console.svg?color=green)](https://pypi.org/project/napari-console)
```

### Comparing `napari-console-0.0.7/README.md` & `napari-console-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `napari-console-0.0.7/docs/Makefile` & `napari-console-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `napari-console-0.0.7/docs/conf.py` & `napari-console-0.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `napari-console-0.0.7/docs/make.bat` & `napari-console-0.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `napari-console-0.0.7/napari_console/_tests/test_qt_console.py` & `napari-console-0.0.8/napari_console/_tests/test_qt_console.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     ):
         viewer = make_test_viewer()
         console = QtConsole(viewer)
         qtbot.addWidget(console)
         assert console.kernel_client is None
 
 
-def test_console_focus_proxy(qtbot, make_test_viewer, linux_wm_local):
+def test_console_focus_proxy(qtbot, make_test_viewer):
     """Test setting/clearing focus on a QtConsole sets/clears focus on the underlying QTextEdit"""
     viewer = make_test_viewer()
 
     # setFocus does nothing if the widget is not shown
     console = viewer.window._qt_viewer.console
     with qtbot.waitExposed(console):
         viewer.show()
```

### Comparing `napari-console-0.0.7/napari_console/qt_console.py` & `napari-console-0.0.8/napari_console/qt_console.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 Pick the older SelectorEventLoopPolicy on Windows
 if the known-incompatible default policy is in use.
 
 FIXME: if/when tornado supports the defaults in asyncio,
 remove and bump tornado requirement for py38
 borrowed from ipykernel:  https://github.com/ipython/ipykernel/pull/456
 """
-if sys.platform.startswith("win") and sys.version_info >= (3, 8):
+if sys.platform.startswith("win"):
     import asyncio
 
     try:
         from asyncio import (
             WindowsProactorEventLoopPolicy,
             WindowsSelectorEventLoopPolicy,
         )
```

### Comparing `napari-console-0.0.7/napari_console.egg-info/PKG-INFO` & `napari-console-0.0.8/napari_console.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: napari-console
-Version: 0.0.7
+Version: 0.0.8
 Summary: A plugin that adds a console to napari
 Home-page: https://github.com/napari/napari-console
 Author: Nicholas Sofroniew
 Author-email: sofroniewn@gmail.com
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # napari-console (WIP, under active development)
 
 [![License](https://img.shields.io/pypi/l/napari-console.svg?color=green)](https://github.com/napari/napari-console/raw/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-console.svg?color=green)](https://pypi.org/project/napari-console)
```

### Comparing `napari-console-0.0.7/napari_console.egg-info/SOURCES.txt` & `napari-console-0.0.8/napari_console.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 napari_console/__init__.py
 napari_console/_hookimpl.py
 napari_console/_version.py
-napari_console/conftest.py
 napari_console/qt_console.py
 napari_console.egg-info/PKG-INFO
 napari_console.egg-info/SOURCES.txt
 napari_console.egg-info/dependency_links.txt
 napari_console.egg-info/entry_points.txt
 napari_console.egg-info/not-zip-safe
 napari_console.egg-info/requires.txt
```

### Comparing `napari-console-0.0.7/setup.cfg` & `napari-console-0.0.8/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Framework :: napari
 	Topic :: Software Development :: Testing
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Operating System :: OS Independent
 	License :: OSI Approved :: BSD License
 
 [options]
 zip_safe = False
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 install_requires = 
 	ipykernel>=5.2.0
 	IPython>=7.7.0
 	napari-plugin-engine>=0.1.9
-	qtconsole>=4.5.1,!=4.7.6
+	qtconsole>=4.5.1,!=4.7.6,!=5.4.2
 	qtpy>=1.7.0
 
 [options.package_data]
 * = *.pyi
 napari_builtins = 
 	builtins.yaml
```

### Comparing `napari-console-0.0.7/tox.ini` & `napari-console-0.0.8/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 [tox]
 envlist = py{38,39,310}-{linux,macos,windows}-{pyqt,pyside}
 toxworkdir=/tmp/.tox
 isolated_build = true
 
 [gh-actions]
 python =
-    3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310
     
 [gh-actions:env]
 PLATFORM =
     ubuntu-latest: linux
@@ -23,15 +22,16 @@
     linux: linux
     windows: win32
 setenv =
     PYTHONPATH = {toxinidir}
 passenv = 
     CI
     GITHUB_ACTIONS
-    DISPLAY XAUTHORITY
+    DISPLAY
+    XAUTHORITY
     NUMPY_EXPERIMENTAL_ARRAY_FUNCTION
     PYVISTA_OFF_SCREEN
 conda_deps =
     # use conda to install numcodecs on mac py3.9
     py39-macos: numcodecs
 conda_channels =
     conda-forge
```

