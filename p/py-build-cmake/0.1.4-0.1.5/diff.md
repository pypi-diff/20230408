# Comparing `tmp/py-build-cmake-0.1.4.tar.gz` & `tmp/py-build-cmake-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-build-cmake-0.1.4.tar", last modified: Sun Apr  2 11:11:57 2023, max compression
+gzip compressed data, was "py-build-cmake-0.1.5.tar", last modified: Sat Apr  8 20:28:58 2023, max compression
```

## Comparing `py-build-cmake-0.1.4.tar` & `py-build-cmake-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1086 2023-04-02 11:11:27.609241 py-build-cmake-0.1.4/LICENSE
--rw-r--r--   0        0        0     4966 2023-04-02 11:11:27.609241 py-build-cmake-0.1.4/README.md
--rw-r--r--   0        0        0     1446 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      137 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/src/py_build_cmake/__init__.py
--rw-r--r--   0        0        0    27818 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/src/py_build_cmake/build.py
--rw-r--r--   0        0        0     9368 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/src/py_build_cmake/build_component.py
--rw-r--r--   0        0        0    10640 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/src/py_build_cmake/cli.py
--rw-r--r--   0        0        0     8112 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/src/py_build_cmake/cmake.py
--rw-r--r--   0        0        0     2478 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/src/py_build_cmake/cmd_runner.py
--rw-r--r--   0        0        0     9707 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/src/py_build_cmake/config.py
--rw-r--r--   0        0        0    27355 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/src/py_build_cmake/config_options.py
--rw-r--r--   0        0        0      279 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/src/py_build_cmake/datastructures.py
--rw-r--r--   0        0        0     4003 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/src/py_build_cmake/help/__init__.py
--rw-r--r--   0        0        0      180 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/src/py_build_cmake/help/__main__.py
--rw-r--r--   0        0        0        0 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/src/py_build_cmake/py.typed
--rw-r--r--   0        0        0    18128 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/src/py_build_cmake/pyproject_options.py
--rw-r--r--   0        0        0     2612 2023-04-02 11:11:27.640445 py-build-cmake-0.1.4/src/py_build_cmake/tags.py
--rw-r--r--   0        0        0     6004 1970-01-01 00:00:00.000000 py-build-cmake-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-08 20:28:29.189327 py-build-cmake-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4966 2023-04-08 20:28:29.189327 py-build-cmake-0.1.5/README.md
+-rw-r--r--   0        0        0     1446 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      137 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/src/py_build_cmake/__init__.py
+-rw-r--r--   0        0        0    30722 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/src/py_build_cmake/build.py
+-rw-r--r--   0        0        0     9368 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/src/py_build_cmake/build_component.py
+-rw-r--r--   0        0        0    10640 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/src/py_build_cmake/cli.py
+-rw-r--r--   0        0        0     8112 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/src/py_build_cmake/cmake.py
+-rw-r--r--   0        0        0     2459 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/src/py_build_cmake/cmd_runner.py
+-rw-r--r--   0        0        0     9848 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/src/py_build_cmake/config.py
+-rw-r--r--   0        0        0    29249 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/src/py_build_cmake/config_options.py
+-rw-r--r--   0        0        0      279 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/src/py_build_cmake/datastructures.py
+-rw-r--r--   0        0        0     4024 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/src/py_build_cmake/help/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/src/py_build_cmake/help/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/src/py_build_cmake/py.typed
+-rw-r--r--   0        0        0    18990 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/src/py_build_cmake/pyproject_options.py
+-rw-r--r--   0        0        0     2612 2023-04-08 20:28:29.220504 py-build-cmake-0.1.5/src/py_build_cmake/tags.py
+-rw-r--r--   0        0        0     6004 1970-01-01 00:00:00.000000 py-build-cmake-0.1.5/PKG-INFO
```

### Comparing `py-build-cmake-0.1.4/LICENSE` & `py-build-cmake-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.4/README.md` & `py-build-cmake-0.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 keywords = ["some", "keywords"]
 classifiers = ["Topic :: Scientific/Engineering"]
 urls = { "Documentation" = "https://tttapa.github.io/py-build-cmake" }
 dependencies = ["numpy"]
 dynamic = ["version", "description"]
 
 [build-system] # How pip and other frontends should build this project
-requires = ["py-build-cmake~=0.1.4"]
+requires = ["py-build-cmake~=0.1.5"]
 build-backend = "py_build_cmake.build"
 
 [tool.py-build-cmake.module] # Where to find the Python module to package
 directory = "src-python"
 
 [tool.py-build-cmake.sdist] # What to include in source distributions
 include = ["CMakeLists.txt", "src/*"]
```

### Comparing `py-build-cmake-0.1.4/pyproject.toml` & `py-build-cmake-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.4/src/py_build_cmake/build.py` & `py-build-cmake-0.1.5/src/py_build_cmake/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,15 @@
             module_name=cfg.module['name'],
         )
 
         # Copy the module's Python source files to the temporary folder
         if not editable:
             self.copy_pkg_source_to(paths.staging_dir, pkg)
         else:
-            self.write_editable_wrapper(paths.staging_dir, pkg)
+            self.do_editable_install(cfg, paths, pkg)
 
         # Create dist-info folder
         distinfo_dir = f'{pkg_info.package_name}-{pkg_info.version}.dist-info'
         distinfo_dir = paths.staging_dir / distinfo_dir
         os.makedirs(distinfo_dir, exist_ok=True)
 
         # Write metadata
@@ -329,15 +329,16 @@
                            native_cmake_cfg, None, package_info,
                            native_install_dir)
         # Then do the actual build
         self.run_cmake(paths.source_dir, paths.staging_dir, cmake_cfg,
                        cfg.cross, package_info, native_install_dir)
         # Finally, move the files from the native build to the staging area
         if native_install_dir:
-            self.copy_native_install(paths.staging_dir, native_install_dir,
+            self.copy_native_install(paths.staging_dir,
+                                     native_install_dir,
                                      cfg.cross['copy_from_native_build'])
 
     def copy_native_install(self, staging_dir, native_install_dir,
                             native_install_patterns):
         """Copy the files that match the patterns from the native installation
         directory to the wheel staging directory."""
         for pattern in native_install_patterns:
@@ -354,21 +355,25 @@
                     "Native build installed no files that matched the "
                     "pattern '" + pattern + "'")
         shutil.rmtree(native_install_dir)
 
     # --- Files installation --------------------------------------------------
 
     @staticmethod
-    def copy_pkg_source_to(staging_dir: Path, pkg: flit_core.common.Module):
+    def copy_pkg_source_to(staging_dir: Path, pkg: flit_core.common.Module,
+                           symlink: bool = False):
         """Copy the files of a Python package to the build directory."""
         for mod_file in pkg.iter_files():
             rel_path = os.path.relpath(mod_file, pkg.path.parent)
             dst = staging_dir / rel_path
             os.makedirs(dst.parent, exist_ok=True)
-            shutil.copy2(mod_file, dst, follow_symlinks=False)
+            if symlink:
+                dst.symlink_to(mod_file, target_is_directory=False)
+            else:
+                shutil.copy2(mod_file, dst, follow_symlinks=False)
 
     @staticmethod
     def write_license_files(license, srcdir: Path, distinfo_dir: Path):
         """Write the LICENSE file from pyproject.toml to the distinfo
         directory."""
         if 'text' in license:
             with (distinfo_dir / 'LICENSE').open('w', encoding='utf-8') as f:
@@ -382,14 +387,26 @@
                                                                       str]]):
         from flit_core.common import write_entry_points
         with (distinfo / 'entry_points.txt').open('w', encoding='utf-8') as f:
             write_entry_points(entrypoints, f)
 
     # --- Editable installs ---------------------------------------------------
 
+    def do_editable_install(self, cfg, paths: BuildPaths,
+                            pkg: flit_core.common.Module):
+        mode = cfg.editable["mode"]
+        if mode == "wrapper":
+            self.write_editable_wrapper(paths.staging_dir, pkg)
+        elif mode == "hook":
+            self.write_editable_hook(paths.staging_dir, pkg),
+        elif mode == "symlink":
+            self.write_editable_links(paths.staging_dir, pkg)
+        else:
+            assert False, "Invalid editable mode"
+
     def write_editable_wrapper(self, staging_dir: Path,
                                pkg: flit_core.common.Module):
         """Write a fake __init__.py file that points to the development 
         folder."""
         tmp_pkg: Path = staging_dir / pkg.name
         pkgpath = Path(pkg.path)
         initpath = pkgpath / '__init__.py'
@@ -420,14 +437,57 @@
         # the C++ extensions
         py_typed: Path = pkg.path / 'py.typed'
         if py_typed.exists():
             shutil.copy2(py_typed, tmp_pkg)
         # Write a path file so IDEs find the correct files as well
         (staging_dir / f'{pkg.name}.pth').write_text(str(pkg.path.parent))
 
+    def write_editable_hook(self, staging_dir: Path,
+                            pkg: flit_core.common.Module):
+        # Write a hook that finds the installed compiled extension modules
+        pkg_hook: Path = staging_dir / (pkg.name + '_editable_hook')
+        os.makedirs(pkg_hook, exist_ok=True)
+        content = f"""\
+            import sys, inspect, os
+            from importlib.machinery import PathFinder
+
+            class EditablePathFinder(PathFinder):
+                def __init__(self, name, extra_path):
+                    self.name = name
+                    self.extra_path = extra_path
+                def find_spec(self, name, path=None, target=None):
+                    if name.split('.', 1)[0] != self.name:
+                        return None
+                    path = (path or []) + [self.extra_path]
+                    return super().find_spec(name, path, target)
+
+            def install(name: str):
+                source_path = os.path.abspath(inspect.getsourcefile(EditablePathFinder))
+                source_dir = os.path.dirname(source_path)
+                installed_path = os.path.join(source_dir, '..', name)
+                sys.meta_path.insert(0, EditablePathFinder(name, installed_path))
+
+            install('{pkg.name}')
+            """
+        (pkg_hook / '__init__.py').write_text(textwrap.dedent(content),
+                                              encoding='utf-8')
+        # Write a path file to find the development files
+        content = f"""\
+            {str(pkg.path.parent)}
+            import {pkg.name}_editable_hook"""
+        (staging_dir / f'{pkg.name}.pth').write_text(
+            textwrap.dedent(content))
+        
+    def write_editable_links(self, staging_dir: Path,
+                             pkg: flit_core.common.Module):
+        self.copy_pkg_source_to(staging_dir, pkg, symlink=True)
+        pth_file = staging_dir / f'{pkg.name}.pth'
+        pth_file.parent.mkdir(exist_ok=True)
+        pth_file.write_text(str(staging_dir))
+
     # --- Invoking CMake builds -----------------------------------------------
 
     def run_cmake(self, pkgdir, install_dir, cmake_cfg, cross_cfg,
                   package_info, native_install_dir):
         """Configure, build and install using CMake."""
 
         cmaker = self.get_cmaker(pkgdir,
@@ -528,27 +588,31 @@
             "Linux": "linux",
             "Windows": "windows",
             "Darwin": "mac",
         }[platform.system()]
 
     @staticmethod
     def print_config_verbose(cfg):
-        print("\npy-build-cmake options")
-        print("======================")
+        from . import __version__
+        print("\npy-build-cmake (" + __version__ + ")")
+        print("options")
+        print("================================")
         print("module:")
         pprint(cfg.module)
+        print("editable:")
+        pprint(cfg.editable)
         print("sdist:")
         pprint(cfg.sdist)
         print("cmake:")
         pprint(cfg.cmake)
         print("stubgen:")
         pprint(cfg.stubgen)
         print("cross:")
         pprint(cfg.cross)
-        print("======================\n")
+        print("================================\n")
 
     @staticmethod
     def normalize_version(version):
         from distlib.version import NormalizedVersion
         norm_version = str(NormalizedVersion(version))
         return norm_version
```

### Comparing `py-build-cmake-0.1.4/src/py_build_cmake/build_component.py` & `py-build-cmake-0.1.5/src/py_build_cmake/build_component.py`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.4/src/py_build_cmake/cli.py` & `py-build-cmake-0.1.5/src/py_build_cmake/cli.py`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.4/src/py_build_cmake/cmake.py` & `py-build-cmake-0.1.5/src/py_build_cmake/cmake.py`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.4/src/py_build_cmake/cmd_runner.py` & `py-build-cmake-0.1.5/src/py_build_cmake/cmd_runner.py`

 * *Files 23% similar despite different names*

```diff
@@ -51,16 +51,16 @@
                 # Check if the version is new enough
                 if minimum_version is not None:
                     if program_version < minimum_version:
                         raise RuntimeError(f"{name} too old")
         except CalledProcessError as e:
             if self.verbose:
                 print(f'{type(e).__module__}.{type(e).__name__}', e, sep=': ')
-                sys.stdout.buffer.write(e.stdout)
-                sys.stdout.buffer.write(e.stderr)
+                print(e.stdout)
+                print(e.stderr, file=sys.stderr)
             return False
         except Exception as e:
             # If any of that failed, return False
             if self.verbose:
                 print(f'{type(e).__module__}.{type(e).__name__}', e, sep=': ')
             return False
         return True
```

### Comparing `py-build-cmake-0.1.4/src/py_build_cmake/config.py` & `py-build-cmake-0.1.5/src/py_build_cmake/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 class Config:
     dynamic_metadata: Set[str] = field(default_factory=set)
     entrypoints: Dict[str, Dict[str, str]] = field(default_factory=dict)
     metadata: Dict[str, Any] = field(default_factory=dict)
     referenced_files: List[str] = field(default_factory=list)
     package_name: str = field(default='')
     module: Dict[str, str] = field(default_factory=dict)
+    editable: Dict[str, Any] = field(default_factory=dict)
     sdist: Dict[str, Dict[str, Any]] = field(default_factory=dict)
     license: Dict[str, str] = field(default_factory=dict)
     cmake: Optional[Dict[str, Any]] = field(default=None)
     stubgen: Optional[Dict[str, Any]] = field(default=None)
     cross: Optional[Dict[str, Any]] = field(default=None)
 
 
@@ -138,14 +139,18 @@
             print(f"Name changed from {tool_cfg[s]['name']} to {normname}")
             # TODO: use logging instead of print
         tool_cfg[s]['name'] = normname
         cfg.module = tool_cfg[s]
     else:
         assert False, "Missing [tools.py-build-cmake.module] section"
 
+    s = 'editable'
+    if s in tool_cfg:
+        cfg.editable = tool_cfg[s]
+
     # Store the sdist folders (this is based on flit)
     def get_sdist_cludes(cfg):
         return {
             cl + '_patterns': _check_glob_patterns(cfg['sdist'][cl], cl)
             for cl in ('include', 'exclude')
         }
```

### Comparing `py-build-cmake-0.1.4/src/py_build_cmake/config_options.py` & `py-build-cmake-0.1.5/src/py_build_cmake/config_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     return path[-1]
 
 
 class ConfigNode:
 
     def __init__(self,
                  value: ConfValue = None,
-                 sub: Dict[str, 'ConfigNode'] = None) -> None:
+                 sub: Optional[Dict[str, 'ConfigNode']] = None) -> None:
         self.value: ConfValue = value
         self.sub: Optional[Dict[str, 'ConfigNode']] = sub
 
     @classmethod
     def from_dict(cls, d: dict):
         node = cls()
         node.sub = {}
@@ -219,15 +219,15 @@
         self.description = description
         self.example = example
         self.sub: Dict[str, 'ConfigOption'] = {}
         self.default: DefaultValue = default
         self.inherit_from: Optional[ConfPath] = inherit_from
         self.create_if_inheritance_target_exists = create_if_inheritance_target_exists
 
-    def get_typename(self):
+    def get_typename(self, md: bool = False):
         return None
 
     def insert(self, opt: 'ConfigOption'):
         assert opt.name not in self.sub
         self.sub[opt.name] = opt
         return self.sub[opt.name]
 
@@ -468,15 +468,15 @@
 class UncheckedConfigOption(ConfigOption):
 
     allow_unknown_keys = True
 
 
 class StrConfigOption(ConfigOption):
 
-    def get_typename(self):
+    def get_typename(self, md: bool = False):
         return 'string'
 
     def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
                           selfpth: ConfPath, overridecfg: ConfigNode,
                           overridepath: ConfPath):
         assert not self.sub
         assert not selfcfg.sub
@@ -488,17 +488,56 @@
         if cfg[cfgpath].sub:
             raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
                               f'{str}, not {dict}')
         elif not isinstance(cfg[cfgpath].value, str):
             raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
                               f'{str}, not {type(cfg[cfgpath].value)}')
 
+class EnumConfigOption(ConfigOption):
+
+    def __init__(self,
+                 name: str,
+                 description: str = '',
+                 example: str = '',
+                 default: DefaultValue = NoDefaultValue(),
+                 inherit_from: Optional[ConfPath] = None,
+                 create_if_inheritance_target_exists: bool = False,
+                 options: List[str] = []) -> None:
+        super().__init__(name, description, example, default, inherit_from, create_if_inheritance_target_exists)
+        self.options = options
+
+    def get_typename(self, md: bool = False):
+        if md:
+            return "`'" + "'` \| `'".join(self.options) + "'`"
+        else:
+            return "'" + "' | '".join(self.options) + "'"
+
+    def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
+                          selfpth: ConfPath, overridecfg: ConfigNode,
+                          overridepath: ConfPath):
+        assert not self.sub
+        assert not selfcfg.sub
+        assert not overridecfg.sub
+        selfcfg.value = deepcopy(overridecfg.value)
+
+    def verify(self, rootopts: 'ConfigOption', cfg: ConfigNode,
+               cfgpath: ConfPath):
+        if cfg[cfgpath].sub:
+            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
+                              f'{str}, not {dict}')
+        elif not isinstance(cfg[cfgpath].value, str):
+            raise ConfigError(f'Type of {pth2str(cfgpath)} should be '
+                              f'{str}, not {type(cfg[cfgpath].value)}')
+        if cfg[cfgpath].value not in self.options:
+            raise ConfigError(f'Value of {pth2str(cfgpath)} should be '
+                              'one of \'' + "', '".join(self.options) + '\'')
+
 class BoolConfigOption(ConfigOption):
 
-    def get_typename(self):
+    def get_typename(self, md: bool = False):
         return 'bool'
 
     def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
                           selfpth: ConfPath, overridecfg: ConfigNode,
                           overridepath: ConfPath):
         assert not self.sub
         assert not selfcfg.sub
@@ -545,15 +584,15 @@
         self.expected_contents = expected_contents
         self.base_path = base_path
         self.allow_abs = allow_abs
         self.is_folder = is_folder
         if self.base_path:
             assert os.path.isabs(self.base_path.project_path)
 
-    def get_typename(self):
+    def get_typename(self, md: bool = False):
         return 'path' if self.is_folder else 'filepath'
 
     def check_path(self, cfg: ConfigNode, cfgpath):
         osp = os.path
         path = osp.normpath(cfg[cfgpath].value)
         # Absolute or relative path?
         if osp.isabs(path):
@@ -611,15 +650,15 @@
                  inherit_from: Optional[ConfPath] = None,
                  create_if_inheritance_target_exists: bool = False,
                  convert_str_to_singleton=False) -> None:
         super().__init__(name, description, example, default, inherit_from,
                          create_if_inheritance_target_exists)
         self.convert_str_to_singleton = convert_str_to_singleton
 
-    def get_typename(self):
+    def get_typename(self, md: bool = False):
         return 'list'
 
     def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
                           selfpth: ConfPath, overridecfg: ConfigNode,
                           overridepath: ConfPath):
         assert not self.sub
         assert not selfcfg.sub
@@ -646,15 +685,15 @@
         elif not all(isinstance(el, str) for el in cfg[cfgpath].value):
             raise ConfigError(f'Type of elements in {pth2str(cfgpath)} should '
                               f'be {str}')
 
 
 class DictOfStrConfigOption(ConfigOption):
 
-    def get_typename(self):
+    def get_typename(self, md: bool = False):
         return 'dict'
 
     def explicit_override(self, opts: 'ConfigOption', selfcfg: ConfigNode,
                           selfpth: ConfPath, overridecfg: ConfigNode,
                           overridepath: ConfPath):
         assert not self.sub
         assert not selfcfg.value
```

### Comparing `py-build-cmake-0.1.4/src/py_build_cmake/help/__init__.py` & `py-build-cmake-0.1.5/src/py_build_cmake/help/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     """
     for k, v in pbc_opts.sub.items():
         print('##', k)
         print(_get_full_description(v), '\n')
         print('| Option | Description | Type | Default |')
         print('|--------|-------------|------|---------|')
         for kk, vv in v.sub.items() or {}:
+            typename = vv.get_typename(md=True) or ''
             print('|', f'`{kk}`', '|', _get_full_description(vv), '|',
-                  vv.get_typename() or '', '|', f'`{get_default_str(vv)}`',
-                  '|')
+                  typename, '|', f'`{get_default_str(vv)}`', '|')
         print()
 
 def _get_full_description(vv: ConfigOption):
     descr = _md_escape(vv.description)
     if isinstance(vv, PathConfigOption):
         descr += '<br/>' + _describe_path_option(vv).capitalize() + '.'
     if vv.inherit_from:
```

### Comparing `py-build-cmake-0.1.4/src/py_build_cmake/pyproject_options.py` & `py-build-cmake-0.1.5/src/py_build_cmake/pyproject_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,33 @@
         PathConfigOption('directory',
                          "Directory containing the Python package.",
                          default=DefaultValueValue("."),
                          base_path=RelativeToProject(project_path),
                          must_exist=not test),
     ])
 
+    # [tool.py-build-cmake.editable]
+    editable = pbc.insert(
+        ConfigOption(
+            "editable",
+            "Defines how to perform an editable install (PEP 660).",
+            default=DefaultValueValue({}),
+        ))
+    editable.insert_multiple([
+        EnumConfigOption('mode',
+                         "Mechanism to use for editable installations. "
+                         "Either write a wrapper __init__.py file, install an "
+                         "import hook, or install symlinks to the original "
+                         "files. See https://tttapa.github.io/py-build-cmake"
+                         "/Editable-install.html for more "
+                         "information.",
+                         default=DefaultValueValue("wrapper"),
+                         options=["wrapper", "hook", "symlink"]),
+    ])
+
     # [tool.py-build-cmake.sdist]
     sdist = pbc.insert(
         ConfigOption(
             "sdist",
             "Specifies the files that should be included in the source "
             "distribution for this package.",
             default=DefaultValueValue({}),
```

### Comparing `py-build-cmake-0.1.4/src/py_build_cmake/tags.py` & `py-build-cmake-0.1.5/src/py_build_cmake/tags.py`

 * *Files identical despite different names*

### Comparing `py-build-cmake-0.1.4/PKG-INFO` & `py-build-cmake-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-build-cmake
-Version: 0.1.4
+Version: 0.1.5
 Summary: Modern, PEP 517 compliant build backend for creating Python packages with
 Keywords: pep517,cmake
 Author-email: Pieter P <pieter.p.dev@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -85,15 +85,15 @@
 keywords = ["some", "keywords"]
 classifiers = ["Topic :: Scientific/Engineering"]
 urls = { "Documentation" = "https://tttapa.github.io/py-build-cmake" }
 dependencies = ["numpy"]
 dynamic = ["version", "description"]
 
 [build-system] # How pip and other frontends should build this project
-requires = ["py-build-cmake~=0.1.4"]
+requires = ["py-build-cmake~=0.1.5"]
 build-backend = "py_build_cmake.build"
 
 [tool.py-build-cmake.module] # Where to find the Python module to package
 directory = "src-python"
 
 [tool.py-build-cmake.sdist] # What to include in source distributions
 include = ["CMakeLists.txt", "src/*"]
```

