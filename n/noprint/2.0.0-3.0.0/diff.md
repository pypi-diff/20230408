# Comparing `tmp/noprint-2.0.0.tar.gz` & `tmp/noprint-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noprint-2.0.0.tar", last modified: Wed Mar  8 14:22:29 2023, max compression
+gzip compressed data, was "noprint-3.0.0.tar", last modified: Sat Apr  8 21:23:14 2023, max compression
```

## Comparing `noprint-2.0.0.tar` & `noprint-3.0.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:22:29.678763 noprint-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-08 14:22:20.000000 noprint-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-03-08 14:22:29.678763 noprint-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-03-08 14:22:20.000000 noprint-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-08 14:22:20.000000 noprint-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 14:22:29.678763 noprint-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:22:29.674763 noprint-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:22:29.674763 noprint-2.0.0/src/noprint/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-08 14:22:20.000000 noprint-2.0.0/src/noprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-03-08 14:22:20.000000 noprint-2.0.0/src/noprint/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-08 14:22:20.000000 noprint-2.0.0/src/noprint/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-08 14:22:20.000000 noprint-2.0.0/src/noprint/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-03-08 14:22:20.000000 noprint-2.0.0/src/noprint/sprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:22:29.674763 noprint-2.0.0/src/noprint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-03-08 14:22:29.000000 noprint-2.0.0/src/noprint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-08 14:22:29.000000 noprint-2.0.0/src/noprint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 14:22:29.000000 noprint-2.0.0/src/noprint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-08 14:22:29.000000 noprint-2.0.0/src/noprint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-08 14:22:29.000000 noprint-2.0.0/src/noprint.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:22:29.678763 noprint-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-03-08 14:22:20.000000 noprint-2.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-08 14:22:20.000000 noprint-2.0.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-03-08 14:22:20.000000 noprint-2.0.0/tests/test_sprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:23:14.370231 noprint-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-08 21:23:02.000000 noprint-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-08 21:23:14.370231 noprint-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-04-08 21:23:02.000000 noprint-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-08 21:23:02.000000 noprint-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 21:23:14.370231 noprint-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:23:14.366231 noprint-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:23:14.370231 noprint-3.0.0/src/noprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-08 21:23:02.000000 noprint-3.0.0/src/noprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-08 21:23:02.000000 noprint-3.0.0/src/noprint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-08 21:23:02.000000 noprint-3.0.0/src/noprint/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-08 21:23:02.000000 noprint-3.0.0/src/noprint/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-08 21:23:02.000000 noprint-3.0.0/src/noprint/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-04-08 21:23:02.000000 noprint-3.0.0/src/noprint/sprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:23:14.370231 noprint-3.0.0/src/noprint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-08 21:23:14.000000 noprint-3.0.0/src/noprint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-08 21:23:14.000000 noprint-3.0.0/src/noprint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:23:14.000000 noprint-3.0.0/src/noprint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-08 21:23:14.000000 noprint-3.0.0/src/noprint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 21:23:14.000000 noprint-3.0.0/src/noprint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:23:14.370231 noprint-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-08 21:23:02.000000 noprint-3.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-08 21:23:02.000000 noprint-3.0.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-04-08 21:23:02.000000 noprint-3.0.0/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-08 21:23:02.000000 noprint-3.0.0/tests/test_sprint.py
```

### Comparing `noprint-2.0.0/LICENSE` & `noprint-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `noprint-2.0.0/PKG-INFO` & `noprint-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noprint
-Version: 2.0.0
+Version: 3.0.0
 Summary: Do not allow prints in your code
 Author-email: Radoslaw Gryta <radek.gryta@gmail.com>
 Project-URL: Homepage, https://github.com/rgryta/NoPrint
 Project-URL: Bug Tracker, https://github.com/rgryta/NoPrint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 Verbosity options for `-v`:
  - Outputs which modules contain print statements at which lines
  - Warning when any of your submodules are missing `__init__.py` files (reported always as warnings) 
  - Receive a warning if one of packages that's being analysed is out of system's scope - it will still be scanned, but that "package" is not reachable outside of that directory, these are e.g. `tests` directories
  - Receive a warning if one of your packages is overshadowing a package available on system/environment level, e.g. if you have requested to analyse your `test` directory, but Python already has an internal package called `test`
 
 Verbosity options for `-vv` (or `-v -v` on older Python versions):
- - All of the options from `-v`
+ - All the options from `-v`
  - NoPrint will tell you specifically which of your submodules are clear of print statements
 
 ## Requirements
 
 There's ***NONE!*** You can use this package to your heart's content. Unless you'd like to develop for it, for this you'll need Black, Pylint and Pytest along with Pytest-cov.
 
 ## Installation
@@ -71,15 +71,15 @@
   --version             show program's version number and exit
 
 Thank you for using NoPrint
 ```
 
 ### Multithreading
 
-Provide number of threads after `-m` parameter. Default's to 1 if not provided or provided without specific number. If 0 or less is givem then it will use number of available vCPUs reported by multiprocessing library.
+Provide number of threads after `-m` parameter. Default's to 1 if not provided or provided without specific number. If 0 or less is given then it will use number of available vCPUs reported by multiprocessing library.
 
 ### Example in Makefile:
 ```bash
 (venv) root@/DummyProject# make test
 { \
         . venv/bin/activate && \
         noprint -evvm 0 tp && \
@@ -96,15 +96,15 @@
 
 This package performs recursive tests on itself before being merged - you can check suggested usage in Makefile. 
 
 ## Development
 
 If you'd like to develop for this package (for some reason) then it's rather straightforward. On Windows start `init.bat` command (WSL2 required). This will install a local WSL2 image with small Ubuntu environment and set up virtual environment for you. If you're already using Unix-based system, you can just use `init.sh` as that will create Python virtual environment.
 
-Before creating Pull Request, make sure that your tests are passing. This is a small package so I want to maintain 100% coverage - `# pragma: no cover` is only allowed in very specific scenarios (like single line method wrapper).
+Before creating Pull Request, make sure that your tests are passing. This is a small package, so I want to maintain 100% coverage - `# pragma: no cover` is only allowed in very specific scenarios (like single line method wrapper).
 
 ## Want to show off?
 
 Feel free to drop this badge into your repo. Glad to have you onboard.
 
 ```md
 <a href="https://github.com/rgryta/NoPrint"><img alt="NoPrint" src="https://img.shields.io/badge/NoPrint-enabled-blueviolet"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: noprint Version: 2.0.0 Summary: Do not allow prints
+Metadata-Version: 2.1 Name: noprint Version: 3.0.0 Summary: Do not allow prints
 in your code Author-email: Radoslaw Gryta
 gryta@gmail.com> Project-URL: Homepage, https://github.com/rgryta/NoPrint
 Project-URL: Bug Tracker, https://github.com/rgryta/NoPrint/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
      [https://raw.githubusercontent.com/rgryta/NoPrint/main/docs/logo.png]
@@ -17,41 +17,41 @@
 any of your submodules are missing `__init__.py` files (reported always as
 warnings) - Receive a warning if one of packages that's being analysed is out
 of system's scope - it will still be scanned, but that "package" is not
 reachable outside of that directory, these are e.g. `tests` directories -
 Receive a warning if one of your packages is overshadowing a package available
 on system/environment level, e.g. if you have requested to analyse your `test`
 directory, but Python already has an internal package called `test` Verbosity
-options for `-vv` (or `-v -v` on older Python versions): - All of the options
-from `-v` - NoPrint will tell you specifically which of your submodules are
-clear of print statements ## Requirements There's ***NONE!*** You can use this
-package to your heart's content. Unless you'd like to develop for it, for this
-you'll need Black, Pylint and Pytest along with Pytest-cov. ## Installation
-Pull straight from this repo to install manually or just use pip: `pip install
+options for `-vv` (or `-v -v` on older Python versions): - All the options from
+`-v` - NoPrint will tell you specifically which of your submodules are clear of
+print statements ## Requirements There's ***NONE!*** You can use this package
+to your heart's content. Unless you'd like to develop for it, for this you'll
+need Black, Pylint and Pytest along with Pytest-cov. ## Installation Pull
+straight from this repo to install manually or just use pip: `pip install
 noprint` will do the trick. ## Usage ### Use as command: ```bash usage: NoPrint
 [-h] [-e] [-f] [-v] [--version] packages [packages ...] [-m [MULTI]] Do not
 allow prints in your code. positional arguments: packages which packages/
 modules to check, syntax: [. ...], e.g. noprint or noprint.cli options: -h, --
 help show this help message and exit -e, --error-out exit with error when print
 is found (by default only warnings are shown) -f, --first-only finish on first
 print found -v, --verbose provide more analysis information (use multiple v's
 to increase logging level) -m [MULTI], --multi [MULTI] set how many threads to
 use --version show program's version number and exit Thank you for using
 NoPrint ``` ### Multithreading Provide number of threads after `-m` parameter.
 Default's to 1 if not provided or provided without specific number. If 0 or
-less is givem then it will use number of available vCPUs reported by
+less is given then it will use number of available vCPUs reported by
 multiprocessing library. ### Example in Makefile: ```bash (venv) root@/
 DummyProject# make test { \ . venv/bin/activate && \ noprint -evvm 0 tp && \
 echo "Finished!" ; \ } [CLEAR]:[tp.exceptions] [CLEAR]:[tp.logger] [CLEAR]:
 [tp.cli] [ERROR]:[tp] Line: 4 [ERROR]:[tp.submodule] Line: 20 [ERROR]:Print
 statements detected make: *** [Makefile:4: test] Error 1 ``` This package
 performs recursive tests on itself before being merged - you can check
 suggested usage in Makefile. ## Development If you'd like to develop for this
 package (for some reason) then it's rather straightforward. On Windows start
 `init.bat` command (WSL2 required). This will install a local WSL2 image with
 small Ubuntu environment and set up virtual environment for you. If you're
 already using Unix-based system, you can just use `init.sh` as that will create
 Python virtual environment. Before creating Pull Request, make sure that your
-tests are passing. This is a small package so I want to maintain 100% coverage
+tests are passing. This is a small package, so I want to maintain 100% coverage
 - `# pragma: no cover` is only allowed in very specific scenarios (like single
 line method wrapper). ## Want to show off? Feel free to drop this badge into
 your repo. Glad to have you onboard. ```md [NoPrint] ```
```

### Comparing `noprint-2.0.0/README.md` & `noprint-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 Verbosity options for `-v`:
  - Outputs which modules contain print statements at which lines
  - Warning when any of your submodules are missing `__init__.py` files (reported always as warnings) 
  - Receive a warning if one of packages that's being analysed is out of system's scope - it will still be scanned, but that "package" is not reachable outside of that directory, these are e.g. `tests` directories
  - Receive a warning if one of your packages is overshadowing a package available on system/environment level, e.g. if you have requested to analyse your `test` directory, but Python already has an internal package called `test`
 
 Verbosity options for `-vv` (or `-v -v` on older Python versions):
- - All of the options from `-v`
+ - All the options from `-v`
  - NoPrint will tell you specifically which of your submodules are clear of print statements
 
 ## Requirements
 
 There's ***NONE!*** You can use this package to your heart's content. Unless you'd like to develop for it, for this you'll need Black, Pylint and Pytest along with Pytest-cov.
 
 ## Installation
@@ -57,15 +57,15 @@
   --version             show program's version number and exit
 
 Thank you for using NoPrint
 ```
 
 ### Multithreading
 
-Provide number of threads after `-m` parameter. Default's to 1 if not provided or provided without specific number. If 0 or less is givem then it will use number of available vCPUs reported by multiprocessing library.
+Provide number of threads after `-m` parameter. Default's to 1 if not provided or provided without specific number. If 0 or less is given then it will use number of available vCPUs reported by multiprocessing library.
 
 ### Example in Makefile:
 ```bash
 (venv) root@/DummyProject# make test
 { \
         . venv/bin/activate && \
         noprint -evvm 0 tp && \
@@ -82,15 +82,15 @@
 
 This package performs recursive tests on itself before being merged - you can check suggested usage in Makefile. 
 
 ## Development
 
 If you'd like to develop for this package (for some reason) then it's rather straightforward. On Windows start `init.bat` command (WSL2 required). This will install a local WSL2 image with small Ubuntu environment and set up virtual environment for you. If you're already using Unix-based system, you can just use `init.sh` as that will create Python virtual environment.
 
-Before creating Pull Request, make sure that your tests are passing. This is a small package so I want to maintain 100% coverage - `# pragma: no cover` is only allowed in very specific scenarios (like single line method wrapper).
+Before creating Pull Request, make sure that your tests are passing. This is a small package, so I want to maintain 100% coverage - `# pragma: no cover` is only allowed in very specific scenarios (like single line method wrapper).
 
 ## Want to show off?
 
 Feel free to drop this badge into your repo. Glad to have you onboard.
 
 ```md
 <a href="https://github.com/rgryta/NoPrint"><img alt="NoPrint" src="https://img.shields.io/badge/NoPrint-enabled-blueviolet"></a>
```

#### html2text {}

```diff
@@ -10,41 +10,41 @@
 any of your submodules are missing `__init__.py` files (reported always as
 warnings) - Receive a warning if one of packages that's being analysed is out
 of system's scope - it will still be scanned, but that "package" is not
 reachable outside of that directory, these are e.g. `tests` directories -
 Receive a warning if one of your packages is overshadowing a package available
 on system/environment level, e.g. if you have requested to analyse your `test`
 directory, but Python already has an internal package called `test` Verbosity
-options for `-vv` (or `-v -v` on older Python versions): - All of the options
-from `-v` - NoPrint will tell you specifically which of your submodules are
-clear of print statements ## Requirements There's ***NONE!*** You can use this
-package to your heart's content. Unless you'd like to develop for it, for this
-you'll need Black, Pylint and Pytest along with Pytest-cov. ## Installation
-Pull straight from this repo to install manually or just use pip: `pip install
+options for `-vv` (or `-v -v` on older Python versions): - All the options from
+`-v` - NoPrint will tell you specifically which of your submodules are clear of
+print statements ## Requirements There's ***NONE!*** You can use this package
+to your heart's content. Unless you'd like to develop for it, for this you'll
+need Black, Pylint and Pytest along with Pytest-cov. ## Installation Pull
+straight from this repo to install manually or just use pip: `pip install
 noprint` will do the trick. ## Usage ### Use as command: ```bash usage: NoPrint
 [-h] [-e] [-f] [-v] [--version] packages [packages ...] [-m [MULTI]] Do not
 allow prints in your code. positional arguments: packages which packages/
 modules to check, syntax: [. ...], e.g. noprint or noprint.cli options: -h, --
 help show this help message and exit -e, --error-out exit with error when print
 is found (by default only warnings are shown) -f, --first-only finish on first
 print found -v, --verbose provide more analysis information (use multiple v's
 to increase logging level) -m [MULTI], --multi [MULTI] set how many threads to
 use --version show program's version number and exit Thank you for using
 NoPrint ``` ### Multithreading Provide number of threads after `-m` parameter.
 Default's to 1 if not provided or provided without specific number. If 0 or
-less is givem then it will use number of available vCPUs reported by
+less is given then it will use number of available vCPUs reported by
 multiprocessing library. ### Example in Makefile: ```bash (venv) root@/
 DummyProject# make test { \ . venv/bin/activate && \ noprint -evvm 0 tp && \
 echo "Finished!" ; \ } [CLEAR]:[tp.exceptions] [CLEAR]:[tp.logger] [CLEAR]:
 [tp.cli] [ERROR]:[tp] Line: 4 [ERROR]:[tp.submodule] Line: 20 [ERROR]:Print
 statements detected make: *** [Makefile:4: test] Error 1 ``` This package
 performs recursive tests on itself before being merged - you can check
 suggested usage in Makefile. ## Development If you'd like to develop for this
 package (for some reason) then it's rather straightforward. On Windows start
 `init.bat` command (WSL2 required). This will install a local WSL2 image with
 small Ubuntu environment and set up virtual environment for you. If you're
 already using Unix-based system, you can just use `init.sh` as that will create
 Python virtual environment. Before creating Pull Request, make sure that your
-tests are passing. This is a small package so I want to maintain 100% coverage
+tests are passing. This is a small package, so I want to maintain 100% coverage
 - `# pragma: no cover` is only allowed in very specific scenarios (like single
 line method wrapper). ## Want to show off? Feel free to drop this badge into
 your repo. Glad to have you onboard. ```md [NoPrint] ```
```

### Comparing `noprint-2.0.0/pyproject.toml` & `noprint-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "noprint"
-version = "2.0.0"
+version = "3.0.0"
 authors = [
   { name="Radoslaw Gryta", email="radek.gryta@gmail.com" },
 ]
 description = "Do not allow prints in your code"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `noprint-2.0.0/src/noprint/cli.py` & `noprint-3.0.0/src/noprint/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,29 +44,29 @@
         "-m",
         "--multi",
         nargs="?",
         const=1,
         type=int,
         help="set how many threads to use",
     )
-    parser.add_argument("--version", action="version", version="%(prog)s 2.0.0")
+    parser.add_argument("--version", action="version", version="%(prog)s 3.0.0")
     args = parser.parse_known_intermixed_args()[0]
 
     error_out = args.error_out
     first_only = args.first_only
     verbose = bool(args.verbose)
     very_verbose = args.verbose >= 2
     packages = args.packages
     multi = (
         cpu_count()
         if args.multi is not None and args.multi <= 0
         else args.multi
         if args.multi
         else 1
-    )
+    )  # cpu_count when <=0; 1 when not given; otherwise multi
 
     lvl = logging.ERROR if error_out else logging.WARNING
 
     prints, exceptions = detect_prints(packages, first_only, verbose, multi)
 
     exitcode = 0
     detected = any(is_print for _, is_print in prints)
```

### Comparing `noprint-2.0.0/src/noprint/logger.py` & `noprint-3.0.0/src/noprint/logger.py`

 * *Files identical despite different names*

### Comparing `noprint-2.0.0/src/noprint.egg-info/PKG-INFO` & `noprint-3.0.0/src/noprint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noprint
-Version: 2.0.0
+Version: 3.0.0
 Summary: Do not allow prints in your code
 Author-email: Radoslaw Gryta <radek.gryta@gmail.com>
 Project-URL: Homepage, https://github.com/rgryta/NoPrint
 Project-URL: Bug Tracker, https://github.com/rgryta/NoPrint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 Verbosity options for `-v`:
  - Outputs which modules contain print statements at which lines
  - Warning when any of your submodules are missing `__init__.py` files (reported always as warnings) 
  - Receive a warning if one of packages that's being analysed is out of system's scope - it will still be scanned, but that "package" is not reachable outside of that directory, these are e.g. `tests` directories
  - Receive a warning if one of your packages is overshadowing a package available on system/environment level, e.g. if you have requested to analyse your `test` directory, but Python already has an internal package called `test`
 
 Verbosity options for `-vv` (or `-v -v` on older Python versions):
- - All of the options from `-v`
+ - All the options from `-v`
  - NoPrint will tell you specifically which of your submodules are clear of print statements
 
 ## Requirements
 
 There's ***NONE!*** You can use this package to your heart's content. Unless you'd like to develop for it, for this you'll need Black, Pylint and Pytest along with Pytest-cov.
 
 ## Installation
@@ -71,15 +71,15 @@
   --version             show program's version number and exit
 
 Thank you for using NoPrint
 ```
 
 ### Multithreading
 
-Provide number of threads after `-m` parameter. Default's to 1 if not provided or provided without specific number. If 0 or less is givem then it will use number of available vCPUs reported by multiprocessing library.
+Provide number of threads after `-m` parameter. Default's to 1 if not provided or provided without specific number. If 0 or less is given then it will use number of available vCPUs reported by multiprocessing library.
 
 ### Example in Makefile:
 ```bash
 (venv) root@/DummyProject# make test
 { \
         . venv/bin/activate && \
         noprint -evvm 0 tp && \
@@ -96,15 +96,15 @@
 
 This package performs recursive tests on itself before being merged - you can check suggested usage in Makefile. 
 
 ## Development
 
 If you'd like to develop for this package (for some reason) then it's rather straightforward. On Windows start `init.bat` command (WSL2 required). This will install a local WSL2 image with small Ubuntu environment and set up virtual environment for you. If you're already using Unix-based system, you can just use `init.sh` as that will create Python virtual environment.
 
-Before creating Pull Request, make sure that your tests are passing. This is a small package so I want to maintain 100% coverage - `# pragma: no cover` is only allowed in very specific scenarios (like single line method wrapper).
+Before creating Pull Request, make sure that your tests are passing. This is a small package, so I want to maintain 100% coverage - `# pragma: no cover` is only allowed in very specific scenarios (like single line method wrapper).
 
 ## Want to show off?
 
 Feel free to drop this badge into your repo. Glad to have you onboard.
 
 ```md
 <a href="https://github.com/rgryta/NoPrint"><img alt="NoPrint" src="https://img.shields.io/badge/NoPrint-enabled-blueviolet"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: noprint Version: 2.0.0 Summary: Do not allow prints
+Metadata-Version: 2.1 Name: noprint Version: 3.0.0 Summary: Do not allow prints
 in your code Author-email: Radoslaw Gryta
 gryta@gmail.com> Project-URL: Homepage, https://github.com/rgryta/NoPrint
 Project-URL: Bug Tracker, https://github.com/rgryta/NoPrint/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
      [https://raw.githubusercontent.com/rgryta/NoPrint/main/docs/logo.png]
@@ -17,41 +17,41 @@
 any of your submodules are missing `__init__.py` files (reported always as
 warnings) - Receive a warning if one of packages that's being analysed is out
 of system's scope - it will still be scanned, but that "package" is not
 reachable outside of that directory, these are e.g. `tests` directories -
 Receive a warning if one of your packages is overshadowing a package available
 on system/environment level, e.g. if you have requested to analyse your `test`
 directory, but Python already has an internal package called `test` Verbosity
-options for `-vv` (or `-v -v` on older Python versions): - All of the options
-from `-v` - NoPrint will tell you specifically which of your submodules are
-clear of print statements ## Requirements There's ***NONE!*** You can use this
-package to your heart's content. Unless you'd like to develop for it, for this
-you'll need Black, Pylint and Pytest along with Pytest-cov. ## Installation
-Pull straight from this repo to install manually or just use pip: `pip install
+options for `-vv` (or `-v -v` on older Python versions): - All the options from
+`-v` - NoPrint will tell you specifically which of your submodules are clear of
+print statements ## Requirements There's ***NONE!*** You can use this package
+to your heart's content. Unless you'd like to develop for it, for this you'll
+need Black, Pylint and Pytest along with Pytest-cov. ## Installation Pull
+straight from this repo to install manually or just use pip: `pip install
 noprint` will do the trick. ## Usage ### Use as command: ```bash usage: NoPrint
 [-h] [-e] [-f] [-v] [--version] packages [packages ...] [-m [MULTI]] Do not
 allow prints in your code. positional arguments: packages which packages/
 modules to check, syntax: [. ...], e.g. noprint or noprint.cli options: -h, --
 help show this help message and exit -e, --error-out exit with error when print
 is found (by default only warnings are shown) -f, --first-only finish on first
 print found -v, --verbose provide more analysis information (use multiple v's
 to increase logging level) -m [MULTI], --multi [MULTI] set how many threads to
 use --version show program's version number and exit Thank you for using
 NoPrint ``` ### Multithreading Provide number of threads after `-m` parameter.
 Default's to 1 if not provided or provided without specific number. If 0 or
-less is givem then it will use number of available vCPUs reported by
+less is given then it will use number of available vCPUs reported by
 multiprocessing library. ### Example in Makefile: ```bash (venv) root@/
 DummyProject# make test { \ . venv/bin/activate && \ noprint -evvm 0 tp && \
 echo "Finished!" ; \ } [CLEAR]:[tp.exceptions] [CLEAR]:[tp.logger] [CLEAR]:
 [tp.cli] [ERROR]:[tp] Line: 4 [ERROR]:[tp.submodule] Line: 20 [ERROR]:Print
 statements detected make: *** [Makefile:4: test] Error 1 ``` This package
 performs recursive tests on itself before being merged - you can check
 suggested usage in Makefile. ## Development If you'd like to develop for this
 package (for some reason) then it's rather straightforward. On Windows start
 `init.bat` command (WSL2 required). This will install a local WSL2 image with
 small Ubuntu environment and set up virtual environment for you. If you're
 already using Unix-based system, you can just use `init.sh` as that will create
 Python virtual environment. Before creating Pull Request, make sure that your
-tests are passing. This is a small package so I want to maintain 100% coverage
+tests are passing. This is a small package, so I want to maintain 100% coverage
 - `# pragma: no cover` is only allowed in very specific scenarios (like single
 line method wrapper). ## Want to show off? Feel free to drop this badge into
 your repo. Glad to have you onboard. ```md [NoPrint] ```
```

### Comparing `noprint-2.0.0/tests/test_cli.py` & `noprint-3.0.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `noprint-2.0.0/tests/test_logger.py` & `noprint-3.0.0/tests/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Module with tests for noprint.print_seeker
+Module with tests for noprint.logger
 """
 import logging
 
 from unittest import mock
 
 import pytest
```

### Comparing `noprint-2.0.0/tests/test_sprint.py` & `noprint-3.0.0/tests/test_sprint.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,117 +1,128 @@
 """
-Module with tests for noprint.print_seeker
+Module with tests for noprint.sprint
 """
 from unittest import mock
 
 import pytest
 
-import noprint.logger as logging
+import noprint
 
-from noprint.sprint import _get_subpackages, _get_prints, _parse_pyfile
-from noprint.exceptions import ImportException
+from noprint.sprint import (
+    PackageFinder,
+    _parse_pyfile,
+    _get_module,
+    _get_subpackages,
+    _parse_module,
+)
+from noprint.exceptions import ImportException, ParentModuleNotFoundException
 
 
 @pytest.mark.parametrize("origin", [None, "origin", "__init__.py"])
-@pytest.mark.parametrize("name", [None, "name", "__pycache__"])
+@pytest.mark.parametrize("name", ["name", "__pycache__"])
 @mock.patch("noprint.sprint.os")
-@mock.patch("noprint.sprint.find_spec")
-def test__get_subpackages__correct(mock_spec, mock_os, origin, name):
+def test_get_subpackages(mock_os, origin, name):
     """Testing function for _get_subpackages - mock several different module specs and finish with a proper one"""
-    if origin is None and name is None:
-        mod_mock = None
-    else:
-        mod_mock = mock.Mock()
-        mod_mock.origin = origin
-        mod_mock.name = name
-        mod_mock.submodule_search_locations = ["loc"]
+    mod_mock = mock.MagicMock()
+    mod_mock.origin = [origin] if origin is not None else []
+    mod_mock.name = name
+    mod_mock.search_path = "loc"
+    mod_mock.submodule_search_locations = ["loc"]
 
-    mod_mock_e = mock.Mock()
-    mod_mock_e.origin = "origin"
+    mod_mock_e = mock.MagicMock()
+    mod_mock_e.origin = ["origin"]
     mod_mock_e.name = "name"
+    mod_mock_e.search_path = "loc"
     mod_mock_e.submodule_search_locations = ["loc"]
 
     mock_os.listdir.return_value = ["name"]
 
-    mock_spec.side_effect = [
-        spec
-        for specs in [[mod_mock] * 2, [mod_mock] * 2, [mod_mock_e] * 2]
-        for spec in specs
-    ]
-    for package in _get_subpackages("noprint", verbose=True):
+    for package in _get_subpackages("noprint", verbose=True, module=mod_mock):
         assert package is not None
 
 
-@pytest.mark.parametrize("spec", [None, mock.Mock(), True])
-@mock.patch("noprint.sprint.logging")
-@mock.patch("noprint.sprint.find_spec")
-def test__get_subpackages__missing_uninstalled_overshadowing(
-    mock_spec, mock_logging, spec
-):
+@pytest.mark.parametrize("sub_pkgs", [[], [mock.Mock()], [mock.Mock(), mock.Mock()]])
+@pytest.mark.parametrize("origin", [None, "origin"])
+def test_parse_module(origin, sub_pkgs):
     """Testing function for _get_subpackages - mock several different module specs and finish with a proper one"""
-    spec_system = mock.Mock()
+    module = mock.Mock()
+    module.origin = origin
+    with mock.patch("noprint.sprint._get_module", return_value=module), mock.patch(
+        "noprint.sprint._get_subpackages", return_value=sub_pkgs
+    ):
+        result = _parse_module(package="noprint")
+        if module.origin:
+            assert result[0] == module
+        else:
+            assert result[0] is None
+        assert len(result[1]) == len(sub_pkgs)
+
+
+def _parse_mock(package, verbose):  # pylint:disable=unused-argument
+    """Helper function for mocking _parse_module (Pool pickling)"""
+    return (package, [])
+
+
+def test_pf_packages_iter():
+    """Testing PackageFinder.packages_iter"""
+    pkg_finder = PackageFinder(1)
 
-    mock_logging.WARNING = logging.WARNING
-    mock_logging.log = mock.MagicMock()
+    noprint.sprint._parse_module = _parse_mock  # pylint:disable=protected-access
 
-    if isinstance(spec, bool):
-        spec = mock.Mock()
-        mock_spec.side_effect = [spec, spec_system]
-
-        for _ in _get_subpackages("noprint", verbose=True):
-            pass
-        args = mock_logging.log.mock_calls
-        assert len(args) == 1
-        assert args[0] == mock.call(
-            "Module [noprint] is overshadowing installed module", 30
-        )
-        return
-    if spec:
-        mock_spec.side_effect = [spec, None]
-
-        for _ in _get_subpackages("noprint", verbose=True):
-            pass
-        args = mock_logging.log.mock_calls
-        assert len(args) == 1
-        assert args[0] == mock.call("Module [noprint] is not installed", 30)
-    else:
-        mock_spec.side_effect = [spec, spec_system]
-        assert (
-            next(_get_subpackages("noprint")).args[0]
-            == "Module [noprint] is not present in current environment, directory or PYTHONPATH"
-        )
+    packages = ("source", "test")
+    assert set(pkg_finder.packages_iter(packages=packages)) == set(packages)
+
+
+@pytest.mark.parametrize(
+    "ret",
+    [
+        [mock.MagicMock(), mock.MagicMock()],
+        [mock.MagicMock(), None],
+        [mock.MagicMock()] * 2,
+    ],
+)
+def test__get_module__mod(ret):
+    """Testing function for _get_subpackages - mock several different module specs and finish with a proper one"""
 
+    with mock.patch("noprint.sprint.Module") as mock_mod:
+        if isinstance(ret[1], mock.MagicMock):
+            ret[1].origin.__len__.return_value = 1
+        mock_mod.side_effect = ret
+        _get_module("noprint", verbose=True)
 
-@mock.patch("noprint.sprint.find_spec")
-def test__get_subpackages__import_exc(mock_spec):
+
+@pytest.mark.parametrize(
+    "ret", [None, ParentModuleNotFoundException("Dummy exception")]
+)
+def test__get_module__import_exc(ret):
     """Testing function for _get_subpackages - mock several different module specs and finish with a proper one"""
-    mock_spec.side_effect = [Exception("Dummy exception")]
-    assert (
-        next(_get_subpackages("noprint")).args[0]
-        == "Module [noprint] raised Exception on import"
-    )
-    assert (
-        next(_get_subpackages("noprint")).args[0]
-        == "Module [noprint] raised StopIteration on import"
-    )
+
+    with mock.patch("noprint.sprint.Module") as mock_mod, pytest.raises(
+        ImportException
+    ):
+        if ret is None:
+            mock_mod.return_value = ret
+        else:
+            mock_mod.side_effect = ret
+        _get_module("noprint", verbose=True)
 
 
 @pytest.mark.parametrize("code", ["print('')", "", "i=1"])
 @pytest.mark.parametrize("first", [True, False])
 @pytest.mark.parametrize("mod", [None, ImportException("X")])
 @mock.patch("builtins.open")
 def test__parse_pyfile(mock_open, mod, first, code):
     """Test method for _parse_python - finding print statements"""
     fin = mock.Mock()
     fin.return_value.readline.return_value = "# -*- coding: utf-8-sig -*-"
     fin.return_value.read.return_value = code
     mock_open.return_value.__enter__ = fin
 
     module = mock.Mock()
-    module.origin = "noprint"
+    module.origin = ["noprint"]
     module.name = "noprint"
 
     if mod is None:
         mod = module
 
     res = _parse_pyfile(mod, first)
 
@@ -139,23 +150,28 @@
         ),
         (
             [],
             ImportException("X"),
         ),
     ],
 )
-@mock.patch("noprint.sprint.Pool")
-def test__get_prints(mock_pool, mod, first):
+@mock.patch(
+    "noprint.sprint._parse_pyfile", side_effect=lambda module, first_only: module
+)
+def test_pf_run(mock_parse, mod, first):  # pylint: disable=unused-argument
     """Testing function for _get_prints - verifying if code contains print statements"""
 
     def _subpackages(package, _):  # pylint: disable=unused-argument
         i = 0
         yield mod
         i = i + 1
         if i == 10:
             return
 
-    mock_pool.return_value.__enter__.return_value.imap.side_effect = _subpackages
-
-    prints = _get_prints(packages=["noprint"], first_only=first, verbose=True)
-    expected = (mod[0], [mod[1]] if mod[1] else [])
-    assert prints == expected
+    with mock.patch(
+        "noprint.sprint.PackageFinder.packages_iter", side_effect=_subpackages
+    ):
+        prints = PackageFinder(1).run(
+            packages=["noprint"], first_only=first, verbose=True
+        )
+        expected = (mod[0], [mod[1]] if mod[1] else [])
+        assert prints == expected
```

