# Comparing `tmp/pcdsutils-0.6.0.tar.gz` & `tmp/pcdsutils-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pcdsutils-0.6.0.tar", last modified: Mon Nov  8 22:35:38 2021, max compression
+gzip compressed data, was "pcdsutils-0.7.0.tar", last modified: Fri Mar 25 17:45:21 2022, max compression
```

## Comparing `pcdsutils-0.6.0.tar` & `pcdsutils-0.7.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      362 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    68573 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/versioneer.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      625 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/docs/Makefile
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/docs/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5450 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/docs/source/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      587 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/docs/source/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      796 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3038 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1026 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/AUTHORS.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/pcdsutils.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1026 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/pcdsutils.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/pcdsutils.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/pcdsutils.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      776 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/pcdsutils.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/pcdsutils.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      161 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/pcdsutils.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      177 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2499 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      631 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/pcdsutils/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2563 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/pcdsutils/release_notes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/pcdsutils/_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/pcdsutils/qt/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12405 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/pcdsutils/qt/popbar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      463 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/pcdsutils/qt/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2374 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/pcdsutils/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      159 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/pcdsutils/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-08 22:35:38.000000 pcdsutils-0.6.0/pcdsutils/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7949 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/pcdsutils/tests/test_logging.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      644 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/pcdsutils/tests/test_requirements.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2384 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/pcdsutils/tests/test_ext_scripts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/pcdsutils/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/pcdsutils/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1692 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/pcdsutils/tests/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25304 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/pcdsutils/log.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8113 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/pcdsutils/requirements.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5186 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/pcdsutils/ext_scripts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2205 2021-11-08 22:35:22.000000 pcdsutils-0.6.0/setup.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-03-25 17:45:21.360521 pcdsutils-0.7.0/
+-rw-r--r--   0 klauer   (1318172782) 1704612529      152 2020-01-24 00:08:39.000000 pcdsutils-0.7.0/AUTHORS.rst
+-rw-r--r--   0 klauer   (1318172782) 1704612529     3038 2020-01-24 00:08:39.000000 pcdsutils-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2499 2021-07-22 18:46:35.000000 pcdsutils-0.7.0/LICENSE
+-rw-r--r--   0 klauer   (1318172782) 1704612529      362 2020-01-24 00:08:39.000000 pcdsutils-0.7.0/MANIFEST.in
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1026 2022-03-25 17:45:21.360710 pcdsutils-0.7.0/PKG-INFO
+-rw-r--r--   0 klauer   (1318172782) 1704612529      631 2020-01-24 00:08:39.000000 pcdsutils-0.7.0/README.rst
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-03-25 17:45:21.349696 pcdsutils-0.7.0/docs/
+-rw-r--r--   0 klauer   (1318172782) 1704612529      625 2021-07-22 18:46:35.000000 pcdsutils-0.7.0/docs/Makefile
+-rw-r--r--   0 klauer   (1318172782) 1704612529      796 2020-01-24 00:08:39.000000 pcdsutils-0.7.0/docs/make.bat
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-03-25 17:45:21.350410 pcdsutils-0.7.0/docs/source/
+-rw-r--r--   0 klauer   (1318172782) 1704612529     5450 2021-07-22 18:46:35.000000 pcdsutils-0.7.0/docs/source/conf.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529      587 2020-01-24 00:08:39.000000 pcdsutils-0.7.0/docs/source/index.rst
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-03-25 17:45:21.362161 pcdsutils-0.7.0/pcdsutils/
+-rw-r--r--   0 klauer   (1318172782) 1704612529      197 2022-03-25 17:45:19.000000 pcdsutils-0.7.0/pcdsutils/__init__.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529      497 2022-03-25 17:45:21.362305 pcdsutils-0.7.0/pcdsutils/_version.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     3108 2022-03-25 17:45:19.000000 pcdsutils-0.7.0/pcdsutils/enum.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     6205 2022-03-25 17:45:19.000000 pcdsutils-0.7.0/pcdsutils/ext_scripts.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    26815 2022-03-25 17:45:19.000000 pcdsutils-0.7.0/pcdsutils/log.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-03-25 17:45:21.357231 pcdsutils-0.7.0/pcdsutils/qt/
+-rw-r--r--   0 klauer   (1318172782) 1704612529      463 2020-05-15 18:20:28.000000 pcdsutils-0.7.0/pcdsutils/qt/__init__.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    12405 2020-05-15 17:59:37.000000 pcdsutils-0.7.0/pcdsutils/qt/popbar.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2563 2021-01-21 18:44:03.000000 pcdsutils-0.7.0/pcdsutils/release_notes.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     8113 2021-07-22 18:28:02.000000 pcdsutils-0.7.0/pcdsutils/requirements.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-03-25 17:45:21.360151 pcdsutils-0.7.0/pcdsutils/tests/
+-rw-r--r--   0 klauer   (1318172782) 1704612529        0 2020-01-24 00:08:39.000000 pcdsutils-0.7.0/pcdsutils/tests/__init__.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529        0 2020-01-24 00:08:39.000000 pcdsutils-0.7.0/pcdsutils/tests/conftest.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2097 2022-03-25 17:45:19.000000 pcdsutils-0.7.0/pcdsutils/tests/test_enum.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2653 2022-03-25 17:45:19.000000 pcdsutils-0.7.0/pcdsutils/tests/test_ext_scripts.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    10104 2022-03-25 17:45:19.000000 pcdsutils-0.7.0/pcdsutils/tests/test_logging.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529      644 2021-07-22 18:46:35.000000 pcdsutils-0.7.0/pcdsutils/tests/test_requirements.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1692 2021-07-22 18:46:35.000000 pcdsutils-0.7.0/pcdsutils/tests/test_utils.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2374 2021-11-29 22:01:24.000000 pcdsutils-0.7.0/pcdsutils/utils.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-03-25 17:45:21.356387 pcdsutils-0.7.0/pcdsutils.egg-info/
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1026 2022-03-25 17:45:21.000000 pcdsutils-0.7.0/pcdsutils.egg-info/PKG-INFO
+-rw-r--r--   0 klauer   (1318172782) 1704612529      823 2022-03-25 17:45:21.000000 pcdsutils-0.7.0/pcdsutils.egg-info/SOURCES.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529        1 2022-03-25 17:45:21.000000 pcdsutils-0.7.0/pcdsutils.egg-info/dependency_links.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529      161 2022-03-25 17:45:21.000000 pcdsutils-0.7.0/pcdsutils.egg-info/entry_points.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529       46 2022-03-25 17:45:21.000000 pcdsutils-0.7.0/pcdsutils.egg-info/requires.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529       10 2022-03-25 17:45:21.000000 pcdsutils-0.7.0/pcdsutils.egg-info/top_level.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529       46 2022-03-25 17:45:14.000000 pcdsutils-0.7.0/requirements.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529      177 2022-03-25 17:45:21.361376 pcdsutils-0.7.0/setup.cfg
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2205 2021-07-22 18:46:35.000000 pcdsutils-0.7.0/setup.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    68573 2021-11-29 22:01:24.000000 pcdsutils-0.7.0/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pcdsutils-0.6.0/versioneer.py` & `pcdsutils-0.7.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `pcdsutils-0.6.0/docs/Makefile` & `pcdsutils-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pcdsutils-0.6.0/docs/source/conf.py` & `pcdsutils-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pcdsutils-0.6.0/docs/source/index.rst` & `pcdsutils-0.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pcdsutils-0.6.0/docs/make.bat` & `pcdsutils-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pcdsutils-0.6.0/CONTRIBUTING.rst` & `pcdsutils-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pcdsutils-0.6.0/PKG-INFO` & `pcdsutils-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdsutils
-Version: 0.6.0
+Version: 0.7.0
 Summary: PCDS Python Utilities
 Home-page: https://github.com/pcdshub/pcdsutils
 Author: SLAC National Accelerator Laboratory
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `pcdsutils-0.6.0/pcdsutils.egg-info/PKG-INFO` & `pcdsutils-0.7.0/pcdsutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdsutils
-Version: 0.6.0
+Version: 0.7.0
 Summary: PCDS Python Utilities
 Home-page: https://github.com/pcdshub/pcdsutils
 Author: SLAC National Accelerator Laboratory
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `pcdsutils-0.6.0/pcdsutils.egg-info/SOURCES.txt` & `pcdsutils-0.7.0/pcdsutils.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 versioneer.py
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 docs/source/index.rst
 pcdsutils/__init__.py
 pcdsutils/_version.py
+pcdsutils/enum.py
 pcdsutils/ext_scripts.py
 pcdsutils/log.py
 pcdsutils/release_notes.py
 pcdsutils/requirements.py
 pcdsutils/utils.py
 pcdsutils.egg-info/PKG-INFO
 pcdsutils.egg-info/SOURCES.txt
@@ -24,11 +25,12 @@
 pcdsutils.egg-info/entry_points.txt
 pcdsutils.egg-info/requires.txt
 pcdsutils.egg-info/top_level.txt
 pcdsutils/qt/__init__.py
 pcdsutils/qt/popbar.py
 pcdsutils/tests/__init__.py
 pcdsutils/tests/conftest.py
+pcdsutils/tests/test_enum.py
 pcdsutils/tests/test_ext_scripts.py
 pcdsutils/tests/test_logging.py
 pcdsutils/tests/test_requirements.py
 pcdsutils/tests/test_utils.py
```

### Comparing `pcdsutils-0.6.0/LICENSE` & `pcdsutils-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pcdsutils-0.6.0/README.rst` & `pcdsutils-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `pcdsutils-0.6.0/pcdsutils/release_notes.py` & `pcdsutils-0.7.0/pcdsutils/release_notes.py`

 * *Files identical despite different names*

### Comparing `pcdsutils-0.6.0/pcdsutils/qt/popbar.py` & `pcdsutils-0.7.0/pcdsutils/qt/popbar.py`

 * *Files identical despite different names*

### Comparing `pcdsutils-0.6.0/pcdsutils/utils.py` & `pcdsutils-0.7.0/pcdsutils/utils.py`

 * *Files identical despite different names*

### Comparing `pcdsutils-0.6.0/pcdsutils/tests/test_requirements.py` & `pcdsutils-0.7.0/pcdsutils/tests/test_requirements.py`

 * *Files identical despite different names*

### Comparing `pcdsutils-0.6.0/pcdsutils/tests/test_ext_scripts.py` & `pcdsutils-0.7.0/pcdsutils/tests/test_ext_scripts.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,14 +28,24 @@
     def fake_hutch_name(*args, **kwargs):
         return 'tst\n'
 
     monkeypatch.setattr(ext, 'call_script', fake_hutch_name)
     assert ext.get_hutch_name() == 'tst'
 
 
+def test_experiment_name(monkeypatch):
+    logger.debug('test_experiment_name')
+
+    def fake_experiment_name(*args, **kwargs):
+        return 'tst\n'
+
+    monkeypatch.setattr(ext, 'call_script', fake_experiment_name)
+    assert ext.get_current_experiment() == 'tst'
+
+
 def test_run_number(monkeypatch):
     logger.debug('test_run_number')
 
     def fake_run_number(*args, **kwargs):
         return '1\n'
 
     monkeypatch.setattr(ext, 'call_script', fake_run_number)
```

### Comparing `pcdsutils-0.6.0/pcdsutils/tests/test_utils.py` & `pcdsutils-0.7.0/pcdsutils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pcdsutils-0.6.0/pcdsutils/log.py` & `pcdsutils-0.7.0/pcdsutils/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -526,14 +526,15 @@
         level: typing.Union[str, int] = logging.DEBUG,
         only_duplicates: bool = True,
     ):
         self.levelno = validate_log_level(level)
         self.levelname = logging.getLevelName(self.levelno)
         self.only_duplicates = only_duplicates
         self.cache = set()
+        self._level_cache = {}
         self.counter = 0
         self._logger = None
 
     @classmethod
     def install(
         cls,
         level: typing.Union[str, int] = logging.DEBUG,
@@ -605,16 +606,42 @@
         except ValueError:
             return True
         if self.should_demote(record, info) and record.levelno > self.levelno:
             if info in self.cache or not self.only_duplicates:
                 record.levelno = self.levelno
                 record.levelname = self.levelname
                 self.counter += 1
+                # Assume we're applied either to a logger or to a handler
+                # Find the logger or handler instance and check the level
+                # If our demoted level is too low, return False here to veto
+                # Required since level is checked before filter
+                # If we've seen the logger before, use the cache
+                try:
+                    return self.levelno >= self._level_cache[record.name].level
+                except KeyError:
+                    ...
+                # Check all parent loggers and handlers until we find it
+                check_logger = logging.getLogger(record.name)
+                depth = 10
+                while depth > 0 and check_logger is not None:
+                    if self in check_logger.filters:
+                        # We found it!
+                        self._level_cache[record.name] = check_logger
+                        return self.levelno >= check_logger.level
+                    for check_handler in check_logger.handlers:
+                        if self in check_handler.filters:
+                            # We found it!
+                            self._level_cache[record.name] = check_handler
+                            return self.levelno >= check_handler.level
+                    check_logger = check_logger.parent
+                    # Escape hatch for potential infinite loops
+                    depth -= 1
             else:
                 self.cache.add(info)
+        # If we got this far, just let the record pass
         return True
 
     def reset_counter(self):
         self.counter = 0
 
     def should_demote(
         self,
```

### Comparing `pcdsutils-0.6.0/pcdsutils/requirements.py` & `pcdsutils-0.7.0/pcdsutils/requirements.py`

 * *Files identical despite different names*

### Comparing `pcdsutils-0.6.0/pcdsutils/ext_scripts.py` & `pcdsutils-0.7.0/pcdsutils/ext_scripts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import re
 import socket
 import subprocess
-
+from typing import Optional
 
 logger = logging.getLogger(__name__)
 CNF = '/reg/g/pcds/dist/pds/{0}/scripts/{0}.cnf'
 SCRIPTS = '/reg/g/pcds/engineering_tools/{}/scripts/{}'
 TOOLS = '/reg/g/pcds/dist/pds/tools/{}/{}'
 
 
@@ -92,15 +92,19 @@
     return name.lower().strip(' \n')
 
 
 # API Backwards compatibility
 hutch_name = get_hutch_name
 
 
-def get_run_number(hutch=None, live=False, timeout=1):
+def get_run_number(
+    hutch: Optional[str] = None,
+    live: bool = False,
+    timeout: float = 1.,
+):
     """
     Call get_lastRun to return the run number of the last daq run.
 
     Parameters
     ----------
     hutch : str, optional
         The name of the hutch to get the run number for. If omitted, the hutch
@@ -124,15 +128,51 @@
         args += ['-i', hutch]
     if live:
         args += ['-l']
     run_number = call_script(args, timeout=timeout)
     return int(run_number)
 
 
-def get_ami_proxy(hutch, timeout=10):
+def get_current_experiment(
+    hutch: Optional[str] = None,
+    live: bool = False,
+    timeout: float = 1.,
+):
+    """
+    Call get_curr_exp to return the current experiment name.
+
+    Parameters
+    ----------
+    hutch : str, optional
+        The name of the hutch to get the experiment for. If omitted, the hutch
+        name will be determined automatically via cli argument.
+
+    live : bool, optional
+        Defaults to False. If True, we'll return the experiment of the current
+        run.
+
+    timeout : int or float, optional
+        Time to wait for get_curr_exp to finish.
+        Defaults to a 1 second timeout.
+
+    Returns
+    -------
+    experiment_name : str
+    """
+    args = [
+        SCRIPTS.format(hutch or "latest", "get_curr_exp")
+    ]
+    if hutch is not None:
+        args += ["-i", hutch]
+    if live:
+        args += ["-l"]
+    return (call_script(args, timeout=timeout) or "unknown").strip()
+
+
+def get_ami_proxy(hutch: str, timeout: float = 10.):
     """
     Call procmgr to determine the lcls-I ami proxy hostname.
 
     This function caches the output.
 
     This works using a regex on the output text from procmgr ami status.
```

### Comparing `pcdsutils-0.6.0/setup.py` & `pcdsutils-0.7.0/setup.py`

 * *Files identical despite different names*

