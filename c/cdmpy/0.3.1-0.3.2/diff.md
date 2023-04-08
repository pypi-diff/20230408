# Comparing `tmp/cdmpy-0.3.1.tar.gz` & `tmp/cdmpy-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdmpy-0.3.1.tar", last modified: Fri Apr  7 19:33:11 2023, max compression
+gzip compressed data, was "cdmpy-0.3.2.tar", last modified: Fri Apr  7 22:15:57 2023, max compression
```

## Comparing `cdmpy-0.3.1.tar` & `cdmpy-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 19:33:11.569326 cdmpy-0.3.1/
-drwxrwxrwx   0        0        0        0 2023-04-07 19:33:11.503022 cdmpy-0.3.1/.github/
-drwxrwxrwx   0        0        0        0 2023-04-07 19:33:11.540315 cdmpy-0.3.1/.github/workflows/
--rw-rw-rw-   0        0        0     1651 2023-04-07 19:32:20.000000 cdmpy-0.3.1/.github/workflows/main.yml
--rw-rw-rw-   0        0        0      144 2023-04-07 17:34:54.000000 cdmpy-0.3.1/.gitignore
--rw-rw-rw-   0        0        0      234 2023-04-07 14:34:19.000000 cdmpy-0.3.1/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      944 2023-04-07 17:34:54.000000 cdmpy-0.3.1/CHANGELOG
--rw-rw-rw-   0        0        0     1061 2023-04-07 18:43:32.000000 cdmpy-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     3586 2023-04-07 19:33:11.568328 cdmpy-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3012 2023-04-07 19:06:56.000000 cdmpy-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 19:33:11.548307 cdmpy-0.3.1/cdm/
--rw-rw-rw-   0        0        0      263 2023-04-07 19:28:42.000000 cdmpy-0.3.1/cdm/__init__.py
--rw-rw-rw-   0        0        0     2888 2023-04-07 19:30:48.000000 cdmpy-0.3.1/cdm/__main__.py
--rw-rw-rw-   0        0        0     8855 2023-04-07 19:29:17.000000 cdmpy-0.3.1/cdm/fio_cdm.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:33:11.560309 cdmpy-0.3.1/cdmpy.egg-info/
--rw-rw-rw-   0        0        0     3586 2023-04-07 19:33:11.000000 cdmpy-0.3.1/cdmpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-04-07 19:33:11.000000 cdmpy-0.3.1/cdmpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 19:33:11.000000 cdmpy-0.3.1/cdmpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-07 19:33:11.000000 cdmpy-0.3.1/cdmpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2023-04-07 19:33:11.000000 cdmpy-0.3.1/cdmpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      683 2023-04-07 19:31:32.000000 cdmpy-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-07 19:33:11.570324 cdmpy-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-07 19:33:11.566307 cdmpy-0.3.1/tests/
--rw-rw-rw-   0        0        0       61 2023-04-07 18:47:59.000000 cdmpy-0.3.1/tests/__init__.py
--rw-rw-rw-   0        0        0      455 2023-04-07 19:24:37.000000 cdmpy-0.3.1/tests/test_cdm.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-04-07 22:15:57.525334 cdmpy-0.3.2/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-04-07 22:15:57.520973 cdmpy-0.3.2/.github/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-04-07 22:15:57.522807 cdmpy-0.3.2/.github/workflows/
+-rw-r--r--   0 thomas     (501) staff       (20)     1651 2023-04-07 21:16:29.000000 cdmpy-0.3.2/.github/workflows/main.yml
+-rw-r--r--   0 thomas     (501) staff       (20)      144 2023-04-07 21:16:29.000000 cdmpy-0.3.2/.gitignore
+-rw-r--r--   0 thomas     (501) staff       (20)      222 2023-04-07 21:16:29.000000 cdmpy-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 thomas     (501) staff       (20)     1127 2023-04-07 22:12:29.000000 cdmpy-0.3.2/CHANGELOG
+-rw-r--r--   0 thomas     (501) staff       (20)     1061 2023-04-07 21:16:29.000000 cdmpy-0.3.2/LICENSE
+-rw-r--r--   0 thomas     (501) staff       (20)     3493 2023-04-07 22:15:57.525119 cdmpy-0.3.2/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)     3012 2023-04-07 21:16:29.000000 cdmpy-0.3.2/README.md
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-04-07 22:15:57.523409 cdmpy-0.3.2/cdm/
+-rw-r--r--   0 thomas     (501) staff       (20)      263 2023-04-07 21:16:29.000000 cdmpy-0.3.2/cdm/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3096 2023-04-07 22:09:53.000000 cdmpy-0.3.2/cdm/__main__.py
+-rw-r--r--   0 thomas     (501) staff       (20)     9271 2023-04-07 22:10:39.000000 cdmpy-0.3.2/cdm/fio_cdm.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-04-07 22:15:57.524416 cdmpy-0.3.2/cdmpy.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)     3493 2023-04-07 22:15:57.000000 cdmpy-0.3.2/cdmpy.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)      335 2023-04-07 22:15:57.000000 cdmpy-0.3.2/cdmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2023-04-07 22:15:57.000000 cdmpy-0.3.2/cdmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       39 2023-04-07 22:15:57.000000 cdmpy-0.3.2/cdmpy.egg-info/entry_points.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        4 2023-04-07 22:15:57.000000 cdmpy-0.3.2/cdmpy.egg-info/top_level.txt
+-rw-r--r--   0 thomas     (501) staff       (20)      683 2023-04-07 22:12:38.000000 cdmpy-0.3.2/pyproject.toml
+-rw-r--r--   0 thomas     (501) staff       (20)       38 2023-04-07 22:15:57.525403 cdmpy-0.3.2/setup.cfg
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-04-07 22:15:57.524801 cdmpy-0.3.2/tests/
+-rw-r--r--   0 thomas     (501) staff       (20)       61 2023-04-07 21:16:29.000000 cdmpy-0.3.2/tests/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)      455 2023-04-07 21:16:29.000000 cdmpy-0.3.2/tests/test_cdm.py
```

### Comparing `cdmpy-0.3.1/.github/workflows/main.yml` & `cdmpy-0.3.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `cdmpy-0.3.1/CHANGELOG` & `cdmpy-0.3.2/CHANGELOG`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+0.3.2 - 2023-04-07
+
+Removed:
+- Support MacOS with posixaio instead of libaio engine.
+
+0.3.1 - 2023-04-07
+
+Removed:
+- Pre-compiled fio executable for Windows due to security reasons.
+
 0.3.0 - 2023-04-07
 
 Changed:
 - Added Windows fio binary, otherwise use installed version
 - Create proper Python project structure
 - Provide entrypoint from __main__ file
```

### Comparing `cdmpy-0.3.1/LICENSE` & `cdmpy-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdmpy-0.3.1/PKG-INFO` & `cdmpy-0.3.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-Metadata-Version: 2.1
-Name: cdmpy
-Version: 0.3.1
-Summary: A python script to generate CrystalDiskMark-style test result with fio. Should work across multi platforms.
-Author-email: Lu Xu <oliver_lew@outlook.com>, Pyhoniasm <26092465+Pythoniasm@users.noreply.github.com>
-License: MIT
-Project-URL: repository, https://github.com/Pythoniasm/cdmpy
-Keywords: CrystalDiskMark,disk utilities,hdd,ssd
-Requires-Python: >=3.9.13
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# cdmpy
-
-Python script packaging of [fio-cdm](https://github.com/OliverLew/fio-cdm), a python script to generate [CrystalDiskMark](https://crystalmark.info/en/software/crystaldiskmark/)-style test result with [fio](https://github.com/axboe/fio). Should work across multi platforms.
-
-## Requirement
-
-- fio
-- python3
-
-## Feature
-
-- Provide some options of CrystalDiskMark, e.g., number of test runs, test file size, mixed r/w tests, zero buffers, etc
-- Show IOPS and latency results for random read/write tests.
-  This actually combines the "default", "peak performance" and "real world performance" tests in CrystalDiskMark
-- Easy to add/customize new tests in command-line arguments
-- Parse `fio` result in json format to achieve more stability
-
-## Installation
-
-Install via Python `pip install .`
-
-## Usage
-
-Call script via `cdm` after pip installation from anywhere.
-
-```
-usage: cdm [target] [-h] [-0] [-a job] [-E] [-f jobfile] [-n number] [-s size] [-x [mix]]
-
-positional arguments:
-  target      The path of the directory to test. Default to current directory.
-
-optional arguments:
-  -h, --help  show this help message and exit
-  -0          Initialize buffers with zeros. Default to use random buffers.
-  -a job      Manually add multiple jobs. Format is "seq|rnd,<queue depth>,<thread number>".
-              This overrides the preset jobs. This option can be used more than once.
-  -E          Disable extra information (iops, latency) for random IO tests. Default is enabled.
-  -f jobfile  Save jobfile and quit without running fio. Use "-" to print to stdout.
-  -n number   Number of tests, default is 5.
-  -s size     The size of file I/O. It is directly passed to fio. Default is 1G.
-  -x [mix]    Add mixed rw test. Default is disabled. <mix> is read percentage. Default is 70.
-
-Note:
-Recommend to put the <target> argument as the first one since some of the optional arguments will consume it.
-```
-
-### Sample output
-
-The default tests are same as [CrystalDiskMark](https://crystalmark.info/en/software/crystaldiskmark/crystaldiskmark-main-menu/)
-
-```
-tests: 5, size: 1G, target: . 173.3GiB/405.1GiB
-|Name        | Read(MB/s)|Write(MB/s)|  Mix(MB/s)|
-|------------|-----------|-----------|-----------|
-|SEQ1M Q8 T1 |    2997.60|    2056.19|    1438.19|
-|SEQ1M Q1 T1 |    1986.94|    1461.67|     941.04|
-|RND4K Q32T16|    1816.04|     456.98|     434.18|
-|... IOPS    |  443350.17|  111546.75|  105987.62|
-|... latency |    1153.89|    4587.90|    2800.43|
-|RND4K Q1 T1 |      54.20|     164.86|      34.43|
-|... IOPS    |   13232.15|   40248.87|    8405.20|
-|... latency |      74.76|      23.04|      67.78|
-```
-
-### Examples
-
-Set test file size to 512MB, 5 test runs with read, write and mix tests:
-
-    cdm -s 512m -n 5 -x
-
-Manually add jobs to replace the default ones:
-
-    cdm -a seq,1,1 -a seq,32,1 -a rnd,16,8
-
-Show the equivalent fio command directly (without running the test):
-
-    cdm -f - | fio --showcmd -
-
-## Similar projects
-
-**Shell version**: https://github.com/buty4649/fio-cdm
+Metadata-Version: 2.1
+Name: cdmpy
+Version: 0.3.2
+Summary: A python script to generate CrystalDiskMark-style test result with fio. Should work across multi platforms.
+Author-email: Lu Xu <oliver_lew@outlook.com>, Pyhoniasm <26092465+Pythoniasm@users.noreply.github.com>
+License: MIT
+Project-URL: repository, https://github.com/Pythoniasm/cdmpy
+Keywords: CrystalDiskMark,disk utilities,hdd,ssd
+Requires-Python: >=3.9.13
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# cdmpy
+
+Python script packaging of [fio-cdm](https://github.com/OliverLew/fio-cdm), a python script to generate [CrystalDiskMark](https://crystalmark.info/en/software/crystaldiskmark/)-style test result with [fio](https://github.com/axboe/fio). Should work across multi platforms.
+
+## Requirement
+
+- fio
+- python3
+
+## Feature
+
+- Provide some options of CrystalDiskMark, e.g., number of test runs, test file size, mixed r/w tests, zero buffers, etc
+- Show IOPS and latency results for random read/write tests.
+  This actually combines the "default", "peak performance" and "real world performance" tests in CrystalDiskMark
+- Easy to add/customize new tests in command-line arguments
+- Parse `fio` result in json format to achieve more stability
+
+## Installation
+
+Install via Python `pip install .`
+
+## Usage
+
+Call script via `cdm` after pip installation from anywhere.
+
+```
+usage: cdm [target] [-h] [-0] [-a job] [-E] [-f jobfile] [-n number] [-s size] [-x [mix]]
+
+positional arguments:
+  target      The path of the directory to test. Default to current directory.
+
+optional arguments:
+  -h, --help  show this help message and exit
+  -0          Initialize buffers with zeros. Default to use random buffers.
+  -a job      Manually add multiple jobs. Format is "seq|rnd,<queue depth>,<thread number>".
+              This overrides the preset jobs. This option can be used more than once.
+  -E          Disable extra information (iops, latency) for random IO tests. Default is enabled.
+  -f jobfile  Save jobfile and quit without running fio. Use "-" to print to stdout.
+  -n number   Number of tests, default is 5.
+  -s size     The size of file I/O. It is directly passed to fio. Default is 1G.
+  -x [mix]    Add mixed rw test. Default is disabled. <mix> is read percentage. Default is 70.
+
+Note:
+Recommend to put the <target> argument as the first one since some of the optional arguments will consume it.
+```
+
+### Sample output
+
+The default tests are same as [CrystalDiskMark](https://crystalmark.info/en/software/crystaldiskmark/crystaldiskmark-main-menu/)
+
+```
+tests: 5, size: 1G, target: . 173.3GiB/405.1GiB
+|Name        | Read(MB/s)|Write(MB/s)|  Mix(MB/s)|
+|------------|-----------|-----------|-----------|
+|SEQ1M Q8 T1 |    2997.60|    2056.19|    1438.19|
+|SEQ1M Q1 T1 |    1986.94|    1461.67|     941.04|
+|RND4K Q32T16|    1816.04|     456.98|     434.18|
+|... IOPS    |  443350.17|  111546.75|  105987.62|
+|... latency |    1153.89|    4587.90|    2800.43|
+|RND4K Q1 T1 |      54.20|     164.86|      34.43|
+|... IOPS    |   13232.15|   40248.87|    8405.20|
+|... latency |      74.76|      23.04|      67.78|
+```
+
+### Examples
+
+Set test file size to 512MB, 5 test runs with read, write and mix tests:
+
+    cdm -s 512m -n 5 -x
+
+Manually add jobs to replace the default ones:
+
+    cdm -a seq,1,1 -a seq,32,1 -a rnd,16,8
+
+Show the equivalent fio command directly (without running the test):
+
+    cdm -f - | fio --showcmd -
+
+## Similar projects
+
+**Shell version**: https://github.com/buty4649/fio-cdm
```

### Comparing `cdmpy-0.3.1/README.md` & `cdmpy-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cdmpy-0.3.1/cdm/__main__.py` & `cdmpy-0.3.2/cdm/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #! /usr/bin/env python
 
 # Author: Lu Xu <oliver_lew@outlook.com">
 # License: MIT
 # Original Repo: https://github.com/OliverLew/fio-cdm
 # Packaging: https://github.com/Pythoniasm/cdmpy
 
+import os
 import argparse
 import logging
 
 from cdm.fio_cdm import Job
 
 
 def get_parser():
@@ -85,23 +86,34 @@
 def entrypoint():
     parser = get_parser()
     args = parser.parse_args()
 
     logging.basicConfig(
         level=logging.DEBUG if args.debug else logging.INFO, format="%(message)s"
     )
-    fio_job = Job(**vars(args))
 
     if args.jobs:
-        for job in args.jobs:
-            rnd_type, qd, tn = job.split(",")
-            fio_job.create_job(rnd_type, int(qd), int(tn))
+        jobs = args.jobs
     else:
-        fio_job.create_job("seq", 8, 1)
-        fio_job.create_job("seq", 1, 1)
-        fio_job.create_job("rnd", 32, 16)
-        fio_job.create_job("rnd", 1, 1)
-    fio_job.run()
+        jobs = [("seq", 8, 1), ("seq", 1, 1), ("rnd", 32, 16), ("rnd", 1, 1)]
+
+    fio_job = Job(**vars(args))
+    for job in jobs:
+        if args.jobs:
+            rnd_type, qd, tn = job.split(",")
+        else:
+            rnd_type, qd, tn = job
+            if os.name == "posix":
+                tn = min(tn, 8)
+
+        fio_job.create_job(rnd_type, int(qd), int(tn))
+
+        if os.name == "posix":
+            fio_job.run()
+            fio_job = Job(**vars(args))
+
+    if os.name != "posix":
+        fio_job.run()
 
 
 if __name__ == "__main__":
     entrypoint()
```

### Comparing `cdmpy-0.3.1/cdm/fio_cdm.py` & `cdmpy-0.3.2/cdm/fio_cdm.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,18 +44,26 @@
 
         self._jobs = []
         self._jobfile_id, self._jobfile_name = tempfile.mkstemp(suffix=".jobfile")
         self._jobfile = os.fdopen(self._jobfile_id, "w")
         self._testfile_name = ".fio_testmark"
         self._blocksize = {"seq": "1m", "rnd": "4k"}
         self._config = configparser.ConfigParser(allow_no_value=True)
+
+        if os.name == "nt":
+            self._ioengine = "windowsaio"
+        elif os.name == "posix":
+            self._ioengine = "posixaio"
+        else:
+            self._ioengine = "libaio"
+
         self._config.read_dict(
             {
                 "global": {
-                    "ioengine": "windowsaio" if os.name == "nt" else "libaio",
+                    "ioengine": self._ioengine,
                     "filename": self._testfile_name,
                     # escape colons, see man page 'filename'
                     "directory": self.target.replace(":", r"\:"),
                     "size": self.size,
                     "direct": "1",
                     # borrowed configuration from shell version
                     "runtime": "5",
@@ -160,16 +168,23 @@
         if self.mix:
             print(
                 "Mixed rw: read {:2.0f}%, write {:2.0f}%".format(
                     self.mix, 100 - self.mix
                 )
             )
 
-        FIO_COMMAND = ["fio", "--output-format", "json", self._jobfile_name]
+        FIO_COMMAND_ARGS = list()
+        if os.name == "posix":  # MacOS
+            FIO_COMMAND_ARGS += ["--ioengine", "posixaio", "--max-jobs=1"]
+
+        FIO_COMMAND_ARGS += ["--output-format", "json"]
+        FIO_COMMAND = ["fio"] + FIO_COMMAND_ARGS + [self._jobfile_name]
+
         try:
+            print(f"$ {' '.join(FIO_COMMAND)}")
             res = Popen(FIO_COMMAND, stdout=PIPE)
             output, _ = res.communicate()
         except KeyboardInterrupt:
             logging.info("interrupted, cleaning up before exit...")
             exit()
         except FileNotFoundError:
             print("fio not found, install from https://github.com/axboe/fio/releases")
```

### Comparing `cdmpy-0.3.1/cdmpy.egg-info/PKG-INFO` & `cdmpy-0.3.2/cdmpy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-Metadata-Version: 2.1
-Name: cdmpy
-Version: 0.3.1
-Summary: A python script to generate CrystalDiskMark-style test result with fio. Should work across multi platforms.
-Author-email: Lu Xu <oliver_lew@outlook.com>, Pyhoniasm <26092465+Pythoniasm@users.noreply.github.com>
-License: MIT
-Project-URL: repository, https://github.com/Pythoniasm/cdmpy
-Keywords: CrystalDiskMark,disk utilities,hdd,ssd
-Requires-Python: >=3.9.13
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# cdmpy
-
-Python script packaging of [fio-cdm](https://github.com/OliverLew/fio-cdm), a python script to generate [CrystalDiskMark](https://crystalmark.info/en/software/crystaldiskmark/)-style test result with [fio](https://github.com/axboe/fio). Should work across multi platforms.
-
-## Requirement
-
-- fio
-- python3
-
-## Feature
-
-- Provide some options of CrystalDiskMark, e.g., number of test runs, test file size, mixed r/w tests, zero buffers, etc
-- Show IOPS and latency results for random read/write tests.
-  This actually combines the "default", "peak performance" and "real world performance" tests in CrystalDiskMark
-- Easy to add/customize new tests in command-line arguments
-- Parse `fio` result in json format to achieve more stability
-
-## Installation
-
-Install via Python `pip install .`
-
-## Usage
-
-Call script via `cdm` after pip installation from anywhere.
-
-```
-usage: cdm [target] [-h] [-0] [-a job] [-E] [-f jobfile] [-n number] [-s size] [-x [mix]]
-
-positional arguments:
-  target      The path of the directory to test. Default to current directory.
-
-optional arguments:
-  -h, --help  show this help message and exit
-  -0          Initialize buffers with zeros. Default to use random buffers.
-  -a job      Manually add multiple jobs. Format is "seq|rnd,<queue depth>,<thread number>".
-              This overrides the preset jobs. This option can be used more than once.
-  -E          Disable extra information (iops, latency) for random IO tests. Default is enabled.
-  -f jobfile  Save jobfile and quit without running fio. Use "-" to print to stdout.
-  -n number   Number of tests, default is 5.
-  -s size     The size of file I/O. It is directly passed to fio. Default is 1G.
-  -x [mix]    Add mixed rw test. Default is disabled. <mix> is read percentage. Default is 70.
-
-Note:
-Recommend to put the <target> argument as the first one since some of the optional arguments will consume it.
-```
-
-### Sample output
-
-The default tests are same as [CrystalDiskMark](https://crystalmark.info/en/software/crystaldiskmark/crystaldiskmark-main-menu/)
-
-```
-tests: 5, size: 1G, target: . 173.3GiB/405.1GiB
-|Name        | Read(MB/s)|Write(MB/s)|  Mix(MB/s)|
-|------------|-----------|-----------|-----------|
-|SEQ1M Q8 T1 |    2997.60|    2056.19|    1438.19|
-|SEQ1M Q1 T1 |    1986.94|    1461.67|     941.04|
-|RND4K Q32T16|    1816.04|     456.98|     434.18|
-|... IOPS    |  443350.17|  111546.75|  105987.62|
-|... latency |    1153.89|    4587.90|    2800.43|
-|RND4K Q1 T1 |      54.20|     164.86|      34.43|
-|... IOPS    |   13232.15|   40248.87|    8405.20|
-|... latency |      74.76|      23.04|      67.78|
-```
-
-### Examples
-
-Set test file size to 512MB, 5 test runs with read, write and mix tests:
-
-    cdm -s 512m -n 5 -x
-
-Manually add jobs to replace the default ones:
-
-    cdm -a seq,1,1 -a seq,32,1 -a rnd,16,8
-
-Show the equivalent fio command directly (without running the test):
-
-    cdm -f - | fio --showcmd -
-
-## Similar projects
-
-**Shell version**: https://github.com/buty4649/fio-cdm
+Metadata-Version: 2.1
+Name: cdmpy
+Version: 0.3.2
+Summary: A python script to generate CrystalDiskMark-style test result with fio. Should work across multi platforms.
+Author-email: Lu Xu <oliver_lew@outlook.com>, Pyhoniasm <26092465+Pythoniasm@users.noreply.github.com>
+License: MIT
+Project-URL: repository, https://github.com/Pythoniasm/cdmpy
+Keywords: CrystalDiskMark,disk utilities,hdd,ssd
+Requires-Python: >=3.9.13
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# cdmpy
+
+Python script packaging of [fio-cdm](https://github.com/OliverLew/fio-cdm), a python script to generate [CrystalDiskMark](https://crystalmark.info/en/software/crystaldiskmark/)-style test result with [fio](https://github.com/axboe/fio). Should work across multi platforms.
+
+## Requirement
+
+- fio
+- python3
+
+## Feature
+
+- Provide some options of CrystalDiskMark, e.g., number of test runs, test file size, mixed r/w tests, zero buffers, etc
+- Show IOPS and latency results for random read/write tests.
+  This actually combines the "default", "peak performance" and "real world performance" tests in CrystalDiskMark
+- Easy to add/customize new tests in command-line arguments
+- Parse `fio` result in json format to achieve more stability
+
+## Installation
+
+Install via Python `pip install .`
+
+## Usage
+
+Call script via `cdm` after pip installation from anywhere.
+
+```
+usage: cdm [target] [-h] [-0] [-a job] [-E] [-f jobfile] [-n number] [-s size] [-x [mix]]
+
+positional arguments:
+  target      The path of the directory to test. Default to current directory.
+
+optional arguments:
+  -h, --help  show this help message and exit
+  -0          Initialize buffers with zeros. Default to use random buffers.
+  -a job      Manually add multiple jobs. Format is "seq|rnd,<queue depth>,<thread number>".
+              This overrides the preset jobs. This option can be used more than once.
+  -E          Disable extra information (iops, latency) for random IO tests. Default is enabled.
+  -f jobfile  Save jobfile and quit without running fio. Use "-" to print to stdout.
+  -n number   Number of tests, default is 5.
+  -s size     The size of file I/O. It is directly passed to fio. Default is 1G.
+  -x [mix]    Add mixed rw test. Default is disabled. <mix> is read percentage. Default is 70.
+
+Note:
+Recommend to put the <target> argument as the first one since some of the optional arguments will consume it.
+```
+
+### Sample output
+
+The default tests are same as [CrystalDiskMark](https://crystalmark.info/en/software/crystaldiskmark/crystaldiskmark-main-menu/)
+
+```
+tests: 5, size: 1G, target: . 173.3GiB/405.1GiB
+|Name        | Read(MB/s)|Write(MB/s)|  Mix(MB/s)|
+|------------|-----------|-----------|-----------|
+|SEQ1M Q8 T1 |    2997.60|    2056.19|    1438.19|
+|SEQ1M Q1 T1 |    1986.94|    1461.67|     941.04|
+|RND4K Q32T16|    1816.04|     456.98|     434.18|
+|... IOPS    |  443350.17|  111546.75|  105987.62|
+|... latency |    1153.89|    4587.90|    2800.43|
+|RND4K Q1 T1 |      54.20|     164.86|      34.43|
+|... IOPS    |   13232.15|   40248.87|    8405.20|
+|... latency |      74.76|      23.04|      67.78|
+```
+
+### Examples
+
+Set test file size to 512MB, 5 test runs with read, write and mix tests:
+
+    cdm -s 512m -n 5 -x
+
+Manually add jobs to replace the default ones:
+
+    cdm -a seq,1,1 -a seq,32,1 -a rnd,16,8
+
+Show the equivalent fio command directly (without running the test):
+
+    cdm -f - | fio --showcmd -
+
+## Similar projects
+
+**Shell version**: https://github.com/buty4649/fio-cdm
```

### Comparing `cdmpy-0.3.1/pyproject.toml` & `cdmpy-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cdmpy"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
     {name = "Lu Xu", email = "oliver_lew@outlook.com"},
     {name = "Pyhoniasm", email = "26092465+Pythoniasm@users.noreply.github.com"}
 ]
 description = "A python script to generate CrystalDiskMark-style test result with fio. Should work across multi platforms."
 keywords = ["CrystalDiskMark", "disk utilities", "hdd", "ssd"]
 license = {text = "MIT"}
```

