# Comparing `tmp/areas-0.1.5.tar.gz` & `tmp/areas-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "areas-0.1.5.tar", max compression
+gzip compressed data, was "areas-0.1.6.tar", max compression
```

## Comparing `areas-0.1.5.tar` & `areas-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1091 2022-07-10 20:34:09.292968 areas-0.1.5/LICENSE
--rw-r--r--   0        0        0     8590 2023-04-05 15:11:22.994752 areas-0.1.5/README.md
--rw-r--r--   0        0        0       60 2022-09-03 17:56:00.424811 areas-0.1.5/areas/__init__.py
--rw-r--r--   0        0        0      357 2023-04-05 15:09:12.614604 areas-0.1.5/areas/config/architectures.py
--rw-r--r--   0        0        0      168 2022-09-03 17:56:00.425471 areas-0.1.5/areas/exception/__init__.py
--rw-r--r--   0        0        0      307 2022-09-03 17:56:00.425628 areas-0.1.5/areas/exception/compile_error.py
--rw-r--r--   0        0        0      162 2022-09-03 17:56:00.425742 areas-0.1.5/areas/exception/runtime_error.py
--rw-r--r--   0        0        0      100 2022-09-03 17:56:00.425867 areas-0.1.5/areas/exception/tool_file_error.py
--rw-r--r--   0        0        0     4165 2023-03-07 17:56:25.298171 areas-0.1.5/areas/main.py
--rw-r--r--   0        0        0      186 2022-09-03 17:56:00.426288 areas-0.1.5/areas/parameters/__init__.py
--rw-r--r--   0        0        0     1853 2023-04-07 13:37:32.479679 areas-0.1.5/areas/parameters/array_parameter.py
--rw-r--r--   0        0        0      807 2023-04-07 13:37:21.737957 areas-0.1.5/areas/parameters/numeric_parameter.py
--rw-r--r--   0        0        0     1243 2023-04-07 13:37:29.419047 areas-0.1.5/areas/parameters/parameter.py
--rw-r--r--   0        0        0      774 2023-04-07 13:37:26.893885 areas-0.1.5/areas/parameters/string_parameter.py
--rw-r--r--   0        0        0      254 2022-09-03 17:56:00.427442 areas-0.1.5/areas/subroutines/__init__.py
--rw-r--r--   0        0        0     3736 2022-09-03 17:56:00.427779 areas-0.1.5/areas/subroutines/array_subroutine.py
--rw-r--r--   0        0        0     3997 2022-09-03 17:56:00.428127 areas-0.1.5/areas/subroutines/mixed_subroutine.py
--rw-r--r--   0        0        0     2103 2022-09-03 17:56:00.428360 areas-0.1.5/areas/subroutines/numeric_subroutine.py
--rw-r--r--   0        0        0     1773 2022-09-03 17:56:00.428562 areas-0.1.5/areas/subroutines/subroutine.py
--rw-r--r--   0        0        0     1356 2022-09-03 17:56:00.428979 areas-0.1.5/areas/subroutines/void_subroutine.py
--rw-r--r--   0        0        0     4589 2023-04-05 12:31:43.067046 areas-0.1.5/areas/test.py
--rw-r--r--   0        0        0    11668 2023-04-07 14:05:32.675390 areas-0.1.5/areas/tester.py
--rw-r--r--   0        0        0        0 2022-09-03 17:56:00.429619 areas-0.1.5/areas/util/__init__.py
--rw-r--r--   0        0        0     3113 2023-04-07 12:58:14.476852 areas-0.1.5/areas/util/subroutine_integrity.py
--rw-r--r--   0        0        0      226 2022-09-03 17:56:00.430092 areas-0.1.5/areas/util/type_casting.py
--rw-r--r--   0        0        0      574 2023-04-07 14:12:50.133755 areas-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     9498 1970-01-01 00:00:00.000000 areas-0.1.5/setup.py
--rw-r--r--   0        0        0     9031 1970-01-01 00:00:00.000000 areas-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-07-10 20:34:09.292968 areas-0.1.6/LICENSE
+-rw-r--r--   0        0        0     8590 2023-04-05 15:11:22.994752 areas-0.1.6/README.md
+-rw-r--r--   0        0        0       60 2022-09-03 17:56:00.424811 areas-0.1.6/areas/__init__.py
+-rw-r--r--   0        0        0      357 2023-04-05 15:09:12.614604 areas-0.1.6/areas/config/architectures.py
+-rw-r--r--   0        0        0      168 2022-09-03 17:56:00.425471 areas-0.1.6/areas/exception/__init__.py
+-rw-r--r--   0        0        0      307 2022-09-03 17:56:00.425628 areas-0.1.6/areas/exception/compile_error.py
+-rw-r--r--   0        0        0      162 2022-09-03 17:56:00.425742 areas-0.1.6/areas/exception/runtime_error.py
+-rw-r--r--   0        0        0      100 2022-09-03 17:56:00.425867 areas-0.1.6/areas/exception/tool_file_error.py
+-rw-r--r--   0        0        0     4165 2023-03-07 17:56:25.298171 areas-0.1.6/areas/main.py
+-rw-r--r--   0        0        0      186 2022-09-03 17:56:00.426288 areas-0.1.6/areas/parameters/__init__.py
+-rw-r--r--   0        0        0     1853 2023-04-07 13:37:32.479679 areas-0.1.6/areas/parameters/array_parameter.py
+-rw-r--r--   0        0        0      807 2023-04-07 13:37:21.737957 areas-0.1.6/areas/parameters/numeric_parameter.py
+-rw-r--r--   0        0        0     1243 2023-04-07 13:37:29.419047 areas-0.1.6/areas/parameters/parameter.py
+-rw-r--r--   0        0        0      774 2023-04-07 13:37:26.893885 areas-0.1.6/areas/parameters/string_parameter.py
+-rw-r--r--   0        0        0      254 2022-09-03 17:56:00.427442 areas-0.1.6/areas/subroutines/__init__.py
+-rw-r--r--   0        0        0     3736 2022-09-03 17:56:00.427779 areas-0.1.6/areas/subroutines/array_subroutine.py
+-rw-r--r--   0        0        0     3997 2022-09-03 17:56:00.428127 areas-0.1.6/areas/subroutines/mixed_subroutine.py
+-rw-r--r--   0        0        0     2103 2022-09-03 17:56:00.428360 areas-0.1.6/areas/subroutines/numeric_subroutine.py
+-rw-r--r--   0        0        0     1773 2022-09-03 17:56:00.428562 areas-0.1.6/areas/subroutines/subroutine.py
+-rw-r--r--   0        0        0     1356 2022-09-03 17:56:00.428979 areas-0.1.6/areas/subroutines/void_subroutine.py
+-rw-r--r--   0        0        0     4589 2023-04-05 12:31:43.067046 areas-0.1.6/areas/test.py
+-rw-r--r--   0        0        0    12042 2023-04-07 21:45:10.022395 areas-0.1.6/areas/tester.py
+-rw-r--r--   0        0        0        0 2022-09-03 17:56:00.429619 areas-0.1.6/areas/util/__init__.py
+-rw-r--r--   0        0        0     1281 2023-04-07 22:04:30.099795 areas-0.1.6/areas/util/parse_errors.py
+-rw-r--r--   0        0        0     3113 2023-04-07 12:58:14.476852 areas-0.1.6/areas/util/subroutine_integrity.py
+-rw-r--r--   0        0        0      226 2022-09-03 17:56:00.430092 areas-0.1.6/areas/util/type_casting.py
+-rw-r--r--   0        0        0      574 2023-04-07 22:06:13.092644 areas-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     9498 1970-01-01 00:00:00.000000 areas-0.1.6/setup.py
+-rw-r--r--   0        0        0     9031 1970-01-01 00:00:00.000000 areas-0.1.6/PKG-INFO
```

### Comparing `areas-0.1.5/LICENSE` & `areas-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `areas-0.1.5/README.md` & `areas-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `areas-0.1.5/areas/main.py` & `areas-0.1.6/areas/main.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.5/areas/parameters/array_parameter.py` & `areas-0.1.6/areas/parameters/array_parameter.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.5/areas/parameters/numeric_parameter.py` & `areas-0.1.6/areas/parameters/numeric_parameter.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.5/areas/parameters/parameter.py` & `areas-0.1.6/areas/parameters/parameter.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.5/areas/parameters/string_parameter.py` & `areas-0.1.6/areas/parameters/string_parameter.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.5/areas/subroutines/array_subroutine.py` & `areas-0.1.6/areas/subroutines/array_subroutine.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.5/areas/subroutines/mixed_subroutine.py` & `areas-0.1.6/areas/subroutines/mixed_subroutine.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.5/areas/subroutines/numeric_subroutine.py` & `areas-0.1.6/areas/subroutines/numeric_subroutine.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.5/areas/subroutines/subroutine.py` & `areas-0.1.6/areas/subroutines/subroutine.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.5/areas/subroutines/void_subroutine.py` & `areas-0.1.6/areas/subroutines/void_subroutine.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.5/areas/test.py` & `areas-0.1.6/areas/test.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.5/areas/tester.py` & `areas-0.1.6/areas/tester.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from shutil import rmtree as delete_dir
 from zipfile import ZipFile as unzip
 
 import unidecode
 
 from areas.config.architectures import ARCHITECTURES
 from areas.exception import *
+from areas.util.parse_errors import parse_compilation_errors
 
 
 class Tester:
     """Evaluator class that grades student's submissions based on test input/output comparison and optional code scoring"""
 
     def __init__(self, subroutines, test_suite, cmd_line_args=None, grading_folder=None,
                  feedback_folder=None, float_threshold=None, timeout=None, save_to_file=True):
@@ -247,14 +248,22 @@
                 tests_list.append(test_object)
 
             subroutine_object['compiled'] = compiled
 
             if not compiled:
                 subroutine_object['compile_output'] = compile_output
 
+                compilation_warnings, compilation_errors = parse_compilation_errors(
+                    compile_output)
+
+                subroutine_object['compilation_errors'] = {
+                    'warnings': compilation_warnings,
+                    'errors': compilation_errors
+                }
+
             subroutine_object['ok'] = compiled and all_tests_passed
             subroutine_object['passed_count'] = passed
             subroutine_object['test_count'] = len(outputs)
             subroutine_object['score'] = float(Decimal(score) / 1000000)
             subroutine_object['tests'] = tests_list
 
             subroutine_list.append(subroutine_object)
```

### Comparing `areas-0.1.5/areas/util/subroutine_integrity.py` & `areas-0.1.6/areas/util/subroutine_integrity.py`

 * *Files identical despite different names*

### Comparing `areas-0.1.5/pyproject.toml` & `areas-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "areas"
-version = "0.1.5"
+version = "0.1.6"
 description = "ARM64 and RISC-V (extensible) assessment system"
 authors = ["Luis Tavares <luistavares10@outlook.pt>"]
 repository = "https://github.com/luist18/areasear"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "areas"}]
```

### Comparing `areas-0.1.5/setup.py` & `areas-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ['PyYAML>=6.0,<7.0', 'Unidecode>=1.3.4,<2.0.0', 'pytest>=7.2.0,<8.0.0']
 
 entry_points = \
 {'console_scripts': ['test = scripts:test']}
 
 setup_kwargs = {
     'name': 'areas',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'ARM64 and RISC-V (extensible) assessment system',
     'long_description': '# areas<!-- omit in toc -->\n\n[![GitHub license](https://img.shields.io/github/license/luist18/areas?color=blue)](https://github.com/luist18/areas/blob/main/LICENSE)\n\n**A**RM64 and **R**ISC-V (**e**xtensible) **A**ssessment **S**ystem.\n\n*areas* is originally a fork from [João Damas\'](https://github.com/cyrilico) [Automatic Observation and (grade) Calculation for (subroutine) Operations tool](https://github.com/cyrilico/aoco-code-correction). It is a tool to automate student\'s grading in the assignments done during the Microprocessor and Personal Computers course unit.\n\n## Differences with the original tool<!-- omit in toc -->\n\nTo ease the communication between the backend server and the tool the output demanded changes. Output `.txt` and `.csv` files are now combined in a more complete `.json` file. Structure of the `.zip` input file is simplified. Unsupported data types such as long and double are now supported. A new input parameter - weight - is introduced.\n\n---\n\n## Table of contents<!-- omit in toc -->\n\n- [1. Installation](#1-installation)\n- [2. Developing](#2-developing)\n- [3. Running](#3-running)\n- [4. Usage](#4-usage)\n- [5. File syntax and structure](#5-file-syntax-and-structure)\n  - [5.1. Available data types](#51-available-data-types)\n    - [5.1.1. Primitive data types](#511-primitive-data-types)\n    - [5.1.2. Array data types](#512-array-data-types)\n  - [5.2. subroutines.yaml](#52-subroutinesyaml)\n  - [5.3. tests.yaml](#53-testsyaml)\n  - [5.4. submission.zip](#54-submissionzip)\n- [6. Results](#6-results)\n\n## 1. Installation\n\nUsing Docker:\n\n```bash\ndocker pull luist188/areas\n```\n\n## 2. Developing\n\nTo develop the tool you must setup a Docker development environment to ease the dependencies installation and setup an isolated environment.\n\n1. Build the Docker development image:\n\n   ```bash\n   docker build -f Dockerfile.dev -t areas .\n   ```\n\n2. Run the image with the shared folder:\n\n   ```bash\n   docker run -it -v $(pwd):/usr/app areas\n   ```\n\nNote: if you are running MacOS with the M1 (or superior) chip you must add `--platform linux/x86_64` to `docker build` and `docker run`.\n\n## 3. Running\n\n1. Place the input files inside any directory.\n2. Run the image with a shared volume pointing to the input directory: `docker run -v input:destination -it luist188/areas` (you can learn more about `docker run` usage [here](https://docs.docker.com/engine/reference/run/))\n3. Run the alias command (assure you are using `/bin/bash`) `areas` or run `python main.py` in the tool\'s source.\n\n## 4. Usage\n\n```console\n$ areas [-h] -sr SR -t T -sm SM [SM ...] [-gfd GFD] [-ffd FFD] [-grf GRF] [-tout TOUT] [-fpre FPRE]\n\n$ areas [args]\n\nOptions:\n  --help, -h                Show help                                         [boolean]\n  -sr <subroutines.yaml>    .yaml file containing subroutine declaration      [required] [string]\n  -t <tests.yaml>           .yaml file containing the test cases              [required] [string]\n  -sm <submission.zip...>   .zip files containing user submission             [required] [string array]\n  -gfd <directory>          path to the directory to store temporary files\n    (e.g., compiled binaries)                                                 [default:grading] [string]\n  -ffd <directory>          path to the directory to store the grading for\n    each submission                                                           [default:feedback] [string]\n  -tout <timeout>           float timeout value                               [default:2.0] [float]\n  -fpre <precision>         floating point threshold for comparing floating\n    points in test cases                                                      [default:1e-6] [float]\n```\n\n## 5. File syntax and structure\n\n### 5.1. Available data types\n\n#### 5.1.1. Primitive data types\n\n- `int`\n- `long`\n- `float`\n- `double`\n- `char`\n- `chari` (char represented as an unsgined intenger - similar to char but has to be used when printed characters are not ASCII characters)\n\n#### 5.1.2. Array data types\n\n- `char*/string`\n- `array int`\n- `array long`\n- `array float`\n- `array double`\n- `array char`\n- `array chari`\n\n### 5.2. subroutines.yaml\n\nThe input file for the subroutine declaration has to follow a specific structure and syntax described as follows:\n\n```yaml\nfoo: \n  params: \n    - int\n    - array char\n    - array int\n    - array int\n  return: \n    - int\n    - array int\n\nbar: \n  params: \n    - long\n  return: \n    - long\n```\n\nEach subroutine has an optional parameter to define the subroutine architecture, the syntax is as follows:\n\n```yaml\nfoo: \n  architecture: arm\n  params: \n    - int\n    - array char\n    - array int\n    - array int\n  return: \n    - int\n    - array int\n```\n\nBy default, if the architecture parameter is omitted, the system will assume ARM64 as the subroutine architecture. The available architectures are the following:\n\n- `arm` - ARM64 architecture\n- `riscv` - RISC-V architecture\n\nThe subroutine name has to match the `.s` to test and is case insensitive. Thus, the subroutine `foo` or `bar` is going to check any `.s` file that matches its name case insensitive. All subroutines must contain an array of parameters, `params`, and an array of returns, `return`.\n\n### 5.3. tests.yaml\n\nThe input file for the test cases declaration has to follow a specific structure and syntax described as follows:\n\n```yaml\nbar:\n  - inputs:\n    - 6\n    outputs: \n    - 36\n    weight: 0.5\n  - inputs:\n    - 5\n    outputs: \n    - 25\n    weight: 0.5\n```\n\nThe root declaration of a test case must match the name declared in the `subroutines.yaml` file. Test cases have an array of inputs that has a list of outputs and a test weight. The sum of the test weights must be 1.0.\n\n### 5.4. submission.zip\n\nThe submission `zip` file must contain a `.s` file in its root. For example, for the subroutine `foo` and `bar` the `zip` structure should be as follows:\n\n```tree\nsubmission.zip\n├── foo.s\n└── bar.s\n```\n\n## 6. Results\n\nFor each submission file a `.json` file is created in the feedback directory with the same name of the `.zip` file. The file contains all information about compilation status and test cases. In addition, a simplified version of the result of all submissions is created in a `result.json`. The content of the files look as follows:\n\nFile **submission.json**\n\n```json\n[\n    {\n        "name": "foo",\n        "compiled": true,\n        "ok": true,\n        "passed_count": 2,\n        "test_count": 2,\n        "score": 1,\n        "tests": [\n            {\n                "weight": 1,\n                "run": true,\n                "input": [\n                    6,\n                    ["-", "+", "+", "-", "-", "+"],\n                    [1, 2, 3, 0, 1, -25],\n                    [13, 2, 8, 4, 5, 25]\n                ],\n                "output": [\n                    "0",\n                    ["12", "4", "11", "4", "4", "0"]\n                ],\n                "passed": true\n            }\n        ]\n    },\n    {\n        "name": "bar",\n        "compiled": true,\n        "ok": true,\n        "passed_count": 2,\n        "test_count": 2,\n        "score": 1,\n        "tests": [\n            {\n                "weight": 0.5,\n                "run": true,\n                "input": [\n                    6\n                ],\n                "output": [\n                    "36"\n                ],\n                "passed": true\n            },\n            {\n                "weight": 0.5,\n                "run": true,\n                "input": [\n                    5\n                ],\n                "output": [\n                    "25"\n                ],\n                "passed": true\n            }\n        ]\n    }\n]\n```\n\nFile **result.json**\n\n```json\n[\n    {\n        "submission_name": "submission",\n        "subroutines": [\n            {\n                "name": "foo",\n                "score": 0\n            },\n            {\n                "name": "bar",\n                "score": 0.5\n            }\n        ]\n    },\n    {\n        "submission_name": "submission2",\n        "subroutines": [\n            {\n                "name": "foo",\n                "score": 1\n            },\n            {\n                "name": "bar",\n                "score": 1\n            }\n        ]\n    }\n]\n```\n\n## License<!-- omit in toc -->\n\n[MIT](https://choosealicense.com/licenses/mit/)\n',
     'author': 'Luis Tavares',
     'author_email': 'luistavares10@outlook.pt',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/luist18/areasear',
```

### Comparing `areas-0.1.5/PKG-INFO` & `areas-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: areas
-Version: 0.1.5
+Version: 0.1.6
 Summary: ARM64 and RISC-V (extensible) assessment system
 Home-page: https://github.com/luist18/areasear
 License: MIT
 Author: Luis Tavares
 Author-email: luistavares10@outlook.pt
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

