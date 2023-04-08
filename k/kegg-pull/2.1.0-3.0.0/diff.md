# Comparing `tmp/kegg_pull-2.1.0.tar.gz` & `tmp/kegg_pull-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kegg_pull-2.1.0.tar", last modified: Wed Feb 15 03:23:41 2023, max compression
+gzip compressed data, was "kegg_pull-3.0.0.tar", last modified: Sat Apr  8 20:06:29 2023, max compression
```

## Comparing `kegg_pull-2.1.0.tar` & `kegg_pull-3.0.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 edhu227  (10152) mlab     (12795)        0 2023-02-15 03:23:41.734456 kegg_pull-2.1.0/
--rw-r--r--   0 edhu227  (10152) mlab     (12795)     1854 2022-09-20 22:01:38.000000 kegg_pull-2.1.0/LICENSE
--rw-r--r--   0 edhu227  (10152) mlab     (12795)     3217 2023-02-15 03:23:41.732456 kegg_pull-2.1.0/PKG-INFO
--rw-r--r--   0 edhu227  (10152) mlab     (12795)     2775 2023-02-12 00:52:33.000000 kegg_pull-2.1.0/README.rst
--rw-r--r--   0 edhu227  (10152) mlab     (12795)       38 2023-02-15 03:23:41.734456 kegg_pull-2.1.0/setup.cfg
--rw-r--r--   0 edhu227  (10152) mlab     (12795)     1185 2023-02-12 00:52:34.000000 kegg_pull-2.1.0/setup.py
-drwxr-xr-x   0 edhu227  (10152) mlab     (12795)        0 2023-02-15 03:23:41.569453 kegg_pull-2.1.0/src/
-drwxr-xr-x   0 edhu227  (10152) mlab     (12795)        0 2023-02-15 03:23:41.688455 kegg_pull-2.1.0/src/kegg_pull/
--rw-r--r--   0 edhu227  (10152) mlab     (12795)      120 2023-02-15 03:19:50.000000 kegg_pull-2.1.0/src/kegg_pull/__init__.py
--rw-r--r--   0 edhu227  (10152) mlab     (12795)     1293 2023-02-12 00:52:34.000000 kegg_pull-2.1.0/src/kegg_pull/__main__.py
--rw-r--r--   0 edhu227  (10152) mlab     (12795)     3646 2023-02-12 00:52:34.000000 kegg_pull-2.1.0/src/kegg_pull/_utils.py
--rw-r--r--   0 edhu227  (10152) mlab     (12795)     4993 2023-02-12 00:52:34.000000 kegg_pull-2.1.0/src/kegg_pull/entry_ids.py
--rw-r--r--   0 edhu227  (10152) mlab     (12795)     2844 2023-02-12 00:52:34.000000 kegg_pull-2.1.0/src/kegg_pull/entry_ids_cli.py
--rw-r--r--   0 edhu227  (10152) mlab     (12795)    33529 2023-02-12 00:52:34.000000 kegg_pull-2.1.0/src/kegg_pull/kegg_url.py
--rw-r--r--   0 edhu227  (10152) mlab     (12795)    23705 2023-02-12 00:52:34.000000 kegg_pull-2.1.0/src/kegg_pull/pull.py
--rw-r--r--   0 edhu227  (10152) mlab     (12795)     6090 2023-02-12 00:52:34.000000 kegg_pull-2.1.0/src/kegg_pull/pull_cli.py
--rw-r--r--   0 edhu227  (10152) mlab     (12795)    13128 2023-02-12 00:52:34.000000 kegg_pull-2.1.0/src/kegg_pull/rest.py
--rw-r--r--   0 edhu227  (10152) mlab     (12795)    11383 2023-02-12 00:52:34.000000 kegg_pull-2.1.0/src/kegg_pull/rest_cli.py
-drwxr-xr-x   0 edhu227  (10152) mlab     (12795)        0 2023-02-15 03:23:41.729456 kegg_pull-2.1.0/src/kegg_pull.egg-info/
--rw-r--r--   0 edhu227  (10152) mlab     (12795)     3217 2023-02-15 03:23:40.000000 kegg_pull-2.1.0/src/kegg_pull.egg-info/PKG-INFO
--rw-r--r--   0 edhu227  (10152) mlab     (12795)      507 2023-02-15 03:23:40.000000 kegg_pull-2.1.0/src/kegg_pull.egg-info/SOURCES.txt
--rw-r--r--   0 edhu227  (10152) mlab     (12795)        1 2023-02-15 03:23:40.000000 kegg_pull-2.1.0/src/kegg_pull.egg-info/dependency_links.txt
--rw-r--r--   0 edhu227  (10152) mlab     (12795)       55 2023-02-15 03:23:40.000000 kegg_pull-2.1.0/src/kegg_pull.egg-info/entry_points.txt
--rw-r--r--   0 edhu227  (10152) mlab     (12795)       21 2023-02-15 03:23:40.000000 kegg_pull-2.1.0/src/kegg_pull.egg-info/requires.txt
--rw-r--r--   0 edhu227  (10152) mlab     (12795)       10 2023-02-15 03:23:40.000000 kegg_pull-2.1.0/src/kegg_pull.egg-info/top_level.txt
+drwxr-xr-x   0 edhu227  (10152) mlab     (12795)        0 2023-04-08 20:06:29.417271 kegg_pull-3.0.0/
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)     1854 2022-09-20 22:01:38.000000 kegg_pull-3.0.0/LICENSE
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)     3232 2023-04-08 20:06:29.415270 kegg_pull-3.0.0/PKG-INFO
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)     2790 2023-03-17 18:41:05.000000 kegg_pull-3.0.0/README.rst
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)       38 2023-04-08 20:06:29.417271 kegg_pull-3.0.0/setup.cfg
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)     1173 2023-03-16 15:45:48.000000 kegg_pull-3.0.0/setup.py
+drwxr-xr-x   0 edhu227  (10152) mlab     (12795)        0 2023-04-08 20:06:29.147267 kegg_pull-3.0.0/src/
+drwxr-xr-x   0 edhu227  (10152) mlab     (12795)        0 2023-04-08 20:06:29.328269 kegg_pull-3.0.0/src/kegg_pull/
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)      128 2023-04-08 18:06:25.000000 kegg_pull-3.0.0/src/kegg_pull/__init__.py
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)     1589 2023-04-08 18:06:25.000000 kegg_pull-3.0.0/src/kegg_pull/__main__.py
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)     5459 2023-03-17 18:41:05.000000 kegg_pull-3.0.0/src/kegg_pull/_utils.py
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)     4833 2023-04-08 18:06:28.000000 kegg_pull-3.0.0/src/kegg_pull/entry_ids.py
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)     2754 2023-03-17 18:41:05.000000 kegg_pull-3.0.0/src/kegg_pull/entry_ids_cli.py
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)    32697 2023-03-17 18:41:05.000000 kegg_pull-3.0.0/src/kegg_pull/kegg_url.py
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)    20976 2023-04-08 18:06:28.000000 kegg_pull-3.0.0/src/kegg_pull/map.py
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)     4734 2023-03-23 18:41:04.000000 kegg_pull-3.0.0/src/kegg_pull/map_cli.py
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)    29198 2023-04-08 18:06:28.000000 kegg_pull-3.0.0/src/kegg_pull/pull.py
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)     6897 2023-03-20 22:33:09.000000 kegg_pull-3.0.0/src/kegg_pull/pull_cli.py
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)    14442 2023-04-08 18:06:28.000000 kegg_pull-3.0.0/src/kegg_pull/rest.py
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)     9923 2023-03-17 18:41:05.000000 kegg_pull-3.0.0/src/kegg_pull/rest_cli.py
+drwxr-xr-x   0 edhu227  (10152) mlab     (12795)        0 2023-04-08 20:06:29.412270 kegg_pull-3.0.0/src/kegg_pull.egg-info/
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)     3232 2023-04-08 20:06:28.000000 kegg_pull-3.0.0/src/kegg_pull.egg-info/PKG-INFO
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)      553 2023-04-08 20:06:29.000000 kegg_pull-3.0.0/src/kegg_pull.egg-info/SOURCES.txt
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)        1 2023-04-08 20:06:28.000000 kegg_pull-3.0.0/src/kegg_pull.egg-info/dependency_links.txt
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)       55 2023-04-08 20:06:28.000000 kegg_pull-3.0.0/src/kegg_pull.egg-info/entry_points.txt
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)       32 2023-04-08 20:06:29.000000 kegg_pull-3.0.0/src/kegg_pull.egg-info/requires.txt
+-rw-r--r--   0 edhu227  (10152) mlab     (12795)       10 2023-04-08 20:06:29.000000 kegg_pull-3.0.0/src/kegg_pull.egg-info/top_level.txt
```

### Comparing `kegg_pull-2.1.0/LICENSE` & `kegg_pull-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kegg_pull-2.1.0/PKG-INFO` & `kegg_pull-3.0.0/src/kegg_pull.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kegg_pull
-Version: 2.1.0
+Name: kegg-pull
+Version: 3.0.0
 Summary: Pulls any and all entries from any and all KEGG databases, pulls KEGG entry IDs, and wraps all the KEGG REST API operations in both Python API and the command line.
 Home-page: https://github.com/MoseleyBioinformaticsLab/KEGGpull
 Author: Erik Huckvale
 Author-email: edhu227@g.uky.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst
@@ -19,15 +19,15 @@
 
 Documentation
 -------------
 The complete documentation for our API and CLI including tutorials can be found `here <https://moseleybioinformaticslab.github.io/kegg_pull/>`__.
 
 Installation
 ------------
-Requires python 3.8 and above.
+Requires python 3.10 and above.
 
 Install on Linux, Mac OS X
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 .. parsed-literal::
    python3 -m pip install kegg-pull
 
 Install on Windows
@@ -56,14 +56,15 @@
 ------------
 Note, the ``pip`` command will install dependencies automatically.
 
 .. parsed-literal::
    docopt
    requests
    tqdm
+   jsonschema
 
 Get the source code
 -------------------
 Code is available on GitHub: https://github.com/MoseleyBioinformaticsLab/kegg_pull.
 
 You can clone the repository via:
```

### Comparing `kegg_pull-2.1.0/README.rst` & `kegg_pull-3.0.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Documentation
 -------------
 The complete documentation for our API and CLI including tutorials can be found `here <https://moseleybioinformaticslab.github.io/kegg_pull/>`__.
 
 Installation
 ------------
-Requires python 3.8 and above.
+Requires python 3.10 and above.
 
 Install on Linux, Mac OS X
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 .. parsed-literal::
    python3 -m pip install kegg-pull
 
 Install on Windows
@@ -44,14 +44,15 @@
 ------------
 Note, the ``pip`` command will install dependencies automatically.
 
 .. parsed-literal::
    docopt
    requests
    tqdm
+   jsonschema
 
 Get the source code
 -------------------
 Code is available on GitHub: https://github.com/MoseleyBioinformaticsLab/kegg_pull.
 
 You can clone the repository via:
```

### Comparing `kegg_pull-2.1.0/setup.py` & `kegg_pull-3.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import setuptools as st
 import re
 
 
 requirements = [
     'docopt',
     'requests',
-    'tqdm'
+    'tqdm',
+    'jsonschema'
 ]
 
 
 def _readme() -> str:
     with open('README.rst') as readme_file:
         return readme_file.read()
 
 
 def _get_version() -> str:
     with open('src/kegg_pull/__init__.py', 'r') as fd:
-        version: str = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
-                            fd.read(), re.MULTILINE).group(1)
+        version: str = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE).group(1)
     if not version:
         raise RuntimeError('Cannot find version information')
-
     return version
 
 
 st.setup(
     name='kegg_pull',
     version=_get_version(),
     package_dir={'': 'src'},
@@ -32,9 +31,8 @@
     install_requires=requirements,
     entry_points={'console_scripts': ['kegg_pull = kegg_pull.__main__:main']},
     author='Erik Huckvale',
     author_email='edhu227@g.uky.edu',
     url='https://github.com/MoseleyBioinformaticsLab/KEGGpull',
     description='Pulls any and all entries from any and all KEGG databases, pulls KEGG entry IDs, and wraps all the KEGG REST API operations in both Python API and the command line.',
     long_description_content_type='text/x-rst',
-    long_description=_readme()
-)
+    long_description=_readme())
```

### Comparing `kegg_pull-2.1.0/src/kegg_pull/__main__.py` & `kegg_pull-3.0.0/src/kegg_pull/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 """
 Usage:
-    kegg_pull -h | --help       Show this help message.
-    kegg_pull -v | --version    Displays the package version.
-    kegg_pull --full-help       Show the help message of all sub commands.
-    kegg_pull pull ...          Pull, separate, and store an arbitrary number of KEGG entries to the local file system.
-    kegg_pull entry-ids ...     Obtain a list of KEGG entry IDs.
-    kegg_pull rest ...          Executes one of the KEGG REST API operations.
+    kegg_pull -h | --help           Show this help message.
+    kegg_pull -v | --version        Displays the package version.
+    kegg_pull --full-help           Show the help message of all sub commands.
+    kegg_pull pull ...              Pull, separate, and store an arbitrary number of KEGG entries to the local file system.
+    kegg_pull entry-ids ...         Obtain a list of KEGG entry IDs.
+    kegg_pull map ...               Obtain a mapping of entry IDs (KEGG or outside databases) to the IDs of related entries.
+    kegg_pull rest ...              Executes one of the KEGG REST API operations.
 """
 import sys
-
 from . import __version__
 from . import pull_cli as p_cli
 from . import entry_ids_cli as ei_cli
+from . import map_cli as map_cli
 from . import rest_cli as r_cli
 
 
-def main():
+def main() -> None:
     first_arg: str = sys.argv[1] if len(sys.argv) > 1 else None
-
     if first_arg == 'pull':
         p_cli.main()
     elif first_arg == 'entry-ids':
         ei_cli.main()
+    elif first_arg == 'map':
+        map_cli.main()
     elif first_arg == 'rest':
         r_cli.main()
     elif first_arg == '--full-help':
         separator = '-'*80
         print(__doc__)
         print(separator)
         print(p_cli.__doc__)
         print(separator)
         print(ei_cli.__doc__)
         print(separator)
+        print(map_cli.__doc__)
+        print(separator)
         print(r_cli.__doc__)
     elif first_arg == '--version' or first_arg == '-v':
         print(__version__)
     else:
         print(__doc__)
```

### Comparing `kegg_pull-2.1.0/src/kegg_pull/entry_ids.py` & `kegg_pull-3.0.0/src/kegg_pull/entry_ids.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,110 +1,89 @@
 """
 Pulling Lists of KEGG Entry IDs
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Functionality for pulling lists of KEGG entry IDs from the KEGG REST API.
+|Functionality| for pulling lists of KEGG entry IDs from the KEGG REST API.
 """
-import typing as t
-
 from . import rest as r
+from . import kegg_url as ku
 
 
-def from_database(database_name: str, kegg_rest: r.KEGGrest = None) -> list:
+def from_database(database: str, kegg_rest: r.KEGGrest | None = None) -> list[str]:
     """ Pulls the KEGG entry IDs of a given database.
 
-    :param database_name: The KEGG database to pull the entry IDs from.
-    :param kegg_rest: Optional KEGGrest object. If None, one is created with the default parameters.
+    :param database: The KEGG database to pull the entry IDs from. If equal to "brite", the "br:" prefix is prepended to each entry ID such that they succeed if used in downstream use of the KEGG "get" operation (e.g. for the "pull" API module or CLI subcommand).
+    :param kegg_rest: The KEGGrest object to request the entry IDs. If None, one is created with the default parameters.
     :return: The list of resulting entry IDs.
     :raises RuntimeError: Raised if the request to the KEGG REST API fails or times out.
     """
-    return _process_response(method='list', kegg_rest=kegg_rest, database_name=database_name)
+    entry_ids = _process_response(KEGGurl=ku.ListKEGGurl, kegg_rest=kegg_rest, database=database)
+    if database == 'brite':
+        entry_ids = [f'br:{entry_id}' for entry_id in entry_ids if not entry_id.startswith('br:')]
+    return entry_ids
 
 
-def _process_response(method: str, kegg_rest: t.Union[r.KEGGrest, None], **kwargs) -> list:
-    """ Extracts the entry IDs from a KEGG response if successful, else raises an exception. The KEGG response arrives from calling
-    an entry IDs related method on a KEGGrest object.
+def _process_response(KEGGurl: type[ku.AbstractKEGGurl], kegg_rest: r.KEGGrest | None, **kwargs) -> list[str]:
+    """ Extracts the entry IDs from a KEGG response if successful, else raises an exception. The KEGG response arrives from making
+    an entry IDs related request with a KEGGrest object.
 
-    :param method: The method to call on the KEGGrest object.
-    :param kegg_rest: The KEGGrest object to call the method on. If None, one is created with the default parameters.
+    :param KEGGurl: The URL class for the request.
+    :param kegg_rest: The KEGGrest object to make the request with. If None, one is created with the default parameters.
     :param kwargs: The arguments to pass into the KEGGrest method.
     :return: The list of KEGG entry IDs.
     :raises RuntimeError: Raised if the KEGG response indicates a failure or time out.
     """
-    kegg_rest = kegg_rest if kegg_rest is not None else r.KEGGrest()
-    method: t.Callable = kegg_rest.__getattribute__(method)
-    kegg_response: r.KEGGresponse = method(**kwargs)
-
-    if kegg_response.status == r.KEGGresponse.Status.FAILED:
-        raise RuntimeError(
-            f'The KEGG request failed to pull the entry IDs from the following URL: {kegg_response.kegg_url.url}'
-        )
-    elif kegg_response.status == r.KEGGresponse.Status.TIMEOUT:
-        raise RuntimeError(
-            f'The KEGG request timed out while trying to pull the entry IDs from the following URL: '
-            f'{kegg_response.kegg_url.url}'
-        )
-
-    entry_ids: list = _parse_entry_ids_string(entry_ids_string=kegg_response.text_body)
-
-    return entry_ids
+    kegg_response: r.KEGGresponse = r.request_and_check_error(kegg_rest=kegg_rest, KEGGurl=KEGGurl, **kwargs)
+    return _parse_entry_ids_string(entry_ids_string=kegg_response.text_body)
 
 
-def _parse_entry_ids_string(entry_ids_string: str) -> list:
+def _parse_entry_ids_string(entry_ids_string: str) -> list[str]:
     """ Parses the entry IDs contained in a string.
 
     :param entry_ids_string: The string containing the entry IDs.
     :return: The list of parsed entry IDs.
     """
-    entry_ids: list = entry_ids_string.strip().split('\n')
-    entry_ids = [entry_id.split('\t')[0].strip() for entry_id in entry_ids if entry_id.strip() != '']
+    entry_ids = entry_ids_string.strip().split('\n')
+    return [entry_id.split('\t')[0].strip() for entry_id in entry_ids if entry_id.strip() != '']
 
-    return entry_ids
 
-
-def from_file(file_path: str) -> list:
+def from_file(file_path: str) -> list[str]:
     """ Loads KEGG entry IDs that are listed in a file with one entry ID on each line.
 
     :param file_path: The path to the file containing the entry IDs.
     :return: The list of entry IDs.
     :raises ValueError: Raised if the file is empty.
     """
     with open(file_path, 'r') as file:
-        entry_ids: str = file.read()
-
+        entry_ids = file.read()
         if entry_ids == '':
             raise ValueError(f'Attempted to load entry IDs from {file_path}. But the file is empty')
-
-        entry_ids: list = _parse_entry_ids_string(entry_ids_string=entry_ids)
-
-    return entry_ids
+        return _parse_entry_ids_string(entry_ids_string=entry_ids)
 
 
-def from_keywords(database_name: str, keywords: list, kegg_rest: r.KEGGrest = None) -> list:
+def from_keywords(database: str, keywords: list[str], kegg_rest: r.KEGGrest | None = None) -> list[str]:
     """ Pulls entry IDs from a KEGG database based on keywords searched in the entries.
 
-    :param database_name: The name of the database to pull entry IDs from.
+    :param database: The name of the database to pull entry IDs from.
     :param keywords: The keywords to search entries in the database with.
-    :param kegg_rest: Optional KEGGrest object. If None, one is created with the default parameters.
+    :param kegg_rest: The KEGGrest object to request the entry IDs. If None, one is created with the default parameters.
     :return: The list of entry IDs.
     :raises RuntimeError: Raised if the request to the KEGG REST API fails or times out.
     """
-    return _process_response(method='keywords_find', kegg_rest=kegg_rest, database_name=database_name, keywords=keywords)
+    return _process_response(KEGGurl=ku.KeywordsFindKEGGurl, kegg_rest=kegg_rest, database=database, keywords=keywords)
 
 
 def from_molecular_attribute(
-    database_name: str, formula: str = None, exact_mass: t.Union[float, tuple] = None, molecular_weight: t.Union[int, tuple] = None,
-    kegg_rest: r.KEGGrest = None
-) -> list:
+        database: str, formula: str | None = None, exact_mass: float | tuple[float, float] | None = None,
+        molecular_weight: int | tuple[int, int] | None = None, kegg_rest: r.KEGGrest | None = None) -> list[str]:
     """ Pulls entry IDs from a KEGG database containing chemical entries based on one (and only one) of three molecular attributes of the entries.
 
-    :param database_name: The name of the database containing chemical entries.
+    :param database: The name of the database containing chemical entries.
     :param formula: The chemical formula to search for.
     :param exact_mass: The exact mass of the compound to search for (a single value or a range).
     :param molecular_weight: The molecular weight of the compound to search for (a single value or a range).
-    :param kegg_rest: Optional KEGGrest object. If None, one is created with the default parameters.
+    :param kegg_rest: The KEGGrest object to request the entry IDs. If None, one is created with the default parameters.
     :return: The list of entry IDs.
     :raises RuntimeError: Raised if the request to the KEGG REST API fails or times out.
     """
     return _process_response(
-        method='molecular_find', kegg_rest=kegg_rest, database_name=database_name, formula=formula, exact_mass=exact_mass,
-        molecular_weight=molecular_weight
-    )
+        KEGGurl=ku.MolecularFindKEGGurl, kegg_rest=kegg_rest, database=database, formula=formula, exact_mass=exact_mass,
+        molecular_weight=molecular_weight)
```

### Comparing `kegg_pull-2.1.0/src/kegg_pull/entry_ids_cli.py` & `kegg_pull-3.0.0/src/kegg_pull/entry_ids_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 """
 Usage:
     kegg_pull entry-ids -h | --help
-    kegg_pull entry-ids database <database-name> [--output=<output>]
-    kegg_pull entry-ids keywords <database-name> <keywords> [--output=<output>]
-    kegg_pull entry-ids molecular-attribute <database-name> (--formula=<formula>|--em=<exact-mass>...|--mw=<molecular-weight>...) [--output=<output>]
+    kegg_pull entry-ids database <database> [--output=<output>]
+    kegg_pull entry-ids keywords <database> <keywords> [--output=<output>]
+    kegg_pull entry-ids molec-attr <database> (--formula=<formula>|--em=<exact-mass>...|--mw=<molecular-weight>...) [--output=<output>]
 
 Options:
     -h --help               Show this help message.
     database                Pulls all the entry IDs within a given database.
-    <database-name>         The KEGG database from which to pull a list of entry IDs.
+    <database>              The KEGG database from which to pull a list of entry IDs.
     --output=<output>       Path to the file (either in a directory or ZIP archive) to store the output (1 entry ID per line). Prints to the console if not specified. If a ZIP archive, the file path must be in the form of /path/to/zip-archive.zip:/path/to/file (e.g. ./archive.zip:file.txt).
     keywords                Searches for entries within a database based on provided keywords.
     <keywords>              Comma separated list of keywords to search entries with (e.g. kw1,kw2,kw3 etc.). Or if equal to "-", keywords are read from standard input, one keyword per line; Press CTRL+D to finalize input or pipe (e.g. cat file.txt | kegg_pull rest find brite - ...).
-    molecular-attribute     Searches a database of molecule-type KEGG entries by molecular attributes.
+    molec-attr              Searches a database of molecule-type KEGG entries by molecular attributes.
     --formula=<formula>     Sequence of atoms in a chemical formula format to search for (e.g. "O5C7" searches for molecule entries containing 5 oxygen atoms and/or 7 carbon atoms).
     --em=<exact-mass>       Either a single number (e.g. "--em=155.5") or two numbers (e.g. "--em=155.5 --em=244.4"). If a single number, searches for molecule entries with an exact mass equal to that value rounded by the last decimal point. If two numbers, searches for molecule entries with an exact mass within the two values (a range).
     --mw=<molecular-weight> Same as "--em=<exact-mass>" but searches based on the molecular weight.
 """
 import docopt as d
-
 from . import entry_ids as ei
 from . import _utils as u
 
 
-def main():
-    args: dict = d.docopt(__doc__)
-    database_name: str = args['<database-name>']
-
+def main() -> None:
+    args = d.docopt(__doc__)
+    database: str = args['<database>']
     if args['database']:
-        entry_ids: list = ei.from_database(database_name=database_name)
+        entry_ids = ei.from_database(database=database)
     elif args['keywords']:
-        keywords: list = u.handle_cli_input(input_source=args['<keywords>'])
-        entry_ids: list = ei.from_keywords(database_name=database_name, keywords=keywords)
+        keywords: list = u.parse_input_sequence(input_source=args['<keywords>'])
+        entry_ids = ei.from_keywords(database=database, keywords=keywords)
     else:
         formula, exact_mass, molecular_weight = u.get_molecular_attribute_args(args=args)
-
-        entry_ids: list = ei.from_molecular_attribute(
-            database_name=database_name, formula=formula, exact_mass=exact_mass, molecular_weight=molecular_weight
-        )
-
-    entry_ids: str = '\n'.join(entry_ids)
-    u.handle_cli_output(output_target=args['--output'], output_content=entry_ids)
+        entry_ids = ei.from_molecular_attribute(
+            database=database, formula=formula, exact_mass=exact_mass, molecular_weight=molecular_weight)
+    entry_ids_str = '\n'.join(entry_ids)
+    u.print_or_save(output_target=args['--output'], output_content=entry_ids_str)
```

### Comparing `kegg_pull-2.1.0/src/kegg_pull/kegg_url.py` & `kegg_pull-3.0.0/src/kegg_pull/kegg_url.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,87 +1,73 @@
 """
 Constructing URLs for the KEGG REST API
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Classes for creating and validating KEGG REST API URLs.
 """
 import requests as rq
-import logging as l
+import logging as log
 import abc
 import typing as t
-
 from . import _utils as u
 
-BASE_URL: str = 'https://rest.kegg.jp'
+BASE_URL = 'https://rest.kegg.jp'
 
 
 class AbstractKEGGurl(abc.ABC):
-    """Abstract class which validates and constructs URLs for accessing the KEGG REST API and contains the base data and functionality for all KEGG URL classes."""
-    _URL_LENGTH_LIMIT = 4000
+    """
+    Abstract class which validates and constructs URLs for accessing the KEGG REST API and contains the base data and functionality for all KEGG URL classes.
 
+    :ivar str url: The constructed and validated KEGG URL.
+    """
+    _URL_LENGTH_LIMIT = 4000
     _valid_kegg_databases = {
         'pathway', 'brite', 'module', 'ko', 'genome', 'vg', 'vp', 'ag', 'compound', 'glycan', 'reaction', 'rclass',
-        'enzyme', 'network', 'variant', 'disease', 'drug', 'dgroup', 'genes', 'ligand', 'kegg'
-    }
-
+        'enzyme', 'network', 'variant', 'disease', 'drug', 'dgroup', 'genes', 'ligand', 'kegg'}
     _valid_medicus_databases = {
-        'disease_ja', 'drug_ja', 'dgroup_ja', 'compound_ja', 'brite_ja', 'atc', 'jtc', 'ndc', 'yj'
-    }
-
-    _organism_set = None
+        'disease_ja', 'drug_ja', 'dgroup_ja', 'compound_ja', 'brite_ja', 'atc', 'jtc', 'ndc', 'yj'}
+    _organism_set: set[str] | None = None
 
     def __init__(self, rest_operation: str, base_url: str = BASE_URL, **kwargs) -> None:
         """
         :param rest_operation: The KEGG REST API operation in the URL.
         :param base_url: The base URL for accessing the KEGG web API.
         :param kwargs: The arguments used to construct the REST options after they are validated.
         :raises ValueError: Raised if the given arguments cannot construct a valid KEGG URL.
         """
         self._validate(**kwargs)
-        url_options: str = self._create_rest_options(**kwargs)
-        self._url = f'{base_url}/{rest_operation}/{url_options}'
-
-        if len(self._url) > AbstractKEGGurl._URL_LENGTH_LIMIT:
-           AbstractKEGGurl._raise_error(
-               reason=f'The KEGG URL length of {len(self._url)} exceeds the limit of {AbstractKEGGurl._URL_LENGTH_LIMIT}'
-           )
+        url_options = self._create_rest_options(**kwargs)
+        self.url = f'{base_url}/{rest_operation}/{url_options}'
+        if len(self.url) > AbstractKEGGurl._URL_LENGTH_LIMIT:
+            AbstractKEGGurl._raise_error(
+                reason=f'The KEGG URL length of {len(self.url)} exceeds the limit of {AbstractKEGGurl._URL_LENGTH_LIMIT}')
 
     # noinspection PyMethodParameters
     @u.staticproperty
-    def organism_set() -> set:
+    def organism_set() -> set[str]:
         """ Obtains the set of valid KEGG organism database names by requesting from the KEGG REST API (caches this result so the request only needs to be done once).
 
         :return: The set of organism database names.
         :raises RuntimeError: Raised in the unlikely case that the request fails.
         """
         if AbstractKEGGurl._organism_set is None:
             url = f'{BASE_URL}/list/organism'
             error_message = 'The request to the KEGG web API {} while fetching the organism set using the URL: {}'
-
             try:
-                response: rq.Response = rq.get(url=url, timeout=60)
+                response = rq.get(url=url, timeout=60)
             except rq.exceptions.Timeout:
-                raise RuntimeError(
-                    error_message.format('timed out', url)
-                )
-
-            status_code: int = response.status_code
-
+                raise RuntimeError(error_message.format('timed out', url))
+            status_code = response.status_code
             if status_code != 200:
-                raise RuntimeError(
-                    error_message.format(f'failed with status code {status_code}', url)
-                )
-
-            organism_list: list = response.text.strip().split('\n')
-            AbstractKEGGurl._organism_set = set()
-
+                raise RuntimeError(error_message.format(f'failed with status code {status_code}', url))
+            organism_list = response.text.strip().split('\n')
+            AbstractKEGGurl._organism_set = set[str]()
             for organism in organism_list:
                 [code, name, _, _] = organism.strip().split('\t')
                 AbstractKEGGurl._organism_set.add(code)
                 AbstractKEGGurl._organism_set.add(name)
-
         return AbstractKEGGurl._organism_set
 
     @abc.abstractmethod
     def _validate(self, **kwargs) -> None:
         """ Ensures the arguments passed into the constructor result in a valid KEGG URL.
 
         :param kwargs: The arguments to validate.
@@ -94,402 +80,342 @@
         """ Creates the string at the end part of a KEGG URL to specify the options for a REST API request.
 
         :param kwargs: The arguments used to create the options.
         :return: The REST API options.
         """
         pass  # pragma: no cover
 
-    @property
-    def url(self) -> str:
-        """The constructed and validated KEGG URL."""
-        return self._url
-
     def __repr__(self) -> str:
         return self.url
 
     @staticmethod
     def _raise_error(reason: str) -> None:
         """ Raises an exception for when a URL is not valid.
 
         :param reason: The reason why the URL was not valid.
         :raises ValueError: The error that is raised.
         """
         raise ValueError(f'Cannot create URL - {reason}')
 
     @staticmethod
-    def _validate_rest_option(
-        option_name: str, option_value: str, valid_rest_options: t.Iterable, add_org: bool = False
-    ) -> None:
+    def _validate_rest_option(option_name: str, option_value: str, valid_rest_options: t.Iterable[str], add_org: bool = False) -> None:
         """ Raises an exception if a provided REST API option is not valid.
 
         :param option_name: The name of the type of option to check.
         :param option_value: The value of the REST API option provided.
         :param valid_rest_options: The collection of valid options to choose from.
         :param add_org: Whether to add the "<org>" option to the valid options in the error message.
         :raises ValueError: Raised when the provided option is not valid.
         """
         if option_value not in valid_rest_options:
             if add_org:
-                valid_rest_options: set = set(valid_rest_options)
+                valid_rest_options = set(valid_rest_options)
                 valid_rest_options.add('<org>')
-
             valid_options = ', '.join(sorted(valid_rest_options))
             error_reason = f'Invalid {option_name}: "{option_value}". Valid values are: {valid_options}.'
-
             if add_org:
                 error_reason += ' Where <org> is an organism code or T number.'
-
             AbstractKEGGurl._raise_error(reason=error_reason)
 
     @staticmethod
-    def _validate_database_name(database_name: str, extra_databases: set = set(), excluded_databases: set = set()):
+    def _validate_database(database: str, extra_databases: set[str] = set[str](), excluded_databases: set[str] = set[str]()) -> None:
         """ Ensures the database provided is a valid KEGG database.
 
-        :param database_name: The name of the database to validate.
+        :param database: The name of the database to validate.
         :param extra_databases: Additional optional database names to add to the core KEGG databases for the validation.
         :param excluded_databases: Optional database names to exclude from the validation. If extra_databases overlaps
         excluded_databases, extra_databases has priority.
         :raises ValueError: Raised when the provided database is not valid.
         """
-        if database_name not in AbstractKEGGurl.organism_set:
+        if database not in AbstractKEGGurl.organism_set:
             valid_databases = AbstractKEGGurl._valid_kegg_databases.union(AbstractKEGGurl._valid_medicus_databases)
-            valid_databases: set = valid_databases - excluded_databases
-            valid_databases: set = valid_databases.union(extra_databases)
-
+            valid_databases = valid_databases - excluded_databases
+            valid_databases = valid_databases.union(extra_databases)
             AbstractKEGGurl._validate_rest_option(
-                option_name='database name', option_value=database_name, valid_rest_options=valid_databases,
-                add_org=True
-            )
+                option_name='database name', option_value=database, valid_rest_options=valid_databases, add_org=True)
 
 
 class ListKEGGurl(AbstractKEGGurl):
     """Contains URL construction and validation functionality of the KEGG API list operation."""
-
-    def __init__(self, database_name: str):
+    def __init__(self, database: str) -> None:
         """
-        :param database_name: The database option for the KEGG list URL.
+        :param database: The database option for the KEGG list URL.
         :raises ValueError: Raised if the provided database is not valid.
         """
-        super().__init__(rest_operation='list', database_name=database_name)
+        super().__init__(rest_operation='list', database=database)
 
-    def _validate(self, database_name: str):
+    def _validate(self, database: str) -> None:
         """ Ensures the database option is a KEGG database supported by the list operation.
 
-        :param database_name: The name of the database to check.
+        :param database: The name of the database to check.
         :raises ValueError: Raised if the provided database is not valid.
         """
-        AbstractKEGGurl._validate_database_name(
-            database_name=database_name, extra_databases={'organism'}, excluded_databases={'genes', 'ligand', 'kegg'}
-        )
+        AbstractKEGGurl._validate_database(
+            database=database, extra_databases={'organism'}, excluded_databases={'genes', 'ligand', 'kegg'})
 
-    def _create_rest_options(self, database_name: str) -> str:
+    def _create_rest_options(self, database: str) -> str:
         """ Implements the KEGG REST API options creation by returning the provided database name (the only option).
 
-        :param database_name: The database option to return.
+        :param database: The database option to return.
         :return: The database option.
         """
-        return database_name
+        return database
 
 
 class InfoKEGGurl(AbstractKEGGurl):
     """Contains URL construction and validation functionality of the KEGG API info operation."""
-
-    def __init__(self, database_name: str) -> None:
+    def __init__(self, database: str) -> None:
         """
-        :param database_name: The database option for the KEGG info URL.
+        :param database: The database option for the KEGG info URL.
         :raises ValueError: Raised if the provided database is not valid.
         """
-        super(InfoKEGGurl, self).__init__(rest_operation='info', database_name=database_name)
+        super(InfoKEGGurl, self).__init__(rest_operation='info', database=database)
 
-    def _validate(self, database_name: str):
+    def _validate(self, database: str) -> None:
         """ Ensures the database option is a KEGG database supported by the info operation.
 
-        :param database_name: The name of the database to check.
+        :param database: The name of the database to check.
         :raises ValueError: Raised if the provided database is not valid.
         """
-        AbstractKEGGurl._validate_database_name(
-            database_name=database_name, excluded_databases=AbstractKEGGurl._valid_medicus_databases
-        )
+        AbstractKEGGurl._validate_database(
+            database=database, excluded_databases=AbstractKEGGurl._valid_medicus_databases)
 
-    def _create_rest_options(self, database_name: str) -> str:
+    def _create_rest_options(self, database: str) -> str:
         """ Implements the KEGG REST API options creation by returning the provided database name (the only option).
 
-        :param database_name: The database option to return.
+        :param database: The database option to return.
         :return: The database option.
         """
-        return database_name
+        return database
 
 
 class GetKEGGurl(AbstractKEGGurl):
-    """Contains URL construction and validation functionality for the KEGG API get operation."""
+    """
+    Contains URL construction and validation functionality for the KEGG API get operation.
 
+    :cvar str MAX_ENTRY_IDS_PER_URL: The maximum number of entry IDs allowed in a single get KEGG URL.
+    :ivar list entry_ids: The entry IDs of the get KEGG URL.
+    """
     _entry_fields = {
         'aaseq': True, 'ntseq': True, 'mol': True, 'kcf': True, 'image': False, 'conf': False, 'kgml': False,
-        'json': False
-    }
-
-    _MAX_ENTRY_IDS_PER_URL = 10
-
-    # noinspection PyMethodParameters
-    @u.staticproperty
-    def MAX_ENTRY_IDS_PER_URL() -> int:
-        """ The maximum number of entry IDs allowed in a single get KEGG URL."""
-        return GetKEGGurl._MAX_ENTRY_IDS_PER_URL
+        'json': False}
+    MAX_ENTRY_IDS_PER_URL = 10
 
-    def __init__(self, entry_ids: list, entry_field: str = None) -> None:
+    def __init__(self, entry_ids: list[str], entry_field: str | None = None) -> None:
         """
         :param entry_ids: Specifies which entry IDs go in the first option of the URL.
         :param entry_field: Specifies which entry field goes in the second option.
         :raises ValueError: Raised if the entry IDs or entry field is not valid.
         """
         super().__init__(rest_operation='get', entry_ids=entry_ids, entry_field=entry_field)
-        self._entry_ids = entry_ids
+        self.entry_ids = entry_ids
         self._entry_field = entry_field
 
     @property
-    def entry_ids(self) -> list:
-        """The entry IDs of the get KEGG URL."""
-        return self._entry_ids
-
-    @property
     def multiple_entry_ids(self) -> bool:
         """Determines whether the get KEGG URL has more than one entry ID."""
         return len(self.entry_ids) > 1
 
-    def _validate(self, entry_ids: list, entry_field: str):
+    def _validate(self, entry_ids: list, entry_field: str | None) -> None:
         """ Ensures valid Entry IDs and a valid entry field are provided.
 
         :param entry_ids: The entry IDs to validate.
         :param entry_field: The entry field to validate.
         :raises ValueError: Raised if the entry IDs or entry field is not valid.
         """
-        n_entry_ids: int = len(entry_ids)
-
+        n_entry_ids = len(entry_ids)
         if n_entry_ids == 0:
             self._raise_error(reason='Entry IDs must be specified for the KEGG get operation')
-
-        max_entry_ids: int = GetKEGGurl._MAX_ENTRY_IDS_PER_URL
-
+        max_entry_ids = GetKEGGurl.MAX_ENTRY_IDS_PER_URL
         if n_entry_ids > max_entry_ids:
-            self._raise_error(
-                reason=f'The maximum number of entry IDs is {max_entry_ids} but {n_entry_ids} were provided'
-            )
-
+            self._raise_error(reason=f'The maximum number of entry IDs is {max_entry_ids} but {n_entry_ids} were provided')
         if entry_field is not None:
             AbstractKEGGurl._validate_rest_option(
-                option_name='KEGG entry field', option_value=entry_field, valid_rest_options=GetKEGGurl._entry_fields
-            )
-
+                option_name='KEGG entry field', option_value=entry_field, valid_rest_options=GetKEGGurl._entry_fields)
             if self.only_one_entry(entry_field=entry_field) and n_entry_ids > 1:
                 self._raise_error(
                     reason=f'The KEGG entry field: "{entry_field}" only supports requests of one KEGG entry '
-                           f'at a time but {n_entry_ids} entry IDs are provided'
-                )
+                           f'at a time but {n_entry_ids} entry IDs are provided')
 
     @staticmethod
-    def only_one_entry(entry_field: str) -> bool:
+    def only_one_entry(entry_field: str | None) -> bool:
         """ Determines whether a KEGG entry field can only be pulled in one entry at a time for the KEGG get API
         operation.
 
         :param entry_field: The KEGG entry field to check.
         """
         return entry_field is not None and not GetKEGGurl._entry_fields[entry_field]
 
     @staticmethod
-    def is_binary(entry_field: str) -> bool:
+    def is_binary(entry_field: str | None) -> bool:
         """ Determines if the entry field is a binary response or not.
 
         :param entry_field: The KEGG entry field to check.
         """
         return entry_field == 'image'
 
-    def _create_rest_options(self, entry_ids: list, entry_field: str) -> str:
+    def _create_rest_options(self, entry_ids: list[str], entry_field: str | None) -> str:
         """ Constructs the REST options for the KEGG API get operation.
 
         :param entry_ids: The entry IDs for the first REST option.
         :param entry_field: The entry field for the second REST option.
         :return: The constructed options.
         """
         entry_ids_url_option = '+'.join(entry_ids)
-
         if entry_field is not None:
             return f'{entry_ids_url_option}/{entry_field}'
         else:
             return entry_ids_url_option
 
 
 class KeywordsFindKEGGurl(AbstractKEGGurl):
     """Contains the URL construction and validation functionality for the KEGG API find operation based on the URL form that searches entries by keywords."""
-
-    def __init__(self, database_name: str, keywords: list):
+    def __init__(self, database: str, keywords: list[str]) -> None:
         """
-        :param database_name: The database name option for the first part of the URL.
+        :param database: The database name option for the first part of the URL.
         :param keywords: The keyword options for the second part of the URL.
         :raises ValueError: Raised if the database name is invalid or keywords are not provided.
         """
-        super(KeywordsFindKEGGurl, self).__init__(rest_operation='find', database_name=database_name, keywords=keywords)
+        super(KeywordsFindKEGGurl, self).__init__(rest_operation='find', database=database, keywords=keywords)
 
-    def _validate(self, database_name: str, keywords: list):
+    def _validate(self, database: str, keywords: list[str]) -> None:
         """ Ensures keywords are provided and the database name is valid.
 
-        :param database_name: The database name to check.
+        :param database: The database name to check.
         :param keywords: The keywords to check.
         :raises ValueError: Raised if the database name is invalid or keywords are not provided.
         """
         if len(keywords) == 0:
             self._raise_error(reason='No search keywords specified')
+        AbstractKEGGurl._validate_database(database=database, excluded_databases={'brite', 'kegg'})
 
-        AbstractKEGGurl._validate_database_name(database_name=database_name, excluded_databases={'brite', 'kegg'})
-
-    def _create_rest_options(self, keywords: list, database_name: str) -> str:
+    def _create_rest_options(self, keywords: list[str], database: str) -> str:
         """ Constructs the options for the URL using the database name followed by the keywords.
 
         :param keywords: The keywords to go in the options.
-        :param database_name: The database name to go in the options.
+        :param database: The database name to go in the options.
         :return: The constructed options.
         """
         keywords_string = '+'.join(keywords)
-
-        return f'{database_name}/{keywords_string}'
+        return f'{database}/{keywords_string}'
 
 
 class MolecularFindKEGGurl(AbstractKEGGurl):
     """Contains the URL construction and validation functionality for the KEGG API find operation based on the URL form that uses chemical / molecular attributes of compounds."""
-
     _valid_molecular_databases = {'compound', 'drug'}
 
-    def __init__(self, database_name: str, formula: str = None, exact_mass: t.Union[float, tuple] = None,
-        molecular_weight: t.Union[int, tuple] = None
-    ):
+    def __init__(
+            self, database: str, formula: str | None = None, exact_mass: float | tuple[float, float] | None = None,
+            molecular_weight: int | tuple[int, int] | None = None) -> None:
         """
-        :param database_name: The database name option for the first part of the URL.
+        :param database: The database name option for the first part of the URL.
         :param formula: The chemical formula option that can go in the second part of the URL.
         :param exact_mass: The exact molecule mass option that can go in the second part of the URL.
         :param molecular_weight: The molecular weight option that can go in the second part of the URL.
         :raises ValueError: Raised if the provided database name or molecular attribute is invalid.
         """
         super(MolecularFindKEGGurl, self).__init__(
-            rest_operation='find', database_name=database_name, formula=formula, exact_mass=exact_mass,
-            molecular_weight=molecular_weight
-        )
+            rest_operation='find', database=database, formula=formula, exact_mass=exact_mass, molecular_weight=molecular_weight)
 
     def _validate(
-        self, database_name: str, formula: str = None, exact_mass: t.Union[float, tuple] = None,
-        molecular_weight: t.Union[int, tuple] = None
-    ):
+            self, database: str, formula: str | None = None, exact_mass: float | tuple[float, float] | None = None,
+            molecular_weight: int | tuple[int, int] | None = None) -> None:
         """ Ensures a valid database name and molecular attributes are provided.
 
-        :param database_name: The database name to check.
+        :param database: The database name to check.
         :param formula: The chemical formula attribute to check.
         :param exact_mass: The exact mass attribute to check.
         :param molecular_weight: The molecular weight attribute to check.
         :raises ValueError: Raised if the provided database name or molecular attribute is invalid.
         """
         AbstractKEGGurl._validate_rest_option(
-            option_name='molecular database name', option_value=database_name,
-            valid_rest_options=MolecularFindKEGGurl._valid_molecular_databases
-        )
-
+            option_name='molecular database name', option_value=database,
+            valid_rest_options=MolecularFindKEGGurl._valid_molecular_databases)
         if formula is None and exact_mass is None and molecular_weight is None:
-            AbstractKEGGurl._raise_error(
-                reason='Must provide either a chemical formula, exact mass, or molecular weight option'
-            )
-
+            AbstractKEGGurl._raise_error(reason='Must provide either a chemical formula, exact mass, or molecular weight option')
         if formula is not None and (exact_mass is not None or molecular_weight is not None):
-            l.warning(
-                'Only a chemical formula, exact mass, or molecular weight is used to construct the URL. Using formula'
-                '...'
-            )
+            log.warning(
+                'Only a chemical formula, exact mass, or molecular weight is used to construct the URL. Using formula...')
         elif formula is None and exact_mass is not None and molecular_weight is not None:
-            l.warning('Both an exact mass and molecular weight are provided. Using exact mass...')
-
+            log.warning('Both an exact mass and molecular weight are provided. Using exact mass...')
         MolecularFindKEGGurl._validate_range(range_values=exact_mass, range_name='Exact mass')
         MolecularFindKEGGurl._validate_range(range_values=molecular_weight, range_name='Molecular weight')
 
     @staticmethod
-    def _validate_range(range_values: tuple, range_name: str):
+    def _validate_range(range_values: int | float | tuple[int, int] | tuple[float, float] | None, range_name: str) -> None:
         """ Ensures a given range is valid.
 
         :param range_values: The two end points of the range (start and end).
         :param range_name: The name of the range for the resulting error message in case of an invalid range.
         :raises ValueError: Raised if the range values are not valid.
         """
         if range_values is not None and type(range_values) is tuple:
             if len(range_values) != 2:
                 provided_values = ', '.join(str(range_value) for range_value in range_values)
-
                 AbstractKEGGurl._raise_error(
                     f'{range_name} range can only be constructed from 2 values but {len(range_values)} are provided: '
-                    f'{provided_values}'
-                )
-
+                    f'{provided_values}')
             min_val, max_val = range_values
-
             if not min_val < max_val:
                 AbstractKEGGurl._raise_error(
                     reason=f'The first value in the range must be less than the second. Values provided:'
-                           f' {min_val}-{max_val}'
-                )
+                           f' {min_val}-{max_val}')
 
-    def _create_rest_options(self, database_name: str, formula: str = None, exact_mass: t.Union[float, tuple] = None,
-        molecular_weight: t.Union[int, tuple] = None
-    ) -> str:
+    def _create_rest_options(
+            self, database: str, formula: str | None = None, exact_mass: float | tuple[float, float] | None = None,
+            molecular_weight: int | tuple[int, int] | None = None) -> str:
         """ Constructs the options for the URL using the database name followed by a molecular attribute.
 
-        :param database_name: The database name option in the first part of the URL.
+        :param database: The database name option in the first part of the URL.
         :param formula: The chemical formula option that can go in the second part of the URL.
         :param exact_mass: The exact mass attribute that can go in the second part of the URL.
         :param molecular_weight: The molecular weight attribute that can go in the second part of the URL.
         :return: The constructed options.
         """
         if formula is not None:
             options = f'{formula}/formula'
         elif exact_mass is not None:
             options = MolecularFindKEGGurl._get_range_options(option_name='exact_mass', option_value=exact_mass)
         else:
             options = MolecularFindKEGGurl._get_range_options(option_name='mol_weight', option_value=molecular_weight)
-
-        return f'{database_name}/{options}'
+        return f'{database}/{options}'
 
     @staticmethod
-    def _get_range_options(option_name: str, option_value: t.Union[float, int, tuple]) -> str:
+    def _get_range_options(option_name: str, option_value: float | int | tuple[int, int] | tuple[float, float]) -> str:
         """ Constructs options for the URL that are either a single number or a range (start and end separated by a
         dash).
 
         :param option_name: The name of the option to go in the third part of the URL.
         :param option_value: The single number or range.
         :return: The constructed option.
         """
         if type(option_value) is int or type(option_value) is float:
             options = option_value
         else:
             minimum, maximum = option_value
-
             options = f'{minimum}-{maximum}'
-
         return f'{options}/{option_name}'
 
 
 class AbstractConvKEGGurl(AbstractKEGGurl):
     """Abstract class containing data shared by the KEGG URL classes that validate and construct URLs for the conv KEGG
     REST API operation."""
-
     _valid_outside_gene_databases = {'ncbi-geneid', 'ncbi-proteinid', 'uniprot'}
     _valid_kegg_molecule_databases = {'compound', 'glycan', 'drug'}
     _valid_outside_molecule_databases = {'pubchem', 'chebi'}
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
         """
         :param kwargs: Arguments for the URL validation and construction.
         :raises ValueError: Raised if the provided arguments cannot construct a valid conv KEGG URL.
         """
         super(AbstractConvKEGGurl, self).__init__(rest_operation='conv', **kwargs)
 
     @abc.abstractmethod
-    def _validate(self, **kwargs):
+    def _validate(self, **kwargs) -> None:
         """ Validates options for a conv KEGG URL.
 
         :param kwargs: The options to validate.
         :raises ValueError: Raised if the provided arguments cannot construct a valid conv KEGG URL.
         """
         pass  # pragma: no cover
 
@@ -501,228 +427,198 @@
         :return: The constructed options.
         """
         pass  # pragma: no cover
 
 
 class DatabaseConvKEGGurl(AbstractConvKEGGurl):
     """Contains the URL construction and validation functionality of the KEGG API conv operation based on the URL form that uses a KEGG database and an outside database."""
-
-    def __init__(self, kegg_database_name: str, outside_database_name: str):
+    def __init__(self, kegg_database: str, outside_database: str) -> None:
         """
-        :param kegg_database_name: The name of the KEGG database.
-        :param outside_database_name: The name of the outside database.
+        :param kegg_database: The name of the KEGG database.
+        :param outside_database: The name of the outside database.
         :raises ValueError: Raised if the database names are not valid or are not of the same type.
         """
-        super(DatabaseConvKEGGurl, self).__init__(
-            kegg_database_name=kegg_database_name, outside_database_name=outside_database_name
-        )
+        super(DatabaseConvKEGGurl, self).__init__(kegg_database=kegg_database, outside_database=outside_database)
 
-    def _validate(self, kegg_database_name: str, outside_database_name: str):
+    def _validate(self, kegg_database: str, outside_database: str) -> None:
         """ Ensures that the database names are valid and that they're both the same type
 
-        :param kegg_database_name: The name of the KEGG database to check.
-        :param outside_database_name: The name of the outside database to check.
+        :param kegg_database: The name of the KEGG database to check.
+        :param outside_database: The name of the outside database to check.
         :raises ValueError: Raised if the database names are not valid or are not of the same type.
         """
-        valid_kegg_gene_databases: set = AbstractKEGGurl.organism_set
-        valid_kegg_molecule_databases: set = AbstractConvKEGGurl._valid_kegg_molecule_databases
-        valid_kegg_databases: set = valid_kegg_molecule_databases.union(valid_kegg_gene_databases)
-
-        if kegg_database_name not in valid_kegg_databases:
+        # noinspection PyTypeChecker
+        valid_kegg_gene_databases: set[str] = AbstractKEGGurl.organism_set
+        valid_kegg_molecule_databases = AbstractConvKEGGurl._valid_kegg_molecule_databases
+        valid_kegg_databases = valid_kegg_molecule_databases.union(valid_kegg_gene_databases)
+        if kegg_database not in valid_kegg_databases:
             AbstractKEGGurl._validate_rest_option(
-                option_name='KEGG database', option_value=kegg_database_name,
-                valid_rest_options=valid_kegg_molecule_databases, add_org=True
-            )
-
-        valid_outside_gene_databases: set = AbstractConvKEGGurl._valid_outside_gene_databases
-        valid_outside_molecule_databases: set = AbstractConvKEGGurl._valid_outside_molecule_databases
-        valid_outside_databases: set = valid_outside_molecule_databases.union(valid_outside_gene_databases)
-
+                option_name='KEGG database', option_value=kegg_database, valid_rest_options=valid_kegg_molecule_databases, add_org=True)
+        valid_outside_gene_databases = AbstractConvKEGGurl._valid_outside_gene_databases
+        valid_outside_molecule_databases = AbstractConvKEGGurl._valid_outside_molecule_databases
+        valid_outside_databases = valid_outside_molecule_databases.union(valid_outside_gene_databases)
         AbstractKEGGurl._validate_rest_option(
-            option_name='outside database', option_value=outside_database_name,
-            valid_rest_options=valid_outside_databases
-        )
-
-        if kegg_database_name in valid_kegg_gene_databases and \
-                outside_database_name not in valid_outside_gene_databases:
+            option_name='outside database', option_value=outside_database, valid_rest_options=valid_outside_databases)
+        if kegg_database in valid_kegg_gene_databases and outside_database not in valid_outside_gene_databases:
             AbstractKEGGurl._raise_error(
-                reason=f'KEGG database "{kegg_database_name}" is a gene database but outside database '
-                       f'"{outside_database_name}" is not.'
-            )
-
-        if kegg_database_name in valid_kegg_molecule_databases and \
-                outside_database_name not in valid_outside_molecule_databases:
+                reason=f'KEGG database "{kegg_database}" is a gene database but outside database '
+                       f'"{outside_database}" is not.')
+        if kegg_database in valid_kegg_molecule_databases and outside_database not in valid_outside_molecule_databases:
             AbstractKEGGurl._raise_error(
-                reason=f'KEGG database "{kegg_database_name}" is a molecule database but outside database '
-                       f'"{outside_database_name}" is not.'
-            )
+                reason=f'KEGG database "{kegg_database}" is a molecule database but outside database '
+                       f'"{outside_database}" is not.')
 
-    def _create_rest_options(self, kegg_database_name: str, outside_database_name: str) -> str:
+    def _create_rest_options(self, kegg_database: str, outside_database: str) -> str:
         """ Constructs the REST options by appending the outside database name to the kegg database name
 
-        :param kegg_database_name: The KEGG database option.
-        :param outside_database_name: The outside database option
+        :param kegg_database: The KEGG database option.
+        :param outside_database: The outside database option
         :return: The constructed options.
         """
-        return f'{kegg_database_name}/{outside_database_name}'
+        return f'{kegg_database}/{outside_database}'
 
 
 class EntriesConvKEGGurl(AbstractConvKEGGurl):
     """Contains the URL construction and validation functionality for the KEGG API conv operation based on the URL form that uses a target database and entry IDs."""
-
-    def __init__(self, target_database_name: str, entry_ids: list):
+    def __init__(self, target_database: str, entry_ids: list[str]) -> None:
         """
-        :param target_database_name: The target database option.
+        :param target_database: The target database option.
         :param entry_ids: The entry IDs options.
         :raises ValueError: Raised if the target database is invalid or entry IDs are not provided.
         """
-        super(EntriesConvKEGGurl, self).__init__(target_database_name=target_database_name, entry_ids=entry_ids)
+        super(EntriesConvKEGGurl, self).__init__(target_database=target_database, entry_ids=entry_ids)
 
-    def _validate(self, target_database_name: str, entry_ids: list):
+    def _validate(self, target_database: str, entry_ids: list[str]) -> None:
         """ Ensures the target database is valid and that the entry IDs are provided.
 
-        :param target_database_name: The name of the target database to check.
+        :param target_database: The name of the target database to check.
         :param entry_ids: The entry IDs to check.
         :raises ValueError: Raised if the target database is invalid or entry IDs are not provided.
         """
-        valid_databases: set = AbstractConvKEGGurl._valid_kegg_molecule_databases
-        valid_databases: set = valid_databases.union(AbstractConvKEGGurl._valid_outside_gene_databases)
-        valid_databases: set = valid_databases.union(AbstractConvKEGGurl._valid_outside_molecule_databases)
+        valid_databases = AbstractConvKEGGurl._valid_kegg_molecule_databases
+        valid_databases = valid_databases.union(AbstractConvKEGGurl._valid_outside_gene_databases)
+        valid_databases = valid_databases.union(AbstractConvKEGGurl._valid_outside_molecule_databases)
         valid_databases.add('genes')
-
-        if target_database_name not in valid_databases.union(AbstractKEGGurl.organism_set):
+        # noinspection PyTypeChecker
+        if target_database not in valid_databases.union(AbstractKEGGurl.organism_set):
             AbstractKEGGurl._validate_rest_option(
-                option_name='target database', option_value=target_database_name, valid_rest_options=valid_databases,
-                add_org=True
-            )
-
+                option_name='target database', option_value=target_database, valid_rest_options=valid_databases, add_org=True)
         if len(entry_ids) == 0:
             self._raise_error(reason='Entry IDs must be specified for this KEGG "conv" operation')
 
-    def _create_rest_options(self, target_database_name: str, entry_ids: list) -> str:
+    def _create_rest_options(self, target_database: str, entry_ids: list) -> str:
         """ Constructs the REST options by appending the entry IDs (separated by '+') to the target database name.
 
-        :param target_database_name: The name of the target database in the first part of the URL.
+        :param target_database: The name of the target database in the first part of the URL.
         :param entry_ids: The entry IDs in the second part of the URL.
         :return: The constructed options.
         """
-        return f'{target_database_name}/{"+".join(entry_ids)}'
+        return f'{target_database}/{"+".join(entry_ids)}'
 
 
 class AbstractLinkKEGGurl(AbstractKEGGurl):
     """Abstract class containing the shared data for the link KEGG URLs."""
+    _extra_databases = {'atc', 'jtc', 'ndc', 'yj', 'pubmed'}
 
-    _extra_database_names = {'atc', 'jtc', 'ndc', 'yj', 'pubmed'}
-
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
         """
         :param kwargs: The arguments to validate and construct the URL.
         :raises ValueError: Raised if the provided arguments are invalid.
         """
         super(AbstractLinkKEGGurl, self).__init__(rest_operation='link', **kwargs)
 
     @abc.abstractmethod
-    def _validate(self, **kwargs):
+    def _validate(self, **kwargs) -> None:
         pass  # pragma: no cover
 
     @abc.abstractmethod
     def _create_rest_options(self, **kwargs) -> str:
         pass  # pragma: no cover
 
 
 class DatabaseLinkKEGGurl(AbstractLinkKEGGurl):
     """Contains the URL construction and validation functionality for the link KEGG REST API operation of the form that uses a target database and a source database."""
 
-    def __init__(self, target_database_name: str, source_database_name: str):
+    def __init__(self, target_database: str, source_database: str) -> None:
         """
-        :param target_database_name: The name of the target database option.
-        :param source_database_name: The name of the source database option.
+        :param target_database: The name of the target database option.
+        :param source_database: The name of the source database option.
         :raises ValueError: Raised if the databases are invalid.
         """
-        super(DatabaseLinkKEGGurl, self).__init__(
-            target_database_name=target_database_name, source_database_name=source_database_name
-        )
+        super(DatabaseLinkKEGGurl, self).__init__(target_database=target_database, source_database=source_database)
 
-    def _validate(self, target_database_name: str, source_database_name: str):
+    def _validate(self, target_database: str, source_database: str) -> None:
         """ Ensures the provided databases are valid
 
-        :param target_database_name: The name of the target database to check.
-        :param source_database_name: The name of the source database to check.
+        :param target_database: The name of the target database to check.
+        :param source_database: The name of the source database to check.
         :raises ValueError: Raised if the databases are invalid.
         """
-        excluded_databases: set = AbstractKEGGurl._valid_medicus_databases.union({'kegg', 'genes', 'ligand'})
-
-        AbstractKEGGurl._validate_database_name(
-            database_name=target_database_name, extra_databases=AbstractLinkKEGGurl._extra_database_names,
-            excluded_databases=excluded_databases
-        )
-
-        AbstractKEGGurl._validate_database_name(
-            database_name=source_database_name, extra_databases=AbstractLinkKEGGurl._extra_database_names,
-            excluded_databases=excluded_databases
-        )
+        if target_database == source_database:
+            AbstractKEGGurl._raise_error(
+                reason=f'The source and target database cannot be identical. Database selected: {source_database}.')
+        excluded_databases = AbstractKEGGurl._valid_medicus_databases.union({'kegg', 'genes', 'ligand'})
+        AbstractKEGGurl._validate_database(
+            database=target_database, extra_databases=AbstractLinkKEGGurl._extra_databases, excluded_databases=excluded_databases)
+        AbstractKEGGurl._validate_database(
+            database=source_database, extra_databases=AbstractLinkKEGGurl._extra_databases, excluded_databases=excluded_databases)
 
-    def _create_rest_options(self, target_database_name: str, source_database_name: str) -> str:
+    def _create_rest_options(self, target_database: str, source_database: str) -> str:
         """ Constructs the options by appending the target database name to the source database name
-        :param target_database_name: The target database name for the first option.
-        :param source_database_name: The source database name for the second option.
+
+        :param target_database: The target database name for the first option.
+        :param source_database: The source database name for the second option.
         :return: The constructed options.
         """
-        return f'{target_database_name}/{source_database_name}'
+        return f'{target_database}/{source_database}'
 
 
 class EntriesLinkKEGGurl(AbstractLinkKEGGurl):
     """Contains the URL construction and validation functionality for the link KEGG REST API operation of the form that uses a target database and entry IDs."""
-
-    def __init__(self, target_database_name: str, entry_ids: list):
+    def __init__(self, target_database: str, entry_ids: list[str]) -> None:
         """
-        :param target_database_name: The name of the target database option.
+        :param target_database: The name of the target database option.
         :param entry_ids: The entry IDs options.
         :raises ValueError: Raised if the target database is invalid or entry IDs are not provided.
         """
-        super(EntriesLinkKEGGurl, self).__init__(target_database_name=target_database_name, entry_ids=entry_ids)
+        super(EntriesLinkKEGGurl, self).__init__(target_database=target_database, entry_ids=entry_ids)
 
-    def _validate(self, target_database_name: str, entry_ids: list):
+    def _validate(self, target_database: str, entry_ids: list[str]) -> None:
         """ Ensures the target database name is valid and that the entry IDs are provided.
 
-        :param target_database_name: The name of the target database to check.
+        :param target_database: The name of the target database to check.
         :param entry_ids: The entry IDs to check.
         :raises ValueError: Raised if the target database is invalid or entry IDs are not provided.
         """
         excluded_databases: set = AbstractKEGGurl._valid_medicus_databases.union({'kegg', 'ligand'})
-
-        AbstractKEGGurl._validate_database_name(
-            database_name=target_database_name, extra_databases=AbstractLinkKEGGurl._extra_database_names,
-            excluded_databases=excluded_databases
-        )
-
+        AbstractKEGGurl._validate_database(
+            database=target_database, extra_databases=AbstractLinkKEGGurl._extra_databases, excluded_databases=excluded_databases)
         if len(entry_ids) == 0:
             AbstractKEGGurl._raise_error(reason='At least one entry ID must be specified to perform the link operation')
 
-    def _create_rest_options(self, target_database_name: str, entry_ids: list) -> str:
+    def _create_rest_options(self, target_database: str, entry_ids: list[str]) -> str:
         """Constructs the options by appending the entry IDs (separated by '+') to the target database name.
 
-        :param target_database_name: The name of the target database for the first options.
+        :param target_database: The name of the target database for the first options.
         :param entry_ids: The entry IDs as the last options.
         :return: The constructed options.
         """
-        return f'{target_database_name}/{"+".join(entry_ids)}'
+        return f'{target_database}/{"+".join(entry_ids)}'
 
 
 class DdiKEGGurl(AbstractKEGGurl):
     """Contains the URL construction and validation functionality for the ddi KEGG REST operation."""
-
-    def __init__(self, drug_entry_ids: list):
+    def __init__(self, drug_entry_ids: list[str]) -> None:
         """
         :param drug_entry_ids: The entry IDs for a drug database.
         :raises ValueError: Raised if the drug entry IDs are not provided.
         """
         super(DdiKEGGurl, self).__init__(rest_operation='ddi', drug_entry_ids=drug_entry_ids)
 
-    def _validate(self, drug_entry_ids: list):
+    def _validate(self, drug_entry_ids: list) -> None:
         """ Ensures the drug entry IDs are provided.
 
         :param drug_entry_ids: The drug entry IDs to check.
         :raises ValueError: Raised if the drug entry IDs are not provided.
         """
         if len(drug_entry_ids) == 0:
             AbstractKEGGurl._raise_error(reason='At least one drug entry ID must be specified for the DDI operation')
```

### Comparing `kegg_pull-2.1.0/src/kegg_pull/pull.py` & `kegg_pull-3.0.0/src/kegg_pull/pull.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,499 +1,525 @@
 """
 Pulling, Parsing, and Saving KEGG Entries
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Functionality for pulling KEGG entries from the KEGG REST API, parsing them, and saving the entries as files.
+|Functionality| for pulling KEGG entries from the KEGG REST API, parsing them, and saving the entries as files.
 """
 import multiprocessing as mp
 import os
 import abc
 import typing as t
 import pickle as p
-import logging as l
-import json as j
+import logging as log
+import json
 import tqdm
-
 from . import kegg_url as ku
 from . import rest as r
 from . import _utils as u
 
+KEGGentryMapping = dict[str, str | bytes]
 
-class PullResult:
-    """The collections of entry IDs, each of which resulted in a particular KEGG Response status after a pull."""
 
+class PullResult(u.NonInstantiable):
+    """The collections of entry IDs, each of which resulted in a particular KEGG Response status after a pull."""
     def __init__(self) -> None:
-        self._successful_entry_ids = []
-        self._failed_entry_ids = []
-        self._timed_out_entry_ids = []
+        super(PullResult, self).__init__()
+        self._successful_entry_ids = list[str]()
+        self._failed_entry_ids = list[str]()
+        self._timed_out_entry_ids = list[str]()
 
-    def __repr__(self):
-        def get_entry_ids_repr(entry_ids) -> str:
+    def __repr__(self) -> str:
+        def get_entry_ids_repr(entry_ids: tuple[str, ...]) -> str:
             return ', '.join(entry_ids) if len(entry_ids) > 0 else 'none'
-
-        successful_entry_ids: str = get_entry_ids_repr(entry_ids=self.successful_entry_ids)
-        failed_entry_ids: str = get_entry_ids_repr(entry_ids=self.failed_entry_ids)
-        timed_out_entry_ids: str = get_entry_ids_repr(entry_ids=self.timed_out_entry_ids)
-
+        successful_entry_ids = get_entry_ids_repr(entry_ids=self.successful_entry_ids)
+        failed_entry_ids = get_entry_ids_repr(entry_ids=self.failed_entry_ids)
+        timed_out_entry_ids = get_entry_ids_repr(entry_ids=self.timed_out_entry_ids)
         return f'Successful Entry Ids: {successful_entry_ids}\n' \
                f'Failed Entry Ids: {failed_entry_ids}\n' \
                f'Timed Out Entry Ids: {timed_out_entry_ids}'
 
     @property
-    def successful_entry_ids(self) -> tuple:
+    def successful_entry_ids(self) -> tuple[str, ...]:
         """The IDs of entries successfully pulled."""
         return tuple(self._successful_entry_ids)
 
     @property
-    def failed_entry_ids(self) -> tuple:
+    def failed_entry_ids(self) -> tuple[str, ...]:
         """The IDs of entries that failed to be pulled."""
         return tuple(self._failed_entry_ids)
 
     @property
-    def timed_out_entry_ids(self) -> tuple:
+    def timed_out_entry_ids(self) -> tuple[str, ...]:
         """The IDs of entries that timed out before being pulled."""
         return tuple(self._timed_out_entry_ids)
 
-    def add_entry_ids(self, *entry_ids, status: r.KEGGresponse.Status) -> None:
+    def _add_entry_ids(self, *entry_ids, status: r.KEGGresponse.Status) -> None:
         """ Adds entry IDs of a given status to the pull result.
 
         :param entry_ids: The entry IDs to add.
         :param status: The status resulting from attempting to pull the entries of the given IDs.
         """
         if status == r.KEGGresponse.Status.SUCCESS:
             self._successful_entry_ids.extend(entry_ids)
         elif status == r.KEGGresponse.Status.FAILED:
             self._failed_entry_ids.extend(entry_ids)
         else:
             self._timed_out_entry_ids.extend(entry_ids)
 
-    def merge_pull_results(self, other) -> int:
+    def _merge_pull_results(self, other) -> int:
         """ Combines two pull results into one.
 
         :param other: The pull result to combine into this one.
         :return: The number of entry IDs added.
         """
         self._successful_entry_ids.extend(other.successful_entry_ids)
         self._failed_entry_ids.extend(other.failed_entry_ids)
         self._timed_out_entry_ids.extend(other.timed_out_entry_ids)
-
-        n_entry_ids_processed: int = len(other.successful_entry_ids)
+        n_entry_ids_processed = len(other.successful_entry_ids)
         n_entry_ids_processed += len(other.failed_entry_ids)
         n_entry_ids_processed += len(other.timed_out_entry_ids)
-
         return n_entry_ids_processed
 
 
 class SinglePull:
     """Class capable of performing a single request to the KEGG REST API for pulling up to a maximum number of entries."""
-    def __init__(
-        self, output: str, kegg_rest: r.KEGGrest = None, entry_field: str = None, multiprocess_lock_save: bool = False
-    ) -> None:
+    def __init__(self, kegg_rest: r.KEGGrest | None = None, multiprocess_lock_save: bool = False) -> None:
         """
-        :param output: Path to the location where entries are saved (treated like a ZIP file if ends in ".zip", else a directory).
         :param kegg_rest: Optional KEGGrest object used to make the requests to the KEGG REST API (a KEGGrest object with the default settings is created if one is not provided).
-        :param entry_field: Optional KEGG entry field to pull.
-        :param multiprocess_lock_save: Whether to block the code that saves KEGG entries in order to be multiprocess safe. Should not be needed unless saving entries to a ZIP archive across multiple processes.
+        :param multiprocess_lock_save: Whether to block the code that saves KEGG entries in order to be multiprocess safe. Should not be needed unless pulling across multiple processes.
         """
-        self._output = output
-
-        if not output.endswith('.zip') and not os.path.isdir(output):
-                os.makedirs(output)
-
+        self._output = None
         self._kegg_rest = kegg_rest if kegg_rest is not None else r.KEGGrest()
-        self.entry_field = entry_field
+        self._entry_field = None
         self._multiprocess_lock = mp.Lock() if multiprocess_lock_save else None
+        self._in_memory_entries = None
 
-    def pull(self, entry_ids: list) -> PullResult:
+    def pull(self, entry_ids: list[str], output: str, entry_field: str | None = None) -> PullResult:
         """ Makes a single request to the KEGG REST API to pull one or more entries and save them as files.
 
         :param entry_ids: The IDs of the entries to pull and save.
+        :param output: Path to the location where entries are saved. Treated like a ZIP file if ends in ".zip", else a directory. If a directory, the directory is created if it doesn't already exist.
+        :param entry_field: An optional field of the entries to pull.
         :return: The pull result.
         """
-        kegg_response: r.KEGGresponse = self._kegg_rest.get(entry_ids=entry_ids, entry_field=self.entry_field)
+        if output is None:
+            raise ValueError('"output" cannot be None')
+        return self._pull(entry_ids=entry_ids, entry_field=entry_field, output=output)
+
+    def pull_dict(self, entry_ids: list[str], entry_field: str | None = None) -> tuple[PullResult, KEGGentryMapping]:
+        """ Rather than saving the KEGG entries to the file system, stores them in-memory as a mapping from the ID to the corresponding entry.
+
+        :param entry_ids: The IDs of the entries to pull and include in the mapping.
+        :param entry_field: An optional field of the entries to pull.
+        :return: The pull result and the mapping from entry IDs to KEGG entries as strings (or bytes if the entries are in binary format).
+        """
+        self._in_memory_entries = KEGGentryMapping()
+        pull_result = self._pull(entry_ids=entry_ids, output=None, entry_field=entry_field)
+        tmp = self._in_memory_entries
+        self._in_memory_entries = None
+        return pull_result, tmp
+
+    def _pull(self, entry_ids: list[str], output: str | None, entry_field: str | None) -> PullResult:
+        """ Generic pull helper function that saves to the file system if output is provided, otherwise saves entries in-memory.
+
+        :param entry_ids: The IDs of the entries to pull.
+        :param output: If set, saves to the file system location specified. Otherwise, stores in-memory.
+        :param entry_field: Optional KEGG entry field to pull.
+        :return: The pull result.
+        """
+        self._entry_field = entry_field
+        self._output = output
+        kegg_response: r.KEGGresponse = self._kegg_rest.get(entry_ids=entry_ids, entry_field=self._entry_field)
+        # noinspection PyTypeChecker
         get_url: ku.GetKEGGurl = kegg_response.kegg_url
         pull_result = PullResult()
-
         if kegg_response.status == r.KEGGresponse.Status.SUCCESS:
             if get_url.multiple_entry_ids:
                 self._save_multi_entry_response(kegg_response=kegg_response, pull_result=pull_result)
             else:
                 self._save_single_entry_response(kegg_response=kegg_response, pull_result=pull_result)
         else:
             self._handle_unsuccessful_url(kegg_response=kegg_response, pull_result=pull_result)
-
         return pull_result
 
     def _save_multi_entry_response(self, kegg_response: r.KEGGresponse, pull_result: PullResult) -> None:
         """ Saves multiple entries within a KEGG response.
 
         :param kegg_response: The response from KEGG with multiple entries.
         :param pull_result: The pull result to update based on the status of the pull(s).
         """
-        entries: list = self._separate_entries(concatenated_entries=kegg_response.text_body)
+        entries = self._separate_entries(concatenated_entries=kegg_response.text_body)
+        # noinspection PyTypeChecker
         get_url: ku.GetKEGGurl = kegg_response.kegg_url
-
         if len(entries) < len(get_url.entry_ids):
             # If we did not get all the entries requested, process each entry one at a time
             self._pull_separate_entries(get_url=get_url, pull_result=pull_result)
         else:
-            pull_result.add_entry_ids(*get_url.entry_ids, status=r.KEGGresponse.Status.SUCCESS)
+            # noinspection PyProtectedMember
+            pull_result._add_entry_ids(*get_url.entry_ids, status=r.KEGGresponse.Status.SUCCESS)
 
             for entry_id, entry in zip(get_url.entry_ids, entries):
-                self._save(entry_id=entry_id, entry=entry, entry_field=self.entry_field)
+                self._save(entry_id=entry_id, entry=entry, entry_field=self._entry_field)
 
     def _separate_entries(self, concatenated_entries: str) -> list:
         """ Separates the entries in a multi-entry response from KEGG.
 
         :param concatenated_entries: The response body with all the entries together.
         :return: The separated KEGG entries.
         """
         field_to_separator = {
             'aaseq': SinglePull._gene_separator, 'kcf': SinglePull._standard_separator,
-            'mol': SinglePull._mol_separator, 'ntseq': SinglePull._gene_separator
-        }
-
-        if self.entry_field is None:
-            separator = SinglePull._standard_separator
+            'mol': SinglePull._mol_separator, 'ntseq': SinglePull._gene_separator}
+        if self._entry_field is None:
+            separator: t.Callable[[str], list[str]] = SinglePull._standard_separator
         else:
-            separator = field_to_separator[self.entry_field]
-
-        entries: list = separator(concatenated_entries=concatenated_entries)
-        entries = [entry.strip() for entry in entries]
-
+            separator = field_to_separator[self._entry_field]
+        entries = separator(concatenated_entries=concatenated_entries)
+        entries = [entry for entry in entries]
         return entries
 
     @staticmethod
-    def _gene_separator(concatenated_entries: str) -> list:
+    def _gene_separator(concatenated_entries: str) -> list[str]:
         """ Separates KEGG entries that are separated by a deliminator for nucleotide and amino acid sequence entries.
         :param concatenated_entries: The response body with the gene-related entries together.
         :return: The separated gene-related entries.
         """
-        entries: list = concatenated_entries.split('>')
-
+        entries = concatenated_entries.split('>')
         if len(entries) > 1:
             return entries[1:]
         else:
             return entries
 
     @staticmethod
-    def _mol_separator(concatenated_entries: str) -> list:
+    def _mol_separator(concatenated_entries: str) -> list[str]:
         """ Separates mol entries.
 
         :param concatenated_entries: The response body with the mol entries together.
         :return: The separated mole entries.
         """
         return SinglePull._split_and_remove_last(concatenated_entries=concatenated_entries, deliminator='$$$$')
 
     @staticmethod
-    def _split_and_remove_last(concatenated_entries: str, deliminator: str) -> list:
+    def _split_and_remove_last(concatenated_entries: str, deliminator: str) -> list[str]:
         """ Splits entries based on a deliminator and removes the resulting empty string at the end of the list.
 
         :param concatenated_entries: The response body with the entries together.
         :param deliminator: The deliminator that separates the entries and is at the end of the response body.
         :return: The separated entries with the empty string removed.
         """
-        entries: list = concatenated_entries.split(deliminator)
-
+        entries = concatenated_entries.split(deliminator)
         if len(entries) > 1:
             return entries[:-1]
         else:
             return entries
 
     @staticmethod
-    def _standard_separator(concatenated_entries: str) -> list:
+    def _standard_separator(concatenated_entries: str) -> list[str]:
         """ The separation method for most types of KEGG entries.
 
         :param concatenated_entries: The response body with the KEGG entries together.
         :return: The separated entries.
         """
         return SinglePull._split_and_remove_last(concatenated_entries=concatenated_entries, deliminator='///')
 
     def _pull_separate_entries(self, get_url: ku.GetKEGGurl, pull_result: PullResult) -> None:
         """ Pulls one entry at a time for a Get KEGG URL that has multiple entry IDs.
 
         :param get_url: The Get KEGG URL with multiple entry IDs to pull one at a time.
         :param pull_result: The pull result to update based on the success of the pulling.
         """
         for entry_id in get_url.entry_ids:
-            kegg_response: r.KEGGresponse = self._kegg_rest.get(entry_ids=[entry_id], entry_field=self.entry_field)
-
+            kegg_response = self._kegg_rest.get(entry_ids=[entry_id], entry_field=self._entry_field)
             if kegg_response.status == r.KEGGresponse.Status.SUCCESS:
                 self._save_single_entry_response(kegg_response=kegg_response, pull_result=pull_result)
             else:
-                pull_result.add_entry_ids(entry_id, status=kegg_response.status)
+                # noinspection PyProtectedMember
+                pull_result._add_entry_ids(entry_id, status=kegg_response.status)
 
-    def _save(self, entry_id: str, entry: t.Union[str, bytes], entry_field: str) -> None:
+    def _save(self, entry_id: str, entry: str | bytes, entry_field: str | None) -> None:
         """ Saves a KEGG entry as a file.
 
         :param entry_id: The entry ID (part of the file name).
         :param entry: The entry to save (contents of the file).
         :param entry_field: The particular field of the entry (file extension). If None, the file extension is ".txt" by default.
         """
-        file_extension = 'txt' if entry_field is None else entry_field
-        file_name = f'{entry_id}.{file_extension}'
-
-        if self._multiprocess_lock is not None:
-            # Writing to a zip file is not multiprocess safe since multiple processes are writing to the same file.
-            # So if another process is currently accessing the zip file, the code below is blocked.
-            self._multiprocess_lock.acquire()
-
-        u.save_file(file_location=self._output, file_content=entry, file_name=file_name)
-
-        if self._multiprocess_lock is not None:
-            # Unblock other processes from accessing the above code.
-            self._multiprocess_lock.release()
+        if self._output is None:
+            self._in_memory_entries[entry_id] = entry
+        else:
+            file_extension = 'txt' if entry_field is None else entry_field
+            file_name = f'{entry_id}.{file_extension}'
+            if self._multiprocess_lock is not None:
+                # Writing to a zip file is not multiprocess safe since multiple processes are writing to the same file.
+                # So if another process is currently accessing the zip file, the code below is blocked.
+                self._multiprocess_lock.acquire()
+            u.save_file(file_location=self._output, file_content=entry, file_name=file_name)
+            if self._multiprocess_lock is not None:
+                # Unblock other processes from accessing the above code.
+                self._multiprocess_lock.release()
 
     def _save_single_entry_response(self, kegg_response: r.KEGGresponse, pull_result: PullResult) -> None:
         """ Saves the entry in a KEGG response that contains only one entry.
 
         :param kegg_response: The KEGG response that only has one entry.
         :param pull_result: The pull result to update with the successful entry ID.
         """
+        # noinspection PyTypeChecker
         get_url: ku.GetKEGGurl = kegg_response.kegg_url
         [entry_id] = get_url.entry_ids
-        pull_result.add_entry_ids(entry_id, status=r.KEGGresponse.Status.SUCCESS)
-
-        if ku.GetKEGGurl.is_binary(entry_field=self.entry_field):
+        # noinspection PyProtectedMember
+        pull_result._add_entry_ids(entry_id, status=r.KEGGresponse.Status.SUCCESS)
+        if ku.GetKEGGurl.is_binary(entry_field=self._entry_field):
             entry: bytes = kegg_response.binary_body
         else:
             entry: str = kegg_response.text_body
-
-        self._save(entry_id=entry_id, entry=entry, entry_field=self.entry_field)
-
+        self._save(entry_id=entry_id, entry=entry, entry_field=self._entry_field)
 
     def _handle_unsuccessful_url(self, kegg_response: r.KEGGresponse, pull_result: PullResult) -> None:
         """ Handles an unsuccessful pull (failed or timed out).
 
         :param kegg_response: The KEGG response resulting from a pull that was not successful.
         :param pull_result: The pull result to update based on how the unsuccessful response is dealt with.
         """
+        # noinspection PyTypeChecker
         get_url: ku.GetKEGGurl = kegg_response.kegg_url
         status: r.KEGGresponse.Status = kegg_response.status
-
         if get_url.multiple_entry_ids:
             self._pull_separate_entries(get_url=get_url, pull_result=pull_result)
         else:
             [entry_id] = get_url.entry_ids
-            pull_result.add_entry_ids(entry_id, status=status)
+            # noinspection PyProtectedMember
+            pull_result._add_entry_ids(entry_id, status=status)
 
 
 class AbstractMultiplePull(abc.ABC):
     """Abstract class that makes multiple requests to the KEGG REST API to pull and save entries of an arbitrary amount."""
-
     ABORTED_PULL_RESULTS_PATH = 'aborted-pull-results.json'
 
-    def __init__(
-        self, single_pull: SinglePull, force_single_entry: bool = False, unsuccessful_threshold: float = None
-    ) -> None:
+    def __init__(self, single_pull: SinglePull, unsuccessful_threshold: float | None = None) -> None:
         """
         :param single_pull: The SinglePull object used for each pull.
-        :param force_single_entry: Whether to pull only one entry at a time regardless of the entry field specified in the SinglePull argument.
         :param unsuccessful_threshold: If set, the ratio of unsuccessful entry IDs to total entry IDs at which execution stops. Details of the aborted process are logged.
         """
         self._single_pull = single_pull
-        self._force_single_entry = force_single_entry
-
         if unsuccessful_threshold is not None and (unsuccessful_threshold <= 0.0 or unsuccessful_threshold >= 1.0):
             raise ValueError(
-                f'Unsuccessful threshold of {unsuccessful_threshold} is out of range. Valid values are within 0.0 and 1.0, non-inclusive'
-            )
-
+                f'Unsuccessful threshold of {unsuccessful_threshold} is out of range. Valid values are within 0.0 and 1.0, non-inclusive')
         self._unsuccessful_threshold = unsuccessful_threshold
+        self._entry_field = None
+        self._force_single_entry = None
+        self._output = None
+        self._in_memory_entries = None
 
-    def pull(
-        self, entry_ids: list, entry_field: t.Optional[str] = '', force_single_entry: t.Optional[bool] = None
-    ) -> PullResult:
+    def pull(self, entry_ids: list[str], output: str, entry_field: str | None = None, force_single_entry: bool = False) -> PullResult:
         """ Makes multiple requests to the KEGG REST API for an arbitrary amount of entry IDs.
 
-        :param entry_ids: The IDs of the entries that are split into multiple pulls.
-        :param entry_field: An optional field of the entries to pull. If specified, updates the underlying SinglePull class's entry_field member.
-        :param force_single_entry: If provided, updates the force_single_single_entry value of this AbstractMultiplePull object just for this call of pull.
+        :param entry_ids: The IDs that are split into multiple pulls, the entries of which are saved to the file system.
+        :param output: Path to the location where entries are saved. Treated like a ZIP file if ends in ".zip", else a directory. If a directory, the directory is created if it doesn't already exist.
+        :param entry_field: An optional field of the entries to pull.
+        :param force_single_entry: Whether to pull only one entry at a time regardless of the entry field specified. Recommended if there are Brite entry IDs.
         :return: The pull result.
         """
-        force_single_entry = force_single_entry if force_single_entry is not None else self._force_single_entry
-        n_entry_ids: int = len(entry_ids)
-        unsuccessful_threshold: float = self._unsuccessful_threshold
-        progress_bar = tqdm.tqdm(total=n_entry_ids)
+        if output is None:
+            raise ValueError('"output" cannot be None')
+        return self._pull(entry_ids=entry_ids, output=output, entry_field=entry_field, force_single_entry=force_single_entry)
+
+    def pull_dict(self, entry_ids: list[str], entry_field: str | None = None, force_single_entry: bool = False) -> tuple[PullResult, KEGGentryMapping]:
+        """ Rather than saving the KEGG entries to the file system, stores them in-memory as a mapping from the ID to the corresponding entry.
+
+        :param entry_ids: The IDs that are split into multiple pulls, the entries of which are stored in the mapping.
+        :param entry_field: An optional field of the entries to pull.
+        :param force_single_entry: Whether to pull only one entry at a time regardless of the entry field specified. Recommended if there are Brite entry IDs.
+        :return: The pull result and the mapping from entry IDs to KEGG entries as strings (or bytes if the entries are in binary format).
+        """
+        self._in_memory_entries = KEGGentryMapping()
+        pull_result = self._pull(entry_ids=entry_ids, output=None, entry_field=entry_field, force_single_entry=force_single_entry)
+        tmp = self._in_memory_entries
+        self._in_memory_entries = None
+        return pull_result, tmp
 
-        def check_progress(single_pull_result: PullResult, multiple_pull_result: PullResult, grouped_entry_ids: list):
-            n_entry_ids_processed: int = multiple_pull_result.merge_pull_results(other=single_pull_result)
+    def _pull(self, entry_ids: list[str], output: str | None, entry_field: str | None, force_single_entry: bool) -> PullResult:
+        """ Generic pull helper function that saves to the file system if output is provided, otherwise saves entries in-memory.
 
-            n_unsuccessful: int = len(multiple_pull_result.failed_entry_ids) + len(
-                multiple_pull_result.timed_out_entry_ids
-            )
-
-            if unsuccessful_threshold is not None and n_unsuccessful / n_entry_ids >= unsuccessful_threshold:
-                total_processed_entry_ids: set = set(multiple_pull_result.successful_entry_ids)
-                total_processed_entry_ids: set = total_processed_entry_ids.union(set(multiple_pull_result.failed_entry_ids))
-                total_processed_entry_ids: set = total_processed_entry_ids.union(set(multiple_pull_result.timed_out_entry_ids))
-                remaining_entry_ids = set()
+        :param entry_ids: The IDs of the entries to pull.
+        :param output: If set, saves to the file system location specified. Otherwise, stores in-memory.
+        :param entry_field: Optional KEGG entry field to pull.
+        :param force_single_entry: Whether to pull only one entry at a time regardless of the entry field specified.
+        :return:
+        """
+        self._output = output
+        self._entry_field = entry_field
+        self._force_single_entry = force_single_entry
+        n_entry_ids = len(entry_ids)
+        progress_bar = tqdm.tqdm(total=n_entry_ids)
 
+        def check_progress(single_pull_result: PullResult, multiple_pull_result: PullResult, grouped_entry_ids: list[list[str]]) -> None:
+            # noinspection PyProtectedMember
+            n_entry_ids_processed = multiple_pull_result._merge_pull_results(other=single_pull_result)
+            n_unsuccessful = len(multiple_pull_result.failed_entry_ids) + len(multiple_pull_result.timed_out_entry_ids)
+            if self._unsuccessful_threshold is not None and n_unsuccessful / n_entry_ids >= self._unsuccessful_threshold:
+                total_processed_entry_ids = set(multiple_pull_result.successful_entry_ids)
+                total_processed_entry_ids = total_processed_entry_ids.union(set(multiple_pull_result.failed_entry_ids))
+                total_processed_entry_ids = total_processed_entry_ids.union(set(multiple_pull_result.timed_out_entry_ids))
+                remaining_entry_ids = set[str]()
                 for entry_ids_group in grouped_entry_ids:
                     for entry_id in entry_ids_group:
                         if entry_id not in total_processed_entry_ids:
                             remaining_entry_ids.add(entry_id)
-
-                l.error(
-                    f'Unsuccessful threshold of {unsuccessful_threshold} met. Aborting. Details saved at '
-                    f'{AbstractMultiplePull.ABORTED_PULL_RESULTS_PATH}'
-                )
-
+                log.error(
+                    f'Unsuccessful threshold of {self._unsuccessful_threshold} met. Aborting. Details saved at '
+                    f'{AbstractMultiplePull.ABORTED_PULL_RESULTS_PATH}')
                 aborted_pull_results = {
                     'num-remaining-entry-ids': len(remaining_entry_ids),
                     'num-successful': len(multiple_pull_result.successful_entry_ids),
                     'num-failed': len(multiple_pull_result.failed_entry_ids),
                     'num-timed-out': len(multiple_pull_result.timed_out_entry_ids),
                     'remaining-entry-ids': sorted(remaining_entry_ids),
                     'successful-entry-ids': multiple_pull_result.successful_entry_ids,
                     'failed-entry-ids': multiple_pull_result.failed_entry_ids,
-                    'timed-out-entry-ids': multiple_pull_result.timed_out_entry_ids,
-                }
-
+                    'timed-out-entry-ids': multiple_pull_result.timed_out_entry_ids}
                 with open(AbstractMultiplePull.ABORTED_PULL_RESULTS_PATH, 'w') as file:
-                    j.dump(aborted_pull_results, file, indent=0)
-
+                    json.dump(aborted_pull_results, file, indent=0)
                 exit(1)
             else:
                 progress_bar.update(n=n_entry_ids_processed)
+        entry_ids = self._group_entry_ids(entry_ids_to_group=entry_ids)
+        return self._concrete_pull(grouped_entry_ids=entry_ids, check_progress=check_progress)
 
-        # If a new entry field is provided, update it
-        if entry_field != '':
-            self._single_pull.entry_field = entry_field
-
-        entry_ids: list = self._group_entry_ids(
-            entry_ids_to_group=entry_ids, force_single_entry=force_single_entry
-        )
-
-        return self._pull(grouped_entry_ids=entry_ids, check_progress=check_progress)
-
-    def _group_entry_ids(self, entry_ids_to_group: list, force_single_entry: bool) -> list:
-        group_size: int = AbstractMultiplePull._get_n_entries_per_url(
-            force_single_entry=force_single_entry, entry_field=self._single_pull.entry_field
-        )
-
-        grouped_entry_ids = []
+    def _group_entry_ids(self, entry_ids_to_group: list[str]) -> list[list[str]]:
+        """ Splits up a list of entry IDs into a list of lists.
 
+        :param entry_ids_to_group: The entry IDs to divide into groups.
+        :return: The list of lists.
+        """
+        group_size = self._get_n_entries_per_url()
+        grouped_entry_ids = list[list[str]]()
         for i in range(0, len(entry_ids_to_group), group_size):
-            entry_id_group: list = entry_ids_to_group[i:i + group_size]
+            entry_id_group = entry_ids_to_group[i:i + group_size]
             grouped_entry_ids.append(entry_id_group)
-
         return grouped_entry_ids
 
-    @staticmethod
-    def _get_n_entries_per_url(force_single_entry: bool, entry_field: str) -> int:
+    def _get_n_entries_per_url(self) -> int:
         """ Gets the number of entries for each Get KEGG URL used to make the pulls.
 
-        :param force_single_entry: If true, returns 1.
-        :param entry_field: If the entry field can only be pulled 1 at a time, return 1.
-        :return: 1 if the above specifications are true, else the maximum number of entries per Get URL.
+        :return: 1 if certain specifications are met, else the maximum number of entries per Get URL.
         """
-        if force_single_entry:
+        if self._force_single_entry:
             return 1
-        elif ku.GetKEGGurl.only_one_entry(entry_field=entry_field):
+        elif ku.GetKEGGurl.only_one_entry(entry_field=self._entry_field):
             return 1
         else:
             return ku.GetKEGGurl.MAX_ENTRY_IDS_PER_URL
 
     @abc.abstractmethod
-    def _pull(self, grouped_entry_ids: list, check_progress: t.Callable) -> PullResult:
+    def _concrete_pull(
+            self, grouped_entry_ids: list[list[str]],
+            check_progress: t.Callable[[PullResult, PullResult, list[list[str]]], None]) -> PullResult:
         """ Pulls the entries of specified IDs in the manner of the extended concrete class.
 
         :param grouped_entry_ids: List of lists of entry IDs, with each list being below or equal to the number allowed per Get KEGG URL.
         :param check_progress: Function that updates the progress bar and pull result if the unsuccessful threshold either isn't set or hasn't been reached. Else aborts.
         :return: The pull result.
         """
         pass  # pragma: no cover
 
 
 class SingleProcessMultiplePull(AbstractMultiplePull):
     """Class that makes multiple requests to the KEGG REST API to pull entries within a single process."""
+    def __init__(self, kegg_rest: r.KEGGrest | None = None, unsuccessful_threshold: float | None = None) -> None:
+        """
+        :param kegg_rest: Optional KEGGrest object used to make the requests to the KEGG REST API (a KEGGrest object with the default settings is created if one is not provided).
+        :param unsuccessful_threshold: If set, the ratio of unsuccessful entry IDs to total entry IDs at which execution stops. Details of the aborted process are logged.
+        """
+        single_pull = SinglePull(kegg_rest=kegg_rest)
+        super(SingleProcessMultiplePull, self).__init__(single_pull=single_pull, unsuccessful_threshold=unsuccessful_threshold)
 
-    def _pull(self, grouped_entry_ids: list, check_progress: t.Callable) -> PullResult:
+    def _concrete_pull(
+            self, grouped_entry_ids: list[list[str]],
+            check_progress: t.Callable[[PullResult, PullResult, list[list[str]]], None]) -> PullResult:
         """ Makes multiple requests to the KEGG REST API to pull entries within a single process.
 
         :param grouped_entry_ids: List of lists of entry IDs, with each list being below or equal to the number allowed per Get KEGG URL.
         :param check_progress: Function that updates the progress bar and pull result if the unsuccessful threshold either isn't set or hasn't been reached. Else aborts.
         :return: The pull result
         """
         multiple_pull_result = PullResult()
-
         for entry_id_group in grouped_entry_ids:
-            single_pull_result: PullResult = self._single_pull.pull(entry_ids=entry_id_group)
-
-            check_progress(
-                single_pull_result=single_pull_result, multiple_pull_result=multiple_pull_result,
-                grouped_entry_ids=grouped_entry_ids
-            )
-
+            if self._output is not None:
+                single_pull_result = self._single_pull.pull(entry_ids=entry_id_group, output=self._output, entry_field=self._entry_field)
+            else:
+                single_pull_result, in_memory_entries = self._single_pull.pull_dict(
+                    entry_ids=entry_id_group, entry_field=self._entry_field)
+                self._in_memory_entries.update(in_memory_entries)
+            check_progress(single_pull_result, multiple_pull_result, grouped_entry_ids)
         return multiple_pull_result
 
 
 class MultiProcessMultiplePull(AbstractMultiplePull):
     """Class that makes multiple requests to the KEGG REST API to pull entries within multiple processes."""
-
-    def __init__(
-        self, single_pull: SinglePull, n_workers: int = None, force_single_entry: bool = False,
-        unsuccessful_threshold: float = None
-    ):
+    def __init__(self, kegg_rest: r.KEGGrest | None = None, unsuccessful_threshold: float | None = None, n_workers: int | None = None):
         """
-        :param single_pull: The SinglePull object used for each pull. If saving to a ZIP archive, must be instantiated with multiprocess_lock_save set to True.
-        :param force_single_entry: Whether to pull only one entry at a time despite the entry field specified in the SinglePull argument.
-        :param n_workers: The number of processes to use. If None, defaults to the number of cores available.
+        :param kegg_rest: Optional KEGGrest object used to make the requests to the KEGG REST API (a KEGGrest object with the default settings is created if one is not provided).
         :param unsuccessful_threshold: If set, the ratio of unsuccessful entry IDs to total entry IDs at which execution stops. Details of the aborted process are logged.
+        :param n_workers: The number of processes to use. If None, defaults to the number of cores available.
         """
-        super(MultiProcessMultiplePull, self).__init__(
-            single_pull=single_pull, force_single_entry=force_single_entry, unsuccessful_threshold=unsuccessful_threshold
-        )
-
+        single_pull = SinglePull(kegg_rest=kegg_rest, multiprocess_lock_save=True)
+        super(MultiProcessMultiplePull, self).__init__(single_pull=single_pull, unsuccessful_threshold=unsuccessful_threshold)
         self._n_workers = n_workers if n_workers is not None else os.cpu_count()
 
-    def _pull(self, grouped_entry_ids: list, check_progress: t.Callable) -> PullResult:
+    def _concrete_pull(
+            self, grouped_entry_ids: list[list[str]],
+            check_progress: t.Callable[[PullResult, PullResult, list[list[str]]], None]) -> PullResult:
         """ Makes multiple requests to the KEGG REST API to pull entries within multiple processes.
 
         :param grouped_entry_ids: List of lists of entry IDs, with each list being below or equal to the number allowed per Get KEGG URL.
         :param check_progress: Function that updates the progress bar and pull result if the unsuccessful threshold either isn't set or hasn't been reached. Else aborts.
-        :return: The pull result
+        :return: The pull result.
         """
         multiple_pull_result = PullResult()
-
         # Passing in _set_single_pull as the "initializer" allows setting the SinglePull object as a global variable.
         # We need to set it as a global since pickling its Lock member is not allowed.
         # Also, this makes it available to each process without pickling it every time it's passed to a worker.
-        with mp.Pool(self._n_workers, initializer=_set_single_pull, initargs=(self._single_pull,)) as pool:
+        with mp.Pool(self._n_workers, initializer=_set_single_pull, initargs=(self._single_pull, self._entry_field, self._output)) as pool:
             async_results = [
-                pool.apply_async(_get_single_pull_result, (entry_ids,)) for entry_ids in grouped_entry_ids
-            ]
-
+                pool.apply_async(_get_single_pull_result, (entry_ids,)) for entry_ids in grouped_entry_ids]
             for async_result in async_results:
                 result: bytes = async_result.get()
-                single_pull_result: PullResult = p.loads(result)
-
-                check_progress(
-                    single_pull_result=single_pull_result, multiple_pull_result=multiple_pull_result,
-                    grouped_entry_ids=grouped_entry_ids
-                )
-
+                if self._output is not None:
+                    single_pull_result: PullResult = p.loads(result)
+                else:
+                    single_pull_result, in_memory_entries = p.loads(result)
+                    self._in_memory_entries.update(in_memory_entries)
+                check_progress(single_pull_result, multiple_pull_result, grouped_entry_ids)
         return multiple_pull_result
 
 
-global_single_pull: SinglePull = None
+_global_single_pull: SinglePull | None = None
+_global_entry_field: str | None = None
+_global_output: str | None = None
 
 
-def _set_single_pull(single_pull: SinglePull) -> None:
-    """ Sets a global SinglePull variable to be used in each process within a multiprocessing pool.
+def _set_single_pull(single_pull: SinglePull, entry_field: str | None, output: str | None) -> None:
+    """ Sets global variables to be used in each process within a multiprocessing pool.
 
     :param single_pull: The SinglePull object to set such that it's accessible to each process.
+    :param entry_field: The entry field to make available to each process.
+    :param output: The output variable to make available to each process.
     """
-    global global_single_pull
-
-    global_single_pull = single_pull  # pragma: no cover
+    global _global_single_pull
+    global _global_entry_field
+    global _global_output
+
+    _global_single_pull = single_pull  # pragma: no cover
+    _global_entry_field = entry_field  # pragma: no cover
+    _global_output = output  # pragma: no cover
 
 
 def _get_single_pull_result(entry_ids: list) -> bytes:
     """ Makes a request to the REST KEGG API to pull one or more entries.
 
     :param entry_ids: The IDs of the entries to pull.
     :return: The pull result.
     """
-    single_pull_result: PullResult = global_single_pull.pull(entry_ids=entry_ids)
-
-    return p.dumps(single_pull_result)
+    if _global_output is not None:
+        return p.dumps(_global_single_pull.pull(
+            entry_ids=entry_ids, output=_global_output, entry_field=_global_entry_field))
+    else:
+        return p.dumps(_global_single_pull.pull_dict(entry_ids=entry_ids, entry_field=_global_entry_field))
```

### Comparing `kegg_pull-2.1.0/src/kegg_pull/pull_cli.py` & `kegg_pull-3.0.0/src/kegg_pull/pull_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,98 +1,97 @@
 """
 Usage:
     kegg_pull pull -h | --help
-    kegg_pull pull database <database-name> [--force-single-entry] [--multi-process] [--n-workers=<n-workers>] [--output=<output>] [--entry-field=<entry-field>] [--n-tries=<n-tries>] [--time-out=<time-out>] [--sleep-time=<sleep-time>] [--ut=<unsuccessful-threshold>]
-    kegg_pull pull entry-ids <entry-ids> [--force-single-entry] [--multi-process] [--n-workers=<n-workers>] [--output=<output>] [--entry-field=<entry-field>] [--n-tries=<n-tries>] [--time-out=<time-out>] [--sleep-time=<sleep-time>] [--ut=<unsuccessful-threshold>]
+    kegg_pull pull database <database> [--force-single-entry] [--multi-process] [--n-workers=<n-workers>] [--output=<output>] [--print] [--sep=<print-separator>] [--entry-field=<entry-field>] [--n-tries=<n-tries>] [--time-out=<time-out>] [--sleep-time=<sleep-time>] [--ut=<unsuccessful-threshold>]
+    kegg_pull pull entry-ids <entry-ids> [--force-single-entry] [--multi-process] [--n-workers=<n-workers>] [--output=<output>] [--print] [--sep=<print-separator>] [--entry-field=<entry-field>] [--n-tries=<n-tries>] [--time-out=<time-out>] [--sleep-time=<sleep-time>] [--ut=<unsuccessful-threshold>]
 
 Options:
     -h --help                       Show this help message.
     database                        Pulls all the entries in a KEGG database.
-    <database-name>                 The KEGG database from which to pull entries.
-    --force-single-entry            Forces pulling only one entry at a time for every request to the KEGG web API. This flag is automatically set if <database-name> is "brite".
+    <database>                      The KEGG database from which to pull entries.
+    --force-single-entry            Forces pulling only one entry at a time for every request to the KEGG web API. This flag is automatically set if <database> is "brite".
     --multi-process                 If set, the entries are pulled across multiple processes to increase speed. Otherwise, the entries are pulled sequentially in a single process.
     --n-workers=<n-workers>         The number of sub-processes to create when pulling. Defaults to the number of cores available. Ignored if --multi-process is not set.
-    --output=<output>               The directory where the pulled KEGG entries will be stored. Defaults to the current working directory. If ends in ".zip", entries are saved to a ZIP archive instead of a directory.
+    --output=<output>               The directory where the pulled KEGG entries will be stored. Defaults to the current working directory. If ends in ".zip", entries are saved to a ZIP archive instead of a directory. Ignored if --print is set.
+    --print                         If set, prints the entries to the screen rather than saving them to the file system. Separates entries by the --sep option if set.
+    --sep=<print-separator>         The string that separates the entries which are printed to the screen when the --print option is set. Ignored if the --print option is not set. Defaults to printing the entry id, followed by the entry, followed by a newline.
     --entry-field=<entry-field>     Optional field to extract from the entries pulled rather than the standard flat file format (or "htext" in the case of brite entries).
     --n-tries=<n-tries>             The number of times to attempt a KEGG request before marking it as timed out or failed. Defaults to 3.
     --time-out=<time-out>           The number of seconds to wait for a KEGG request before marking it as timed out. Defaults to 60.
     --sleep-time=<sleep-time>       The amount of time to wait after a KEGG request times out (or potentially blacklists with a 403 error code) before attempting it again. Defaults to 5.0.
     --ut=<unsuccessful-threshold>   If set, the ratio of unsuccessful entry IDs (failed or timed out) to total entry IDs at which kegg_pull quits. Valid values are between 0.0 and 1.0 non-inclusive.
     entry-ids                       Pulls entries specified by a comma separated list. Or from standard input: one entry ID per line; Press CTRL+D to finalize input or pipe (e.g. cat file.txt | kegg_pull pull entry-ids - ...).
     <entry-ids>                     Comma separated list of entry IDs to pull (e.g. id1,id2,id3 etc.). Or if equal to "-", entry IDs are read from standard input. Will likely need to set --force-single-entry if any of the entries are from the brite database.
 """
 import docopt as d
-import json as j
-import time as t
-
+import json
+import time
+import logging as log
 from . import pull as p
 from . import rest as r
 from . import entry_ids as ei
+from . import kegg_url as ku
 from . import _utils as u
 
 
 def main():
-    args: dict = d.docopt(__doc__)
-    n_tries: int = int(args['--n-tries']) if args['--n-tries'] is not None else None
-    time_out: int = int(args['--time-out']) if args['--time-out'] is not None else None
-    sleep_time: float = float(args['--sleep-time']) if args['--sleep-time'] is not None else None
+    args = d.docopt(__doc__)
+    n_tries = int(args['--n-tries']) if args['--n-tries'] is not None else None
+    time_out = int(args['--time-out']) if args['--time-out'] is not None else None
+    sleep_time = float(args['--sleep-time']) if args['--sleep-time'] is not None else None
     kegg_rest = r.KEGGrest(n_tries=n_tries, time_out=time_out, sleep_time=sleep_time)
-    output: str = args['--output'] if args['--output'] is not None else '.'
+    output = args['--output'] if args['--output'] is not None else '.'
+    print_to_screen: bool = args['--print']
     entry_field: str = args['--entry-field']
-    multiprocess_lock_save: bool = args['--multi-process'] and output.endswith('.zip')
-    single_pull = p.SinglePull(output=output, kegg_rest=kegg_rest, entry_field=entry_field, multiprocess_lock_save=multiprocess_lock_save)
     force_single_entry: bool = args['--force-single-entry']
-
     if args['database']:
-        database_name: str = args['<database-name>']
-
-        if database_name == 'brite':
+        database: str = args['<database>']
+        if database == 'brite':
             force_single_entry = True
-
-        entry_ids: list = ei.from_database(database_name=database_name)
+        entry_ids = ei.from_database(database=database)
     else:
-        entry_ids: list = u.handle_cli_input(input_source=args['<entry-ids>'])
-
-    unsuccessful_threshold: float = float(args['--ut']) if args['--ut'] is not None else None
-
+        entry_ids = u.parse_input_sequence(input_source=args['<entry-ids>'])
+    unsuccessful_threshold = float(args['--ut']) if args['--ut'] is not None else None
     if args['--multi-process']:
         n_workers = int(args['--n-workers']) if args['--n-workers'] is not None else None
-
-        multiple_pull = p.MultiProcessMultiplePull(
-            single_pull=single_pull, force_single_entry=force_single_entry, n_workers=n_workers,
-            unsuccessful_threshold=unsuccessful_threshold
-        )
+        multiple_pull = p.MultiProcessMultiplePull(kegg_rest=kegg_rest, unsuccessful_threshold=unsuccessful_threshold, n_workers=n_workers)
     else:
-        multiple_pull = p.SingleProcessMultiplePull(
-            single_pull=single_pull, force_single_entry=force_single_entry, unsuccessful_threshold=unsuccessful_threshold
-        )
-
-    time1: float = _testable_time()
-    pull_result: p.PullResult = multiple_pull.pull(entry_ids=entry_ids)
-    time2: float = _testable_time()
-
-    n_total_entry_ids: int = len(pull_result.successful_entry_ids) + len(pull_result.failed_entry_ids)
+        multiple_pull = p.SingleProcessMultiplePull(kegg_rest=kegg_rest, unsuccessful_threshold=unsuccessful_threshold)
+    time1 = _testable_time()
+    if print_to_screen:
+        pull_result, kegg_entry_mapping = multiple_pull.pull_dict(
+            entry_ids=entry_ids, entry_field=entry_field, force_single_entry=force_single_entry)
+        if ku.GetKEGGurl.is_binary(entry_field=entry_field):
+            log.warning('Printing binary output...')
+        print_separator: str = args['--sep']
+        if print_separator:
+            print(f'\n{print_separator}\n'.join(kegg_entry_mapping.values()))
+        else:
+            for entry_id, entry in kegg_entry_mapping.items():
+                print(entry_id)
+                print(f'{entry}\n')
+    else:
+        pull_result = multiple_pull.pull(entry_ids=entry_ids, output=output, entry_field=entry_field, force_single_entry=force_single_entry)
+    time2 = _testable_time()
+    n_total_entry_ids = len(pull_result.successful_entry_ids) + len(pull_result.failed_entry_ids)
     n_total_entry_ids += len(pull_result.timed_out_entry_ids)
-    percent_success: float = len(pull_result.successful_entry_ids) / n_total_entry_ids * 100
-
+    percent_success = len(pull_result.successful_entry_ids) / n_total_entry_ids * 100
     pull_results = {
         'percent-success': float(f'{percent_success:.2f}'),
         'pull-minutes': float(f'{(time2 - time1) / 60:.2f}'),
         'num-successful': len(pull_result.successful_entry_ids),
         'num-failed': len(pull_result.failed_entry_ids),
         'num-timed-out': len(pull_result.timed_out_entry_ids),
         'num-total': n_total_entry_ids,
         'successful-entry-ids': pull_result.successful_entry_ids,
         'failed-entry-ids': pull_result.failed_entry_ids,
-        'timed-out-entry-ids': pull_result.timed_out_entry_ids
-    }
-
+        'timed-out-entry-ids': pull_result.timed_out_entry_ids}
     with open('pull-results.json', 'w') as file:
-        j.dump(pull_results, file, indent=0)
+        json.dump(pull_results, file, indent=0)
 
 
 def _testable_time() -> float:
     """ The time.time() function causes issues when mocked in tests, so we create this wrapper that can be safely mocked
 
     :return: The result of time.time()
     """
-    return t.time()  # pragma: no cover
+    return time.time()  # pragma: no cover
```

### Comparing `kegg_pull-2.1.0/src/kegg_pull/rest.py` & `kegg_pull-3.0.0/src/kegg_pull/rest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,266 +1,248 @@
 """
 KEGG REST API Operations
 ~~~~~~~~~~~~~~~~~~~~~~~~
-Interface for the KEGG REST API including all its operations.
+|Interface for| the KEGG REST API including all its operations.
 """
+import typing as t
 import enum as e
 import requests as rq
 import time
-import typing as t
 import inspect as ins
-import logging as l
-
+import logging as log
 from . import kegg_url as ku
+from . import _utils as u
 
 
-class KEGGresponse:
-    """Class containing details of a response from the KEGG REST API."""
-
+class KEGGresponse(u.NonInstantiable):
+    """
+    Class containing details of a response from the KEGG REST API.
+
+    :ivar Status status: The status of the KEGG response.
+    :ivar AbstractKEGGurl kegg_url: The URL used in the request to the KEGG REST API that resulted in the KEGG response.
+    :ivar str text_body: The text version of the response body.
+    :ivar bytes binary_body: The binary version of the response body.
+    """
     class Status(e.Enum):
         """The status of a KEGG response."""
         SUCCESS = 1
         FAILED = 2
         TIMEOUT = 3
 
     def __init__(self, status: Status, kegg_url: ku.AbstractKEGGurl, text_body: str = None, binary_body: bytes = None) -> None:
         """
         :param status: The status of the KEGG response.
         :param kegg_url: The URL used in the request to the KEGG REST API that resulted in the KEGG response.
         :param text_body: The text version of the response body.
         :param binary_body: The binary version of the response body.
         :raises ValueError: Raised if the status is SUCCESS but a response body is not provided.
         """
-        if status == KEGGresponse.Status.SUCCESS and (
-            text_body is None or binary_body is None or text_body == '' or binary_body == b''
-        ):
+        super(KEGGresponse, self).__init__()
+        if status == KEGGresponse.Status.SUCCESS and (text_body is None or binary_body is None or text_body == '' or binary_body == b''):
             raise ValueError('A KEGG response cannot be marked as successful if its response body is empty')
-
-        self._status = status
-        self._kegg_url = kegg_url
-        self._text_body = text_body
-        self._binary_body = binary_body
-
-    @property
-    def status(self) -> Status:
-        return self._status
-
-    @property
-    def kegg_url(self) -> ku.AbstractKEGGurl:
-        return self._kegg_url
-
-    @property
-    def text_body(self) -> str:
-        return self._text_body
-
-    @property
-    def binary_body(self) -> bytes:
-        return self._binary_body
+        self.status = status
+        self.kegg_url = kegg_url
+        self.text_body = text_body
+        self.binary_body = binary_body
 
 
 class KEGGrest:
     """Class containing methods for making requests to the KEGG REST API, including all the KEGG REST API operations."""
-    def __init__(self, n_tries: int = 3, time_out: int = 60, sleep_time: float = 5.0):
+    def __init__(self, n_tries: int | None = 3, time_out: int | None = 60, sleep_time: float | None = 5.0):
         """
         :param n_tries: The number of times to try to make a request (can succeed the first time, or any of n_tries, or none of the tries).
         :param time_out: The number of seconds to wait for a request until marking it as timed out.
         :param sleep_time: The number of seconds to wait in between timed out requests or blacklisted requests.
         """
         self._n_tries = n_tries if n_tries is not None else 3
         self._time_out = time_out if time_out is not None else 60
         self._sleep_time = sleep_time if sleep_time is not None else 5.0
-
         if self._n_tries < 1:
             raise ValueError(f'{self._n_tries} is not a valid number of tries to make a KEGG request.')
 
-    def request(self, KEGGurl: type = None, kegg_url: ku.AbstractKEGGurl = None, **kwargs) -> KEGGresponse:
+    def request(self, KEGGurl: type[ku.AbstractKEGGurl] = None, kegg_url: ku.AbstractKEGGurl = None, **kwargs) -> KEGGresponse:
         """ General KEGG request function based on a given KEGG URL (either a class that is instantiated or an already instantiated KEGG URL object).
 
         :param KEGGurl: Optional KEGG URL class (extended from AbstractKEGGurl) that's instantiated with provided keyword arguments.
         :param kegg_url: Optional KEGGurl object that's already instantiated (used if KEGGurl class is not provided).
         :param kwargs: The keyword arguments used to instantiate the KEGGurl class, if provided.
         :return: The KEGG response.
         """
-        kegg_url: ku.AbstractKEGGurl = KEGGrest._get_kegg_url(KEGGurl=KEGGurl, kegg_url=kegg_url, **kwargs)
-        status = None
-
+        kegg_url = KEGGrest._get_kegg_url(KEGGurl=KEGGurl, kegg_url=kegg_url, **kwargs)
+        status: KEGGresponse.Status | None = None
         for _ in range(self._n_tries):
             try:
-                response: rq.Response = rq.get(url=kegg_url.url, timeout=self._time_out)
-
+                response = rq.get(url=kegg_url.url, timeout=self._time_out)
                 if response.status_code == 200:
                     return KEGGresponse(
-                        status=KEGGresponse.Status.SUCCESS, kegg_url=kegg_url, text_body=response.text,
-                        binary_body=response.content
-                    )
+                        status=KEGGresponse.Status.SUCCESS, kegg_url=kegg_url, text_body=response.text, binary_body=response.content)
                 else:
                     status = KEGGresponse.Status.FAILED
-
                 if response.status_code == 403:
                     # 403 forbidden. KEGG may have blocked the request due to too many requests in too little time.
                     # In case blacklisting, sleep to allow time for KEGG to unblock further requests.
                     time.sleep(self._sleep_time)
             except rq.exceptions.Timeout:
                 status = KEGGresponse.Status.TIMEOUT
                 time.sleep(self._sleep_time)
-
         return KEGGresponse(status=status, kegg_url=kegg_url)
 
     @staticmethod
-    def _get_kegg_url(KEGGurl: type = None, kegg_url: ku.AbstractKEGGurl = None, **kwargs) -> ku.AbstractKEGGurl:
+    def _get_kegg_url(
+            KEGGurl: type[ku.AbstractKEGGurl] | None = None, kegg_url: ku.AbstractKEGGurl | None = None, **kwargs) -> ku.AbstractKEGGurl:
         """ Gets the KEGGurl object to be used to make the request to KEGG.
 
         :param KEGGurl: Optional KEGGurl class to instantiate a KEGGurl object using keyword arguments.
         :param kegg_url: Instantiated KEGGurl object that's simply returned if provided (used if the KEGGurl class is not provided).
         :param kwargs: The keyword arguments used to instantiate the KEGGurl object if a KEGGurl class is provided.
         :return: The KEGGurl object.
         :raises ValueError: Raised if both a class and object are provided or the class does not inherit from AbstractKEGGurl.
         """
         if KEGGurl is None and kegg_url is None:
             raise ValueError(
                 f'Either an instantiated kegg_url object must be provided or an extended class of '
-                f'{ku.AbstractKEGGurl.__name__} along with the corresponding kwargs for its constructor.'
-            )
-
+                f'{ku.AbstractKEGGurl.__name__} along with the corresponding kwargs for its constructor.')
         if kegg_url is not None and KEGGurl is not None:
-            l.warning(
-                'Both an instantiated kegg_url object and KEGGurl class are provided. Using the instantiated object...'
-            )
-
+            log.warning(
+                'Both an instantiated kegg_url object and KEGGurl class are provided. Using the instantiated object...')
         if kegg_url is not None:
             return kegg_url
-
         if ku.AbstractKEGGurl not in ins.getmro(KEGGurl):
             raise ValueError(
                 f'The value for KEGGurl must be an inherited class of {ku.AbstractKEGGurl.__name__}. '
-                f'The class "{KEGGurl.__name__}" is not.'
-            )
-
-        kegg_url: ku.AbstractKEGGurl = KEGGurl(**kwargs)
-
+                f'The class "{KEGGurl.__name__}" is not.')
+        kegg_url = KEGGurl(**kwargs)
         return kegg_url
 
-    def test(self, KEGGurl: type = None, kegg_url: ku.AbstractKEGGurl = None, **kwargs) -> bool:
+    def test(
+            self, KEGGurl: type[ku.AbstractKEGGurl] | None = None, kegg_url: ku.AbstractKEGGurl | None = None,
+            **kwargs) -> bool:
         """ Tests if a KEGGurl will succeed upon being used in a request to the KEGG REST API.
 
         :param KEGGurl: Optional KEGGurl class used to instantiate a KEGGurl object given keyword arguments.
         :param kegg_url: KEGGurl object that's already instantiated (used if a KEGGurl class is not provided).
         :param kwargs: The keyword arguments used to instantiated the KEGGurl object from the KEGGurl class, if provided.
         :return: True if the URL would succeed, false if it would fail or time out.
         """
-        kegg_url: ku.AbstractKEGGurl = KEGGrest._get_kegg_url(KEGGurl=KEGGurl, kegg_url=kegg_url, **kwargs)
-
+        kegg_url = KEGGrest._get_kegg_url(KEGGurl=KEGGurl, kegg_url=kegg_url, **kwargs)
         for _ in range(self._n_tries):
             try:
-                response: rq.Response = rq.head(url=kegg_url.url, timeout=self._time_out)
-
+                response = rq.head(url=kegg_url.url, timeout=self._time_out)
                 if response.status_code == 200:
                     return True
             except rq.exceptions.Timeout:
                 time.sleep(self._sleep_time)
-
         return False
 
-    def list(self, database_name: str) -> KEGGresponse:
+    def list(self, database: str) -> KEGGresponse:
         """ Executes the "list" KEGG API operation, pulling the entry IDs of the provided database.
 
-        :param database_name: The database from which to pull entry IDs.
+        :param database: The database from which to pull entry IDs.
         :return: The KEGG response.
         """
-        return self.request(KEGGurl=ku.ListKEGGurl, database_name=database_name)
+        return self.request(KEGGurl=ku.ListKEGGurl, database=database)
 
-    def get(self, entry_ids: list, entry_field: str = None) -> KEGGresponse:
+    def get(self, entry_ids: t.List[str], entry_field: str | None = None) -> KEGGresponse:
         """ Executes the "get" KEGG API operation, pulling the entries of the provided entry IDs.
 
         :param entry_ids: The IDs of entries to pull.
         :param entry_field: Optional field to extract from the entries.
         :return: The KEGG response.
         """
         return self.request(KEGGurl=ku.GetKEGGurl, entry_ids=entry_ids, entry_field=entry_field)
 
-    def info(self, database_name: str) -> KEGGresponse:
+    def info(self, database: str) -> KEGGresponse:
         """ Executes the "info" KEGG API operation, pulling information about a KEGG database.
 
-        :param database_name: The database to pull information about.
+        :param database: The database to pull information about.
         :return: The KEGG response
         """
-        return self.request(KEGGurl=ku.InfoKEGGurl, database_name=database_name)
+        return self.request(KEGGurl=ku.InfoKEGGurl, database=database)
 
-    def keywords_find(self, database_name: str, keywords: list) -> KEGGresponse:
+    def keywords_find(self, database: str, keywords: t.List[str]) -> KEGGresponse:
         """ Executes the "find" KEGG API operation, finding entry IDs based on keywords to search in entries.
 
-        :param database_name: The name of the database containing entries to search for.
+        :param database: The name of the database containing entries to search for.
         :param keywords: The keywords to search in entries.
         :return: The KEGG response
         """
-        return self.request(KEGGurl=ku.KeywordsFindKEGGurl, database_name=database_name, keywords=keywords)
+        return self.request(KEGGurl=ku.KeywordsFindKEGGurl, database=database, keywords=keywords)
 
     def molecular_find(
-        self, database_name: str, formula: str = None, exact_mass: t.Union[float, tuple] = None,
-        molecular_weight: t.Union[int, tuple] = None
-    ) -> KEGGresponse:
+            self, database: str, formula: str | None = None, exact_mass: float | tuple[float, float] | None = None,
+            molecular_weight: int | tuple[int, int] | None = None) -> KEGGresponse:
         """ Executes the "find" KEGG API operation, finding entry IDs in chemical databases based on one (and only one) choice of three molecular attributes of the entries.
 
-        :param database_name: The name of the chemical database to search for entries in.
+        :param database: The name of the chemical database to search for entries in.
         :param formula: The chemical formula (one of three choices) of chemical entries to search for.
         :param exact_mass: The exact mass (one of three choices) of chemical entries to search for (single value or range).
         :param molecular_weight: The molecular weight (one of three choices) of chemical entries to search for (single value or range).
         :return: The KEGG response
         """
         return self.request(
-            KEGGurl=ku.MolecularFindKEGGurl, database_name=database_name, formula=formula, exact_mass=exact_mass,
-            molecular_weight=molecular_weight
-        )
+            KEGGurl=ku.MolecularFindKEGGurl, database=database, formula=formula, exact_mass=exact_mass, molecular_weight=molecular_weight)
 
-    def database_conv(self, kegg_database_name: str, outside_database_name: str) -> KEGGresponse:
+    def database_conv(self, kegg_database: str, outside_database: str) -> KEGGresponse:
         """ Executes the "conv" KEGG API operation, converting the entry IDs of a KEGG database to those of an outside database.
 
-        :param kegg_database_name: The name of the KEGG database to pull converted entry IDs from.
-        :param outside_database_name: The name of the outside database to pull converted entry IDs from.
+        :param kegg_database: The name of the KEGG database to pull converted entry IDs from.
+        :param outside_database: The name of the outside database to pull converted entry IDs from.
         :return: The KEGG response.
         """
-        return self.request(
-            KEGGurl=ku.DatabaseConvKEGGurl, kegg_database_name=kegg_database_name,
-            outside_database_name=outside_database_name
-        )
+        return self.request(KEGGurl=ku.DatabaseConvKEGGurl, kegg_database=kegg_database, outside_database=outside_database)
 
-    def entries_conv(self, target_database_name: str, entry_ids: list) -> KEGGresponse:
+    def entries_conv(self, target_database: str, entry_ids: t.List[str]) -> KEGGresponse:
         """ Executes the "conv" KEGG API operation, converting provided entry IDs from one database to the form of a target database.
 
-        :param target_database_name: The name of the database to get converted entry IDs from.
+        :param target_database: The name of the database to get converted entry IDs from.
         :param entry_ids: The entry IDs to convert to the form of the target database.
         :return: The KEGG response.
         """
-        return self.request(
-            KEGGurl=ku.EntriesConvKEGGurl, target_database_name=target_database_name, entry_ids=entry_ids
-        )
+        return self.request(KEGGurl=ku.EntriesConvKEGGurl, target_database=target_database, entry_ids=entry_ids)
 
-    def database_link(self, target_database_name: str, source_database_name: str) -> KEGGresponse:
+    def database_link(self, target_database: str, source_database: str) -> KEGGresponse:
         """ Executes the "link" KEGG API operation, showing the IDs of entries in one KEGG database that are connected/related to entries of another KEGG database.
 
-        :param target_database_name: One of the two KEGG databases to pull linked entries from.
-        :param source_database_name: The other KEGG database to link entries from the target database.
+        :param target_database: One of the two KEGG databases to pull linked entries from.
+        :param source_database: The other KEGG database to link entries from the target database.
         :return: The KEGG response
         """
-        return self.request(
-            KEGGurl=ku.DatabaseLinkKEGGurl, target_database_name=target_database_name,
-            source_database_name=source_database_name
-        )
+        return self.request(KEGGurl=ku.DatabaseLinkKEGGurl, target_database=target_database, source_database=source_database)
 
-    def entries_link(self, target_database_name: str, entry_ids: list) -> KEGGresponse:
+    def entries_link(self, target_database: str, entry_ids: t.List[str]) -> KEGGresponse:
         """ Executes the "link" KEGG API operation, showing the IDs of entries that are connected/related to entries of a provided databases.
 
-        :param target_database_name: The KEGG database to find links to the provided entries.
+        :param target_database: The KEGG database to find links to the provided entries.
         :param entry_ids: The IDs of the entries to link to entries in the target database.
         :return: The KEGG response
         """
-        return self.request(
-            KEGGurl=ku.EntriesLinkKEGGurl, target_database_name=target_database_name, entry_ids=entry_ids
-        )
+        return self.request(KEGGurl=ku.EntriesLinkKEGGurl, target_database=target_database, entry_ids=entry_ids)
 
-    def ddi(self, drug_entry_ids: list) -> KEGGresponse:
+    def ddi(self, drug_entry_ids: t.List[str]) -> KEGGresponse:
         """ Executes the "ddi" KEGG API operation, searching for drug to drug interactions. Providing one entry ID reports all known interactions, while providing multiple checks if any drug pair in a given set of drugs is CI or P. If providing multiple, all entries must belong to the same database.
 
         :param drug_entry_ids: The IDs of the drug entries within which search for drug interactions.
         :return: The KEGG response
         """
         return self.request(KEGGurl=ku.DdiKEGGurl, drug_entry_ids=drug_entry_ids)
+
+
+def request_and_check_error(
+        kegg_rest: KEGGrest | None = None, KEGGurl: type[ku.AbstractKEGGurl] | None = None,
+        kegg_url: ku.AbstractKEGGurl = None, **kwargs) -> KEGGresponse:
+    """ Makes a general request to the KEGG REST API using a KEGGrest object. Creates the KEGGrest object if one is not provided.
+    Additionally, raises an exception if the request is not successful, specifying the URL that was unsuccessful.
+
+    :param kegg_rest: The KEGGrest object to perform the request. If None, one is created with the default parameters.
+    :param KEGGurl: Optional KEGG URL class (extended from AbstractKEGGurl) that's instantiated with provided keyword arguments.
+    :param kegg_url: Optional KEGGurl object that's already instantiated (used if KEGGurl class is not provided).
+    :param kwargs: The keyword arguments used to instantiate the KEGGurl class, if provided.
+    :return: The KEGG response
+    :raises RuntimeError: Raised if the request fails or times out.
+    """
+    kegg_rest = kegg_rest if kegg_rest is not None else KEGGrest()
+    kegg_response = kegg_rest.request(KEGGurl=KEGGurl, kegg_url=kegg_url, **kwargs)
+    if kegg_response.status == KEGGresponse.Status.FAILED:
+        raise RuntimeError(f'The KEGG request failed with the following URL: {kegg_response.kegg_url.url}')
+    elif kegg_response.status == KEGGresponse.Status.TIMEOUT:
+        raise RuntimeError(f'The KEGG request timed out with the following URL: {kegg_response.kegg_url.url}')
+    return kegg_response
```

### Comparing `kegg_pull-2.1.0/src/kegg_pull/rest_cli.py` & `kegg_pull-3.0.0/src/kegg_pull/rest_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,176 +1,140 @@
 """
 Usage:
     kegg_pull rest -h | --help
-    kegg_pull rest info <database-name> [--test] [--output=<output>]
-    kegg_pull rest list <database-name> [--test] [--output=<output>]
+    kegg_pull rest info <database> [--test] [--output=<output>]
+    kegg_pull rest list <database> [--test] [--output=<output>]
     kegg_pull rest get <entry-ids> [--entry-field=<entry-field>] [--test] [--output=<output>]
-    kegg_pull rest find <database-name> <keywords> [--test] [--output=<output>]
-    kegg_pull rest find <database-name> (--formula=<formula>|--em=<exact-mass>...|--mw=<molecular-weight>...) [--test] [--output=<output>]
-    kegg_pull rest conv <kegg-database-name> <outside-database-name> [--test] [--output=<output>]
-    kegg_pull rest conv --conv-target=<target-database-name> <entry-ids> [--test] [--output=<output>]
-    kegg_pull rest link <target-database-name> <source-database-name> [--test] [--output=<output>]
-    kegg_pull rest link --link-target=<target-database-name> <entry-ids> [--test] [--output=<output>]
+    kegg_pull rest find <database> <keywords> [--test] [--output=<output>]
+    kegg_pull rest find <database> (--formula=<formula>|--em=<exact-mass>...|--mw=<molecular-weight>...) [--test] [--output=<output>]
+    kegg_pull rest conv <kegg-database> <outside-database> [--test] [--output=<output>]
+    kegg_pull rest conv entry-ids <entry-ids> <target-database> [--test] [--output=<output>]
+    kegg_pull rest link <target-database> <source-database> [--test] [--output=<output>]
+    kegg_pull rest link entry-ids <entry-ids> <target-database> [--test] [--output=<output>]
     kegg_pull rest ddi <drug-entry-ids> [--test] [--output=<output>]
 
 Options:
-    -h --help                               Show this help message.
-    info                                    Executes the "info" KEGG API operation, pulling information about a KEGG database.
-    <database-name>                         The name of the database to pull information about or entry IDs from.
-    --test                                  If set, test the request to ensure it works rather than sending it. Print True if the request would succeed and False if the request would fail. Ignores --output if this options is set along with --test.
-    --output=<output>                       Path to the file (either in a directory or ZIP archive) to store the response body from the KEGG web API operation. Prints to the console if not specified. If a ZIP archive, the file path must be in the form of /path/to/zip-archive.zip:/path/to/file (e.g. ./archive.zip:file.txt).
-    list                                    Executes the "list" KEGG API operation, pulling the entry IDs of the provided database.
-    get                                     Executes the "get" KEGG API operation, pulling the entries of the provided entry IDs.
-    <entry-ids>                             Comma separated list of entry IDs (e.g. id1,id2,id3 etc.). Or if equal to "-", entry IDs are read from standard input, one entry ID per line; Press CTRL+D to finalize input or pipe (e.g. cat file.txt | kegg_pull rest get - ...).
-    --entry-field=<entry-field>             Optional field to extract from an entry instead of the default entry info (i.e. flat file or htext in the case of brite entries).
-    find                                    Executes the "find" KEGG API operation, finding entry IDs based on provided queries.
-    <keywords>                              Comma separated list of keywords to search entries with (e.g. kw1,kw2,kw3 etc.). Or if equal to "-", keywords are read from standard input, one keyword per line; Press CTRL+D to finalize input or pipe (e.g. cat file.txt | kegg_pull rest find brite - ...).
-    --formula=<formula>                     Sequence of atoms in a chemical formula format to search for (e.g. "O5C7" searches for molecule entries containing 5 oxygen atoms and/or 7 carbon atoms).
-    --em=<exact-mass>                       Either a single number (e.g. --em=155.5) or two numbers (e.g. --em=155.5 --em=244.4). If a single number, searches for molecule entries with an exact mass equal to that value rounded by the last decimal point. If two numbers, searches for molecule entries with an exact mass within the two values (a range).
-    --mw=<molecular-weight>                 Same as --em but searches based on the molecular weight.
-    conv                                    Executes the "conv" KEGG API operation, converting entry IDs from an outside database to those of a KEGG database and vice versa.
-    <kegg-database-name>                    The name of the KEGG database from which to view equivalent outside database entry IDs.
-    <outside-database-name>                 The name of the non-KEGG database from which to view equivalent KEGG database entry IDs.
-    --conv-target=<target-database-name>    The outside or KEGG database from which to view equivalent versions of the provided entry IDs. If a KEGG database, the provided entry IDs must be from an outside database and vice versa.
-    link                                    Executes the "link" KEGG API operation, showing the IDs of entries that are connected/related to entries of other databases.
-    <target-database-name>                  The name of the database to find cross-references in the source database.
-    <source-database-name>                  The name of the database from which cross-references are found in the target database.
-    --link-target-<target-database-name>    The name of the database to find cross-references in the provided entry IDs.
-    ddi                                     Executes the "ddi" KEGG API operation, searching for drug to drug interactions. Providing one entry ID reports all known interactions, while providing multiple checks if any drug pair in a given set of drugs is CI or P. If providing multiple, all entries must belong to the same database.
-    <drug-entry-ids>                        Comma separated list of drug entry IDs from the following databases: drug, ndc, or yj (e.g. id1,id2,id3 etc.). Or if equal to "-", entry IDs are read from standard input, one entry ID per line; Press CTRL+D to finalize input or pipe (e.g. cat file.txt | kegg_pull rest ddi - ...).
+    -h --help                   Show this help message.
+    info                        Executes the "info" KEGG API operation, pulling information about a KEGG database.
+    <database>                  The name of the database to pull information about or entry IDs from.
+    --test                      If set, test the request to ensure it works rather than sending it. Print True if the request would succeed and False if the request would fail. Ignores --output if this options is set along with --test.
+    --output=<output>           Path to the file (either in a directory or ZIP archive) to store the response body from the KEGG web API operation. Prints to the console if not specified. If a ZIP archive, the file path must be in the form of /path/to/zip-archive.zip:/path/to/file (e.g. ./archive.zip:file.txt).
+    list                        Executes the "list" KEGG API operation, pulling the entry IDs of the provided database.
+    get                         Executes the "get" KEGG API operation, pulling the entries of the provided entry IDs.
+    <entry-ids>                 Comma separated list of entry IDs (e.g. id1,id2,id3 etc.). Or if equal to "-", entry IDs are read from standard input, one entry ID per line; Press CTRL+D to finalize input or pipe (e.g. cat file.txt | kegg_pull rest get - ...).
+    --entry-field=<entry-field> Optional field to extract from an entry instead of the default entry info (i.e. flat file or htext in the case of brite entries).
+    find                        Executes the "find" KEGG API operation, finding entry IDs based on provided queries.
+    <keywords>                  Comma separated list of keywords to search entries with (e.g. kw1,kw2,kw3 etc.). Or if equal to "-", keywords are read from standard input, one keyword per line; Press CTRL+D to finalize input or pipe (e.g. cat file.txt | kegg_pull rest find brite - ...).
+    --formula=<formula>         Sequence of atoms in a chemical formula format to search for (e.g. "O5C7" searches for molecule entries containing 5 oxygen atoms and/or 7 carbon atoms).
+    --em=<exact-mass>           Either a single number (e.g. --em=155.5) or two numbers (e.g. --em=155.5 --em=244.4). If a single number, searches for molecule entries with an exact mass equal to that value rounded by the last decimal point. If two numbers, searches for molecule entries with an exact mass within the two values (a range).
+    --mw=<molecular-weight>     Same as --em but searches based on the molecular weight.
+    conv                        Executes the "conv" KEGG API operation, converting entry IDs from an outside database to those of a KEGG database and vice versa.
+    <kegg-database>             The name of the KEGG database from which to view equivalent outside database entry IDs.
+    <outside-database>          The name of the non-KEGG database from which to view equivalent KEGG database entry IDs.
+    entry-ids                   Perform the "conv" or "link" operation of the form that maps specific provided entry IDs to a target database.
+    link                        Executes the "link" KEGG API operation, showing the IDs of entries that are connected/related to entries of other databases.
+    <target-database>           The name of the database that the entry IDs of the source database or provided entry IDs are mapped to.
+    <source-database>           The name of the database from which cross-references are found in the target database.
+    ddi                         Executes the "ddi" KEGG API operation, searching for drug to drug interactions. Providing one entry ID reports all known interactions, while providing multiple checks if any drug pair in a given set of drugs is CI or P. If providing multiple, all entries must belong to the same database.
+    <drug-entry-ids>            Comma separated list of drug entry IDs from the following databases: drug, ndc, or yj (e.g. id1,id2,id3 etc.). Or if equal to "-", entry IDs are read from standard input, one entry ID per line; Press CTRL+D to finalize input or pipe (e.g. cat file.txt | kegg_pull rest ddi - ...).
 """
 import docopt as d
-
 from . import kegg_url as ku
 from . import rest as r
 from . import _utils as u
 
 
 def main():
-    args: dict = d.docopt(__doc__)
-    database_name: str = args['<database-name>']
-    entry_ids: str = args['<entry-ids>']
+    args = d.docopt(__doc__)
+    database: str = args['<database>']
+    entry_ids: str | list[str] = args['<entry-ids>']
+    target_database: str = args['<target-database>']
     test: bool = args['--test']
     is_binary = False
-    test_result: bool = None
-    kegg_response: r.KEGGresponse = None
+    test_result: bool | None = None
+    kegg_response: r.KEGGresponse | None = None
     kegg_rest = r.KEGGrest()
-
     if args['info']:
         if test:
-            test_result: bool = kegg_rest.test(KEGGurl=ku.InfoKEGGurl, database_name=database_name)
+            test_result = kegg_rest.test(KEGGurl=ku.InfoKEGGurl, database=database)
         else:
-            kegg_response: r.KEGGresponse = kegg_rest.info(database_name=database_name)
+            kegg_response = kegg_rest.info(database=database)
     elif args['list']:
         if test:
-            test_result: bool = kegg_rest.test(KEGGurl=ku.ListKEGGurl, database_name=database_name)
+            test_result = kegg_rest.test(KEGGurl=ku.ListKEGGurl, database=database)
         else:
-            kegg_response: r.KEGGresponse = kegg_rest.list(database_name=database_name)
+            kegg_response = kegg_rest.list(database=database)
     elif args['get']:
-        entry_ids: list = u.handle_cli_input(input_source=entry_ids)
+        entry_ids = u.parse_input_sequence(input_source=entry_ids)
         entry_field: str = args['--entry-field']
-
         if test:
-            test_result: bool = kegg_rest.test(KEGGurl=ku.GetKEGGurl, entry_ids=entry_ids, entry_field=entry_field)
+            test_result = kegg_rest.test(KEGGurl=ku.GetKEGGurl, entry_ids=entry_ids, entry_field=entry_field)
         else:
             if ku.GetKEGGurl.is_binary(entry_field=entry_field):
                 is_binary = True
-
-            kegg_response: r.KEGGresponse = kegg_rest.get(entry_ids=entry_ids, entry_field=entry_field)
+            kegg_response = kegg_rest.get(entry_ids=entry_ids, entry_field=entry_field)
     elif args['find']:
         if args['<keywords>']:
-            keywords: list = u.handle_cli_input(input_source=args['<keywords>'])
-
+            keywords = u.parse_input_sequence(input_source=args['<keywords>'])
             if test:
-                test_result: bool = kegg_rest.test(
-                    KEGGurl=ku.KeywordsFindKEGGurl, database_name=database_name, keywords=keywords
-                )
+                test_result = kegg_rest.test(KEGGurl=ku.KeywordsFindKEGGurl, database=database, keywords=keywords)
             else:
-                kegg_response: r.KEGGresponse = kegg_rest.keywords_find(database_name=database_name, keywords=keywords)
+                kegg_response = kegg_rest.keywords_find(database=database, keywords=keywords)
         else:
             formula, exact_mass, molecular_weight = u.get_molecular_attribute_args(args=args)
-
             if test:
-                test_result: bool = kegg_rest.test(
-                    KEGGurl=ku.MolecularFindKEGGurl, database_name=database_name, formula=formula,
-                    exact_mass=exact_mass, molecular_weight=molecular_weight
-                )
-            else:
-                kegg_response: r.KEGGresponse = kegg_rest.molecular_find(
-                    database_name=database_name, formula=formula, exact_mass=exact_mass, molecular_weight=molecular_weight
-                )
+                test_result = kegg_rest.test(
+                    KEGGurl=ku.MolecularFindKEGGurl, database=database, formula=formula,
+                    exact_mass=exact_mass, molecular_weight=molecular_weight)
+            else:
+                kegg_response = kegg_rest.molecular_find(
+                    database=database, formula=formula, exact_mass=exact_mass, molecular_weight=molecular_weight)
     elif args['conv']:
-        if args['--conv-target']:
-            target_database_name: str = args['--conv-target']
-            entry_ids: list = u.handle_cli_input(input_source=entry_ids)
-
+        if args['entry-ids']:
+            entry_ids = u.parse_input_sequence(input_source=entry_ids)
             if test:
-                test_result: bool = kegg_rest.test(KEGGurl=ku.EntriesConvKEGGurl, target_database_name=target_database_name, entry_ids=entry_ids)
+                test_result = kegg_rest.test(KEGGurl=ku.EntriesConvKEGGurl, target_database=target_database, entry_ids=entry_ids)
             else:
-                kegg_response: r.KEGGresponse = kegg_rest.entries_conv(
-                    target_database_name=target_database_name, entry_ids=entry_ids
-                )
+                kegg_response = kegg_rest.entries_conv(target_database=target_database, entry_ids=entry_ids)
         else:
-            kegg_database_name = args['<kegg-database-name>']
-            outside_database_name = args['<outside-database-name>']
-
+            kegg_database = args['<kegg-database>']
+            outside_database = args['<outside-database>']
             if test:
-                test_result: bool = kegg_rest.test(
-                    KEGGurl=ku.DatabaseConvKEGGurl, kegg_database_name=kegg_database_name,
-                    outside_database_name=outside_database_name
-                )
-            else:
-                kegg_response: r.KEGGresponse = kegg_rest.database_conv(
-                    kegg_database_name=kegg_database_name, outside_database_name=outside_database_name
-                )
+                test_result = kegg_rest.test(
+                    KEGGurl=ku.DatabaseConvKEGGurl, kegg_database=kegg_database, outside_database=outside_database)
+            else:
+                kegg_response = kegg_rest.database_conv(kegg_database=kegg_database, outside_database=outside_database)
     elif args['link']:
-        if args['--link-target']:
-            target_database_name: str = args['--link-target']
-            entry_ids: list = u.handle_cli_input(input_source=entry_ids)
-
+        if args['entry-ids']:
+            entry_ids = u.parse_input_sequence(input_source=entry_ids)
             if test:
-                test_result: bool = kegg_rest.test(
-                    KEGGurl=ku.EntriesLinkKEGGurl, target_database_name=target_database_name, entry_ids=entry_ids
-                )
-            else:
-                kegg_response: r.KEGGresponse = kegg_rest.entries_link(
-                    target_database_name=target_database_name, entry_ids=entry_ids
-                )
+                test_result = kegg_rest.test(KEGGurl=ku.EntriesLinkKEGGurl, target_database=target_database, entry_ids=entry_ids)
+            else:
+                kegg_response = kegg_rest.entries_link(target_database=target_database, entry_ids=entry_ids)
         else:
-            target_database_name: str = args['<target-database-name>']
-            source_database_name: str = args['<source-database-name>']
-
+            source_database: str = args['<source-database>']
             if test:
-                test_result: bool = kegg_rest.test(
-                    KEGGurl=ku.DatabaseLinkKEGGurl, target_database_name=target_database_name,
-                    source_database_name=source_database_name
-                )
-            else:
-                kegg_response: r.KEGGresponse = kegg_rest.database_link(
-                    target_database_name=target_database_name, source_database_name=source_database_name
-                )
+                test_result = kegg_rest.test(
+                    KEGGurl=ku.DatabaseLinkKEGGurl, target_database=target_database, source_database=source_database)
+            else:
+                kegg_response = kegg_rest.database_link(
+                    target_database=target_database, source_database=source_database)
     else:
-        drug_entry_ids: list = u.handle_cli_input(input_source=args['<drug-entry-ids>'])
-
+        drug_entry_ids = u.parse_input_sequence(input_source=args['<drug-entry-ids>'])
         if test:
-            test_result: bool = kegg_rest.test(KEGGurl=ku.DdiKEGGurl, drug_entry_ids=drug_entry_ids)
+            test_result = kegg_rest.test(KEGGurl=ku.DdiKEGGurl, drug_entry_ids=drug_entry_ids)
         else:
-            kegg_response: r.KEGGresponse = kegg_rest.ddi(drug_entry_ids=drug_entry_ids)
-
+            kegg_response = kegg_rest.ddi(drug_entry_ids=drug_entry_ids)
     if test:
         print(test_result)
     else:
         if kegg_response.status == r.KEGGresponse.Status.FAILED:
             raise RuntimeError(
-                f'The request to the KEGG web API failed with the following URL: {kegg_response.kegg_url.url}'
-            )
+                f'The request to the KEGG web API failed with the following URL: {kegg_response.kegg_url.url}')
         elif kegg_response.status == r.KEGGresponse.Status.TIMEOUT:
             raise RuntimeError(
-                f'The request to the KEGG web API timed out with the following URL: {kegg_response.kegg_url.url}'
-            )
-
+                f'The request to the KEGG web API timed out with the following URL: {kegg_response.kegg_url.url}')
         if is_binary:
             response_body: bytes = kegg_response.binary_body
         else:
             response_body: str = kegg_response.text_body
-
-        u.handle_cli_output(output_target=args['--output'], output_content=response_body)
+        u.print_or_save(output_target=args['--output'], output_content=response_body)
```

### Comparing `kegg_pull-2.1.0/src/kegg_pull.egg-info/PKG-INFO` & `kegg_pull-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kegg-pull
-Version: 2.1.0
+Name: kegg_pull
+Version: 3.0.0
 Summary: Pulls any and all entries from any and all KEGG databases, pulls KEGG entry IDs, and wraps all the KEGG REST API operations in both Python API and the command line.
 Home-page: https://github.com/MoseleyBioinformaticsLab/KEGGpull
 Author: Erik Huckvale
 Author-email: edhu227@g.uky.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst
@@ -19,15 +19,15 @@
 
 Documentation
 -------------
 The complete documentation for our API and CLI including tutorials can be found `here <https://moseleybioinformaticslab.github.io/kegg_pull/>`__.
 
 Installation
 ------------
-Requires python 3.8 and above.
+Requires python 3.10 and above.
 
 Install on Linux, Mac OS X
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 .. parsed-literal::
    python3 -m pip install kegg-pull
 
 Install on Windows
@@ -56,14 +56,15 @@
 ------------
 Note, the ``pip`` command will install dependencies automatically.
 
 .. parsed-literal::
    docopt
    requests
    tqdm
+   jsonschema
 
 Get the source code
 -------------------
 Code is available on GitHub: https://github.com/MoseleyBioinformaticsLab/kegg_pull.
 
 You can clone the repository via:
```

