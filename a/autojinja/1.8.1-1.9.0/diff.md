# Comparing `tmp/autojinja-1.8.1.tar.gz` & `tmp/autojinja-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autojinja-1.8.1.tar", last modified: Mon Jan  2 19:33:30 2023, max compression
+gzip compressed data, was "autojinja-1.9.0.tar", last modified: Mon Mar 20 22:29:30 2023, max compression
```

## Comparing `autojinja-1.8.1.tar` & `autojinja-1.9.0.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-01-02 19:33:30.900188 autojinja-1.8.1/
--rw-rw-rw-   0        0        0     1542 2021-08-12 18:18:54.000000 autojinja-1.8.1/LICENSE
--rw-rw-rw-   0        0        0     7414 2023-01-02 19:33:30.899185 autojinja-1.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     5328 2022-11-22 20:52:46.000000 autojinja-1.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-02 19:33:30.866187 autojinja-1.8.1/autojinja/
--rw-rw-rw-   0        0        0      355 2023-01-02 19:33:06.000000 autojinja-1.8.1/autojinja/__init__.py
--rw-rw-rw-   0        0        0      275 2022-12-30 00:13:55.000000 autojinja-1.8.1/autojinja/__main__.py
--rw-rw-rw-   0        0        0     2576 2023-01-01 22:54:31.000000 autojinja-1.8.1/autojinja/defaults.py
--rw-rw-rw-   0        0        0    18939 2023-01-02 18:23:05.000000 autojinja-1.8.1/autojinja/exceptions.py
--rw-rw-rw-   0        0        0    13956 2023-01-01 20:08:28.000000 autojinja-1.8.1/autojinja/main.py
--rw-rw-rw-   0        0        0    17963 2022-12-29 23:15:27.000000 autojinja-1.8.1/autojinja/parser.py
--rw-rw-rw-   0        0        0    10813 2022-12-30 12:23:00.000000 autojinja-1.8.1/autojinja/path.py
--rw-rw-rw-   0        0        0    21071 2023-01-02 17:35:30.000000 autojinja-1.8.1/autojinja/templates.py
--rw-rw-rw-   0        0        0     7929 2023-01-02 17:26:27.000000 autojinja-1.8.1/autojinja/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-02 19:33:30.898185 autojinja-1.8.1/autojinja.egg-info/
--rw-rw-rw-   0        0        0     7414 2023-01-02 19:33:30.000000 autojinja-1.8.1/autojinja.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-01-02 19:33:30.000000 autojinja-1.8.1/autojinja.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-02 19:33:30.000000 autojinja-1.8.1/autojinja.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-01-02 19:33:30.000000 autojinja-1.8.1/autojinja.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-01-02 19:33:30.000000 autojinja-1.8.1/autojinja.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-02 19:33:30.000000 autojinja-1.8.1/autojinja.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-02 19:33:30.901183 autojinja-1.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1338 2023-01-02 19:33:05.000000 autojinja-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-20 22:29:30.084915 autojinja-1.9.0/
+-rw-rw-rw-   0        0        0     1542 2021-08-12 18:18:54.000000 autojinja-1.9.0/LICENSE
+-rw-rw-rw-   0        0        0     6264 2023-03-20 22:29:30.083917 autojinja-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5328 2022-11-22 20:52:46.000000 autojinja-1.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-03-20 22:29:30.059913 autojinja-1.9.0/autojinja/
+-rw-rw-rw-   0        0        0      994 2023-03-20 22:27:34.000000 autojinja-1.9.0/autojinja/__init__.py
+-rw-rw-rw-   0        0        0      250 2023-01-19 14:19:59.000000 autojinja-1.9.0/autojinja/__main__.py
+-rw-rw-rw-   0        0        0     2715 2023-03-20 16:20:26.000000 autojinja-1.9.0/autojinja/defaults.py
+-rw-rw-rw-   0        0        0    20252 2023-03-20 22:12:33.000000 autojinja-1.9.0/autojinja/exceptions.py
+-rw-rw-rw-   0        0        0    14240 2023-03-20 22:18:10.000000 autojinja-1.9.0/autojinja/main.py
+-rw-rw-rw-   0        0        0    18935 2023-03-20 22:18:22.000000 autojinja-1.9.0/autojinja/parser.py
+-rw-rw-rw-   0        0        0    14784 2023-03-20 22:18:32.000000 autojinja-1.9.0/autojinja/path.py
+-rw-rw-rw-   0        0        0    25221 2023-03-20 22:20:28.000000 autojinja-1.9.0/autojinja/templates.py
+-rw-rw-rw-   0        0        0     8785 2023-03-20 22:18:45.000000 autojinja-1.9.0/autojinja/utils.py
+drwxrwxrwx   0        0        0        0 2023-03-20 22:29:30.072915 autojinja-1.9.0/autojinja.egg-info/
+-rw-rw-rw-   0        0        0     6264 2023-03-20 22:29:29.000000 autojinja-1.9.0/autojinja.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2023-03-20 22:29:29.000000 autojinja-1.9.0/autojinja.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-20 22:29:29.000000 autojinja-1.9.0/autojinja.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-03-20 22:29:29.000000 autojinja-1.9.0/autojinja.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-03-20 22:29:29.000000 autojinja-1.9.0/autojinja.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-03-20 22:29:29.000000 autojinja-1.9.0/autojinja.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-20 22:29:30.084915 autojinja-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1338 2023-03-20 22:27:34.000000 autojinja-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-20 22:29:30.082917 autojinja-1.9.0/tests/
+-rw-rw-rw-   0        0        0    68357 2023-03-20 18:54:06.000000 autojinja-1.9.0/tests/test_exceptions.py
+-rw-rw-rw-   0        0        0    21083 2023-03-20 22:27:34.000000 autojinja-1.9.0/tests/test_main.py
+-rw-rw-rw-   0        0        0    48209 2023-03-20 18:52:13.000000 autojinja-1.9.0/tests/test_parser.py
+-rw-rw-rw-   0        0        0    73767 2023-03-20 22:05:26.000000 autojinja-1.9.0/tests/test_path.py
+-rw-rw-rw-   0        0        0    69060 2023-03-20 22:15:37.000000 autojinja-1.9.0/tests/test_templates.py
+-rw-rw-rw-   0        0        0    26819 2023-03-20 18:55:12.000000 autojinja-1.9.0/tests/test_utils.py
```

### Comparing `autojinja-1.8.1/LICENSE` & `autojinja-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autojinja-1.8.1/PKG-INFO` & `autojinja-1.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,168 +1,169 @@
 Metadata-Version: 2.1
 Name: autojinja
-Version: 1.8.1
+Version: 1.9.0
 Summary: Content generation with Jinja templates in between comments
 Home-page: https://github.com/ldflo/autojinja
 Author: Florian Popek
 Author-email: florian.popek@gmail.com
 License: BSD
-Description: # autojinja
-        
-        **autojinja** is a Python3 module that allows generating code inside any file using [Jinja templates](https://github.com/pallets/jinja) in between comments. It aims to assist development workflows by using simple Python3 scripts that perform content generation of neighboring files, which enables generating code next to traditionally hand-made code efficiently.
-        
-        It includes :
-        - Content generation in any file that accepts comments
-        - Ability to maintain hand-made code inside generated code
-        - Simple integration in build pipelines and existing codebases
-        
-        **autojinja** can be seen as a _preprocessor_ for most file formats, and works great with any codebase as it automates writing code manually. It shines out even more when working with metadata files (such as XML or JSON files) that centralize information which later needs to be generated across various scattered files in the codebase.
-        
-        ## Installation
-        
-        ```shell
-        $ pip install autojinja
-        ```
-        
-        ## Usage
-        
-        ```shell
-        $ autojinja script1.py script2.py
-        ```
-        ```shell
-        $ autojinja -a .
-        ```
-        
-        ## Content generation
-        
-        Content generation consists in generating parts of an existing file thanks to dedicated sections that delimit where the generation takes place. This technique is made possible for all files accepting comments, and allows defining [Jinja templates](https://github.com/pallets/jinja) directly in such files without breaking them.
-        
-        For example, let's suppose we have a C++ file we want to generate inside. To do this, we need to write our Jinja template between `[[[` and `]]]` markers, followed by an `[[[end]]]` marker :
-        
-        ```cpp
-        // main.cpp
-        #include <iostream>
-        
-        int main() {
-          std::cout << "Hello world !" << std::endl;
-          // [[[ std::cout << "{{ value }}" << std::endl; ]]]  // Jinja template
-          // [[[ end ]]]                                       // Code will be generated in between
-          return 0;
-        }
-        ```
-        
-        The template can then be generated with a Python3 script that provides the `value` variable :
-        
-        ```python
-        # main.py
-        from autojinja import CogTemplate
-        
-        template = CogTemplate.from_file("main.cpp")
-        template.context(value = "Python here !").render_file()
-        ```
-        
-        Calling the script will modify our C++ file as such :
-        
-        ```cpp
-        // main.cpp
-        #include <iostream>
-        
-        int main() {
-          std::cout << "Hello world !" << std::endl;
-          // [[[ std::cout << "{{ value }}" << std::endl; ]]]  // Jinja template
-          std::cout << "Python here !" << std::endl;
-          // [[[ end ]]]                                       // Code will be generated in between
-          return 0;
-        }
-        ```
-        
-        This technique is greatly inspired by [Cog](https://github.com/nedbat/cog), but adapted to work with Jinja templating engine. When performing generation again, the content inside the markers is entirely replaced by the new generation.
-        
-        ## Hand-made modifications
-        
-        Modification by hand of generated code is made possible by using special sections that are preserved across new generations. To do this, we need to name a section between `<<[` and `]>>` markers, followed by an `<<[end]>>` marker :
-        
-        ```cpp
-        // main.cpp
-        #include <iostream>
-        
-        // [[[
-        // int main() {
-        //
-        //   std::cout << "{{ value }}" << std::endl;
-        //   // <<[ impl ]>>  // Manually editable section named 'impl'
-        //   return 0;
-        //   // <<[ end ]>>   // End of section
-        //
-        // }
-        // ]]]
-        int main() {
-        
-          std::cout << "Python here !" << std::endl;
-          // <<[ impl ]>>  // Manually editable section named 'impl'
-          std::cout << "Modified by hand" << std::endl;
-          return 1;
-          // <<[ end ]>>   // End of section
-        
-        }
-        // [[[ end ]]]
-        ```
-        
-        When a new generation occurs, all previous sections are retrieved from the destination file and then reinserted into the new generation, inside each corresponding section with same name.
-        
-        All previous sections of a destination file must be reinserted when performing a new generation, otherwise it will be considered as code loss and generation will be aborted. Human intervention is required to deal with such scenarios.
-        
-        ## Integration in build pipelines
-        
-        **autojinja** generation mechanism can be integrated as a build step by listing all Python3 scripts that perform generation :
-        
-        ```shell
-        $ autojinja script1.py dir/script2.py ...
-        ```
-        
-        **autojinja** also provides discover mechanisms to find and execute the concerned Python3 scripts in listed directories :
-        
-        - `-r -f` recursively executes all Python3 scripts named `__jinja__.py`
-        
-            ```shell
-            $ autojinja -r -f .
-            ```
-        
-        - `-r -t` recursively executes all Python3 scripts whose first line contains `autojinja` keyword (can be for instance `import autojinja` or `from autojinja import *`)
-        
-            ```shell
-            $ autojinja -r -t .
-            ```
-        
-        - `-a` equivalent to `-r -f -t`
-        
-            ```shell
-            $ autojinja -a .
-            ```
-        
-        Centralized metadata files (such as XML or JSON files) can easily be accessed inside Python3 scripts using environment variables and environment files :
-        
-        ```shell
-        $ autojinja -a . -e FILE1=/tmp/file1.xml -e file.env
-        ```
-        
-        ## Links
-        - [Documentation](https://github.com/ldflo/autojinja/blob/main/docs/doc_autojinja.md)
-        - [Examples](https://github.com/ldflo/autojinja/blob/main/examples)
-        - [PyPI](https://pypi.org/project/autojinja)
-        - [Jinja2](https://github.com/pallets/jinja)
-        - [Cog](https://github.com/nedbat/cog)
-        
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Code Generators
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# autojinja
+
+**autojinja** is a Python3 module that allows generating code inside any file using [Jinja templates](https://github.com/pallets/jinja) in between comments. It aims to assist development workflows by using simple Python3 scripts that perform content generation of neighboring files, which enables generating code next to traditionally hand-made code efficiently.
+
+It includes :
+- Content generation in any file that accepts comments
+- Ability to maintain hand-made code inside generated code
+- Simple integration in build pipelines and existing codebases
+
+**autojinja** can be seen as a _preprocessor_ for most file formats, and works great with any codebase as it automates writing code manually. It shines out even more when working with metadata files (such as XML or JSON files) that centralize information which later needs to be generated across various scattered files in the codebase.
+
+## Installation
+
+```shell
+$ pip install autojinja
+```
+
+## Usage
+
+```shell
+$ autojinja script1.py script2.py
+```
+```shell
+$ autojinja -a .
+```
+
+## Content generation
+
+Content generation consists in generating parts of an existing file thanks to dedicated sections that delimit where the generation takes place. This technique is made possible for all files accepting comments, and allows defining [Jinja templates](https://github.com/pallets/jinja) directly in such files without breaking them.
+
+For example, let's suppose we have a C++ file we want to generate inside. To do this, we need to write our Jinja template between `[[[` and `]]]` markers, followed by an `[[[end]]]` marker :
+
+```cpp
+// main.cpp
+#include <iostream>
+
+int main() {
+  std::cout << "Hello world !" << std::endl;
+  // [[[ std::cout << "{{ value }}" << std::endl; ]]]  // Jinja template
+  // [[[ end ]]]                                       // Code will be generated in between
+  return 0;
+}
+```
+
+The template can then be generated with a Python3 script that provides the `value` variable :
+
+```python
+# main.py
+from autojinja import CogTemplate
+
+template = CogTemplate.from_file("main.cpp")
+template.context(value = "Python here !").render_file()
+```
+
+Calling the script will modify our C++ file as such :
+
+```cpp
+// main.cpp
+#include <iostream>
+
+int main() {
+  std::cout << "Hello world !" << std::endl;
+  // [[[ std::cout << "{{ value }}" << std::endl; ]]]  // Jinja template
+  std::cout << "Python here !" << std::endl;
+  // [[[ end ]]]                                       // Code will be generated in between
+  return 0;
+}
+```
+
+This technique is greatly inspired by [Cog](https://github.com/nedbat/cog), but adapted to work with Jinja templating engine. When performing generation again, the content inside the markers is entirely replaced by the new generation.
+
+## Hand-made modifications
+
+Modification by hand of generated code is made possible by using special sections that are preserved across new generations. To do this, we need to name a section between `<<[` and `]>>` markers, followed by an `<<[end]>>` marker :
+
+```cpp
+// main.cpp
+#include <iostream>
+
+// [[[
+// int main() {
+//
+//   std::cout << "{{ value }}" << std::endl;
+//   // <<[ impl ]>>  // Manually editable section named 'impl'
+//   return 0;
+//   // <<[ end ]>>   // End of section
+//
+// }
+// ]]]
+int main() {
+
+  std::cout << "Python here !" << std::endl;
+  // <<[ impl ]>>  // Manually editable section named 'impl'
+  std::cout << "Modified by hand" << std::endl;
+  return 1;
+  // <<[ end ]>>   // End of section
+
+}
+// [[[ end ]]]
+```
+
+When a new generation occurs, all previous sections are retrieved from the destination file and then reinserted into the new generation, inside each corresponding section with same name.
+
+All previous sections of a destination file must be reinserted when performing a new generation, otherwise it will be considered as code loss and generation will be aborted. Human intervention is required to deal with such scenarios.
+
+## Integration in build pipelines
+
+**autojinja** generation mechanism can be integrated as a build step by listing all Python3 scripts that perform generation :
+
+```shell
+$ autojinja script1.py dir/script2.py ...
+```
+
+**autojinja** also provides discover mechanisms to find and execute the concerned Python3 scripts in listed directories :
+
+- `-r -f` recursively executes all Python3 scripts named `__jinja__.py`
+
+    ```shell
+    $ autojinja -r -f .
+    ```
+
+- `-r -t` recursively executes all Python3 scripts whose first line contains `autojinja` keyword (can be for instance `import autojinja` or `from autojinja import *`)
+
+    ```shell
+    $ autojinja -r -t .
+    ```
+
+- `-a` equivalent to `-r -f -t`
+
+    ```shell
+    $ autojinja -a .
+    ```
+
+Centralized metadata files (such as XML or JSON files) can easily be accessed inside Python3 scripts using environment variables and environment files :
+
+```shell
+$ autojinja -a . -e FILE1=/tmp/file1.xml -e file.env
+```
+
+## Links
+- [Documentation](https://github.com/ldflo/autojinja/blob/main/docs/doc_autojinja.md)
+- [Examples](https://github.com/ldflo/autojinja/blob/main/examples)
+- [PyPI](https://pypi.org/project/autojinja)
+- [Jinja2](https://github.com/pallets/jinja)
+- [Cog](https://github.com/nedbat/cog)
```

### Comparing `autojinja-1.8.1/README.md` & `autojinja-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `autojinja-1.8.1/autojinja/defaults.py` & `autojinja-1.9.0/autojinja/defaults.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from typing import Optional
 
 AUTOJINJA_DEFAULT_FILENAME   = "__jinja__.py"
 AUTOJINJA_DEFAULT_TAG        = "autojinja"
 AUTOJINJA_DEFAULT_COG_OPEN   = "[[["
 AUTOJINJA_DEFAULT_COG_CLOSE  = "]]]"
 AUTOJINJA_DEFAULT_COG_END    = "end"
 AUTOJINJA_DEFAULT_EDIT_OPEN  = "<<["
@@ -11,57 +12,57 @@
 
 AUTOJINJA_DEBUG          = "AUTOJINJA_DEBUG"
 AUTOJINJA_REMOVE_MARKERS = "AUTOJINJA_REMOVE_MARKERS"
 AUTOJINJA_SILENT         = "AUTOJINJA_SILENT"
 AUTOJINJA_SUMMARY        = "AUTOJINJA_SUMMARY"
 AUTOJINJA_THIS_DIRPATH   = "THIS_DIRPATH"
 
-def osenviron_debug(env = None):
+def osenviron_debug(env: os._Environ = None) -> int:
     env = env or os.environ
     if AUTOJINJA_DEBUG not in env:
         return 0
     value = env[AUTOJINJA_DEBUG]
     is_valid = True
     if len(value) != 1:
         is_valid = False
     elif value != "0" and value != "1":
         is_valid = False
     if not is_valid:
         raise Exception(f"Expected 0 or 1 for environment variable '{AUTOJINJA_DEBUG}'")
     return 1 if value == "1" else 0
 
-def osenviron_remove_markers(env = None):
+def osenviron_remove_markers(env: os._Environ = None) -> int:
     env = env or os.environ
     if AUTOJINJA_REMOVE_MARKERS not in env:
         return 0
     value = env[AUTOJINJA_REMOVE_MARKERS]
     is_valid = True
     if len(value) != 1:
         is_valid = False
     elif value != "0" and value != "1":
         is_valid = False
     if not is_valid:
         raise Exception(f"Expected 0 or 1 for environment variable '{AUTOJINJA_REMOVE_MARKERS}'")
     return 1 if value == "1" else 0
 
-def osenviron_silent(env = None):
+def osenviron_silent(env: os._Environ = None) -> int:
     env = env or os.environ
     if AUTOJINJA_SILENT not in env:
         return 0
     value = env[AUTOJINJA_SILENT]
     is_valid = True
     if len(value) != 1:
         is_valid = False
     elif value != "0" and value != "1":
         is_valid = False
     if not is_valid:
         raise Exception(f"Expected 0 or 1 for environment variable '{AUTOJINJA_SILENT}'")
     return 1 if value == "1" else 0
 
-def osenviron_summary(env = None):
+def osenviron_summary(env: os._Environ = None) -> str:
     env = env or os.environ
     if AUTOJINJA_SUMMARY not in env:
         return "1"
     value = env[AUTOJINJA_SUMMARY]
     is_valid = True
     if len(value) != 1 and len(value) != 3:
         is_valid = False
@@ -70,10 +71,10 @@
             if c != "0" and c != "1":
                 is_valid = False
                 break
     if not is_valid:
         raise Exception(f"Expected 0, 1 or flags for environment variable '{AUTOJINJA_SUMMARY}'")
     return value
 
-def osenviron_this_dirpath(env = None):
+def osenviron_this_dirpath(env: os._Environ = None) -> Optional[str]:
     env = env or os.environ
     return env.get(AUTOJINJA_THIS_DIRPATH)
```

### Comparing `autojinja-1.8.1/autojinja/exceptions.py` & `autojinja-1.9.0/autojinja/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,248 +1,253 @@
+from . import parser
+
 import io
 import os
+from typing import Callable, Generic, Tuple, Type, TypeVar
 import traceback
 
-def wrap_callable(callable):
+def wrap_callable(callable: Callable):
     """ Wraps the given callable in order to bypass AttributeError
         handling of Jinja and provide better exception stacktraces.
     """
     def autojinja_wrapped_fcall(*args, **kwargs):
         try:
             result = callable(*args, **kwargs)
             return wrap_object_attributes(result)
         except AttributeError as e:
             message = clean_wrapped_stacktrace(e)
             raise DebugAttributeError(message) from None
-        except BaseException as e:
+        except Exception as e:
             message = clean_wrapped_stacktrace(e)
             raise wrap_exception(e, message).with_traceback(None)
     return autojinja_wrapped_fcall
 
+_TException = TypeVar("_TException", bound=Exception)
+
 ### Base exception
 
-class CommonException(Exception):
+class CommonException(Exception, Generic[_TException]):
     @staticmethod
-    def from_marker(exceptionType, marker, pos, size, message):
+    def from_marker(exceptionType: Type[_TException], marker: parser.Marker, pos: int, size: int, message: str) -> _TException:
         line = line_at_index(marker.string, pos)
         (l, c) = index_to_coordinates(marker.string, pos)
         message = f"{message}\n{line}\n{' ' * (c-1)}{'^' * size} line {l}, column {c}"
         exception = exceptionType(message)
         exception.coordinates = (l, c)
         return exception
     @staticmethod
-    def from_exception(exception, marker):
+    def from_exception(exception: _TException, marker: parser.Marker) -> _TException:
         exception = prepend_jinja2_traceback(exception)
         text = format_text(marker.header)
         (l, c) = index_to_coordinates(marker.string, marker.header_open)
         stack = f"\n  During {'reinsertion' if marker.is_edit else 'generation'} of \"{marker.open} {text} {marker.close}\" at line {l}, column {c}"
         message = str(exception).lstrip('\n')
         message = f"{stack}\n{message}"
         exception = wrap_exception(exception, message)
         exception.coordinates = (l, c)
         return exception
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 ### Parsing exception
 
 class ParsingException(CommonException):
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 class OpenMarkerNotFoundException(ParsingException):
     @staticmethod
-    def from_marker(marker):
+    def from_marker(marker: parser.Marker) -> "OpenMarkerNotFoundException":
         return CommonException.from_marker(OpenMarkerNotFoundException,
                                            marker,
                                            marker.header_open,
                                            len(marker.open),
                                            f"Couldn't find corresponding open marker \"{marker.open} {marker.close}\":")
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 class CloseMarkerNotFoundException(ParsingException):
     @staticmethod
-    def from_marker(marker):
+    def from_marker(marker: parser.Marker) -> "CloseMarkerNotFoundException":
         return CommonException.from_marker(CloseMarkerNotFoundException,
                                            marker,
                                            marker.header_open,
                                            len(marker.open),
                                            f"Couldn't find corresponding close marker \"{marker.close}\":")
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 class EndMarkerNotFoundException(ParsingException):
     @staticmethod
-    def from_marker(marker):
+    def from_marker(marker: parser.Marker) -> "EndMarkerNotFoundException":
         return CommonException.from_marker(EndMarkerNotFoundException,
                                            marker,
                                            marker.header_close - len(marker.close),
                                            len(marker.close),
                                            f"Couldn't find corresponding end marker \"{marker.open} {marker.end} {marker.close}\":")
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 class RequireHeaderInlineException(ParsingException):
     @staticmethod
-    def from_marker(marker):
+    def from_marker(marker: parser.Marker) -> "RequireHeaderInlineException":
         return CommonException.from_marker(RequireHeaderInlineException,
                                            marker,
                                            marker.header_open,
                                            len(marker.open),
                                            f"Marker can't have a multiline header:")
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 class RequireHeaderMultilineException(ParsingException):
     @staticmethod
-    def from_marker(marker):
+    def from_marker(marker: parser.Marker) -> "RequireHeaderMultilineException":
         return CommonException.from_marker(RequireHeaderMultilineException,
                                            marker,
                                            marker.header_open,
                                            len(marker.open),
                                            f"Marker can't have a one line header:")
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 class WrongHeaderIndentationException(ParsingException):
     @staticmethod
-    def from_marker(marker, pos):
+    def from_marker(marker: parser.Marker, pos) -> "WrongHeaderIndentationException":
         return CommonException.from_marker(WrongHeaderIndentationException,
                                            marker,
                                            pos,
                                            len(marker.open),
                                            f"Wrong marker header indentation:")
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 class RequireNewlineException(ParsingException):
     @staticmethod
-    def from_marker(marker):
+    def from_marker(marker: parser.Marker) -> "RequireNewlineException":
         return CommonException.from_marker(RequireNewlineException,
                                            marker,
                                            marker.header_open,
                                            len(marker.open),
                                            f"Marker can't start on same line as previous end marker:")
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 class RequireInlineException(ParsingException):
     @staticmethod
-    def from_marker(marker):
+    def from_marker(marker: parser.Marker) -> "RequireInlineException":
         return CommonException.from_marker(RequireInlineException,
                                            marker,
                                            marker.header_open,
                                            len(marker.open),
                                            f"Marker must start on same line as previous marker:")
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 class WrongInclusionException(ParsingException):
     @staticmethod
-    def from_marker(marker):
+    def from_marker(marker: parser.Marker) -> "WrongInclusionException":
         return CommonException.from_marker(WrongInclusionException,
                                            marker,
                                            marker.header_open,
                                            len(marker.open),
                                            f"Marker has wrong inclusion regarding enclosing markers:")
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 class DuplicateEditException(ParsingException):
     @staticmethod
-    def from_marker(marker):
+    def from_marker(marker: parser.Marker) -> "DuplicateEditException":
         return CommonException.from_marker(DuplicateEditException,
                                            marker,
                                            marker.header_open,
                                            len(marker.open),
                                            f"Duplicate edit marker \"{marker.open} {marker.header} {marker.close}\", consider reusing/removing duplicates:")
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 class DirectlyEnclosedEditException(ParsingException):
     @staticmethod
-    def from_marker(marker):
+    def from_marker(marker: parser.Marker) -> "DirectlyEnclosedEditException":
         return CommonException.from_marker(DirectlyEnclosedEditException,
                                            marker,
                                            marker.header_open,
                                            len(marker.open),
                                            f"Directly enclosed edit marker \"{marker.open} {marker.header} {marker.close}\", consider reusing/removing it:")
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 ### Generation exception
 
 class GenerationException(CommonException):
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 class RequireBodyInlineException(GenerationException):
     @staticmethod
-    def from_marker(marker):
+    def from_marker(marker: parser.Marker) -> "RequireBodyInlineException":
         return CommonException.from_marker(RequireBodyInlineException,
                                            marker,
                                            marker.header_open,
                                            len(marker.open),
                                            f"Generated body must contain only one line to be inlined:")
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 class NonGeneratedEditException(GenerationException):
     @staticmethod
-    def from_marker(marker):
+    def from_marker(marker: parser.Marker) -> "NonGeneratedEditException":
         return CommonException.from_marker(NonGeneratedEditException,
                                            marker,
                                            marker.header_open,
                                            len(marker.open),
                                            f"Non-generated edit marker \"{marker.open} {marker.header} {marker.close}\", consider reusing/removing it:")
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 class AlreadyGeneratedEditException(GenerationException):
     @staticmethod
-    def from_marker(marker):
+    def from_marker(marker: parser.Marker) -> "AlreadyGeneratedEditException":
         return CommonException.from_marker(AlreadyGeneratedEditException,
                                            marker,
                                            marker.header_open,
                                            len(marker.open),
                                            f"Already generated edit marker \"{marker.open} {marker.header} {marker.close}\", consider fixing generation:")
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
 ### Utils
 
-def index_to_coordinates(string, index):
+def index_to_coordinates(string: str, index: int) -> Tuple[int, int]:
     """ Returns the corresponding tuple (line, column) of the character at the given index of the given string.
     """
     if index < 0:
         index =  index % len(string)
     sp = string[:index+1].splitlines(keepends=True)
     return len(sp), len(sp[-1])
 
-def line_at_index(string, index):
+def line_at_index(string: str, index: int) -> str:
     """ Returns the line at the given index of the given string.
     """
     if index < 0:
         index =  index % len(string)
     start = string.rfind('\n', 0, index)+1
     end = string.find('\n', index)
     suffix = '\\n' if end >= 0 else '\\0'
     if end < 0:
         end = len(string)
     return f"{string[start:end]}{suffix}"
 
-def format_text(text, max_length = 50, suffix = "..."):
+def format_text(text: str, max_length = 50, suffix = "...") -> str:
     """ Replaces tabulations and ends of line.
     """
     text = text if len(text) <= max_length else f"{text[:max_length]}{suffix}"
     return text.replace('\t', "\\t").replace('\n', "\\n")
 
-def split_traceback(tb, remove_class_name = False):
+def split_traceback(tb: str, remove_class_name = False) -> Tuple[str, str]:
     """ Splits the given traceback into (stacktrace, message).
     """
     startidx = -1
     while True:
         startidx = tb.find('\n', startidx+1)
         if startidx < 0:
             break # No stacktrace
@@ -269,15 +274,15 @@
     "__getattribute__",
     "__init__",
     "__new__",
     "__setattr__",
     "__str__",
 ]
 
-def wrap_exception(exception, message):
+def wrap_exception(exception: _TException, message) -> _TException:
     """ Wraps the given exception with a custom message.
         Creates an object that mocks the exception class.
     """
     if hasattr(exception, "_wrapped_exception") and hasattr(exception, "_wrapped_message"):
         exception._wrapped_message = message
         return exception
     try:
@@ -295,15 +300,15 @@
             setattr(mock, key, value)
         mock._wrapped_exception = exception
         mock._wrapped_message = message
         return mock
     except:
         return exception
 
-def prepend_jinja2_traceback(exception, tb = None):
+def prepend_jinja2_traceback(exception: _TException, tb: str = None) -> _TException:
     """ Prepends the Jinja2 traceback to the given exception.
         Creates an object that derives the exception class.
     """
     if tb == None:
         tb = traceback.format_exc().rstrip('\n')
     (stacktrace, message) = split_traceback(tb, True)
     if stacktrace != None:
@@ -344,46 +349,46 @@
                 else:
                     stacktrace = stacktrace[:startidx]
     if message == None:
         message = ""
     message = f"\n{stacktrace}\n{message}" if stacktrace else f"\n{message}"
     return wrap_exception(exception, message)
 
-def clean_traceback(exception):
+def clean_traceback(exception: _TException) -> _TException:
     """ Removes the traceback of the given exception.
     """
     return prepend_jinja2_traceback(exception).with_traceback(None)
 
 ### --debug option enabled
 
-class DebugAttributeError(BaseException):
-    def __init__(self, message):
+class DebugAttributeError(Exception):
+    def __init__(self, message: str):
         super().__init__(message)
 
 _disallowed_stacktraces = [
     "autojinja_wrapped_fcall",
     "autojinja_fcall",
     "autojinja_fget",
     "autojinja_fset",
     "autojinja_fdel"
 ]
 
-def clean_wrapped_stacktrace(exception):
+def clean_wrapped_stacktrace(exception: _TException) -> str:
     """ Cleans the the given exception's stacktrace from useless wrapper calls.
     """
     if exception.__class__.__module__ != "builtins":
         fullname = f"{exception.__class__.__module__}.{exception.__class__.__qualname__}: "
     else:
         fullname = f"{exception.__class__.__qualname__}: "
     stacktrace = traceback.format_exc()
     lines = stacktrace.splitlines()
     start = -1
     for i in range(0, len(lines), 1):
-        if lines[i].endswith("line 15, in autojinja_wrapped_fcall") \
-        or lines[i].endswith("line 18, in autojinja_wrapped_fcall"): # /!\ easily breakable
+        if lines[i].endswith("line 18, in autojinja_wrapped_fcall") \
+        or lines[i].endswith("line 21, in autojinja_wrapped_fcall"): # /!\ easily breakable
             start = i
             break
     end = -1
     if start > 0:
         for i in range(len(lines)-1, start, -1):
             if lines[i] == fullname:
                 end = i+1
@@ -401,30 +406,30 @@
             state = 1 # Skip
     for line in lines[end:]:
         message.write(f"\n{line}")
     return message.getvalue()
 
 _wrapped_properties = set()
 
-def _autojinja_fcall(wrapped_callable):
+def _autojinja_fcall(wrapped_callable: Callable):
     def autojinja_fcall(*args, **kwargs):
         return wrapped_callable(*args, **kwargs)
     return wrap_callable(autojinja_fcall)
 
-def _autojinja_fget(wrapped_property):
+def _autojinja_fget(wrapped_property: property):
     def autojinja_fget(self):
         return wrapped_property.fget(self)
     return wrap_callable(autojinja_fget)
 
-def _autojinja_fset(wrapped_property):
+def _autojinja_fset(wrapped_property: property):
     def autojinja_fset(self, value):
         return wrapped_property.fset(self, value)
     return wrap_callable(autojinja_fset)
 
-def _autojinja_fdel(wrapped_property):
+def _autojinja_fdel(wrapped_property: property):
     def autojinja_fdel(self):
         return wrapped_property.fdel(self)
     return wrap_callable(autojinja_fdel)
 
 _disallowed_modules = set([
     "autojinja.defaults",
     "autojinja.exceptions",
@@ -432,15 +437,17 @@
     "autojinja.parser",
     "autojinja.path",
     "autojinja.templates",
     "autojinja.utils",
     "builtins",
 ])
 
-def wrap_object_attributes(obj):
+_TObject = TypeVar("_TObject")
+
+def wrap_object_attributes(obj: _TObject) -> _TObject:
     """ Wraps all properties and methods of the given objects in order to bypass
         AttributeError handling of Jinja and provide better exception stacktraces.
     """
     if str(obj.__class__.__module__) in _disallowed_modules:
         return obj
     for name in dir(obj):
         try:
```

### Comparing `autojinja-1.8.1/autojinja/main.py` & `autojinja-1.9.0/autojinja/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,22 +57,23 @@
                                               1: [autojinja]  -------  <abs_path>  (from <abs_path>)
                                       001
                                         ^------ notification when changed only (1)
                                               0: [autojinja]  -------  <path>  (from <path>)
                                               1: [autojinja]  changed  <path>  (from <path>)
 """
 
-from .defaults import *
+from . import defaults
 from . import path
 from . import utils
 
 import argparse
-import os.path
+import os
 import subprocess
 import sys
+from typing import List
 
 this_module = sys.modules[__name__]
 
 def main(*arguments):
     ### Parse arguments
     parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter,
                                      description="Visits directories and executes python scripts to perform content generation")
@@ -83,61 +84,61 @@
                              "    The filepath must end with '.py' extension\n\n"
                              "DIRECTORY:\n"
                              "    Directory to visit\n"
                              "    Only works if '--search-filename' or '--search-tag' is enabled")
     parser.add_argument("-f",
                         "--search-filename",
                         action="store_true",
-                        help=f"searches for python scripts named '{AUTOJINJA_DEFAULT_FILENAME}' in visited directories")
+                        help=f"searches for python scripts named '{defaults.AUTOJINJA_DEFAULT_FILENAME}' in visited directories")
     parser.add_argument("-t",
                         "--search-tag",
                         action="store_true",
-                        help=f"searches for python scripts tagged '{AUTOJINJA_DEFAULT_TAG}' in visited directories")
+                        help=f"searches for python scripts tagged '{defaults.AUTOJINJA_DEFAULT_TAG}' in visited directories")
     parser.add_argument("-r",
                         "--recursive",
                         action="store_true",
                         help="recursively visits subdirectories of visited directories")
     parser.add_argument("-a",
                         "--all",
                         action="store_true",
                         help="all above options simultaneously (equivalent to '-ftr')")
     parser.add_argument("--filename",
-                        default=AUTOJINJA_DEFAULT_FILENAME,
-                        help=f"filename searched by '--search-filename'. Default filename is '{AUTOJINJA_DEFAULT_FILENAME}'")
+                        default=defaults.AUTOJINJA_DEFAULT_FILENAME,
+                        help=f"filename searched by '--search-filename'. Default filename is '{defaults.AUTOJINJA_DEFAULT_FILENAME}'")
     parser.add_argument("--tag",
-                        default=AUTOJINJA_DEFAULT_TAG,
-                        help=f"tag searched by '--search-tag'. Default tag is '{AUTOJINJA_DEFAULT_TAG}'\n"
-                             f"Python scripts' first line must contain this tag (ex: '### {AUTOJINJA_DEFAULT_TAG} ###')")
+                        default=defaults.AUTOJINJA_DEFAULT_TAG,
+                        help=f"tag searched by '--search-tag'. Default tag is '{defaults.AUTOJINJA_DEFAULT_TAG}'\n"
+                             f"Python scripts' first line must contain this tag (ex: '### {defaults.AUTOJINJA_DEFAULT_TAG} ###')")
     parser.add_argument("-e",
                         "--env",
                         action="append",
                         help="additional environment variable or .env file")
     parser.add_argument("-i",
                         "--includes",
                         action="append",
                         help="additional import directories for executed python scripts\n"
                              "Directory list separated by ':' (Unix only) or ';' (Windows and Unix)\n"
                              "Appended to environment variable 'PYTHONPATH'")
     parser.add_argument("--remove-markers",
                         help=f"removes markers from generated outputs\n"
-                             f"Default value is '0' or environment variable '{AUTOJINJA_REMOVE_MARKERS}'\n"
-                             f"Overrides environment variable '{AUTOJINJA_REMOVE_MARKERS}'")
+                             f"Default value is '0' or environment variable '{defaults.AUTOJINJA_REMOVE_MARKERS}'\n"
+                             f"Overrides environment variable '{defaults.AUTOJINJA_REMOVE_MARKERS}'")
     parser.add_argument("--silent",
                         action="store_true",
                         help=f"prevents executed python scripts from writing to stdout/stderr\n"
-                             f"Enabled if environment variable '{AUTOJINJA_SILENT}' == 1\n"
-                             f"Overrides environment variable '{AUTOJINJA_SILENT}'")
+                             f"Enabled if environment variable '{defaults.AUTOJINJA_SILENT}' == 1\n"
+                             f"Overrides environment variable '{defaults.AUTOJINJA_SILENT}'")
     parser.add_argument("--debug",
                         action="store_true",
                         help=f"enhances stacktraces for exceptions raised from Jinja context variables\n"
-                             f"Enabled if environment variable '{AUTOJINJA_DEBUG}' == 1\n"
-                             f"Overrides environment variable '{AUTOJINJA_DEBUG}'")
+                             f"Enabled if environment variable '{defaults.AUTOJINJA_DEBUG}' == 1\n"
+                             f"Overrides environment variable '{defaults.AUTOJINJA_DEBUG}'")
     parser.add_argument("--summary",
                         help=f"enables notifications for generated files to stdout\n"
-                             f"Overrides environment variable '{AUTOJINJA_SUMMARY}'\n"
+                             f"Overrides environment variable '{defaults.AUTOJINJA_SUMMARY}'\n"
                              f"Default value is '1':\n"
                              f"    0: nothing\n"
                              f"    1: [autojinja]  -------  <abs_path>  (from <abs_path>)\n"
                              f"Also accepts 3 flags instead:\n"
                              f"    100\n"
                              f"    ^------ show (1) / hide (0) executing script path\n"
                              f"            0: [autojinja]  -------  <path>\n"
@@ -158,15 +159,15 @@
 
     # Additional environment variables
     if args.env:
         utils.parse_envvars(env, args.env)
 
     # Additional import directories
     if args.includes:
-        includes = [path[include].abspath for includes in args.includes for include in includes.split(utils.os_pathsep(includes))]
+        includes = [path.Path(include).slash.abspath for includes in args.includes for include in includes.split(utils.os_pathsep(includes))]
         if "PYTHONPATH" in env:
             env["PYTHONPATH"] = f"{env['PYTHONPATH']}{os.pathsep}{os.pathsep.join(includes)}"
         else:
             env["PYTHONPATH"] = os.pathsep.join(includes)
 
     ### Verify options
     if args.all:
@@ -176,59 +177,59 @@
 
     # remove_markers
     if args.remove_markers != None:
         if args.remove_markers == True:
             args.remove_markers = 1
         elif args.remove_markers == False:
             args.remove_markers = 0
-        env[AUTOJINJA_REMOVE_MARKERS] = str(args.remove_markers)
-    args.remove_markers = osenviron_remove_markers(env)
-    env[AUTOJINJA_REMOVE_MARKERS] = str(args.remove_markers)
+        env[defaults.AUTOJINJA_REMOVE_MARKERS] = str(args.remove_markers)
+    args.remove_markers = defaults.osenviron_remove_markers(env)
+    env[defaults.AUTOJINJA_REMOVE_MARKERS] = str(args.remove_markers)
 
     # silent
     if args.silent == None or args.silent == False:
-        args.silent = osenviron_silent(env)
+        args.silent = defaults.osenviron_silent(env)
     else:
         args.silent = 1
-    env[AUTOJINJA_SILENT] = str(args.silent)
+    env[defaults.AUTOJINJA_SILENT] = str(args.silent)
 
     # debug
     if args.debug == None or args.debug == False:
-        args.debug = osenviron_debug(env)
+        args.debug = defaults.osenviron_debug(env)
     else:
         args.debug = 1
-    env[AUTOJINJA_DEBUG] = str(args.debug)
+    env[defaults.AUTOJINJA_DEBUG] = str(args.debug)
 
     # summary
     if args.summary != None:
-        env[AUTOJINJA_SUMMARY] = str(args.summary)
-    args.summary = osenviron_summary(env)
-    env[AUTOJINJA_SUMMARY] = str(args.summary)
+        env[defaults.AUTOJINJA_SUMMARY] = str(args.summary)
+    args.summary = defaults.osenviron_summary(env)
+    env[defaults.AUTOJINJA_SUMMARY] = str(args.summary)
 
     ### Parse arguments
-    def is_file_tagged(script):
+    def is_file_tagged(script: path.Path):
         try:
             return utils.is_file_tagged(script, args.tag)
         except:
             sys.stderr.write(f"[autojinja]  Couldn't read file at path  {script.abspath}\n")
 
-    files = []
-    for x in [path(x) for x in args.arguments]:
+    files: List[path.Path] = []
+    for x in [path.Path(x) for x in args.arguments]:
         if x.isfile:
             if x.ext != ".py":
                 raise Exception(f"File at path \"{x.abspath}\" is not a python script (.py extension)")
             files.append(x)
         elif not x.isdir:
             raise Exception(f"File or directory at path \"{x.abspath}\" doesn't exist")
         else:
             if not args.search_filename and not args.search_tag:
                 raise Exception("Directory arguments require '--search-filename' or '--search-tag'")
             if args.recursive:
                 for wroot, _, wfiles in os.walk(x):
-                    for script in [path(wroot).join(x) for x in wfiles]:
+                    for script in [path.Path(wroot).join(x) for x in wfiles]:
                         ## JINJA
                         if args.search_filename:
                             if script.filename == args.filename:
                                 files.append(script)
                         ## PYTHON
                         if args.search_tag:
                             if script.ext == ".py":
```

### Comparing `autojinja-1.8.1/autojinja/parser.py` & `autojinja-1.9.0/autojinja/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,247 +1,58 @@
-from .defaults import *
-from .exceptions import *
+from . import defaults
+from . import exceptions
 
 import io
-import os
-
-class ParserSettings:
-    def __init__(self,
-                 cog_open = AUTOJINJA_DEFAULT_COG_OPEN,
-                 cog_close = AUTOJINJA_DEFAULT_COG_CLOSE,
-                 cog_end = AUTOJINJA_DEFAULT_COG_END,
-                 cog_as_comment = False,
-                 edit_open = AUTOJINJA_DEFAULT_EDIT_OPEN,
-                 edit_close = AUTOJINJA_DEFAULT_EDIT_CLOSE,
-                 edit_end = AUTOJINJA_DEFAULT_EDIT_END,
-                 edit_as_comment = False,
-                 remove_markers = None,
-                 encoding = None,
-                 newline = None):
-        self.cog_open = cog_open
-        self.cog_close = cog_close
-        self.cog_end = cog_end
-        self.cog_as_comment = cog_as_comment
-        self.edit_open = edit_open
-        self.edit_close = edit_close
-        self.edit_end = edit_end
-        self.edit_as_comment = edit_as_comment
-        self.remove_markers = remove_markers
-        self.encoding = encoding
-        self.newline = newline
-
-    @property
-    def remove_markers(self):
-        return self._removeMarkers
-    @remove_markers.setter
-    def remove_markers(self, remove_markers):
-        self._removeMarkers = remove_markers or osenviron_remove_markers()
-
-class Parser:
-    def __init__(self, string, settings):
-        self.string = string
-        self.settings = settings
-        self.markers = None # List[Marker]
-        self.blocks = None # List[Block]
-        self.cog_blocks = None # List[CogBlock]
-        self.edit_blocks = None # List[EditBlock]
-
-    @property
-    def edits(self):
-        return { key: edit_block.body for key, edit_block in self.edit_blocks.items() }
-
-    def parse(self):
-        idx = 0
-        cog_markers = []
-        edit_markers = []
-        ### Find all [[[ ]]] pairs
-        while True:
-            marker = Marker(self.string, False, self.settings.cog_open, self.settings.cog_close, self.settings.cog_end, self.settings.cog_as_comment, None, True)
-            marker, idx = self.find_marker(marker, idx, len(self.string))
-            if not marker:
-                break
-            cog_markers.append(marker)
-        ### Find all <<[ ]>> pairs not in [[[ ]]]
-        sections = [[0,-1]]
-        for cog_marker in cog_markers:
-            sections[-1][1] = cog_marker.header_open
-            sections.append([cog_marker.header_close, -1])
-        sections[-1][1] = len(self.string)
-        for section in sections:
-            idx = section[0]
-            while True:
-                marker = Marker(self.string, True, self.settings.edit_open, self.settings.edit_close, self.settings.edit_end, self.settings.edit_as_comment, True, False)
-                marker, idx = self.find_marker(marker, idx, section[1])
-                if not marker:
-                    break
-                edit_markers.append(marker)
-        ### Properly resolve [[[ ]]] and <<[ ]>>
-        self.markers = cog_markers + edit_markers
-        self.markers.sort(key=lambda x: x.header_open)
-        self.check_markers()
-        ### Collect blocks
-        self.blocks = []
-        self.cog_blocks = []
-        self.edit_blocks = {}
-        for marker in self.markers:
-            if not marker.is_end:
-                if marker.is_edit:
-                    block = EditBlock(marker)
-                    if block.name in self.edit_blocks:
-                        raise DuplicateEditException.from_marker(marker)
-                    self.edit_blocks[block.name] = block
-                else:
-                    block = CogBlock(marker)
-                    self.cog_blocks.append(block)
-                self.blocks.append(block)
-
-    def find_marker(self, marker, idx, end):
-        ### Find open
-        found, idx = self.find_token(marker.open, idx, end)
-        if not found:
-            return None, idx
-        ### Set open location
-        marker.header_open = idx
-        ### Find close
-        idx = idx + len(marker.open)
-        found, idx = self.find_token(marker.close, idx, end)
-        if not found:
-            raise CloseMarkerNotFoundException.from_marker(marker)
-        ### Set close location
-        idx = idx + len(marker.close)
-        marker.header_close = idx
-        ### Extract header
-        marker.extract_indent()
-        marker.extract_header()
-        return marker, idx
-
-    def find_token(self, token, idx, end):
-        i = self.string.find(token, idx, end)
-        if i < 0:
-            return False, idx
-        return True, i
-
-    def check_markers(self):
-        stack = []
-        prev_inline = []
-        mkrstate = 0 # 0: none, 1: cog, 2: edit, 3: cog end, 4: edit end
-        state = 0 # 0: no requirement, 1: waiting for requirement, 2: require other line, 3: require same line
-        prev_marker = None
-        for marker in self.markers:
-            ### Check cog & edit markers enclosure
-            newstate = 1 + marker.is_edit + 2 * marker.is_end
-            if mkrstate == 1 and newstate == 4:
-                raise WrongInclusionException.from_marker(marker)
-            if mkrstate == 2 and newstate == 3:
-                raise WrongInclusionException.from_marker(marker)
-            mkrstate = newstate
-            ### Check direct enclosure
-            if not marker.is_end and not marker.direct_enclosure and stack and stack[-1].is_edit == marker.is_edit:
-                raise DirectlyEnclosedEditException.from_marker(marker)
-            ### Check requirements with previous marker
-            if prev_marker:
-                same_line = marker.same_line(prev_marker.header_close, marker.header_open)
-                if state == 0:
-                    pass
-                elif state == 1:
-                    state = 3 if same_line else 0
-                elif state == 2:
-                    if same_line:
-                        raise RequireNewlineException.from_marker(marker)
-                    state = 0
-                elif state == 3:
-                    if not same_line:
-                        raise RequireInlineException.from_marker(marker)
-                    state = 0
-            ### Ensure marker subtree is correctly inlined
-            if prev_inline:
-                if prev_inline[-1] == None: # No requirement
-                    prev_inline[-1] = same_line
-                elif prev_inline[-1] == False: # Should be multiline
-                    if same_line:
-                        raise RequireNewlineException.from_marker(marker)
-                elif not same_line: # Should be inlined
-                    raise RequireInlineException.from_marker(marker)
-            ### Deal marker
-            if not marker.is_end:
-                stack.append(marker)
-                prev_inline.append(True if prev_inline and prev_inline[-1] else None)
-                prev_marker = marker
-            else:
-                if not stack:
-                    raise OpenMarkerNotFoundException.from_marker(marker)
-                openMarker = stack.pop()
-                same_line = prev_inline.pop()
-                prev_marker = marker
-                ### Set duals
-                openMarker.dual = marker
-                marker.dual = openMarker
-                ### Extract body
-                openMarker.extract_body(marker, same_line)
-                if same_line:
-                    state = 1
-                    # Set start / end indexes
-                    openMarker.header_start = openMarker.header_open
-                    openMarker.header_end = openMarker.header_close
-                    marker.header_start = marker.header_open
-                    marker.header_end = marker.header_close
-                else:
-                    state = 2
-                    # Set end indexes
-                    openMarker.header_end = openMarker.header_close
-                    i = self.string.find('\n', marker.header_close)
-                    marker.header_end = i+1 if i >= 0 else len(self.string)
-        if stack:
-            raise EndMarkerNotFoundException.from_marker(stack[-1])
+from typing import Dict, List, Optional, Tuple
 
 class Marker:
-    def __init__(self, string, is_edit, open, close, end, as_comment, headerInline, directEnclosure):
-        self.string = string
-        self.is_edit = is_edit
-        self.is_end = False
-        self.open = open
-        self.close = close
-        self.end = end
-        self.as_comment = as_comment # True or False
-        self.direct_enclosure = directEnclosure # True or False
+    def __init__(self, string: str, is_edit: bool, open: str, close: str, end: str, as_comment: bool, headerInline: Optional[bool], directEnclosure: bool):
+        self.string: str = string
+        self.is_edit: bool = is_edit
+        self.is_end: bool = False
+        self.open: str = open
+        self.close: str = close
+        self.end: str = end
+        self.as_comment: bool = as_comment
+        self.direct_enclosure: bool = directEnclosure
         # Header
-        self.header_inline = headerInline # True: inline, False: Multiline, None: Both
-        self.header_empty = True
-        self.header_column = 0
-        self.header = ""
-        self._header_stripped = None
-        self.header_start = 0 # Index, multiline / inline dependant
-        self.header_end = 0 # Index, multiline / inline dependant
-        self.header_open = 0 # Index, l-prolonged
-        self.header_close = 0 # Index, r-prolonged
-        self.header_indent_column = 0
-        self.header_indent = ""
+        self.header_inline: Optional[bool] = headerInline # True: inline, False: Multiline, None: Both
+        self.header_empty: bool = True
+        self.header_column: int = 0
+        self.header: str = ""
+        self._header_stripped: str = None
+        self.header_start: int = 0 # Index, multiline / inline dependant
+        self.header_end: int = 0 # Index, multiline / inline dependant
+        self.header_open: int = 0 # Index, l-prolonged
+        self.header_close: int = 0 # Index, r-prolonged
+        self.header_indent_column: int = 0
+        self.header_indent: str = ""
         # Body
-        self.body_inline = False
-        self.body_empty = True
-        self.body_column = 0
-        self.body = ""
-        self._body_dedented = None
-        self.body_start = 0 # Index, with indentation
-        self.body_end = 0 # Index
+        self.body_inline: bool = False
+        self.body_empty: bool = True
+        self.body_column: int = 0
+        self.body: str = ""
+        self._body_dedented: str = None
+        self.body_start: int = 0 # Index, with indentation
+        self.body_end: int = 0 # Index
         # Dual
-        self.dual = None # Open or end marker
+        self.dual: Marker = None # Open or end marker
 
     @property
-    def header_stripped(self):
+    def header_stripped(self) -> str:
         if self._header_stripped == None:
             self._header_stripped = self.header.strip()
         return self._header_stripped
     @property
-    def body_dedented(self):
+    def body_dedented(self) -> str:
         if self._body_dedented == None:
             self._body_dedented = self.dedent_body()
         return self._body_dedented
 
-    def same_line(self, startidx, idx):
+    def same_line(self, startidx: int, idx: int) -> bool:
         i = self.string.rfind('\n', startidx, idx)
         return i < 0
 
     def extract_indent(self):
         start = self.string.rfind('\n', 0, self.header_open)+1
         end = start
         body = self.header_open
@@ -268,25 +79,25 @@
         marker_content = io.StringIO()
         self.header_empty = True
         idx = self.header_close - len(self.close)
         start = self.header_open + len(self.open)
         ### Same line
         if self.same_line(self.header_open, idx):
             if self.header_inline == False:
-                raise RequireHeaderMultilineException.from_marker(self)
+                raise exceptions.RequireHeaderMultilineException.from_marker(self)
             if self.string[start] == ' ':
                 start += 1
             if self.string[idx-1] == ' ':
                 idx -= 1
             marker_content.write(self.string[start:idx])
             self.header_empty = idx <= start
         ### Different lines
         else:
             if self.header_inline == True:
-                raise RequireHeaderInlineException.from_marker(self)
+                raise exceptions.RequireHeaderInlineException.from_marker(self)
             # First line
             i = self.string.find('\n', start, idx)
             if i > start:
                 if self.string[start] == ' ':
                     start += 1
                 marker_content.write(self.string[start:i])
                 self.header_empty = False
@@ -311,15 +122,15 @@
                             marker_content.write('\n')
                         marker_content.write(self.string[start+self.header_column:idx])
                         self.header_empty = False
                     break
         self.header = marker_content.getvalue()
         self.is_end = self.header == self.end
 
-    def extract_body(self, end_marker, same_line):
+    def extract_body(self, end_marker: "Marker", same_line: bool):
         body = io.StringIO()
         ### Same line
         if same_line:
             self.body_inline = True
             i = self.string.find(' ', self.header_close, end_marker.header_open)
             if i < 0:
                 self.body_start = self.header_close
@@ -339,35 +150,35 @@
             self.body_start = self.string.find('\n', self.header_close) + 1
             self.body_end = self.string.rfind('\n', self.header_close, end_marker.header_open) + 1
             self.header_close = self.body_start
             body.write(self.string[self.body_start:self.body_end-1])
         self.body = body.getvalue()
         self.body_empty = len(self.body) == 0
 
-    def check_indent(self, start, end):
+    def check_indent(self, start: int, end: int):
         idx = start + self.header_indent_column
         for i in range(start, start+self.header_column):
             if i < end:
                 if self.string[i] == ' ':
                     if self.header_indent[i-start] != '\t': continue
                 elif self.string[i] == '\t':
                     if self.header_indent[i-start] == '\t': continue
                 elif i < idx: continue # Eat until comment end
             elif i >= idx and self.string[i] == '\n':
                 break
-            raise WrongHeaderIndentationException.from_marker(self, i)
+            raise exceptions.WrongHeaderIndentationException.from_marker(self, i)
 
-    def dedent_body(self):
+    def dedent_body(self) -> str:
         if self.body_empty:
             return None
         if self.body_inline:
             return self.body
         return self.dedent(self.body)
 
-    def dedent(self, output):
+    def dedent(self, output: str) -> str:
         result = io.StringIO()
         start = 0
         while True:
             idx = output.find('\n', start, len(output))
             mid = min(start + self.body_column, len(output) if idx < 0 else idx)
             for i in range(start, mid):
                 if output[i] != ' ' and output[i] != '\t':
@@ -379,32 +190,32 @@
             else:
                 end = idx+1
                 result.write(output[mid:end])
                 start = end
         return result.getvalue()
 
 class Block:
-    def __init__(self, marker):
-        self.marker = marker
+    def __init__(self, marker: Marker):
+        self.marker: Marker = marker
 
     @property
-    def raw_header(self):
+    def raw_header(self) -> str:
         return self.marker.header
     @property
-    def header(self):
+    def header(self) -> str:
         return self.marker.header_stripped
 
     @property
-    def raw_body(self):
+    def raw_body(self) -> str:
         return self.marker.body
     @property
-    def body(self):
+    def body(self) -> str:
         return self.marker.body_dedented
 
-    def get_code(self, additional_lines = (0, 0)):
+    def get_code(self, additional_lines: Tuple[int, int] = (0, 0)) -> str:
         if self.marker.body_inline:
             start = self.marker.header_start
             end = self.marker.dual.header_end
             # Complete line
             start = self.marker.string.rfind('\n', 0, start)+1
             i = self.marker.string.find('\n', end)
             if i >= 0:
@@ -427,28 +238,217 @@
             else:
                 end = len(self.marker.string)
         if end > 0 and self.marker.string[end-1] == '\n':
             end -= 1
         return self.marker.string[start:end]
 
 class CogBlock(Block):
-    def __init__(self, marker):
+    def __init__(self, marker: Marker):
         super().__init__(marker)
 
 class EditBlock(Block):
-    def __init__(self, marker):
+    def __init__(self, marker: Marker):
         super().__init__(marker)
-        self._body = None
-        self.allow_code_loss = False # Use at your own risk
+        self._body: str = None
+        self.allow_code_loss: bool = False # Use at your own risk
     def __str__(self):
         return f"{self.__repr__()} named {self.name}"
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self.header
 
     @property
-    def body(self):
+    def body(self) -> str:
         return self._body or super().body
     @body.setter
-    def body(self, body):
+    def body(self, body: str):
         self._body = body
+
+class ParserSettings:
+    def __init__(self,
+                 cog_open = defaults.AUTOJINJA_DEFAULT_COG_OPEN,
+                 cog_close = defaults.AUTOJINJA_DEFAULT_COG_CLOSE,
+                 cog_end = defaults.AUTOJINJA_DEFAULT_COG_END,
+                 cog_as_comment = False,
+                 edit_open = defaults.AUTOJINJA_DEFAULT_EDIT_OPEN,
+                 edit_close = defaults.AUTOJINJA_DEFAULT_EDIT_CLOSE,
+                 edit_end = defaults.AUTOJINJA_DEFAULT_EDIT_END,
+                 edit_as_comment = False,
+                 remove_markers: Optional[bool] = None,
+                 encoding: Optional[str] = None,
+                 newline: Optional[str] = None):
+        self.cog_open: str = cog_open
+        self.cog_close: str = cog_close
+        self.cog_end: str = cog_end
+        self.cog_as_comment: bool = cog_as_comment
+        self.edit_open: str = edit_open
+        self.edit_close: str = edit_close
+        self.edit_end: str = edit_end
+        self.edit_as_comment: bool = edit_as_comment
+        self.remove_markers: Optional[bool] = remove_markers
+        self.encoding: Optional[str] = encoding
+        self.newline: Optional[str] = newline
+
+    @property
+    def remove_markers(self) -> bool:
+        return self._removeMarkers
+    @remove_markers.setter
+    def remove_markers(self, remove_markers: Optional[bool]):
+        self._removeMarkers = remove_markers or defaults.osenviron_remove_markers()
+
+class Parser:
+    def __init__(self, string: str, settings: ParserSettings):
+        self.string: str = string
+        self.settings: ParserSettings = settings
+        self.markers: List[Marker] = None
+        self.blocks: List[Block] = None
+        self.cog_blocks: List[CogBlock] = None
+        self.edit_blocks: Dict[str, EditBlock] = None
+
+    @property
+    def edits(self) -> Dict[str, str]:
+        return { key: edit_block.body for key, edit_block in self.edit_blocks.items() }
+
+    def parse(self):
+        idx = 0
+        cog_markers: List[Marker] = []
+        edit_markers: List[Marker] = []
+        ### Find all [[[ ]]] pairs
+        while True:
+            marker = Marker(self.string, False, self.settings.cog_open, self.settings.cog_close, self.settings.cog_end, self.settings.cog_as_comment, None, True)
+            marker, idx = self.find_marker(marker, idx, len(self.string))
+            if not marker:
+                break
+            cog_markers.append(marker)
+        ### Find all <<[ ]>> pairs not in [[[ ]]]
+        sections = [[0,-1]]
+        for cog_marker in cog_markers:
+            sections[-1][1] = cog_marker.header_open
+            sections.append([cog_marker.header_close, -1])
+        sections[-1][1] = len(self.string)
+        for section in sections:
+            idx = section[0]
+            while True:
+                marker = Marker(self.string, True, self.settings.edit_open, self.settings.edit_close, self.settings.edit_end, self.settings.edit_as_comment, True, False)
+                marker, idx = self.find_marker(marker, idx, section[1])
+                if not marker:
+                    break
+                edit_markers.append(marker)
+        ### Properly resolve [[[ ]]] and <<[ ]>>
+        self.markers = cog_markers + edit_markers
+        self.markers.sort(key=lambda x: x.header_open)
+        self.check_markers()
+        ### Collect blocks
+        self.blocks = []
+        self.cog_blocks = []
+        self.edit_blocks = {}
+        for marker in self.markers:
+            if not marker.is_end:
+                if marker.is_edit:
+                    block = EditBlock(marker)
+                    if block.name in self.edit_blocks:
+                        raise exceptions.DuplicateEditException.from_marker(marker)
+                    self.edit_blocks[block.name] = block
+                else:
+                    block = CogBlock(marker)
+                    self.cog_blocks.append(block)
+                self.blocks.append(block)
+
+    def find_marker(self, marker: Marker, idx: int, end: int) -> Tuple[Marker, int]:
+        ### Find open
+        found, idx = self.find_token(marker.open, idx, end)
+        if not found:
+            return None, idx
+        ### Set open location
+        marker.header_open = idx
+        ### Find close
+        idx = idx + len(marker.open)
+        found, idx = self.find_token(marker.close, idx, end)
+        if not found:
+            raise exceptions.CloseMarkerNotFoundException.from_marker(marker)
+        ### Set close location
+        idx = idx + len(marker.close)
+        marker.header_close = idx
+        ### Extract header
+        marker.extract_indent()
+        marker.extract_header()
+        return marker, idx
+
+    def find_token(self, token: str, idx, end: int) -> Tuple[bool, int]:
+        i = self.string.find(token, idx, end)
+        if i < 0:
+            return False, idx
+        return True, i
+
+    def check_markers(self):
+        stack: List[Marker] = []
+        prev_inline: List[bool] = []
+        mkrstate = 0 # 0: none, 1: cog, 2: edit, 3: cog end, 4: edit end
+        state = 0 # 0: no requirement, 1: waiting for requirement, 2: require other line, 3: require same line
+        prev_marker: Marker = None
+        for marker in self.markers:
+            ### Check cog & edit markers enclosure
+            newstate = 1 + marker.is_edit + 2 * marker.is_end
+            if mkrstate == 1 and newstate == 4:
+                raise exceptions.WrongInclusionException.from_marker(marker)
+            if mkrstate == 2 and newstate == 3:
+                raise exceptions.WrongInclusionException.from_marker(marker)
+            mkrstate = newstate
+            ### Check direct enclosure
+            if not marker.is_end and not marker.direct_enclosure and stack and stack[-1].is_edit == marker.is_edit:
+                raise exceptions.DirectlyEnclosedEditException.from_marker(marker)
+            ### Check requirements with previous marker
+            if prev_marker:
+                same_line = marker.same_line(prev_marker.header_close, marker.header_open)
+                if state == 0:
+                    pass
+                elif state == 1:
+                    state = 3 if same_line else 0
+                elif state == 2:
+                    if same_line:
+                        raise exceptions.RequireNewlineException.from_marker(marker)
+                    state = 0
+                elif state == 3:
+                    if not same_line:
+                        raise exceptions.RequireInlineException.from_marker(marker)
+                    state = 0
+            ### Ensure marker subtree is correctly inlined
+            if prev_inline:
+                if prev_inline[-1] == None: # No requirement
+                    prev_inline[-1] = same_line
+                elif prev_inline[-1] == False: # Should be multiline
+                    if same_line:
+                        raise exceptions.RequireNewlineException.from_marker(marker)
+                elif not same_line: # Should be inlined
+                    raise exceptions.RequireInlineException.from_marker(marker)
+            ### Deal marker
+            if not marker.is_end:
+                stack.append(marker)
+                prev_inline.append(True if prev_inline and prev_inline[-1] else None)
+                prev_marker = marker
+            else:
+                if not stack:
+                    raise exceptions.OpenMarkerNotFoundException.from_marker(marker)
+                openMarker = stack.pop()
+                same_line = prev_inline.pop()
+                prev_marker = marker
+                ### Set duals
+                openMarker.dual = marker
+                marker.dual = openMarker
+                ### Extract body
+                openMarker.extract_body(marker, same_line)
+                if same_line:
+                    state = 1
+                    # Set start / end indexes
+                    openMarker.header_start = openMarker.header_open
+                    openMarker.header_end = openMarker.header_close
+                    marker.header_start = marker.header_open
+                    marker.header_end = marker.header_close
+                else:
+                    state = 2
+                    # Set end indexes
+                    openMarker.header_end = openMarker.header_close
+                    i = self.string.find('\n', marker.header_close)
+                    marker.header_end = i+1 if i >= 0 else len(self.string)
+        if stack:
+            raise exceptions.EndMarkerNotFoundException.from_marker(stack[-1])
```

### Comparing `autojinja-1.8.1/autojinja/utils.py` & `autojinja-1.9.0/autojinja/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,185 +1,186 @@
 from . import defaults
 from . import exceptions
 from . import parser
 from . import path
 
 import os
 import sys
+from typing import Dict, List, Optional
 
-def is_file_tagged(filepath, tag = defaults.AUTOJINJA_DEFAULT_TAG, encoding = None):
+def is_file_tagged(filepath: str, tag = defaults.AUTOJINJA_DEFAULT_TAG, encoding: str = None) -> bool:
     """ Returns True if the file at the given filepath is tagged with the given tag.
         The file's first line must contain this tag (ex: '### autojinja ###').
         Raises an error if the file can't be read.
     """
     with open(filepath, 'r', encoding = encoding or "utf-8") as file:
         return tag in file.readline()
 
-def generate_file(filepath, new_content, old_content = None, encoding = None, newline = None):
+def generate_file(filepath: str, new_content: str, old_content: str = None, encoding: str = None, newline: str = None):
     """ Generates the given content to the given filepath.
         Only writes the content to the file if the content is new.
         The previous content can be directly provided to avoid reading the file.
         Raises an error if the file can't be read/write.
     """
     assert filepath != None, "output filepath parameter can't be None"
     ### Compare old content
-    filepath = path(filepath).abspath
+    filepath: path.Path = path.Path(filepath).abspath
     created = not filepath.isfile
     if not created and not old_content:
         with open(filepath, 'r', encoding = encoding or "utf-8") as file:
             old_content = file.read()
     ### Save new generation
     changed = new_content != old_content
     if created or changed:
         with open(filepath, 'w', encoding = encoding or "utf-8", newline = newline) as file:
             file.write(new_content)
     ### Print summary
-    message = None
+    message: str = None
     summary = defaults.osenviron_summary()
     if summary == "0":
         pass
     elif summary == "1":
         message = f"[autojinja]  {'  new  ' if created else 'changed' if changed else '-------'}  {filepath}  (from {path.no_antislash(sys.argv[0])})"
     elif summary[2] == "1" and (not created and not changed):
         pass
     else:
-        executing_script = path(sys.argv[0])
+        executing_script = path.Path(sys.argv[0])
         message = f"[autojinja]  {'  new  ' if created else 'changed' if changed else '-------'}  "
         message += filepath if summary[1] == "1" else filepath.relpath(executing_script.dirpath)
         if summary[0] == "1":
             message += f"  (from {executing_script})"
     if message != None:
         print(message)
 
-def parse_file(filepath, settings = None, encoding = None):
+def parse_file(filepath: str, settings: parser.ParserSettings = None, encoding: str = None) -> Optional[parser.Parser]:
     """ Parses the given file and return the parsing result.
-        Returns an empty dictionary if the file doesn't exist.
+        Returns None if the file doesn't exist.
         Raises an error if the file can't be read.
     """
-    if not os.path.isfile(filepath):
-        return {}
+    if not path.isfile(filepath):
+        return None
     with open(filepath, 'r', encoding = encoding or (settings.encoding if settings else None) or "utf-8") as file:
         return parse_string(file.read(), settings)
 
-def parse_string(string, settings = None):
+def parse_string(string: str, settings: parser.ParserSettings = None) -> parser.Parser:
     """ Parses the given string and returns the parsing result.
     """
     try:
         object = parser.Parser(string, settings or parser.ParserSettings())
         object.parse()
         return object
-    except BaseException as e:
+    except Exception as e:
         raise e.with_traceback(None)
 
-def parse_envvars(env, values):
+def parse_envvars(env: os._Environ, values: List[str]):
     """ Loads the given environment variables to the given environment dictionary.
         Variable format must be 'name=value', otherwise considered as an environment file.
     """
     for arg in values:
         if '=' in arg: # Environment variable
             splits = arg.split('=', 1)
             env[splits[0].strip()] = evaluate_env(env, splits[1].strip())
         else: # Environment file
             parse_envfile(env, arg)
 
-def parse_envfile(env, envfile):
+def parse_envfile(env: os._Environ, envfile: str):
     """ Loads the given environment file and appends all environment variables to the given environment dictionary.
         The special environment variable ${THIS_DIRPATH} can be used to refer to the environment file location.
     """
     with open(envfile, encoding = "utf-8") as file:
         lines = [line.split('#', 1)[0].strip() for line in file.readlines()] # Remove comments
         lines = [line for line in lines if line] # Remove empty lines
         for line in lines:
             splits = line.split('=', 1)
             name = splits[0].strip()
             if len(splits) == 1:
                 env[name] = "" # No value defined
             else:
                 exists = defaults.AUTOJINJA_THIS_DIRPATH in env
                 if not exists:
-                    env[defaults.AUTOJINJA_THIS_DIRPATH] = path(envfile).abspath.dirpath[:-1]
+                    env[defaults.AUTOJINJA_THIS_DIRPATH] = path.Path(envfile).abspath.dirpath[:-1]
                 value = evaluate_env(env, splits[1].strip())
                 env[name] = value.strip()
                 if not exists:
                     del env[defaults.AUTOJINJA_THIS_DIRPATH]
 
-def evaluate_env(env, value):
+def evaluate_env(env: os._Environ, value: str) -> str:
     """ Evaluates the given string with the appropriate environment variables' value.
         /dir1/${VAR1}/file.txt -> /dir1/dir2/file.txt
     """
     old_env = os.environ
     try:
         os.environ = env
-        return os.path.expandvars(value)
+        return path.expandvars(value)
     finally:
         os.environ = old_env
 
-def os_pathsep(value):
+def os_pathsep(value: str) -> str:
     """ Returns the appropriate path separator based the given value and the host OS.
     """
     if os.name != "nt": # Unix
         return ':' if ':' in value else ';'
     else: # Windows
         return ';'
 
-def blocks_from_file(filepath, settings = None, encoding = None):
+def blocks_from_file(filepath: str, settings: parser.ParserSettings = None, encoding: str = None) -> List[parser.Block]:
     """ Returns a list with all pairs of markers in the given file.
         Returns an empty list if the file doesn't exist.
         Raises an error if the file can't be read.
     """
-    object = parse_file(filepath, settings, encoding)
-    return object.blocks
+    parser_obj = parse_file(filepath, settings, encoding)
+    return parser_obj.blocks if parser_obj else []
 
-def blocks_from_string(string, settings = None):
+def blocks_from_string(string: str, settings: parser.ParserSettings = None) -> List[parser.Block]:
     """ Returns a list with all pairs of markers in the given string.
     """
-    object = parse_string(string, settings)
-    return object.blocks
+    parser_obj = parse_string(string, settings)
+    return parser_obj.blocks
 
-def cog_blocks_from_file(filepath, settings = None, encoding = None):
+def cog_blocks_from_file(filepath: str, settings: parser.ParserSettings = None, encoding: str = None) -> List[parser.CogBlock]:
     """ Returns a list with all pairs of cog markers in the given file.
         Returns an empty list if the file doesn't exist.
         Raises an error if the file can't be read.
     """
-    object = parse_file(filepath, settings, encoding)
-    return object.cog_blocks
+    parser_obj = parse_file(filepath, settings, encoding)
+    return parser_obj.cog_blocks if parser_obj else []
 
-def cog_blocks_from_string(string, settings = None):
+def cog_blocks_from_string(string: str, settings: parser.ParserSettings = None) -> List[parser.CogBlock]:
     """ Returns a list with all paris of cog markers in the given string.
     """
-    object = parse_string(string, settings)
-    return object.cog_blocks
+    parser_obj = parse_string(string, settings)
+    return parser_obj.cog_blocks
 
-def edit_blocks_from_file(filepath, settings = None, encoding = None):
+def edit_blocks_from_file(filepath: str, settings: parser.ParserSettings = None, encoding: str = None) -> Dict[str, parser.EditBlock]:
     """ Returns a dictionary with all pairs of edit markers in the given file.
         Returns an empty dictionary if the file doesn't exist.
         Raises an error if the file can't be read.
     """
-    object = parse_file(filepath, settings, encoding)
-    return object.edit_blocks
+    parser_obj = parse_file(filepath, settings, encoding)
+    return parser_obj.edit_blocks if parser_obj else {}
 
-def edit_blocks_from_string(string, settings = None):
+def edit_blocks_from_string(string: str, settings: parser.ParserSettings = None) -> Dict[str, parser.EditBlock]:
     """ Returns a dictionary with all pairs of edit markers in the given string.
     """
     object = parse_string(string, settings)
     return object.edit_blocks
 
-def edits_from_file(filepath, settings = None, encoding = None):
+def edits_from_file(filepath: str, settings: parser.ParserSettings = None, encoding: str = None) -> Dict[str, str]:
     """ Returns a dictionary with all manual edits in the given file.
         Returns an empty dictionary if the file doesn't exist.
         Raises an error if the file can't be read.
     """
-    object = parse_file(filepath, settings, encoding)
-    return object.edits
+    parser_obj = parse_file(filepath, settings, encoding)
+    return parser_obj.edits if parser_obj else {}
 
-def edits_from_string(string, settings = None):
+def edits_from_string(string: str, settings: parser.ParserSettings = None) -> Dict[str, str]:
     """ Returns a dictionary with all manual edits in the given string.
     """
-    object = parse_string(string, settings)
-    return object.edits
+    parser_obj = parse_string(string, settings)
+    return parser_obj.edits
 
 def wrap_objects(*args, **kwargs):
     """ Wraps the given objects when the --debug option is enabled.
     """
     if len(args) > 0:
         args = list(args)
         for i in range(len(args)):
```

### Comparing `autojinja-1.8.1/autojinja.egg-info/PKG-INFO` & `autojinja-1.9.0/autojinja.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,168 +1,169 @@
 Metadata-Version: 2.1
 Name: autojinja
-Version: 1.8.1
+Version: 1.9.0
 Summary: Content generation with Jinja templates in between comments
 Home-page: https://github.com/ldflo/autojinja
 Author: Florian Popek
 Author-email: florian.popek@gmail.com
 License: BSD
-Description: # autojinja
-        
-        **autojinja** is a Python3 module that allows generating code inside any file using [Jinja templates](https://github.com/pallets/jinja) in between comments. It aims to assist development workflows by using simple Python3 scripts that perform content generation of neighboring files, which enables generating code next to traditionally hand-made code efficiently.
-        
-        It includes :
-        - Content generation in any file that accepts comments
-        - Ability to maintain hand-made code inside generated code
-        - Simple integration in build pipelines and existing codebases
-        
-        **autojinja** can be seen as a _preprocessor_ for most file formats, and works great with any codebase as it automates writing code manually. It shines out even more when working with metadata files (such as XML or JSON files) that centralize information which later needs to be generated across various scattered files in the codebase.
-        
-        ## Installation
-        
-        ```shell
-        $ pip install autojinja
-        ```
-        
-        ## Usage
-        
-        ```shell
-        $ autojinja script1.py script2.py
-        ```
-        ```shell
-        $ autojinja -a .
-        ```
-        
-        ## Content generation
-        
-        Content generation consists in generating parts of an existing file thanks to dedicated sections that delimit where the generation takes place. This technique is made possible for all files accepting comments, and allows defining [Jinja templates](https://github.com/pallets/jinja) directly in such files without breaking them.
-        
-        For example, let's suppose we have a C++ file we want to generate inside. To do this, we need to write our Jinja template between `[[[` and `]]]` markers, followed by an `[[[end]]]` marker :
-        
-        ```cpp
-        // main.cpp
-        #include <iostream>
-        
-        int main() {
-          std::cout << "Hello world !" << std::endl;
-          // [[[ std::cout << "{{ value }}" << std::endl; ]]]  // Jinja template
-          // [[[ end ]]]                                       // Code will be generated in between
-          return 0;
-        }
-        ```
-        
-        The template can then be generated with a Python3 script that provides the `value` variable :
-        
-        ```python
-        # main.py
-        from autojinja import CogTemplate
-        
-        template = CogTemplate.from_file("main.cpp")
-        template.context(value = "Python here !").render_file()
-        ```
-        
-        Calling the script will modify our C++ file as such :
-        
-        ```cpp
-        // main.cpp
-        #include <iostream>
-        
-        int main() {
-          std::cout << "Hello world !" << std::endl;
-          // [[[ std::cout << "{{ value }}" << std::endl; ]]]  // Jinja template
-          std::cout << "Python here !" << std::endl;
-          // [[[ end ]]]                                       // Code will be generated in between
-          return 0;
-        }
-        ```
-        
-        This technique is greatly inspired by [Cog](https://github.com/nedbat/cog), but adapted to work with Jinja templating engine. When performing generation again, the content inside the markers is entirely replaced by the new generation.
-        
-        ## Hand-made modifications
-        
-        Modification by hand of generated code is made possible by using special sections that are preserved across new generations. To do this, we need to name a section between `<<[` and `]>>` markers, followed by an `<<[end]>>` marker :
-        
-        ```cpp
-        // main.cpp
-        #include <iostream>
-        
-        // [[[
-        // int main() {
-        //
-        //   std::cout << "{{ value }}" << std::endl;
-        //   // <<[ impl ]>>  // Manually editable section named 'impl'
-        //   return 0;
-        //   // <<[ end ]>>   // End of section
-        //
-        // }
-        // ]]]
-        int main() {
-        
-          std::cout << "Python here !" << std::endl;
-          // <<[ impl ]>>  // Manually editable section named 'impl'
-          std::cout << "Modified by hand" << std::endl;
-          return 1;
-          // <<[ end ]>>   // End of section
-        
-        }
-        // [[[ end ]]]
-        ```
-        
-        When a new generation occurs, all previous sections are retrieved from the destination file and then reinserted into the new generation, inside each corresponding section with same name.
-        
-        All previous sections of a destination file must be reinserted when performing a new generation, otherwise it will be considered as code loss and generation will be aborted. Human intervention is required to deal with such scenarios.
-        
-        ## Integration in build pipelines
-        
-        **autojinja** generation mechanism can be integrated as a build step by listing all Python3 scripts that perform generation :
-        
-        ```shell
-        $ autojinja script1.py dir/script2.py ...
-        ```
-        
-        **autojinja** also provides discover mechanisms to find and execute the concerned Python3 scripts in listed directories :
-        
-        - `-r -f` recursively executes all Python3 scripts named `__jinja__.py`
-        
-            ```shell
-            $ autojinja -r -f .
-            ```
-        
-        - `-r -t` recursively executes all Python3 scripts whose first line contains `autojinja` keyword (can be for instance `import autojinja` or `from autojinja import *`)
-        
-            ```shell
-            $ autojinja -r -t .
-            ```
-        
-        - `-a` equivalent to `-r -f -t`
-        
-            ```shell
-            $ autojinja -a .
-            ```
-        
-        Centralized metadata files (such as XML or JSON files) can easily be accessed inside Python3 scripts using environment variables and environment files :
-        
-        ```shell
-        $ autojinja -a . -e FILE1=/tmp/file1.xml -e file.env
-        ```
-        
-        ## Links
-        - [Documentation](https://github.com/ldflo/autojinja/blob/main/docs/doc_autojinja.md)
-        - [Examples](https://github.com/ldflo/autojinja/blob/main/examples)
-        - [PyPI](https://pypi.org/project/autojinja)
-        - [Jinja2](https://github.com/pallets/jinja)
-        - [Cog](https://github.com/nedbat/cog)
-        
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Code Generators
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# autojinja
+
+**autojinja** is a Python3 module that allows generating code inside any file using [Jinja templates](https://github.com/pallets/jinja) in between comments. It aims to assist development workflows by using simple Python3 scripts that perform content generation of neighboring files, which enables generating code next to traditionally hand-made code efficiently.
+
+It includes :
+- Content generation in any file that accepts comments
+- Ability to maintain hand-made code inside generated code
+- Simple integration in build pipelines and existing codebases
+
+**autojinja** can be seen as a _preprocessor_ for most file formats, and works great with any codebase as it automates writing code manually. It shines out even more when working with metadata files (such as XML or JSON files) that centralize information which later needs to be generated across various scattered files in the codebase.
+
+## Installation
+
+```shell
+$ pip install autojinja
+```
+
+## Usage
+
+```shell
+$ autojinja script1.py script2.py
+```
+```shell
+$ autojinja -a .
+```
+
+## Content generation
+
+Content generation consists in generating parts of an existing file thanks to dedicated sections that delimit where the generation takes place. This technique is made possible for all files accepting comments, and allows defining [Jinja templates](https://github.com/pallets/jinja) directly in such files without breaking them.
+
+For example, let's suppose we have a C++ file we want to generate inside. To do this, we need to write our Jinja template between `[[[` and `]]]` markers, followed by an `[[[end]]]` marker :
+
+```cpp
+// main.cpp
+#include <iostream>
+
+int main() {
+  std::cout << "Hello world !" << std::endl;
+  // [[[ std::cout << "{{ value }}" << std::endl; ]]]  // Jinja template
+  // [[[ end ]]]                                       // Code will be generated in between
+  return 0;
+}
+```
+
+The template can then be generated with a Python3 script that provides the `value` variable :
+
+```python
+# main.py
+from autojinja import CogTemplate
+
+template = CogTemplate.from_file("main.cpp")
+template.context(value = "Python here !").render_file()
+```
+
+Calling the script will modify our C++ file as such :
+
+```cpp
+// main.cpp
+#include <iostream>
+
+int main() {
+  std::cout << "Hello world !" << std::endl;
+  // [[[ std::cout << "{{ value }}" << std::endl; ]]]  // Jinja template
+  std::cout << "Python here !" << std::endl;
+  // [[[ end ]]]                                       // Code will be generated in between
+  return 0;
+}
+```
+
+This technique is greatly inspired by [Cog](https://github.com/nedbat/cog), but adapted to work with Jinja templating engine. When performing generation again, the content inside the markers is entirely replaced by the new generation.
+
+## Hand-made modifications
+
+Modification by hand of generated code is made possible by using special sections that are preserved across new generations. To do this, we need to name a section between `<<[` and `]>>` markers, followed by an `<<[end]>>` marker :
+
+```cpp
+// main.cpp
+#include <iostream>
+
+// [[[
+// int main() {
+//
+//   std::cout << "{{ value }}" << std::endl;
+//   // <<[ impl ]>>  // Manually editable section named 'impl'
+//   return 0;
+//   // <<[ end ]>>   // End of section
+//
+// }
+// ]]]
+int main() {
+
+  std::cout << "Python here !" << std::endl;
+  // <<[ impl ]>>  // Manually editable section named 'impl'
+  std::cout << "Modified by hand" << std::endl;
+  return 1;
+  // <<[ end ]>>   // End of section
+
+}
+// [[[ end ]]]
+```
+
+When a new generation occurs, all previous sections are retrieved from the destination file and then reinserted into the new generation, inside each corresponding section with same name.
+
+All previous sections of a destination file must be reinserted when performing a new generation, otherwise it will be considered as code loss and generation will be aborted. Human intervention is required to deal with such scenarios.
+
+## Integration in build pipelines
+
+**autojinja** generation mechanism can be integrated as a build step by listing all Python3 scripts that perform generation :
+
+```shell
+$ autojinja script1.py dir/script2.py ...
+```
+
+**autojinja** also provides discover mechanisms to find and execute the concerned Python3 scripts in listed directories :
+
+- `-r -f` recursively executes all Python3 scripts named `__jinja__.py`
+
+    ```shell
+    $ autojinja -r -f .
+    ```
+
+- `-r -t` recursively executes all Python3 scripts whose first line contains `autojinja` keyword (can be for instance `import autojinja` or `from autojinja import *`)
+
+    ```shell
+    $ autojinja -r -t .
+    ```
+
+- `-a` equivalent to `-r -f -t`
+
+    ```shell
+    $ autojinja -a .
+    ```
+
+Centralized metadata files (such as XML or JSON files) can easily be accessed inside Python3 scripts using environment variables and environment files :
+
+```shell
+$ autojinja -a . -e FILE1=/tmp/file1.xml -e file.env
+```
+
+## Links
+- [Documentation](https://github.com/ldflo/autojinja/blob/main/docs/doc_autojinja.md)
+- [Examples](https://github.com/ldflo/autojinja/blob/main/examples)
+- [PyPI](https://pypi.org/project/autojinja)
+- [Jinja2](https://github.com/pallets/jinja)
+- [Cog](https://github.com/nedbat/cog)
```

### Comparing `autojinja-1.8.1/setup.py` & `autojinja-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 THIS_DIR = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(THIS_DIR, "README.md")) as file:
     README = file.read()
 
 setuptools.setup(
     name="autojinja",
-    version="1.8.1",
+    version="1.9.0",
     description="Content generation with Jinja templates in between comments",
     author="Florian Popek",
     author_email="florian.popek@gmail.com",
     url="https://github.com/ldflo/autojinja",
     license="BSD",
     long_description_content_type="text/markdown",
     long_description=README,
```

