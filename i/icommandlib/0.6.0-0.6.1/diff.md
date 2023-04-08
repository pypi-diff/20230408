# Comparing `tmp/icommandlib-0.6.0.tar.gz` & `tmp/icommandlib-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icommandlib-0.6.0.tar", last modified: Tue Apr  4 12:58:22 2023, max compression
+gzip compressed data, was "icommandlib-0.6.1.tar", last modified: Sat Apr  8 16:26:27 2023, max compression
```

## Comparing `icommandlib-0.6.0.tar` & `icommandlib-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 12:58:22.740829 icommandlib-0.6.0/
--rw-r--r--   0 root         (0) root         (0)     1057 2023-04-04 12:57:47.000000 icommandlib-0.6.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-04 12:57:47.000000 icommandlib-0.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      863 2023-04-04 12:58:22.740829 icommandlib-0.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      405 2023-04-04 12:57:47.000000 icommandlib-0.6.0/README.rst
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-04 12:57:47.000000 icommandlib-0.6.0/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 12:58:22.736829 icommandlib-0.6.0/icommandlib/
--rw-r--r--   0 root         (0) root         (0)      216 2023-04-04 12:57:47.000000 icommandlib-0.6.0/icommandlib/__init__.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-04-04 12:57:47.000000 icommandlib-0.6.0/icommandlib/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     9083 2023-04-04 12:57:47.000000 icommandlib-0.6.0/icommandlib/handle.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-04-04 12:57:47.000000 icommandlib-0.6.0/icommandlib/icommand.py
--rw-r--r--   0 root         (0) root         (0)    10156 2023-04-04 12:57:47.000000 icommandlib-0.6.0/icommandlib/iprocess.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-04-04 12:57:47.000000 icommandlib-0.6.0/icommandlib/messages.py
--rw-r--r--   0 root         (0) root         (0)     1939 2023-04-04 12:57:47.000000 icommandlib-0.6.0/icommandlib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 12:58:22.736829 icommandlib-0.6.0/icommandlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      863 2023-04-04 12:58:22.000000 icommandlib-0.6.0/icommandlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      439 2023-04-04 12:58:22.000000 icommandlib-0.6.0/icommandlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 12:58:22.000000 icommandlib-0.6.0/icommandlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 12:57:57.000000 icommandlib-0.6.0/icommandlib.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-04 12:58:22.000000 icommandlib-0.6.0/icommandlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-04 12:58:22.000000 icommandlib-0.6.0/icommandlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1136 2023-04-04 12:57:47.000000 icommandlib-0.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-04 12:58:22.740829 icommandlib-0.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1842 2023-04-04 12:57:47.000000 icommandlib-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 16:26:27.233124 icommandlib-0.6.1/
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-04-08 16:26:00.000000 icommandlib-0.6.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-04-08 16:26:00.000000 icommandlib-0.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-04-08 16:26:27.233124 icommandlib-0.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2023-04-08 16:26:00.000000 icommandlib-0.6.1/README.md
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-08 16:26:00.000000 icommandlib-0.6.1/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 16:26:27.233124 icommandlib-0.6.1/icommandlib/
+-rw-r--r--   0 root         (0) root         (0)      216 2023-04-08 16:26:00.000000 icommandlib-0.6.1/icommandlib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-04-08 16:26:00.000000 icommandlib-0.6.1/icommandlib/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-04-08 16:26:00.000000 icommandlib-0.6.1/icommandlib/icommand.py
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-04-08 16:26:00.000000 icommandlib-0.6.1/icommandlib/iprocess.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-04-08 16:26:00.000000 icommandlib-0.6.1/icommandlib/messages.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-04-08 16:26:00.000000 icommandlib-0.6.1/icommandlib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 16:26:27.233124 icommandlib-0.6.1/icommandlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-04-08 16:26:27.000000 icommandlib-0.6.1/icommandlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      382 2023-04-08 16:26:27.000000 icommandlib-0.6.1/icommandlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-08 16:26:27.000000 icommandlib-0.6.1/icommandlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-08 16:26:27.000000 icommandlib-0.6.1/icommandlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-08 16:26:27.000000 icommandlib-0.6.1/icommandlib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-04-08 16:26:00.000000 icommandlib-0.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-08 16:26:27.233124 icommandlib-0.6.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-08 16:26:00.000000 icommandlib-0.6.1/setup.py
```

### Comparing `icommandlib-0.6.0/LICENSE.txt` & `icommandlib-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `icommandlib-0.6.0/PKG-INFO` & `icommandlib-0.6.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: icommandlib
-Version: 0.6.0
+Version: 0.6.1
 Summary: Pythonic interactive command runner.
-Home-page: https://github.com/crdoconnor/icommandlib
-Author: Colm O'Connor
 Author-email: Colm O'Connor <colm.oconnor.github@gmail.com>
 License: MIT
 Project-URL: homepage, https://hitchdev.com/icommandlib
 Project-URL: documentation, https://hitchdev.com/icommandlib/using
 Project-URL: repository, https://github.com/icommandlib/hitchstory
 Project-URL: changelog, https://hitchdev.com/icommandlib/changelog
 Keywords: subprocess,cli,interactive
@@ -15,7 +13,26 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+
+# ICommandLib
+
+The interactive command library.
+
+ICommandLib is a pythonic tool for running UNIX processes in a virtual terminal
+and interacting with them. It's a bit like pexpect.
+
+It depends upon [CommandLib](https://hitchdev.com/commandlib), which is necessary for defining the commands which you want to run.
+
+To install:
+
+```sh
+$ pip install icommandlib
+```
+
+## Documentation
+
+Coming soon.
```

### Comparing `icommandlib-0.6.0/icommandlib/exceptions.py` & `icommandlib-0.6.1/icommandlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `icommandlib-0.6.0/icommandlib/icommand.py` & `icommandlib-0.6.1/icommandlib/icommand.py`

 * *Files identical despite different names*

### Comparing `icommandlib-0.6.0/icommandlib/iprocess.py` & `icommandlib-0.6.1/icommandlib/iprocess.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,28 +37,14 @@
     An interactive process.
 
         Start process by initializing with an commandlib.Command object.
     """
 
     def __init__(self, icommand):
         self._icommand = icommand
-        # self._order_queue = queue.Queue()
-        # self._event_queue = queue.Queue()
-        # self._handle = threading.Thread(
-        # target=IProcessHandle,
-        # args=(icommand, self._order_queue, self._event_queue)
-        # )
-        # self._handle.start()
-
-        # self._running_process = self._wait_for_event(message.ProcessStartedMessage)
-
-        # self._pid = self._running_process._pid
-        # self._master_fd = self._running_process._stdin
-        # self._async_send = self._wait_for_event(message.AsyncSendMethodMessage)
-
         self._ptyprocess = PtyProcessUnicode.spawn(
             argv=icommand._command.arguments,
             env=icommand._command.env,
             cwd=icommand._command.directory,
             dimensions=(icommand.width, icommand.height),
         )
         self.psutil = psutil.Process(self._ptyprocess.pid)
@@ -81,60 +67,14 @@
     def _die_gracefully(self, *args):
         proc = psutil.Process(self.pid)
         for descendant in proc.children(recursive=True):
             descendant.kill()
         self._read()
         proc.kill()
 
-    # def _check_events(self, expected=None):
-    # try:
-    # response = self._event_queue.get(block=False)
-    # except queue.Empty:
-    # response = None
-
-    # if response is not None:
-    # return self._handle_event(response, of_kind=expected)
-
-    # def _handle_event(self, response, of_kind=None):
-    # if isinstance(response, message.ExceptionMessage):
-    # raise response.value
-    # if isinstance(response, message.TimeoutMessage):
-    # raise exceptions.IProcessTimeout(
-    # "Timed out after {0} seconds:\n\n{1}".format(
-    # response.after,
-    # stripshot(response.screenshot),
-    # )
-    # )
-    # if isinstance(response, message.ExitMessage):
-    # self._running = False
-    # self._pid = None
-    # self._exit_code = response.value.exit_code
-    # self._final_screenshot = response.value.screenshot
-    # if of_kind != message.ExitMessage:
-    # raise exceptions.UnexpectedExit(
-    # response.value.exit_code,
-    # response.value.screenshot,
-    # )
-    # if not isinstance(response, of_kind):
-    # raise Exception(
-    # "Threading error expected {0} got {1}".format(
-    # type(of_kind), type(of_kind)
-    # )
-    # )
-    # return response.value
-
-    # def _wait_for_event(self, of_kind, timeout=None):
-    # try:
-    # response = self._event_queue.get(timeout=timeout)
-    # except queue.Empty:
-    # raise exceptions.IProcessTimeout(
-    # "Timed out waiting for exit."
-    # )
-    # return self._handle_event(response, of_kind=of_kind)
-
     @property
     def pid(self):
         if not self.running:
             return None
         return self._ptyprocess.pid
 
     @property
@@ -147,38 +87,38 @@
                 return False
         except psutil.NoSuchProcess:
             return False
         return self.psutil.is_running()
 
     @property
     def exit_code(self):
-        # self._check_events(expected=message.ExitMessage)
         if self.running:
             return None
         try:
             if self.psutil.status() == "zombie":
                 self._ptyprocess.wait()
                 return self._ptyprocess.exitstatus
         except psutil.NoSuchProcess:
             pass
         if self._ptyprocess.exitstatus is None:
-            import web_pdb
-
-            web_pdb.set_trace()
+            raise Exception(
+                (
+                    "This shouldn't happen. "
+                    "Please raise bug at https://github.com/crdoconnor/icommandlib"
+                )
+            )
         return self._ptyprocess.exitstatus
 
     def _read(self):
         fd = self._ptyprocess.fd
 
         if fd != -1:
             readable, _, _ = select.select([fd], [], [], 0.01)
 
-            if len(readable) == 0:
-                time.sleep(0.01)
-            else:
+            if len(readable) != 0:
                 try:
                     text = self._ptyprocess.read()
                     self.iscreen.feed(text)
                 except EOFError:
                     pass
 
     def wait_until(self, condition_function, timeout=None):
@@ -277,42 +217,36 @@
         """
         if timeout is None:
             timeout = 10.0
 
         start_time = time.time()
 
         while True:
+            self._read()
+
             if not self._ptyprocess.isalive():
-                self._read()
                 self._ptyprocess.close()
                 self.finished = True
                 return
 
-            time.sleep(0.01)
-
             if time.time() - start_time > timeout:
-                self._read()
                 raise exceptions.IProcessTimeout(
                     "Timed out after {0} seconds:\n\n{1}".format(
                         timeout,
                         stripshot(self.iscreen.text),
                     )
                 )
 
     def wait_for_successful_exit(self, timeout=None):
         """
         Wait until the process exits successfully. Raises exception
         if the process is still open after timeout or it exits
         with an exit code other than 0.
         """
         self.wait_for_finish(timeout=timeout)
-
-        # self._ptyprocess.wait()
-        # assert self._ptyprocess.exitstatus is not None
-
         exit_status = self.exit_code
 
         if exit_status != 0:
             raise exceptions.ExitWithError(
                 exit_status,
                 stripshot(self.iscreen.text),
             )
```

### Comparing `icommandlib-0.6.0/icommandlib/messages.py` & `icommandlib-0.6.1/icommandlib/messages.py`

 * *Files identical despite different names*

### Comparing `icommandlib-0.6.0/icommandlib/utils.py` & `icommandlib-0.6.1/icommandlib/utils.py`

 * *Files identical despite different names*

### Comparing `icommandlib-0.6.0/icommandlib.egg-info/PKG-INFO` & `icommandlib-0.6.1/icommandlib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: icommandlib
-Version: 0.6.0
+Version: 0.6.1
 Summary: Pythonic interactive command runner.
-Home-page: https://github.com/crdoconnor/icommandlib
-Author: Colm O'Connor
 Author-email: Colm O'Connor <colm.oconnor.github@gmail.com>
 License: MIT
 Project-URL: homepage, https://hitchdev.com/icommandlib
 Project-URL: documentation, https://hitchdev.com/icommandlib/using
 Project-URL: repository, https://github.com/icommandlib/hitchstory
 Project-URL: changelog, https://hitchdev.com/icommandlib/changelog
 Keywords: subprocess,cli,interactive
@@ -15,7 +13,26 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+
+# ICommandLib
+
+The interactive command library.
+
+ICommandLib is a pythonic tool for running UNIX processes in a virtual terminal
+and interacting with them. It's a bit like pexpect.
+
+It depends upon [CommandLib](https://hitchdev.com/commandlib), which is necessary for defining the commands which you want to run.
+
+To install:
+
+```sh
+$ pip install icommandlib
+```
+
+## Documentation
+
+Coming soon.
```

### Comparing `icommandlib-0.6.0/pyproject.toml` & `icommandlib-0.6.1/pyproject.toml`

 * *Files identical despite different names*

