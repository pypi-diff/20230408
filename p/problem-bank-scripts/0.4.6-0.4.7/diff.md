# Comparing `tmp/problem_bank_scripts-0.4.6.tar.gz` & `tmp/problem_bank_scripts-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problem_bank_scripts-0.4.6.tar", max compression
+gzip compressed data, was "problem_bank_scripts-0.4.7.tar", max compression
```

## Comparing `problem_bank_scripts-0.4.6.tar` & `problem_bank_scripts-0.4.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.4.6/LICENSE
--rw-r--r--   0        0        0     1244 2021-05-17 01:13:34.351180 problem_bank_scripts-0.4.6/README.md
--rw-r--r--   0        0        0     1052 2022-09-18 02:50:37.715098 problem_bank_scripts-0.4.6/pyproject.toml
--rw-r--r--   0        0        0       59 2022-09-18 02:50:48.267616 problem_bank_scripts-0.4.6/src/problem_bank_scripts/__init__.py
--rw-r--r--   0        0        0    13476 2021-08-13 04:07:58.134898 problem_bank_scripts-0.4.6/src/problem_bank_scripts/prairielearn.py
--rw-r--r--   0        0        0    40322 2022-09-18 02:49:50.750142 problem_bank_scripts-0.4.6/src/problem_bank_scripts/problem_bank_scripts.py
--rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.4.6/src/problem_bank_scripts/qti_export.py
--rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.4.6/src/problem_bank_scripts/webwork_to_md.py
--rw-r--r--   0        0        0     2263 2022-09-18 02:51:53.946469 problem_bank_scripts-0.4.6/setup.py
--rw-r--r--   0        0        0     2318 2022-09-18 02:51:53.946679 problem_bank_scripts-0.4.6/PKG-INFO
+-rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.4.7/LICENSE
+-rw-r--r--   0        0        0     1244 2021-05-17 01:13:34.351180 problem_bank_scripts-0.4.7/README.md
+-rw-r--r--   0        0        0     1052 2023-04-07 23:27:39.750468 problem_bank_scripts-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-04-07 23:28:12.952165 problem_bank_scripts-0.4.7/src/problem_bank_scripts/__init__.py
+-rw-r--r--   0        0        0    13476 2021-08-13 04:07:58.134898 problem_bank_scripts-0.4.7/src/problem_bank_scripts/prairielearn.py
+-rw-r--r--   0        0        0    40343 2023-04-07 23:29:22.781343 problem_bank_scripts-0.4.7/src/problem_bank_scripts/problem_bank_scripts.py
+-rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.4.7/src/problem_bank_scripts/qti_export.py
+-rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.4.7/src/problem_bank_scripts/webwork_to_md.py
+-rw-r--r--   0        0        0     2263 2023-04-07 23:30:53.100157 problem_bank_scripts-0.4.7/setup.py
+-rw-r--r--   0        0        0     2318 2023-04-07 23:30:53.100387 problem_bank_scripts-0.4.7/PKG-INFO
```

### Comparing `problem_bank_scripts-0.4.6/README.md` & `problem_bank_scripts-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.4.6/pyproject.toml` & `problem_bank_scripts-0.4.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "problem_bank_scripts"
-version = "0.4.6"
+version = "0.4.7"
 description = "A package with useful functions to convert between different problem bank formats."
 authors = ["Open Problem Bank Team"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://problem_bank_scripts.readthedocs.io/en/latest/"
 homepage = "https://github.com/open-resources/problem_bank_scripts"
 repository = "https://github.com/open-resources/problem_bank_scripts"
```

### Comparing `problem_bank_scripts-0.4.6/src/problem_bank_scripts/prairielearn.py` & `problem_bank_scripts-0.4.7/src/problem_bank_scripts/prairielearn.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.4.6/src/problem_bank_scripts/problem_bank_scripts.py` & `problem_bank_scripts-0.4.7/src/problem_bank_scripts/problem_bank_scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -817,15 +817,15 @@
         header.pop("server", None)
 
         # Remove correct answers from the data2 dict
         data2_sanitized = defdict_to_dict(data2, {})
         data2_sanitized = remove_correct_answers(data2_sanitized)
 
         # Update the YAML header to add substitutions
-        header.update({"substitutions": defdict_to_dict(data2_sanitized, {})})
+        header.update({"myst": {"substitutions": defdict_to_dict(data2_sanitized, {})} })
 
         # Update the YAML header to add substitutions, unsort it, and process for file
         header_yml = yaml.dump(header, sort_keys=False, allow_unicode=True)
 
         # Write the YAML to a file
         output_path.parent.mkdir(parents=True, exist_ok=True)
         output_path.write_text(
@@ -845,15 +845,15 @@
             + "\n## Attribution\n\n"
             + process_attribution(header.get("attribution")),
             encoding="utf8",
         )
 
     else:
         # Update the YAML header to add substitutions
-        header.update({"substitutions": defdict_to_dict(data2, {})})
+        header.update({"myst": {"substitutions": defdict_to_dict(data2, {})}})
 
         # return {'header':header,
         #         'body_parts':body_parts,
         #         'output_path':output_path}
 
         # Update the YAML header to add substitutions, unsort it, and process for file
         header_yml = yaml.dump(header, sort_keys=False, allow_unicode=True)
```

### Comparing `problem_bank_scripts-0.4.6/src/problem_bank_scripts/webwork_to_md.py` & `problem_bank_scripts-0.4.7/src/problem_bank_scripts/webwork_to_md.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.4.6/setup.py` & `problem_bank_scripts-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'numpy>=1.22,<2.0',
  'pandas>=1.2.4,<2.0.0',
  'problem-bank-helpers>=0.1.12,<0.2.0',
  'sympy>=1.8,<2.0']
 
 setup_kwargs = {
     'name': 'problem-bank-scripts',
-    'version': '0.4.6',
+    'version': '0.4.7',
     'description': 'A package with useful functions to convert between different problem bank formats.',
     'long_description': '# Problem Bank Scripts \n\n[![Python](https://img.shields.io/badge/python-3.9-blue)]()\n[![codecov](https://codecov.io/gh/open-resources/problem_bank_scripts/branch/main/graph/badge.svg)](https://codecov.io/gh/open-resources/problem_bank_scripts)\n[![Documentation Status](https://readthedocs.org/projects/problem_bank_scripts/badge/?version=latest)](https://problem_bank_scripts.readthedocs.io/en/latest/?badge=latest)\n\n\n## Installation\n\n```bash\n$ pip install -i https://test.pypi.org/simple/ problem_bank_scripts\n```\n\n## Features\n\n- TODO\n\n## Dependencies\n\n- TODO\n\n## Usage\n\n- TODO\n\n## Documentation\n\nThe official documentation is hosted on Read the Docs: https://problem_bank_scripts.readthedocs.io/en/latest/\n\n## Contributors\n\nWe welcome and recognize all contributions. You can see a list of current contributors in the [contributors tab](https://github.com/open-resources/problem_bank_scripts/graphs/contributors).\n\n### Credits\n\nThis package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).\n',
     'author': 'Open Problem Bank Team',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/open-resources/problem_bank_scripts',
```

### Comparing `problem_bank_scripts-0.4.6/PKG-INFO` & `problem_bank_scripts-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: problem-bank-scripts
-Version: 0.4.6
+Version: 0.4.7
 Summary: A package with useful functions to convert between different problem bank formats.
 Home-page: https://github.com/open-resources/problem_bank_scripts
 License: MIT
 Author: Open Problem Bank Team
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

