# Comparing `tmp/psdm_qs_cli-0.3.5.tar.gz` & `tmp/psdm_qs_cli-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdm_qs_cli-0.3.5.tar", last modified: Fri May  6 22:25:50 2022, max compression
+gzip compressed data, was "psdm_qs_cli-0.3.6.tar", last modified: Tue Apr  4 19:54:20 2023, max compression
```

## Comparing `psdm_qs_cli-0.3.5.tar` & `psdm_qs_cli-0.3.6.tar`

### file list

```diff
@@ -1,23 +1,48 @@
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-05-06 22:25:50.060942 psdm_qs_cli-0.3.5/
--rw-r--r--   0 klauer   (1318172782) 1704612529     1065 2020-03-17 00:29:19.000000 psdm_qs_cli-0.3.5/LICENSE
--rw-r--r--   0 klauer   (1318172782) 1704612529       95 2021-01-15 18:05:21.000000 psdm_qs_cli-0.3.5/MANIFEST.in
--rw-r--r--   0 klauer   (1318172782) 1704612529      304 2022-05-06 22:25:50.061139 psdm_qs_cli-0.3.5/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529      205 2022-05-06 22:23:02.000000 psdm_qs_cli-0.3.5/README.md
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-05-06 22:25:50.062371 psdm_qs_cli-0.3.5/psdm_qs_cli/
--rwxr-xr-x   0 klauer   (1318172782) 1704612529     3128 2022-05-06 22:23:02.000000 psdm_qs_cli-0.3.5/psdm_qs_cli/QSGenerateExcelSpreadSheet.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2170 2021-01-15 18:05:21.000000 psdm_qs_cli-0.3.5/psdm_qs_cli/QSGenerateJSON.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    15103 2022-05-06 22:23:02.000000 psdm_qs_cli-0.3.5/psdm_qs_cli/QuestionnaireClient.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      161 2022-05-06 22:23:02.000000 psdm_qs_cli-0.3.5/psdm_qs_cli/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      497 2022-05-06 22:25:50.062475 psdm_qs_cli-0.3.5/psdm_qs_cli/_version.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-05-06 22:25:50.060504 psdm_qs_cli-0.3.5/psdm_qs_cli.egg-info/
--rw-r--r--   0 klauer   (1318172782) 1704612529      304 2022-05-06 22:25:49.000000 psdm_qs_cli-0.3.5/psdm_qs_cli.egg-info/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529      480 2022-05-06 22:25:49.000000 psdm_qs_cli-0.3.5/psdm_qs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        1 2022-05-06 22:25:49.000000 psdm_qs_cli-0.3.5/psdm_qs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      146 2022-05-06 22:25:49.000000 psdm_qs_cli-0.3.5/psdm_qs_cli.egg-info/entry_points.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        1 2020-03-17 17:59:43.000000 psdm_qs_cli-0.3.5/psdm_qs_cli.egg-info/not-zip-safe
--rw-r--r--   0 klauer   (1318172782) 1704612529       32 2022-05-06 22:25:49.000000 psdm_qs_cli-0.3.5/psdm_qs_cli.egg-info/requires.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       12 2022-05-06 22:25:49.000000 psdm_qs_cli-0.3.5/psdm_qs_cli.egg-info/top_level.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       32 2022-05-06 22:23:02.000000 psdm_qs_cli-0.3.5/requirements.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      181 2022-05-06 22:25:50.061675 psdm_qs_cli-0.3.5/setup.cfg
--rw-r--r--   0 klauer   (1318172782) 1704612529      784 2022-05-06 22:23:02.000000 psdm_qs_cli-0.3.5/setup.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    80044 2022-05-06 22:23:02.000000 psdm_qs_cli-0.3.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:54:20.217014 psdm_qs_cli-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:54:20.205014 psdm_qs_cli-0.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:54:20.209014 psdm_qs_cli-0.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1167 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3032 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-04-04 19:54:20.217014 psdm_qs_cli-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:54:20.209014 psdm_qs_cli-0.3.6/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      637 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:54:20.209014 psdm_qs_cli-0.3.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:54:20.213014 psdm_qs_cli-0.3.6/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:54:20.213014 psdm_qs_cli-0.3.6/psdm_qs_cli/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3123 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/psdm_qs_cli/QSGenerateExcelSpreadSheet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/psdm_qs_cli/QSGenerateJSON.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15081 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/psdm_qs_cli/QuestionnaireClient.py
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/psdm_qs_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-04 19:54:20.000000 psdm_qs_cli-0.3.6/psdm_qs_cli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/psdm_qs_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:54:20.217014 psdm_qs_cli-0.3.6/psdm_qs_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-04-04 19:54:20.000000 psdm_qs_cli-0.3.6/psdm_qs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-04-04 19:54:20.000000 psdm_qs_cli-0.3.6/psdm_qs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-04 19:54:20.000000 psdm_qs_cli-0.3.6/psdm_qs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-04 19:54:20.000000 psdm_qs_cli-0.3.6/psdm_qs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-04-04 19:54:20.000000 psdm_qs_cli-0.3.6/psdm_qs_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-04 19:54:20.000000 psdm_qs_cli-0.3.6/psdm_qs_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:54:20.217014 psdm_qs_cli-0.3.6/reports/
+-rw-r--r--   0 runner    (1001) docker     (122)     4716 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/reports/xray_only.json
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-04 19:54:20.217014 psdm_qs_cli-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:54:20.217014 psdm_qs_cli-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-04 19:53:48.000000 psdm_qs_cli-0.3.6/tests/test_psdm_qs_cli.py
```

### Comparing `psdm_qs_cli-0.3.5/psdm_qs_cli/QSGenerateExcelSpreadSheet.py` & `psdm_qs_cli-0.3.6/psdm_qs_cli/QSGenerateExcelSpreadSheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """
     Generate a Excel spreadsheet with data from a run.
     :param: qs - A Questionnaire client
     :run: The number number/name; this is a string like run15 which is what the
         questionnaire uses in its URL
     """
     column2Names = [("proposal_id", "Proposal")]
-    with open(attributes_file, "r") as f:
+    with open(attributes_file) as f:
         attrs = json.load(f)
         column2Names.extend((x["attr"], x["label"]) for x in attrs)
 
     wb = Workbook()
     ws = wb.active
     ws.title = run
     fontStyle = Font(name="Times New Roman", size=12, color=colors.BLACK)
```

### Comparing `psdm_qs_cli-0.3.5/psdm_qs_cli/QSGenerateJSON.py` & `psdm_qs_cli-0.3.6/psdm_qs_cli/QSGenerateJSON.py`

 * *Files identical despite different names*

### Comparing `psdm_qs_cli-0.3.5/psdm_qs_cli/QuestionnaireClient.py` & `psdm_qs_cli-0.3.6/psdm_qs_cli/QuestionnaireClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 """
 Various web service calls to the Questionnaire backend to get data for reporting.
 """
 import datetime
 import getpass
 import logging
 from functools import partial
+from urllib.parse import urlparse
 
 import requests
-from six.moves.urllib.parse import urlparse
 
 logger = logging.getLogger(__name__)
 
 try:
     from krtc import KerberosTicket
 except ImportError:
     KerberosTicket = None
@@ -148,42 +148,42 @@
             for belocid, repid in {
                 "hutch-be-top-d": "Be-TOP",
                 "hutch-be-mid-d": "Be-MID",
                 "hutch-be-bot-d": "Be-BTM",
                 "hutch-be-sam-d": "Be-AIR",
             }.items():
                 tpls = sorted(
-                    [
+                    (
                         (
                             c["id"]
                             .split("-")[3]
                             .replace("d1", "1D")
                             .replace("d2", "2D"),
                             c["id"].split("-")[4],
                             "x",
                             c["val"],
                         )
                         for c in proposalData.get("hutch", [])
                         if c["id"].startswith(belocid) and int(c["val"])
-                    ],
+                    ),
                     key=lambda x: (x[0], int(x[1])),
                 )
                 if tpls:
                     h_or_v = "".join(
                         [
                             hzvr.get(x["val"], "VERT/HORZ")
                             for x in proposalData["hutch"]
                             if x["id"] == belocid.replace("-d", "-orientation")
                         ]
                     )
                     tpls = [x + (h_or_v,) if x[0] == "1D" else x for x in tpls]
-                    ret[repid] = "  ".join(("".join(_) for _ in tpls))
+                    ret[repid] = "  ".join("".join(_) for _ in tpls)
             combined_be = "\n".join(
                 [
-                    "{}:{}".format(fnl_be_attr, ret[fnl_be_attr])
+                    f"{fnl_be_attr}:{ret[fnl_be_attr]}"
                     for fnl_be_attr in ["Be-TOP", "Be-MID", "Be-BTM", "Be-AIR"]
                     if fnl_be_attr in ret
                 ]
             )
             if combined_be:
                 ret["Be-All Beryllium Lens Stack Recipes"] = combined_be
         else:
```

