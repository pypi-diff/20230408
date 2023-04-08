# Comparing `tmp/scription-0.86.8.tar.gz` & `tmp/scription-0.86.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scription-0.86.8.tar", last modified: Tue Aug  3 03:35:59 2021, max compression
+gzip compressed data, was "scription-0.86.9.tar", last modified: Fri Apr 29 04:02:17 2022, max compression
```

## Comparing `scription-0.86.8.tar` & `scription-0.86.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2021-08-03 03:35:59.208917 scription-0.86.8/
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     4945 2021-08-03 03:35:59.208917 scription-0.86.8/PKG-INFO
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     3488 2021-08-03 03:25:47.000000 scription-0.86.8/README
-drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2021-08-03 03:35:59.208917 scription-0.86.8/scription/
--rw-rw-r--   0 ethan     (1000) ethan     (1000)    12761 2021-08-03 03:25:47.000000 scription-0.86.8/scription/CHANGES
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     1359 2021-08-03 03:25:47.000000 scription-0.86.8/scription/LICENSE
--rw-rw-r--   0 ethan     (1000) ethan     (1000)   146547 2021-08-03 03:25:47.000000 scription-0.86.8/scription/__init__.py
--rw-rw-r--   0 ethan     (1000) ethan     (1000)   158950 2021-08-03 03:25:47.000000 scription-0.86.8/scription/test.py
-drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2021-08-03 03:35:59.208917 scription-0.86.8/scription.egg-info/
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     4945 2021-08-03 03:35:59.000000 scription-0.86.8/scription.egg-info/PKG-INFO
--rw-rw-r--   0 ethan     (1000) ethan     (1000)      255 2021-08-03 03:35:59.000000 scription-0.86.8/scription.egg-info/SOURCES.txt
--rw-rw-r--   0 ethan     (1000) ethan     (1000)        1 2021-08-03 03:35:59.000000 scription-0.86.8/scription.egg-info/dependency_links.txt
--rw-rw-r--   0 ethan     (1000) ethan     (1000)       13 2021-08-03 03:35:59.000000 scription-0.86.8/scription.egg-info/requires.txt
--rw-rw-r--   0 ethan     (1000) ethan     (1000)       10 2021-08-03 03:35:59.000000 scription-0.86.8/scription.egg-info/top_level.txt
--rw-rw-r--   0 ethan     (1000) ethan     (1000)       38 2021-08-03 03:35:59.208917 scription-0.86.8/setup.cfg
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     4761 2021-08-03 03:25:47.000000 scription-0.86.8/setup.py
+drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2022-04-29 04:02:17.577573 scription-0.86.9/
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     4265 2022-04-29 04:02:17.577573 scription-0.86.9/PKG-INFO
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     3488 2022-04-29 03:50:35.000000 scription-0.86.9/README
+drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2022-04-29 04:02:17.577573 scription-0.86.9/scription/
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)    12761 2022-04-29 03:50:35.000000 scription-0.86.9/scription/CHANGES
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     1359 2022-04-29 03:50:35.000000 scription-0.86.9/scription/LICENSE
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)   148062 2022-04-29 03:50:35.000000 scription-0.86.9/scription/__init__.py
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)   159201 2022-04-29 03:50:35.000000 scription-0.86.9/scription/test.py
+drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2022-04-29 04:02:17.577573 scription-0.86.9/scription.egg-info/
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     4265 2022-04-29 04:02:17.000000 scription-0.86.9/scription.egg-info/PKG-INFO
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)      255 2022-04-29 04:02:17.000000 scription-0.86.9/scription.egg-info/SOURCES.txt
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)        1 2022-04-29 04:02:17.000000 scription-0.86.9/scription.egg-info/dependency_links.txt
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)       13 2022-04-29 04:02:17.000000 scription-0.86.9/scription.egg-info/requires.txt
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)       10 2022-04-29 04:02:17.000000 scription-0.86.9/scription.egg-info/top_level.txt
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)       38 2022-04-29 04:02:17.577573 scription-0.86.9/setup.cfg
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     4816 2022-04-29 03:50:35.000000 scription-0.86.9/setup.py
```

### Comparing `scription-0.86.8/PKG-INFO` & `scription-0.86.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,106 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: scription
-Version: 0.86.8
+Version: 0.86.9
 Summary: simple script parameter parser
 Home-page: https://github.com/ethanfurman/scription.git
 Author: Ethan Furman
 Author-email: ethan@stoneleaf.us
 License: BSD License
-Description: scription
-        
-        light-weight library to enhance command-line scripts; includes conversion of
-        parameters to specified data types, parameter checking, basic input/output with
-        users, support for suid [1], sending email, executing sub-programs, and having
-        sub-commands within a script
-        
-        
-        decorators
-        
-          - Script:  sets global variables and/or parameters for Commands; the decorated
-            function will be called by Main/Run before any specified Command
-        
-          - Command:  marks function as a subcommand for the script (e.g. add, delete,
-            list, etc.); if no subcommand is specified on the command-line, scription
-            will look for a Command with the same name as the script
-        
-          - Alias:  registers other names for Commands (e.g. delete / remove / kill)
-        
-        
-        functions
-        
-          - Main:  if the importing module's __name__ is __main__, call Run() (this
-            allows for importing the script as a module)
-        
-          - Run:  unconditionally attempts to run the Script function (if any) and the
-            Command found on the command-line
-        
-          Main() or Run() should be the last thing in the script
-        
-        
-        classes
-        
-          - Spec:  can be used when defining the command-line parameters (can also just
-            use tuples)
-        
-        
-        helper functions/classes
-        
-          - abort: quits immediately by raising SystemExit
-        
-          - Execute:  class for executing other programs; uses subprocess.Popen by
-            default, but if `pty=True` is specified then `pty.fork` will be used
-            (handy for programs that only accept input from a pty)
-        
-          - get_response:  function for displaying text and getting feedback
-        
-          - help: quits immediately, but adds a reference to --help in the quit message
-        
-          - log_exception:  logs an exception with logging.logger
-        
-          - mail: rudimentary mail sender
-        
-          - OrmFile:  lightweight orm -- supports str, int, float, date, time,
-            datetime, bool, and path (which defaults to str); custom data types can
-            also be specified
-        
-          - print: wrapper around print that adds a 'verbose_level' keyword (default: 1);
-            default verbosity is 0 (so print does nothing), but can be increased using
-            -v, -vv, --verbose, or --verbose=2 (in Python 2 the script must use
-            'from __future__ import print_function' to use scription's print)
-        
-          - user_ids:  context manager useful for suid scripts -- all actions taken
-            within the context are run as the user/group specified
-        
-        
-        features
-        
-          - extra parameters defined by Script are global, and can be accessed from any
-            function or Command
-        
-          - 'module' is a namespace inserted into the script
-        
-          - 'script_command' is the Command selected from the command line (useful when
-            one needs to call the subcommand directly from a main() function)
-        
-          - 'script_command_name' is the name of the script_command
-        
-          - 'script_verbosity' is the level of verboseness selected (defaults to 0)
-        
-          - 'script_name' is the name of the script
-        
-          - builtin options are:  --help, --verbose (-v or -vv), --version, --all-versions
-            --version attempts to display the version of the main package in use
-            --all-versions attempts to display the versions of any imported packages
-        
-          - command-line is decoded to unicode under Python 2 (Python 3 does this for us)
-        
-        
-        [1] I use the suid-python program, available at http://selliott.org/python/suid-python.c
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
@@ -110,7 +19,101 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+
+scription
+
+light-weight library to enhance command-line scripts; includes conversion of
+parameters to specified data types, parameter checking, basic input/output with
+users, support for suid [1], sending email, executing sub-programs, and having
+sub-commands within a script
+
+
+decorators
+
+  - Script:  sets global variables and/or parameters for Commands; the decorated
+    function will be called by Main/Run before any specified Command
+
+  - Command:  marks function as a subcommand for the script (e.g. add, delete,
+    list, etc.); if no subcommand is specified on the command-line, scription
+    will look for a Command with the same name as the script
+
+  - Alias:  registers other names for Commands (e.g. delete / remove / kill)
+
+
+functions
+
+  - Main:  if the importing module's __name__ is __main__, call Run() (this
+    allows for importing the script as a module)
+
+  - Run:  unconditionally attempts to run the Script function (if any) and the
+    Command found on the command-line
+
+  Main() or Run() should be the last thing in the script
+
+
+classes
+
+  - Spec:  can be used when defining the command-line parameters (can also just
+    use tuples)
+
+
+helper functions/classes
+
+  - abort: quits immediately by raising SystemExit
+
+  - Execute:  class for executing other programs; uses subprocess.Popen by
+    default, but if `pty=True` is specified then `pty.fork` will be used
+    (handy for programs that only accept input from a pty)
+
+  - get_response:  function for displaying text and getting feedback
+
+  - help: quits immediately, but adds a reference to --help in the quit message
+
+  - log_exception:  logs an exception with logging.logger
+
+  - mail: rudimentary mail sender
+
+  - OrmFile:  lightweight orm -- supports str, int, float, date, time,
+    datetime, bool, and path (which defaults to str); custom data types can
+    also be specified
+
+  - print: wrapper around print that adds a 'verbose_level' keyword (default: 1);
+    default verbosity is 0 (so print does nothing), but can be increased using
+    -v, -vv, --verbose, or --verbose=2 (in Python 2 the script must use
+    'from __future__ import print_function' to use scription's print)
+
+  - user_ids:  context manager useful for suid scripts -- all actions taken
+    within the context are run as the user/group specified
+
+
+features
+
+  - extra parameters defined by Script are global, and can be accessed from any
+    function or Command
+
+  - 'module' is a namespace inserted into the script
+
+  - 'script_command' is the Command selected from the command line (useful when
+    one needs to call the subcommand directly from a main() function)
+
+  - 'script_command_name' is the name of the script_command
+
+  - 'script_verbosity' is the level of verboseness selected (defaults to 0)
+
+  - 'script_name' is the name of the script
+
+  - builtin options are:  --help, --verbose (-v or -vv), --version, --all-versions
+    --version attempts to display the version of the main package in use
+    --all-versions attempts to display the versions of any imported packages
+
+  - command-line is decoded to unicode under Python 2 (Python 3 does this for us)
+
+
+[1] I use the suid-python program, available at http://selliott.org/python/suid-python.c
+
+
```

### Comparing `scription-0.86.8/README` & `scription-0.86.9/README`

 * *Files identical despite different names*

### Comparing `scription-0.86.8/scription/CHANGES` & `scription-0.86.9/scription/CHANGES`

 * *Files identical despite different names*

### Comparing `scription-0.86.8/scription/LICENSE` & `scription-0.86.9/scription/LICENSE`

 * *Files identical despite different names*

### Comparing `scription-0.86.8/scription/__init__.py` & `scription-0.86.9/scription/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,38 +29,56 @@
     specified, or type becomes the default value's type if unspecified
 """
 
 # future imports
 from __future__ import print_function
 
 # version
-version = 0, 86, 8
+version = 0, 86, 9
 
 # imports
 import sys
-py_ver = sys.version_info[:2]
+pyver = sys.version_info[:2]
+PY2 = pyver < (3, )
+PY3 = pyver >= (3, )
+PY25 = (2, 5)
+PY26 = (2, 6)
+PY33 = (3, 3)
+PY34 = (3, 4)
+PY35 = (3, 5)
+PY36 = (3, 6)
+
 is_win = sys.platform.startswith('win')
 if is_win:
     import signal
     KILL_SIGNALS = [getattr(signal, sig) for sig in ('SIGTERM') if hasattr(signal, sig)]
     from subprocess import Popen, PIPE
 else:
     from pty import fork
     import resource
     import termios
     # from syslog import syslog
     import signal
     KILL_SIGNALS = [getattr(signal, sig) for sig in ('SIGTERM', 'SIGQUIT', 'SIGKILL') if hasattr(signal, sig)]
     from subprocess import Popen, PIPE
+
 from threading import Thread
 try:
     from Queue import Queue, Empty
 except ImportError:
     from queue import Queue, Empty
 
+if PY3:
+    from inspect import getfullargspec
+    def getargspec(method):
+        args, varargs, keywords, defaults, _, _, _ = getfullargspec(method)
+        return args, varargs, keywords, defaults
+else:
+    from inspect import getargspec
+
 import ast
 import codecs
 import datetime
 import email
 import errno
 import inspect
 import locale
@@ -82,15 +100,15 @@
 
 # locks, etc.
 print_lock = threading.RLock()
 io_lock = threading.Lock()
 
 # py 2/3 compatibility shims
 raise_with_traceback = None
-if py_ver < (3, 0):
+if PY2:
     b = str
     u = unicode
     bytes = b
     str = u
     unicode = u
     basestring = bytes, unicode
     integer = int, long
@@ -388,15 +406,15 @@
 
 # internal
 def _add_annotations(func, annotations, script=False):
     '''
     add annotations as __scription__ to func
     '''
     scription_debug('adding annotations to %r' % (func.__name__, ))
-    params, varargs, keywords, defaults = inspect.getargspec(func)
+    params, varargs, keywords, defaults = getargspec(func)
     radio = {}
     if varargs:
         params.append(varargs)
     if keywords:
         params.append(keywords)
     errors = []
     default_order = 128
@@ -459,15 +477,15 @@
         return ''
 empty = empty()
 
 def _func_globals(func):
     '''
     return the function's globals
     '''
-    if py_ver < (3, 0):
+    if PY2:
         return func.func_globals
     else:
         return func.__globals__
 
 def _get_version(from_module, _try_other=True):
     for ver in _version_strings:
         if from_module.get(ver):
@@ -508,15 +526,15 @@
     return versions
 
 def _help(func, script=False):
     '''
     create help from __scription__ annotations and header defaults
     '''
     scription_debug('_help for', func.__name__, verbose=3)
-    params, vararg, keywordarg, defaults = inspect.getargspec(func)
+    params, vararg, keywordarg, defaults = getargspec(func)
     scription_debug('  PARAMS', params, vararg, keywordarg, defaults, verbose=3)
     params = func.params = list(params)
     vararg = func.vararg = [vararg] if vararg else []
     keywordarg = func.keywordarg = [keywordarg] if keywordarg else []
     annotations = func.__scription__
     pos = None
     max_pos = 0
@@ -1415,15 +1433,15 @@
     "parses command-line and compares with either func or, if None, script_module['script_main']"
     global SYS_ARGS
     scription_debug('Run entered')
     if globals().get('HAS_BEEN_RUN'):
         scription_debug('Run already called once, returning')
         return
     globals()['HAS_BEEN_RUN'] = True
-    if py_ver < (3, 0):
+    if PY2:
         SYS_ARGS = [arg.decode(LOCALE_ENCODING) for arg in sys.argv]
     else:
         SYS_ARGS = sys.argv[:]
     Script = script_module['script_main']
     Command = script_module['script_commands']
     try:
         prog_path, prog_name = os.path.split(SYS_ARGS[0])
@@ -1526,14 +1544,16 @@
 def Execute(args, cwd=None, password=None, password_timeout=None, input=None, input_delay=2.5, timeout=None, pty=None, interactive=None, env=None, **new_env_vars):
     scription_debug('creating job:', args)
     job = Job(args, cwd=cwd, pty=pty, env=env, **new_env_vars)
     try:
         scription_debug('communicating')
         job.communicate(timeout=timeout, interactive=interactive, password=password, password_timeout=password_timeout, input=input, input_delay=input_delay)
     except BaseException as exc:
+        if getattr(exc, 'process', None) is None:
+            exc.process = job
         if interactive is None:
             echo(job.stdout)
             echo(job.stderr)
             echo()
         scription_debug(exc)
         raise
     finally:
@@ -1583,14 +1603,16 @@
             # use subprocess
             scription_debug('subprocess args:', args)
             try:
                 self.process = process = Popen(args, stdin=PIPE, stdout=PIPE, stderr=PIPE, cwd=cwd, env=env)
             except OSError as exc:
                 scription_debug('subprocess cwd:', cwd)
                 scription_debug('subprocess env:', env)
+                if exc.errno == 2:
+                    abort('cannot find %r' % (args[0], ))
                 raise
             self.pid = process.pid
             self.child_fd_out = process.stdout
             self.child_fd_in = process.stdin
             self.child_fd_err = process.stderr
             self.poll = self._log_wrap(process.poll, 'polling')
             self.terminate = self._log_wrap(process.terminate, 'terminating')
@@ -1813,15 +1835,23 @@
                         try:
                             # pty -- look for echo off first
                             remaining_timeout = password_timeout
                             while remaining_timeout > 0 and self.get_echo() and self.is_alive():
                                 scription_debug('[echo: %s] waiting for echo off (%s remaining)' % (self.get_echo(), remaining_timeout))
                                 remaining_timeout -= 0.1
                                 time.sleep(0.1)
-                            if self.get_echo():
+                            if not self.is_alive():
+                                # job died
+                                try:
+                                    raise ExecuteError('job died', process=self)
+                                except ExecuteError:
+                                    cls, exc, tb = sys.exc_info()
+                                    self._set_exc(exc, traceback=tb)
+                                    raise exc
+                            elif self.get_echo():
                                 # too long
                                 try:
                                     raise TimeoutError('Password prompt not seen.')
                                 except TimeoutError:
                                     cls, exc, tb = sys.exc_info()
                                     self._set_exc(exc, traceback=tb)
                                     self.kill()
@@ -1888,17 +1918,20 @@
                         self.kill(error='ignore')
                         time.sleep(0.1)
                         self.is_alive()
                 # shutdown stdin thread
                 self._all_input.put(None)
                 # close handles and pipes
                 if self.process is not None:
-                    self.child_fd_in.close()
-                    self.child_fd_out.close()
-                    self.child_fd_err.close()
+                    if not isinstance(self.child_fd_in, int):
+                        self.child_fd_in.close()
+                    if not isinstance(self.child_fd_out, int):
+                        self.child_fd_out.close()
+                    if not isinstance(self.child_fd_err, int):
+                        self.child_fd_err.close()
                 else:
                     for fd in (self.child_fd, self.child_fd_err):
                         try:
                             os.close(fd)
                         except OSError:
                             exc_type, exc, tb = sys.exc_info()
                             if exc_type is OSError and exc.errno == errno.EBADF:
@@ -2222,22 +2255,22 @@
             self._saveable = False
         self._section = section
         self._filename = filename
         defaults = OrderedDict()
         settings = self._settings = OrmSection(name=filename)
         if not os.path.exists(filename):
             open(filename, 'w').close()
-        if py_ver < (3, 0):
+        if PY2:
             fh = open(filename)
         else:
             fh = open(filename, encoding=encoding)
         try:
             section = None
             for line in fh:
-                if py_ver < (3, 0):
+                if PY2:
                     line = line.decode(encoding)
                 line = line.strip()
                 if not line or line.startswith(('#',';')):
                     continue
                 if line[0] == '[':
                     # better be a section header
                     if line[-1] != ']':
@@ -3699,35 +3732,45 @@
 
 _Var_Sentinel = Sentinel("Var")
 class Var(object):
     '''
     := for Python's less than 3.8
     '''
     def __init__(self, func=None):
-        self.data = _Var_Sentinel
-        self.func = func
+        self._data = _Var_Sentinel
+        self._func = func
     #
-    def __call__(self, *args):
-        if not args and self.data is _Var_Sentinel:
-            raise ValueError('nothing saved in var')
-        elif not args:
-            return self.data
-        elif self.func is not None:
+    def __call__(self, *args, **kwds):
+        if not args:
+            if self._data is _Var_Sentinel:
+                raise ValueError('nothing saved in var')
+            else:
+                return self._data
+        # we have args, what shall we do with them?
+        if self._func is not None:
             # run user-supplied function
-            self.data = self.func(*args)
-            return self.data
-        elif len(args) == 0:
-            # reset
-            self.data = _Var_Sentinel
+            self._data = self._func(*args, **kwds)
+            return self._data
+        elif kwds:
+            raise ValueError('keywords not supported unless function is specified')
         elif len(args) == 1:
-            self.data = args[0]
-            return self.data
+            self._data = args[0]
+            return self._data
         else:
-            self.data = args
-            return self.data
+            self._data = args
+            return self._data
+    #
+    def __getattr__(self, name):
+        if self._data is _Var_Sentinel:
+            raise ValueError('nothing saved in var')
+        try:
+            return getattr(self._data, name)
+        except AttributeError:
+            raise AttributeError('%r has no %r' % (self._data, name))
+
 
 
 class user_ids(object):
     """
     maintains root as one of the ids
     """
     def __init__(self, uid, gid):
```

### Comparing `scription-0.86.8/scription/test.py` & `scription-0.86.9/scription/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import sys
 sys.path.insert(0, os.path.split(os.path.split(__file__)[0]))
 
 from antipathy import Path
 from scription import *
 from scription import _usage, version, empty, pocket, ormclassmethod, aenum_version
+from scription import pyver, PY2, PY25, PY33
 from textwrap import dedent
 from unittest import skip, skipUnless, SkipTest, TestCase as unittest_TestCase, main
 import datetime
 import errno
 import functools
 import pty
 import re
@@ -40,28 +41,27 @@
     elif arg.lower() == '-v':
         UNITTEST_VERBOSE = True
 for i in remove[::-1]:
     sys.argv.pop(i)
 del remove
 
 is_win = sys.platform.startswith('win')
-py_ver = sys.version_info[:2]
 gubed = False
 
 class UTC(datetime.tzinfo):
     """UTC"""
     def utcoffset(self, dt):
         return datetime.timedelta(0)
     def tzname(self, dt):
         return "UTC"
     def dst(self, dt):
         return datetime.timedelta(0)
 UTC = UTC()
 
-print('Scription %s.%s.%s, aenum %s.%s.%s -- Python %d.%d' % (version[:3] + aenum_version[:3] + py_ver), verbose=0)
+print('Scription %s.%s.%s, aenum %s.%s.%s -- Python %d.%d' % (version[:3] + aenum_version[:3] + pyver), verbose=0)
 
 def test_func_parsing(obj, func, tests, test_type=False):
     global gubed, script_name, script_main, script_commands, script_command, script_commandname
     try:
         for i, (params, main_args, main_kwds, sub_args, sub_kwds) in enumerate(tests):
             if UNITTEST_VERBOSE:
                 echo(i, end=' ')
@@ -203,14 +203,21 @@
     def test_no_function_multi_arg(self):
         var = Var()
         if var(3+8, 7*7):
             self.assertEqual(var(), (11, 49))
         else:
             self.assertTrue(False, 'var returned %r (should be (11, 49))' % (var(), ))
 
+    def test_data_attributes(self):
+        match = Var(re.match)
+        if match(r"it.*(worked)!", "it   worked!"):
+            self.assertEqual(match.groups(), ('worked', ))
+        else:
+            self.assertTrue(False, 'match returned %r' % match())
+
 
 class TestExports(TestCase):
 
     def test_speckind_exported(self):
         for member in scription.SpecKind:
             self.assertTrue(member.name in globals(), '%s is missing from globals()' % member)
             self.assertIs(globals()[member.name], member)
@@ -1790,15 +1797,15 @@
         self.subp_password_file = password_file_name = os.path.join(tempdir, 'get_subp_pass')
         password_file = open(password_file_name, 'w')
         try:
             password_file.write(
                     "print('super secret santa soda sizzle?')\n"
                     "password = %sinput('make sure no one is watching you type!: ')\n"
                     "print('%%r?  Are you sure??' %% password)"
-                    % ('', 'raw_')[py_ver < (3, 0)]
+                    % ('', 'raw_')[PY2]
                     )
         finally:
             password_file.close()
         #
         self.echo_off_file = echo_off_name = os.path.join(tempdir, 'echo_off')
         echo_off = open(echo_off_name, 'w')
         try:
@@ -1871,15 +1878,15 @@
                     raise
                 self.assertEqual(job.stdout, 'usage message here\n')
             else:
                 self.assertEqual(job.stdout, 'anybody there?\nusage message here\n')
             self.assertTrue(job.returncode)
 
     if is_win:
-        if py_ver >= (3, 3):
+        if pyver >= PY33:
             def test_timeout(self):
                 "test timeout with subprocess alone"
                 command = Execute([sys.executable, '-c', 'import time; time.sleep(30)'], timeout=3, pty=False)
                 self.assertTrue(command.returncode)
         else:
             def test_timeout(self):
                 "no timeout in this version"
@@ -3492,29 +3499,29 @@
             huh = Trivalent(true)
             self.assertEqual(huh == True, True)
             self.assertEqual(huh != True, False)
             self.assertEqual(huh == False, False, "%r is not True" % true)
             self.assertEqual(huh != False, True)
             self.assertEqual(huh == None, False)
             self.assertEqual(huh != None, True)
-            if py_ver >= (2, 5):
+            if pyver >= PY25:
                 self.assertEqual((0, 1, -1)[huh], 1)
         self.assertTrue(bool(true))
 
     def test_false(self):
         "false"
         for false in 'false', 'No', 'F', 'n', -1, False:
             huh = Trivalent(false)
             self.assertEqual(huh != False, False)
             self.assertEqual(huh == False, True)
             self.assertEqual(huh != True, True)
             self.assertEqual(huh == True, False)
             self.assertEqual(huh != None, True)
             self.assertEqual(huh == None, False)
-            if py_ver >= (2, 5):
+            if pyver >= PY25:
                 self.assertEqual((0, 1, -1)[huh], -1)
         self.assertFalse(bool(false))
 
     def test_singletons(self):
         "singletons"
         heh = Trivalent(True)
         hah = Trivalent('Yes')
```

### Comparing `scription-0.86.8/scription.egg-info/PKG-INFO` & `scription-0.86.9/scription.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,106 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: scription
-Version: 0.86.8
+Version: 0.86.9
 Summary: simple script parameter parser
 Home-page: https://github.com/ethanfurman/scription.git
 Author: Ethan Furman
 Author-email: ethan@stoneleaf.us
 License: BSD License
-Description: scription
-        
-        light-weight library to enhance command-line scripts; includes conversion of
-        parameters to specified data types, parameter checking, basic input/output with
-        users, support for suid [1], sending email, executing sub-programs, and having
-        sub-commands within a script
-        
-        
-        decorators
-        
-          - Script:  sets global variables and/or parameters for Commands; the decorated
-            function will be called by Main/Run before any specified Command
-        
-          - Command:  marks function as a subcommand for the script (e.g. add, delete,
-            list, etc.); if no subcommand is specified on the command-line, scription
-            will look for a Command with the same name as the script
-        
-          - Alias:  registers other names for Commands (e.g. delete / remove / kill)
-        
-        
-        functions
-        
-          - Main:  if the importing module's __name__ is __main__, call Run() (this
-            allows for importing the script as a module)
-        
-          - Run:  unconditionally attempts to run the Script function (if any) and the
-            Command found on the command-line
-        
-          Main() or Run() should be the last thing in the script
-        
-        
-        classes
-        
-          - Spec:  can be used when defining the command-line parameters (can also just
-            use tuples)
-        
-        
-        helper functions/classes
-        
-          - abort: quits immediately by raising SystemExit
-        
-          - Execute:  class for executing other programs; uses subprocess.Popen by
-            default, but if `pty=True` is specified then `pty.fork` will be used
-            (handy for programs that only accept input from a pty)
-        
-          - get_response:  function for displaying text and getting feedback
-        
-          - help: quits immediately, but adds a reference to --help in the quit message
-        
-          - log_exception:  logs an exception with logging.logger
-        
-          - mail: rudimentary mail sender
-        
-          - OrmFile:  lightweight orm -- supports str, int, float, date, time,
-            datetime, bool, and path (which defaults to str); custom data types can
-            also be specified
-        
-          - print: wrapper around print that adds a 'verbose_level' keyword (default: 1);
-            default verbosity is 0 (so print does nothing), but can be increased using
-            -v, -vv, --verbose, or --verbose=2 (in Python 2 the script must use
-            'from __future__ import print_function' to use scription's print)
-        
-          - user_ids:  context manager useful for suid scripts -- all actions taken
-            within the context are run as the user/group specified
-        
-        
-        features
-        
-          - extra parameters defined by Script are global, and can be accessed from any
-            function or Command
-        
-          - 'module' is a namespace inserted into the script
-        
-          - 'script_command' is the Command selected from the command line (useful when
-            one needs to call the subcommand directly from a main() function)
-        
-          - 'script_command_name' is the name of the script_command
-        
-          - 'script_verbosity' is the level of verboseness selected (defaults to 0)
-        
-          - 'script_name' is the name of the script
-        
-          - builtin options are:  --help, --verbose (-v or -vv), --version, --all-versions
-            --version attempts to display the version of the main package in use
-            --all-versions attempts to display the versions of any imported packages
-        
-          - command-line is decoded to unicode under Python 2 (Python 3 does this for us)
-        
-        
-        [1] I use the suid-python program, available at http://selliott.org/python/suid-python.c
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
@@ -110,7 +19,101 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+
+scription
+
+light-weight library to enhance command-line scripts; includes conversion of
+parameters to specified data types, parameter checking, basic input/output with
+users, support for suid [1], sending email, executing sub-programs, and having
+sub-commands within a script
+
+
+decorators
+
+  - Script:  sets global variables and/or parameters for Commands; the decorated
+    function will be called by Main/Run before any specified Command
+
+  - Command:  marks function as a subcommand for the script (e.g. add, delete,
+    list, etc.); if no subcommand is specified on the command-line, scription
+    will look for a Command with the same name as the script
+
+  - Alias:  registers other names for Commands (e.g. delete / remove / kill)
+
+
+functions
+
+  - Main:  if the importing module's __name__ is __main__, call Run() (this
+    allows for importing the script as a module)
+
+  - Run:  unconditionally attempts to run the Script function (if any) and the
+    Command found on the command-line
+
+  Main() or Run() should be the last thing in the script
+
+
+classes
+
+  - Spec:  can be used when defining the command-line parameters (can also just
+    use tuples)
+
+
+helper functions/classes
+
+  - abort: quits immediately by raising SystemExit
+
+  - Execute:  class for executing other programs; uses subprocess.Popen by
+    default, but if `pty=True` is specified then `pty.fork` will be used
+    (handy for programs that only accept input from a pty)
+
+  - get_response:  function for displaying text and getting feedback
+
+  - help: quits immediately, but adds a reference to --help in the quit message
+
+  - log_exception:  logs an exception with logging.logger
+
+  - mail: rudimentary mail sender
+
+  - OrmFile:  lightweight orm -- supports str, int, float, date, time,
+    datetime, bool, and path (which defaults to str); custom data types can
+    also be specified
+
+  - print: wrapper around print that adds a 'verbose_level' keyword (default: 1);
+    default verbosity is 0 (so print does nothing), but can be increased using
+    -v, -vv, --verbose, or --verbose=2 (in Python 2 the script must use
+    'from __future__ import print_function' to use scription's print)
+
+  - user_ids:  context manager useful for suid scripts -- all actions taken
+    within the context are run as the user/group specified
+
+
+features
+
+  - extra parameters defined by Script are global, and can be accessed from any
+    function or Command
+
+  - 'module' is a namespace inserted into the script
+
+  - 'script_command' is the Command selected from the command line (useful when
+    one needs to call the subcommand directly from a main() function)
+
+  - 'script_command_name' is the name of the script_command
+
+  - 'script_verbosity' is the level of verboseness selected (defaults to 0)
+
+  - 'script_name' is the name of the script
+
+  - builtin options are:  --help, --verbose (-v or -vv), --version, --all-versions
+    --version attempts to display the version of the main package in use
+    --all-versions attempts to display the versions of any imported packages
+
+  - command-line is decoded to unicode under Python 2 (Python 3 does this for us)
+
+
+[1] I use the suid-python program, available at http://selliott.org/python/suid-python.c
+
+
```

### Comparing `scription-0.86.8/setup.py` & `scription-0.86.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 '''
 py2_only = ()
 py3_only = ()
 make = []
 
 data = dict(
         name='scription',
-        version='0.86.8',
+        version='0.86.9',
         license='BSD License',
         description='simple script parameter parser',
         long_description=description,
         url='https://github.com/ethanfurman/scription.git',
         install_requires=['aenum >= 3.1.0'],
         packages=['scription'],
         package_data={
@@ -126,12 +126,13 @@
              'Programming Language :: Python :: 3.3',
              'Programming Language :: Python :: 3.4',
              'Programming Language :: Python :: 3.5',
              'Programming Language :: Python :: 3.6',
              'Programming Language :: Python :: 3.7',
              'Programming Language :: Python :: 3.8',
              'Programming Language :: Python :: 3.9',
+             'Programming Language :: Python :: 3.10',
              ],
     )
 
 if __name__ == '__main__':
     setup(**data)
```

