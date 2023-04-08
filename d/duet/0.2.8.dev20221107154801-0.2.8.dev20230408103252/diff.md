# Comparing `tmp/duet-0.2.8.dev20221107154801.tar.gz` & `tmp/duet-0.2.8.dev20230408103252.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duet-0.2.8.dev20221107154801.tar", last modified: Mon Nov  7 23:48:03 2022, max compression
+gzip compressed data, was "duet-0.2.8.dev20230408103252.tar", last modified: Sat Apr  8 17:32:52 2023, max compression
```

## Comparing `duet-0.2.8.dev20221107154801.tar` & `duet-0.2.8.dev20230408103252.tar`

### file list

```diff
@@ -1,39 +1,29 @@
-drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2022-11-07 23:48:03.232554 duet-0.2.8.dev20221107154801/
-drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2022-11-07 23:48:03.228554 duet-0.2.8.dev20221107154801/.github/
-drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2022-11-07 23:48:03.232554 duet-0.2.8.dev20221107154801/.github/workflows/
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     3106 2022-06-17 16:43:02.000000 duet-0.2.8.dev20221107154801/.github/workflows/ci.yml
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1819 2021-10-20 18:54:16.000000 duet-0.2.8.dev20221107154801/.gitignore
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)      383 2022-03-31 21:10:31.000000 duet-0.2.8.dev20221107154801/.mypy.ini
--rw-r-----   0 maffoo   (237528) primarygroup (89939)      945 2021-02-10 21:37:09.000000 duet-0.2.8.dev20221107154801/.pylintrc
--rw-r-----   0 maffoo   (237528) primarygroup (89939)      296 2021-02-06 15:18:23.000000 duet-0.2.8.dev20221107154801/AUTHORS
--rw-r-----   0 maffoo   (237528) primarygroup (89939)     1103 2021-02-05 22:48:38.000000 duet-0.2.8.dev20221107154801/CONTRIBUTING.md
--rw-r-----   0 maffoo   (237528) primarygroup (89939)    11357 2021-02-05 22:48:38.000000 duet-0.2.8.dev20221107154801/LICENSE
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)       70 2022-03-31 21:10:31.000000 duet-0.2.8.dev20221107154801/MANIFEST.in
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1994 2022-11-07 23:48:03.232554 duet-0.2.8.dev20221107154801/PKG-INFO
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1496 2021-10-20 18:54:16.000000 duet-0.2.8.dev20221107154801/README.md
-drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2022-11-07 23:48:03.232554 duet-0.2.8.dev20221107154801/dev/
--rwxr-x---   0 maffoo   (237528) primarygroup (89939)      688 2021-09-30 08:10:16.000000 duet-0.2.8.dev20221107154801/dev/build
--rwxr-x---   0 maffoo   (237528) primarygroup (89939)       80 2021-02-10 21:37:09.000000 duet-0.2.8.dev20221107154801/dev/check
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)       95 2022-04-12 22:55:13.000000 duet-0.2.8.dev20221107154801/dev/requirements.txt
-drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2022-11-07 23:48:03.232554 duet-0.2.8.dev20221107154801/duet/
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     2247 2021-10-20 18:54:16.000000 duet-0.2.8.dev20221107154801/duet/__init__.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)      608 2022-07-15 23:14:24.000000 duet-0.2.8.dev20221107154801/duet/_version.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     3543 2021-10-20 18:54:16.000000 duet-0.2.8.dev20221107154801/duet/aitertools.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)    16725 2022-11-07 23:35:49.000000 duet-0.2.8.dev20221107154801/duet/api.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)    19623 2022-11-07 21:58:06.000000 duet-0.2.8.dev20221107154801/duet/api_test.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     6041 2022-03-31 21:10:31.000000 duet-0.2.8.dev20221107154801/duet/futuretools.py
--rw-r-----   0 maffoo   (237528) primarygroup (89939)     1657 2021-02-10 21:37:09.000000 duet-0.2.8.dev20221107154801/duet/futuretools_test.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)    16643 2022-11-07 23:20:27.000000 duet-0.2.8.dev20221107154801/duet/impl.py
--rw-r-----   0 maffoo   (237528) primarygroup (89939)     2486 2021-02-10 21:37:09.000000 duet-0.2.8.dev20221107154801/duet/impl_test.py
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)       59 2021-10-20 18:54:16.000000 duet-0.2.8.dev20221107154801/duet/py.typed
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     3297 2022-11-07 21:58:06.000000 duet-0.2.8.dev20221107154801/duet/typing.py
-drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2022-11-07 23:48:03.232554 duet-0.2.8.dev20221107154801/duet.egg-info/
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1994 2022-11-07 23:48:02.000000 duet-0.2.8.dev20221107154801/duet.egg-info/PKG-INFO
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)      527 2022-11-07 23:48:03.000000 duet-0.2.8.dev20221107154801/duet.egg-info/SOURCES.txt
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)        1 2022-11-07 23:48:02.000000 duet-0.2.8.dev20221107154801/duet.egg-info/dependency_links.txt
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)      148 2022-11-07 23:48:02.000000 duet-0.2.8.dev20221107154801/duet.egg-info/requires.txt
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)        5 2022-11-07 23:48:02.000000 duet-0.2.8.dev20221107154801/duet.egg-info/top_level.txt
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)      247 2022-04-12 22:55:13.000000 duet-0.2.8.dev20221107154801/pyproject.toml
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)       53 2022-06-17 16:43:02.000000 duet-0.2.8.dev20221107154801/requirements.txt
--rw-r-----   0 maffoo   (237528) primarygroup (89939)       73 2022-11-07 23:48:03.232554 duet-0.2.8.dev20221107154801/setup.cfg
--rw-r--r--   0 maffoo   (237528) primarygroup (89939)     2387 2022-06-17 16:43:02.000000 duet-0.2.8.dev20221107154801/setup.py
+drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2023-04-08 17:32:52.850382 duet-0.2.8.dev20230408103252/
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)    11357 2022-05-04 07:11:02.000000 duet-0.2.8.dev20230408103252/LICENSE
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)       70 2023-04-08 17:31:34.000000 duet-0.2.8.dev20230408103252/MANIFEST.in
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1994 2023-04-08 17:32:52.850382 duet-0.2.8.dev20230408103252/PKG-INFO
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1496 2022-05-04 07:11:02.000000 duet-0.2.8.dev20230408103252/README.md
+drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2023-04-08 17:32:52.850382 duet-0.2.8.dev20230408103252/dev/
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)       95 2023-04-08 17:31:34.000000 duet-0.2.8.dev20230408103252/dev/requirements.txt
+drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2023-04-08 17:32:52.850382 duet-0.2.8.dev20230408103252/duet/
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     2247 2023-04-08 17:31:34.000000 duet-0.2.8.dev20230408103252/duet/__init__.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)      608 2023-04-08 17:31:34.000000 duet-0.2.8.dev20230408103252/duet/_version.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     3543 2022-05-04 07:11:02.000000 duet-0.2.8.dev20230408103252/duet/aitertools.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)    17205 2023-04-08 17:31:42.000000 duet-0.2.8.dev20230408103252/duet/api.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)    19623 2023-04-08 17:31:34.000000 duet-0.2.8.dev20230408103252/duet/api_test.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     6041 2023-04-08 17:31:34.000000 duet-0.2.8.dev20230408103252/duet/futuretools.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1657 2022-05-04 07:11:02.000000 duet-0.2.8.dev20230408103252/duet/futuretools_test.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)    15991 2023-04-08 17:31:42.000000 duet-0.2.8.dev20230408103252/duet/impl.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     2486 2022-05-04 07:11:02.000000 duet-0.2.8.dev20230408103252/duet/impl_test.py
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)       59 2022-05-04 07:11:02.000000 duet-0.2.8.dev20230408103252/duet/py.typed
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     3297 2023-04-08 17:31:34.000000 duet-0.2.8.dev20230408103252/duet/typing.py
+drwxr-xr-x   0 maffoo   (237528) primarygroup (89939)        0 2023-04-08 17:32:52.850382 duet-0.2.8.dev20230408103252/duet.egg-info/
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     1994 2023-04-08 17:32:52.000000 duet-0.2.8.dev20230408103252/duet.egg-info/PKG-INFO
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)      427 2023-04-08 17:32:52.000000 duet-0.2.8.dev20230408103252/duet.egg-info/SOURCES.txt
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)        1 2023-04-08 17:32:52.000000 duet-0.2.8.dev20230408103252/duet.egg-info/dependency_links.txt
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)      148 2023-04-08 17:32:52.000000 duet-0.2.8.dev20230408103252/duet.egg-info/requires.txt
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)        5 2023-04-08 17:32:52.000000 duet-0.2.8.dev20230408103252/duet.egg-info/top_level.txt
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)      247 2023-04-08 17:31:34.000000 duet-0.2.8.dev20230408103252/pyproject.toml
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)       53 2023-04-08 17:31:34.000000 duet-0.2.8.dev20230408103252/requirements.txt
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)       73 2023-04-08 17:32:52.850382 duet-0.2.8.dev20230408103252/setup.cfg
+-rw-r--r--   0 maffoo   (237528) primarygroup (89939)     2387 2023-04-08 17:31:34.000000 duet-0.2.8.dev20230408103252/setup.py
```

### Comparing `duet-0.2.8.dev20221107154801/LICENSE` & `duet-0.2.8.dev20230408103252/LICENSE`

 * *Files identical despite different names*

### Comparing `duet-0.2.8.dev20221107154801/PKG-INFO` & `duet-0.2.8.dev20230408103252/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duet
-Version: 0.2.8.dev20221107154801
+Version: 0.2.8.dev20230408103252
 Summary: A simple future-based async library for python.
 Home-page: http://github.com/google/duet
 Author: The Duet Authors
 Author-email: maffoo@google.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.7.0
```

### Comparing `duet-0.2.8.dev20221107154801/README.md` & `duet-0.2.8.dev20230408103252/README.md`

 * *Files identical despite different names*

### Comparing `duet-0.2.8.dev20221107154801/duet/__init__.py` & `duet-0.2.8.dev20230408103252/duet/__init__.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.8.dev20221107154801/duet/_version.py` & `duet-0.2.8.dev20230408103252/duet/_version.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.8.dev20221107154801/duet/aitertools.py` & `duet-0.2.8.dev20230408103252/duet/aitertools.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.8.dev20221107154801/duet/api.py` & `duet-0.2.8.dev20230408103252/duet/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,33 @@
         func: The async function to run.
         *args: Positional arguments to pass to func.
         **kwds: Keyword arguments to pass to func.
 
     Returns:
         The final result of the async function.
     """
-    with impl.Scheduler() as scheduler:
+    scheduler = impl.Scheduler()
+    scheduler.init_signals()
+    try:
         task = scheduler.spawn(func(*args, **kwds))
-    return task.result
+        try:
+            while scheduler.active_tasks:
+                scheduler.tick()
+        except BaseException as exc:
+            for task in scheduler.active_tasks:
+                task.interrupt(None, exc)
+            while scheduler.active_tasks:
+                try:
+                    scheduler.tick()
+                except BaseException:
+                    pass
+            raise
+        return task.result
+    finally:
+        scheduler.cleanup_signals()
 
 
 def sync(f: Callable[..., Awaitable[T]]) -> Callable[..., T]:
     """Decorator that adds a sync version of async function or method."""
     if isinstance(f, classmethod):
         raise TypeError(f"duet.sync cannot be applied to classmethod {f.__func__}")
     sig = inspect.signature(f)
```

### Comparing `duet-0.2.8.dev20221107154801/duet/api_test.py` & `duet-0.2.8.dev20230408103252/duet/api_test.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.8.dev20221107154801/duet/futuretools.py` & `duet-0.2.8.dev20230408103252/duet/futuretools.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.8.dev20221107154801/duet/futuretools_test.py` & `duet-0.2.8.dev20230408103252/duet/futuretools_test.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.8.dev20221107154801/duet/impl.py` & `duet-0.2.8.dev20230408103252/duet/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -437,39 +437,17 @@
     def _in_task(self, frame) -> bool:
         while frame is not None:
             if frame.f_locals.get(LOCALS_TASK_SCHEDULER, None) is self:
                 return True
             frame = frame.f_back
         return False
 
-    def __enter__(self):
+    def init_signals(self):
         if (
             threading.current_thread() == threading.main_thread()
             and signal.getsignal(signal.SIGINT) == signal.default_int_handler
         ):
             self._prev_signal = signal.signal(signal.SIGINT, self._interrupt)
-        return self
 
-    def __exit__(self, exc_type, exc, tb):
-        def finish_tasks(error=None):
-            if error:
-                for task in self.active_tasks:
-                    task.interrupt(None, error)
-            while self.active_tasks:
-                try:
-                    self.tick()
-                except BaseException:
-                    if not error:
-                        raise
-
-        try:
-            if exc:
-                finish_tasks(exc)
-            else:
-                try:
-                    finish_tasks()
-                except BaseException as exc:
-                    finish_tasks(exc)
-                    raise
-        finally:
-            if self._prev_signal:
-                signal.signal(signal.SIGINT, self._prev_signal)
+    def cleanup_signals(self):
+        if self._prev_signal:
+            signal.signal(signal.SIGINT, self._prev_signal)
```

### Comparing `duet-0.2.8.dev20221107154801/duet/impl_test.py` & `duet-0.2.8.dev20230408103252/duet/impl_test.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.8.dev20221107154801/duet/typing.py` & `duet-0.2.8.dev20230408103252/duet/typing.py`

 * *Files identical despite different names*

### Comparing `duet-0.2.8.dev20221107154801/duet.egg-info/PKG-INFO` & `duet-0.2.8.dev20230408103252/duet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duet
-Version: 0.2.8.dev20221107154801
+Version: 0.2.8.dev20230408103252
 Summary: A simple future-based async library for python.
 Home-page: http://github.com/google/duet
 Author: The Duet Authors
 Author-email: maffoo@google.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.7.0
```

### Comparing `duet-0.2.8.dev20221107154801/setup.py` & `duet-0.2.8.dev20230408103252/setup.py`

 * *Files identical despite different names*

