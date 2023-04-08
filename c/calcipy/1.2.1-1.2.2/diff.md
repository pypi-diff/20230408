# Comparing `tmp/calcipy-1.2.1.tar.gz` & `tmp/calcipy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcipy-1.2.1.tar", max compression
+gzip compressed data, was "calcipy-1.2.2.tar", max compression
```

## Comparing `calcipy-1.2.1.tar` & `calcipy-1.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1066 2023-04-06 13:01:00.709942 calcipy-1.2.1/LICENSE
--rw-r--r--   0        0        0      167 2023-04-07 23:08:26.432610 calcipy-1.2.1/calcipy/__init__.py
--rw-r--r--   0        0        0     1259 2023-02-23 02:19:12.612069 calcipy-1.2.1/calcipy/can_skip.py
--rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.2.1/calcipy/check_for_stale_packages/__init__.py
--rw-r--r--   0        0        0     8214 2023-03-02 02:41:41.090176 calcipy-1.2.1/calcipy/check_for_stale_packages/_check_for_stale_packages.py
--rw-r--r--   0        0        0     5641 2023-04-01 13:12:52.506798 calcipy-1.2.1/calcipy/cli.py
--rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.2.1/calcipy/code_tag_collector/__init__.py
--rw-r--r--   0        0        0     9790 2023-02-26 00:17:08.509359 calcipy-1.2.1/calcipy/code_tag_collector/_collector.py
--rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.2.1/calcipy/dot_dict/__init__.py
--rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.2.1/calcipy/dot_dict/_dot_dict.py
--rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.2.1/calcipy/experiments/__init__.py
--rw-r--r--   0        0        0     1915 2023-04-06 23:41:07.217109 calcipy-1.2.1/calcipy/experiments/check_duplicate_test_names.py
--rw-r--r--   0        0        0     3271 2023-02-23 02:19:12.613926 calcipy-1.2.1/calcipy/file_search.py
--rw-r--r--   0        0        0     1814 2023-04-07 21:04:03.754244 calcipy-1.2.1/calcipy/invoke_helpers.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.2.1/calcipy/md_writer/__init__.py
--rw-r--r--   0        0        0     7815 2023-02-23 02:19:12.614596 calcipy-1.2.1/calcipy/md_writer/_writer.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.2.1/calcipy/noxfile/__init__.py
--rw-r--r--   0        0        0     6513 2023-02-23 13:23:19.364723 calcipy-1.2.1/calcipy/noxfile/_noxfile.py
--rw-r--r--   0        0        0     1193 2023-03-02 02:45:23.652620 calcipy-1.2.1/calcipy/scripts.py
--rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.2.1/calcipy/tasks/__init__.py
--rw-r--r--   0        0        0     3104 2023-04-05 22:06:13.047283 calcipy-1.2.1/calcipy/tasks/all_tasks.py
--rw-r--r--   0        0        0     1876 2023-04-06 12:55:27.782578 calcipy-1.2.1/calcipy/tasks/cl.py
--rw-r--r--   0        0        0     1132 2023-02-23 02:54:45.453854 calcipy-1.2.1/calcipy/tasks/defaults.py
--rw-r--r--   0        0        0     3589 2023-04-06 12:54:31.902116 calcipy-1.2.1/calcipy/tasks/doc.py
--rw-r--r--   0        0        0     3869 2023-04-07 23:08:02.132045 calcipy-1.2.1/calcipy/tasks/lint.py
--rw-r--r--   0        0        0      454 2023-02-23 02:19:12.617085 calcipy-1.2.1/calcipy/tasks/nox.py
--rw-r--r--   0        0        0     1275 2023-02-23 02:19:12.617365 calcipy-1.2.1/calcipy/tasks/pack.py
--rw-r--r--   0        0        0      557 2023-02-23 02:19:12.617596 calcipy-1.2.1/calcipy/tasks/stale.py
--rw-r--r--   0        0        0     1498 2023-02-23 02:19:12.617900 calcipy-1.2.1/calcipy/tasks/tags.py
--rw-r--r--   0        0        0     3510 2023-04-06 23:41:29.742135 calcipy-1.2.1/calcipy/tasks/test.py
--rw-r--r--   0        0        0      634 2023-02-23 02:19:12.618406 calcipy-1.2.1/calcipy/tasks/types.py
--rw-r--r--   0        0        0     6651 2023-04-07 23:08:33.866805 calcipy-1.2.1/docs/README.md
--rw-r--r--   0        0        0     6455 2023-04-07 23:08:26.471212 calcipy-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     9950 1970-01-01 00:00:00.000000 calcipy-1.2.1/setup.py
--rw-r--r--   0        0        0    11358 1970-01-01 00:00:00.000000 calcipy-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-06 13:01:00.709942 calcipy-1.2.2/LICENSE
+-rw-r--r--   0        0        0      167 2023-04-08 17:25:10.138550 calcipy-1.2.2/calcipy/__init__.py
+-rw-r--r--   0        0        0     1259 2023-02-23 02:19:12.612069 calcipy-1.2.2/calcipy/can_skip.py
+-rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.2.2/calcipy/check_for_stale_packages/__init__.py
+-rw-r--r--   0        0        0     8214 2023-03-02 02:41:41.090176 calcipy-1.2.2/calcipy/check_for_stale_packages/_check_for_stale_packages.py
+-rw-r--r--   0        0        0     6261 2023-04-08 00:38:00.312188 calcipy-1.2.2/calcipy/cli.py
+-rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.2.2/calcipy/code_tag_collector/__init__.py
+-rw-r--r--   0        0        0     9790 2023-02-26 00:17:08.509359 calcipy-1.2.2/calcipy/code_tag_collector/_collector.py
+-rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.2.2/calcipy/dot_dict/__init__.py
+-rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.2.2/calcipy/dot_dict/_dot_dict.py
+-rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.2.2/calcipy/experiments/__init__.py
+-rw-r--r--   0        0        0     1915 2023-04-06 23:41:07.217109 calcipy-1.2.2/calcipy/experiments/check_duplicate_test_names.py
+-rw-r--r--   0        0        0     3271 2023-02-23 02:19:12.613926 calcipy-1.2.2/calcipy/file_search.py
+-rw-r--r--   0        0        0     1814 2023-04-07 21:04:03.754244 calcipy-1.2.2/calcipy/invoke_helpers.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.2.2/calcipy/md_writer/__init__.py
+-rw-r--r--   0        0        0     7815 2023-02-23 02:19:12.614596 calcipy-1.2.2/calcipy/md_writer/_writer.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.2.2/calcipy/noxfile/__init__.py
+-rw-r--r--   0        0        0     6513 2023-02-23 13:23:19.364723 calcipy-1.2.2/calcipy/noxfile/_noxfile.py
+-rw-r--r--   0        0        0     1193 2023-03-02 02:45:23.652620 calcipy-1.2.2/calcipy/scripts.py
+-rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.2.2/calcipy/tasks/__init__.py
+-rw-r--r--   0        0        0     3104 2023-04-05 22:06:13.047283 calcipy-1.2.2/calcipy/tasks/all_tasks.py
+-rw-r--r--   0        0        0     1876 2023-04-06 12:55:27.782578 calcipy-1.2.2/calcipy/tasks/cl.py
+-rw-r--r--   0        0        0     1132 2023-02-23 02:54:45.453854 calcipy-1.2.2/calcipy/tasks/defaults.py
+-rw-r--r--   0        0        0     3589 2023-04-06 12:54:31.902116 calcipy-1.2.2/calcipy/tasks/doc.py
+-rw-r--r--   0        0        0     3869 2023-04-07 23:08:02.132045 calcipy-1.2.2/calcipy/tasks/lint.py
+-rw-r--r--   0        0        0      454 2023-02-23 02:19:12.617085 calcipy-1.2.2/calcipy/tasks/nox.py
+-rw-r--r--   0        0        0     1275 2023-02-23 02:19:12.617365 calcipy-1.2.2/calcipy/tasks/pack.py
+-rw-r--r--   0        0        0      557 2023-02-23 02:19:12.617596 calcipy-1.2.2/calcipy/tasks/stale.py
+-rw-r--r--   0        0        0     1498 2023-02-23 02:19:12.617900 calcipy-1.2.2/calcipy/tasks/tags.py
+-rw-r--r--   0        0        0     3510 2023-04-06 23:41:29.742135 calcipy-1.2.2/calcipy/tasks/test.py
+-rw-r--r--   0        0        0      634 2023-02-23 02:19:12.618406 calcipy-1.2.2/calcipy/tasks/types.py
+-rw-r--r--   0        0        0     6651 2023-04-08 17:25:19.332845 calcipy-1.2.2/docs/README.md
+-rw-r--r--   0        0        0     6455 2023-04-08 17:25:10.180844 calcipy-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     9950 1970-01-01 00:00:00.000000 calcipy-1.2.2/setup.py
+-rw-r--r--   0        0        0    11358 1970-01-01 00:00:00.000000 calcipy-1.2.2/PKG-INFO
```

### Comparing `calcipy-1.2.1/LICENSE` & `calcipy-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/can_skip.py` & `calcipy-1.2.2/calcipy/can_skip.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/check_for_stale_packages/_check_for_stale_packages.py` & `calcipy-1.2.2/calcipy/check_for_stale_packages/_check_for_stale_packages.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/cli.py` & `calcipy-1.2.2/calcipy/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 
     file_args: List[Path] = Field(default_factory=list)
     """List of Paths to modify."""
 
     verbose: PositiveInt = Field(default=0, lte=3)
     """Verbosity level."""
 
+    keep_going: bool = False
+    """Continue task execution regardless of failure."""
+
 
 class _CalcipyProgram(Program):  # type: ignore[misc]
     """Customized version of Invoke's `Program`."""
 
     def print_help(self) -> None:
         """Extend print_help with calcipy-specific global configuration.
 
@@ -84,16 +87,20 @@
     # Manipulate 'sys.argv' to hide arguments that invoke can't parse
     _gto = GlobalTaskOptions()
     sys_argv: List[str] = sys.argv[:1]
     last_argv = ''
     for argv in sys.argv[1:]:
         if not last_argv.startswith('-') and Path(argv).is_file():
             _gto.file_args.append(Path(argv))
+        # Check for CLI flags
         elif argv in {'-v', '-vv', '-vvv', '--verbose'}:
             _gto.verbose = argv.count('v')
+        elif argv == '--keep-going':
+            _gto.keep_going = True
+        # Check for CLI arguments with values
         elif last_argv in {'--working-dir'}:
             _gto.working_dir = Path(argv).resolve()
         elif argv not in {'--working-dir'}:
             sys_argv.append(argv)
         last_argv = argv
     _gto.file_args = [
         _f if _f.is_absolute() else Path.cwd() / _f
@@ -110,14 +117,24 @@
         version=pkg_version,
         namespace=Collection.from_module(module) if module else collection,
         config_class=_CalcipyConfig,
     ).run()
 
 
 @beartype
+def _configure_logger(ctx: Context) -> None:
+    """Configure the logger based on task context."""
+    verbose = ctx.config.gto.verbose
+    log_lookup = {3: logging.NOTSET, 2: logging.DEBUG, 1: logging.INFO, 0: logging.WARNING}
+    raw_log_level = log_lookup.get(verbose)
+    log_level = logging.ERROR if raw_log_level is None else raw_log_level
+    configure_logger(log_level=log_level)
+
+
+@beartype
 def _run_task(func: Any, ctx: Context, *args: Any, show_task_info: bool, **kwargs: Any) -> Any:
     """Run the task function with optional logging."""
     if show_task_info:
         summary = func.__doc__.split('\n')[0]
         logger.text(f'Running {func.__name__}', is_header=True, summary=summary)
         logger.text_debug('With task arguments', args=args, kwargs=kwargs)
 
@@ -127,38 +144,39 @@
         logger.text('')
         logger.text_debug(f'Completed {func.__name__}', result=result)
 
     return result
 
 
 @beartype
-def _configure_logger(ctx: Context) -> None:
-    """Configure the logger based on task context."""
-    verbose = ctx.config.gto.verbose
-    log_lookup = {3: logging.NOTSET, 2: logging.DEBUG, 1: logging.INFO, 0: logging.WARNING}
-    raw_log_level = log_lookup.get(verbose)
-    log_level = logging.ERROR if raw_log_level is None else raw_log_level
-    configure_logger(log_level=log_level)
+def _inner_runner(*, func: Any, ctx: Context, show_task_info: bool, args: Any, kwargs: Any) -> Any:
+    try:
+        ctx.config.gto  # noqa: B018
+    except AttributeError:
+        ctx.config.gto = GlobalTaskOptions()
+
+    # Begin utilizing Global Task Options
+    os.chdir(ctx.config.gto.working_dir)
+    _configure_logger(ctx)
+
+    try:
+        return _run_task(func, ctx, *args, show_task_info=show_task_info, **kwargs)
+    except Exception:
+        if not ctx.config.gto.keep_going:
+            raise
+        logger.exception('Task Failed', func=str(func), args=args, kwargs=kwargs)
 
 
 @beartype
 def task(*task_args: Any, show_task_info: bool = True, **task_kwargs: Any) -> Callable[[Any], Task]:
     """Wrapper to accept arguments for an invoke task."""
     @beartype
     def wrapper(func: Any) -> Task:  # noqa: ANN001
         """Wraps the decorated task."""
         @invoke_task(*task_args, **task_kwargs)  # type: ignore[misc]
         @beartype
         @wraps(func)
         def inner(ctx: Context, *args: Any, **kwargs: Any) -> Task:
             """Wrap the task with settings configured in `gto` for working_dir and logging."""
-            try:
-                ctx.config.gto  # noqa: B018
-            except AttributeError:
-                ctx.config.gto = GlobalTaskOptions()
-
-            os.chdir(ctx.config.gto.working_dir)
-            _configure_logger(ctx)
-
-            return _run_task(func, ctx, *args, show_task_info=show_task_info, **kwargs)
+            return _inner_runner(func=func, ctx=ctx, show_task_info=show_task_info, args=args, kwargs=kwargs)
         return inner
     return wrapper
```

### Comparing `calcipy-1.2.1/calcipy/code_tag_collector/_collector.py` & `calcipy-1.2.2/calcipy/code_tag_collector/_collector.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/dot_dict/_dot_dict.py` & `calcipy-1.2.2/calcipy/dot_dict/_dot_dict.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/experiments/check_duplicate_test_names.py` & `calcipy-1.2.2/calcipy/experiments/check_duplicate_test_names.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/file_search.py` & `calcipy-1.2.2/calcipy/file_search.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/invoke_helpers.py` & `calcipy-1.2.2/calcipy/invoke_helpers.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/md_writer/_writer.py` & `calcipy-1.2.2/calcipy/md_writer/_writer.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/noxfile/_noxfile.py` & `calcipy-1.2.2/calcipy/noxfile/_noxfile.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/scripts.py` & `calcipy-1.2.2/calcipy/scripts.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/tasks/all_tasks.py` & `calcipy-1.2.2/calcipy/tasks/all_tasks.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/tasks/cl.py` & `calcipy-1.2.2/calcipy/tasks/cl.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/tasks/defaults.py` & `calcipy-1.2.2/calcipy/tasks/defaults.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/tasks/doc.py` & `calcipy-1.2.2/calcipy/tasks/doc.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/tasks/lint.py` & `calcipy-1.2.2/calcipy/tasks/lint.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/tasks/pack.py` & `calcipy-1.2.2/calcipy/tasks/pack.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/tasks/stale.py` & `calcipy-1.2.2/calcipy/tasks/stale.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/tasks/tags.py` & `calcipy-1.2.2/calcipy/tasks/tags.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/tasks/test.py` & `calcipy-1.2.2/calcipy/tasks/test.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/calcipy/tasks/types.py` & `calcipy-1.2.2/calcipy/tasks/types.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/docs/README.md` & `calcipy-1.2.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.1/pyproject.toml` & `calcipy-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.2.1"
+version = "1.2.2"
 version_files = ["calcipy/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
@@ -26,25 +26,25 @@
 include = ["LICENSE"]
 keywords = ["nox", "python-poetry"]
 license = "MIT"
 maintainers = []
 name = "calcipy"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/calcipy"
-version = "1.2.1"
+version = "1.2.2"
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
 arrow = {optional = true, version = ">=1.2.3"} # tags
 autopep8 = {optional = true, version = ">=2.0.1"} # flake8
 bandit = {optional = true, version = ">=1.7.4"} # lint
 beartype = ">=0.12.0"
 bidict = {optional = true, version = ">=0.22.1"} # stale
 commitizen = {optional = true, version = ">=2.42.0"} # doc
-corallium = ">=0.1.0"
+corallium = ">=0.1.1"
 dlint = {optional = true, version = ">=0.14.0"} # flake8
 flake8 = {optional = true, version = ">=6.0.0"} # flake8
 flake8-adjustable-complexity = {optional = true, version = ">=0.0.6"} # flake8
 flake8-annotations-complexity = {optional = true, version = ">=0.0.7"} # flake8
 flake8-executable = {optional = true, version = ">=2.1.3"} # flake8
 flake8-expression-complexity = {optional = true, version = ">=0.0.11"} # flake8
 flake8-functions = {optional = true, version = ">=0.0.7"} # flake8
```

### Comparing `calcipy-1.2.1/setup.py` & `calcipy-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
  'calcipy.noxfile',
  'calcipy.tasks']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['beartype>=0.12.0', 'corallium>=0.1.0', 'invoke>=2.0.0', 'pydantic>=1.10.5']
+['beartype>=0.12.0', 'corallium>=0.1.1', 'invoke>=2.0.0', 'pydantic>=1.10.5']
 
 extras_require = \
 {'ddict': ['python-box>=6.0.2'],
  'doc': ['commitizen>=2.42.0',
          'mkdocs>=1.4.1',
          'mkdocs-build-plantuml-plugin>=1.7.4',
          'mkdocs-gen-files>=0.4.0',
@@ -74,15 +74,15 @@
 {'console_scripts': ['calcipy = calcipy.scripts:start',
                      'calcipy_lint = calcipy.scripts:start_lint',
                      'calcipy_tags = calcipy.scripts:start_tags',
                      'calcipy_types = calcipy.scripts:start_types']}
 
 setup_kwargs = {
     'name': 'calcipy',
-    'version': '1.2.1',
+    'version': '1.2.2',
     'description': 'Python package to simplify development',
     'long_description': '# calcipy\n\n![./calcipy-banner-wide.svg](https://raw.githubusercontent.com/KyleKing/calcipy/main/docs/calcipy-banner-wide.svg)\n\n`calcipy` is a Python package that implements best practices such as code style (linting, auto-fixes), documentation, CI/CD, and logging. Like the calcium carbonate in hard coral, packages can be built on the `calcipy` foundation.\n\n`calcipy` has some configurability, but is tailored for my particular use cases. If you want the same sort of functionality, there are a number of alternatives to consider:\n\n- [pyscaffold](https://github.com/pyscaffold/pyscaffold) is a much more mature project that aims for the same goals, but with a slightly different approach and tech stack (tox vs. nox, cookiecutter vs. copier, etc.)\n- [tidypy](https://github.com/jayclassless/tidypy#features), [pylama](https://github.com/klen/pylama), and [codecheck](https://pypi.org/project/codecheck/) offer similar functionality of bundling and running static checkers, but makes far fewer assumptions\n- [pytoil](https://github.com/FollowTheProcess/pytoil) is a general CLI tool for developer automation\n- And many more such as [pyta](https://github.com/pyta-uoft/pyta), [prospector](https://github.com/PyCQA/prospector), [wemake-python-styleguide](https://github.com/wemake-services/wemake-python-styleguide) / [cjolowicz/cookiecutter-hypermodern-python](https://github.com/cjolowicz/cookiecutter-hypermodern-python), [formate](https://github.com/python-formate/formate), [johnthagen/python-blueprint](https://github.com/johnthagen/python-blueprint), [oxsecurity/megalinter](https://github.com/oxsecurity/megalinter), etc.\n\n## Installation\n\nCalcipy needs a few static files managed using copier and a template project: [kyleking/calcipy_template](https://github.com/KyleKing/calcipy_template/)\n\nYou can quickly use the template to create a new project or add calcipy to an existing one:\n\n```sh\n# Install copier. pipx is recommended\npipx install copier\n\n# To create a new project\ncopier copy gh:KyleKing/calcipy_template new_project\ncd new_project\n\n# Or convert/update an existing one\ncd my_project\ncopier copy gh:KyleKing/calcipy_template .\ncopier update\n```\n\nSee [./Advanced_Configuration.md](./Advanced_Configuration.md) for documentation on the configurable aspects of `calcipy`\n\n### Calcipy CLI\n\nAdditionally, `calcipy` can be run as a CLI application without adding the package as a dependency.\n\nQuick Start:\n\n```sh\npipx install calcipy\n\n# Use \'tags\' to create a CODE_TAG_SUMMARY of the specified directory\ncalcipy tags --help\ncalcipy tags --base-dir=~/path/to/my_project\n\n# See additional documentation from the CLI help\n> calcipy\n\nSubcommands:\n\nmain                                     Main task pipeline.\nother                                    Run tasks that are otherwise not exercised in main.\nrelease                                  Release pipeline.\ncl.bump                                  Bumps project version based on commits & settings in pyproject.toml.\ncl.write                                 Write a Changelog file with the raw Git history.\ndoc.build                                Build documentation with mkdocs.\ndoc.deploy                               Deploy docs to the Github `gh-pages` branch.\ndoc.watch                                Serve local documentation for local editing.\nlint.autopep8                            Run autopep8.\nlint.check (lint)                        Run ruff as check-only.\nlint.fix                                 Run ruff and apply fixes.\nlint.flake8                              Run ruff and apply fixes.\nlint.pre-commit                          Run pre-commit.\nlint.pylint                              Run ruff and apply fixes.\nlint.security                            Attempt to identify possible security vulnerabilities.\nlint.watch                               Run ruff as check-only.\nnox.noxfile (nox)                        Run nox from the local noxfile.\npack.check-licenses                      Check licenses for compatibility with `licensecheck`.\npack.lock                                Ensure poetry.lock is  up-to-date.\npack.publish                             Build the distributed format(s) and publish.\nstale.check-for-stale-packages (stale)   Identify stale dependencies.\ntags.collect-code-tags (tags)            Create a `CODE_TAG_SUMMARY.md` with a table for TODO- and FIXME-style code comments.\ntest.coverage                            Generate useful coverage outputs after running pytest.\ntest.pytest (test)                       Run pytest with default arguments.\ntest.step                                Run pytest optimized to stop on first error.\ntest.watch                               Run pytest with polling and optimized to stop on first error.\ntypes.mypy                               Run mypy.\ntypes.pyright                            Run pyright.\n\nGlobal Task Options:\n\nworking_dir   Set the cwd for the program. Example: "../run --working-dir .. lint test"\n*file_args    List of Paths available globally to all tasks. Will resolve paths with working_dir\nverbose       Globally configure logger verbosity (-vvv for most verbose)\n```\n\n### Calcipy Pre-Commit\n\n`calcipy` can also be used as a `pre-commit` task by adding the below snippet to your `pre-commit` file:\n\n```yaml\nrepos:\n  - repo: https://github.com/KyleKing/calcipy\n    rev: main\n    hooks:\n      - id: tags\n      - id: lint-fix\n      - id: types\n```\n\n## Project Status\n\nSee the `Open Issues` and/or the [CODE_TAG_SUMMARY]. For release history, see the [CHANGELOG].\n\n## Contributing\n\nWe welcome pull requests! For your pull request to be accepted smoothly, we suggest that you first open a GitHub issue to discuss your idea. For resources on getting started with the code base, see the below documentation:\n\n- [DEVELOPER_GUIDE]\n- [STYLE_GUIDE]\n\n## Code of Conduct\n\nWe follow the [Contributor Covenant Code of Conduct][contributor-covenant].\n\n### Open Source Status\n\nWe try to reasonably meet most aspects of the "OpenSSF scorecard" from [Open Source Insights](https://deps.dev/pypi/calcipy)\n\n## Responsible Disclosure\n\nIf you have any security issue to report, please contact the project maintainers privately. You can reach us at [dev.act.kyle@gmail.com](mailto:dev.act.kyle@gmail.com).\n\n## License\n\n[LICENSE]\n\n[changelog]: https://calcipy.kyleking.me/docs/CHANGELOG\n[code_tag_summary]: https://calcipy.kyleking.me/docs/CODE_TAG_SUMMARY\n[contributor-covenant]: https://www.contributor-covenant.org\n[developer_guide]: https://calcipy.kyleking.me/docs/DEVELOPER_GUIDE\n[license]: https://github.com/kyleking/calcipy/blob/main/LICENSE\n[style_guide]: https://calcipy.kyleking.me/docs/STYLE_GUIDE\n',
     'author': 'Kyle King',
     'author_email': 'dev.act.kyle@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyleking/calcipy',
```

### Comparing `calcipy-1.2.1/PKG-INFO` & `calcipy-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcipy
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python package to simplify development
 Home-page: https://github.com/kyleking/calcipy
 License: MIT
 Keywords: nox,python-poetry
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.8.12,<4.0.0
@@ -35,15 +35,15 @@
 Provides-Extra: types
 Requires-Dist: arrow (>=1.2.3) ; extra == "stale" or extra == "tags"
 Requires-Dist: autopep8 (>=2.0.1) ; extra == "lint"
 Requires-Dist: bandit (>=1.7.4) ; extra == "lint"
 Requires-Dist: beartype (>=0.12.0)
 Requires-Dist: bidict (>=0.22.1) ; extra == "stale"
 Requires-Dist: commitizen (>=2.42.0) ; extra == "doc"
-Requires-Dist: corallium (>=0.1.0)
+Requires-Dist: corallium (>=0.1.1)
 Requires-Dist: dlint (>=0.14.0) ; extra == "flake8"
 Requires-Dist: flake8 (>=6.0.0) ; extra == "flake8"
 Requires-Dist: flake8-adjustable-complexity (>=0.0.6) ; extra == "flake8"
 Requires-Dist: flake8-annotations-complexity (>=0.0.7) ; extra == "flake8"
 Requires-Dist: flake8-executable (>=2.1.3) ; extra == "flake8"
 Requires-Dist: flake8-expression-complexity (>=0.0.11) ; extra == "flake8"
 Requires-Dist: flake8-functions (>=0.0.7) ; extra == "flake8"
```

