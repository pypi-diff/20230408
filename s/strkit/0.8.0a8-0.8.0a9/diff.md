# Comparing `tmp/strkit-0.8.0a8.tar.gz` & `tmp/strkit-0.8.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strkit-0.8.0a8.tar", last modified: Mon Mar 27 14:00:04 2023, max compression
+gzip compressed data, was "strkit-0.8.0a9.tar", last modified: Tue Mar 28 19:12:30 2023, max compression
```

## Comparing `strkit-0.8.0a8.tar` & `strkit-0.8.0a9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:04.154816 strkit-0.8.0a8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-27 13:59:40.000000 strkit-0.8.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-27 13:59:40.000000 strkit-0.8.0a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-03-27 14:00:04.154816 strkit-0.8.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-03-27 13:59:40.000000 strkit-0.8.0a8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-27 13:59:40.000000 strkit-0.8.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 14:00:04.154816 strkit-0.8.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-27 13:59:40.000000 strkit-0.8.0a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:04.146816 strkit-0.8.0a8/strkit/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:04.150816 strkit-0.8.0a8/strkit/call/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12728 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/allele.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:04.150816 strkit-0.8.0a8/strkit/call/caller/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/caller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/caller/align_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    37765 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/caller/call_locus.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/caller/call_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/caller/cigar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/caller/realign.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/caller/repeats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/caller/snvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/caller/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/caller/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/re_caller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/repeathmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/straglr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/call/tandem_genotypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:04.150816 strkit-0.8.0a8/strkit/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/catalog/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:04.150816 strkit-0.8.0a8/strkit/convert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/convert/_bed_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/convert/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/convert/expansionhunter.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/convert/gangstr.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/convert/hipstr.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/convert/straglr.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/convert/tandem_genotypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    24340 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:04.154816 strkit-0.8.0a8/strkit/mi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/mi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/mi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/mi/expansionhunter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/mi/gangstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/mi/repeathmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    23963 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/mi/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/mi/straglr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/mi/strkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/mi/tandem_genotypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/mi/vcf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:04.154816 strkit-0.8.0a8/strkit/viz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/viz/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:04.154816 strkit-0.8.0a8/strkit/viz/static/
--rw-r--r--   0 runner    (1001) docker     (123)   408225 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/viz/static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:04.154816 strkit-0.8.0a8/strkit/viz/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    34285 2023-03-27 13:59:40.000000 strkit-0.8.0a8/strkit/viz/templates/browser.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:00:04.146816 strkit-0.8.0a8/strkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-03-27 14:00:04.000000 strkit-0.8.0a8/strkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-27 14:00:04.000000 strkit-0.8.0a8/strkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:00:04.000000 strkit-0.8.0a8/strkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-27 14:00:04.000000 strkit-0.8.0a8/strkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-27 14:00:04.000000 strkit-0.8.0a8/strkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-27 14:00:04.000000 strkit-0.8.0a8/strkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:30.940623 strkit-0.8.0a9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-28 19:12:22.000000 strkit-0.8.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-28 19:12:22.000000 strkit-0.8.0a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-03-28 19:12:30.940623 strkit-0.8.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-03-28 19:12:22.000000 strkit-0.8.0a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-28 19:12:22.000000 strkit-0.8.0a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 19:12:30.940623 strkit-0.8.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-28 19:12:22.000000 strkit-0.8.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:30.932623 strkit-0.8.0a9/strkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:30.936623 strkit-0.8.0a9/strkit/call/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/allele.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:30.936623 strkit-0.8.0a9/strkit/call/caller/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/caller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/caller/align_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38765 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/caller/call_locus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10163 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/caller/call_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/caller/cigar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/caller/realign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/caller/repeats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/caller/snvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/caller/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/caller/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/re_caller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/repeathmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/straglr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/call/tandem_genotypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:30.936623 strkit-0.8.0a9/strkit/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/catalog/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:30.940623 strkit-0.8.0a9/strkit/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/convert/_bed_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/convert/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/convert/expansionhunter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/convert/gangstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/convert/hipstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/convert/straglr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/convert/tandem_genotypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24340 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:30.940623 strkit-0.8.0a9/strkit/mi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/mi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/mi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/mi/expansionhunter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/mi/gangstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/mi/repeathmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23963 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/mi/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/mi/straglr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/mi/strkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/mi/tandem_genotypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/mi/vcf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:30.940623 strkit-0.8.0a9/strkit/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/viz/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:30.940623 strkit-0.8.0a9/strkit/viz/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   408225 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/viz/static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:30.940623 strkit-0.8.0a9/strkit/viz/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    34285 2023-03-28 19:12:22.000000 strkit-0.8.0a9/strkit/viz/templates/browser.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:12:30.932623 strkit-0.8.0a9/strkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-03-28 19:12:30.000000 strkit-0.8.0a9/strkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-28 19:12:30.000000 strkit-0.8.0a9/strkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 19:12:30.000000 strkit-0.8.0a9/strkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-28 19:12:30.000000 strkit-0.8.0a9/strkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-28 19:12:30.000000 strkit-0.8.0a9/strkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-28 19:12:30.000000 strkit-0.8.0a9/strkit.egg-info/top_level.txt
```

### Comparing `strkit-0.8.0a8/LICENSE` & `strkit-0.8.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/PKG-INFO` & `strkit-0.8.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strkit
-Version: 0.8.0a8
+Version: 0.8.0a9
 Summary: A toolkit for analyzing variation in short(ish) tandem repeats.
 Home-page: https://github.com/davidlougheed/strkit
 Author: David Lougheed
 Author-email: david.lougheed@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `strkit-0.8.0a8/README.md` & `strkit-0.8.0a9/README.md`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/setup.py` & `strkit-0.8.0a9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     name="strkit",
     version=version,
 
     python_requires="~=3.9",
     install_requires=[
         "Flask>=2.2.2,<2.3",
         "pysam>=0.19,<0.21",
-        "numpy>=1.24.1,<=1.25",
+        "numpy>=1.23.4,<1.25",
         "parasail>=1.2.4,<1.4",
         "scikit-learn>=1.2.1,<1.3",
         "scipy>=1.10,<1.11",
         "statsmodels>=0.13.5,<0.14",
     ],
     extras_require={
         "rustdeps": [
```

### Comparing `strkit-0.8.0a8/strkit/call/allele.py` & `strkit-0.8.0a9/strkit/call/allele.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from sklearn.exceptions import ConvergenceWarning
 from sklearn.mixture import GaussianMixture
 from sklearn.preprocessing import normalize
 from warnings import simplefilter
 
 from numpy.typing import NDArray
-from typing import Iterable, Optional, TypedDict, Union
+from typing import Iterable, Literal, Optional, TypedDict, Union
 
 import strkit.constants as cc
 
 __all__ = [
     "RepeatCounts",
     "CallDict",
     "get_n_alleles",
@@ -71,24 +71,31 @@
 def fit_gmm(
     rng: np.random.Generator,
     sample: np.array,
     n_alleles: int,
     allele_filter: float,
     hq: bool,
     gm_filter_factor: int,
+    init_params: Literal["kmeans", "k-means++"] = "k-means++",  # TODO: parameterize outside
 ) -> Optional[object]:
     sample_rs = sample.reshape(-1, 1)
-    g = None
+    g: Optional[object] = None
 
     n_components = n_alleles
     while n_components > 0:
+        if n_components == 1:  # Don't need to do the full fit for a single peak, just calculate the parameters
+            g = type("", (), {})()
+            g.means_ = np.array([[np.mean(sample_rs)]])
+            g.weights_ = np.array([[1.0]])
+            g.covariances_ = np.array([[np.var(sample_rs)]])
+            return g
+
         g = GaussianMixture(
             n_components=n_components,
-            # init_params="kmeans",  TODO: parameterize
-            init_params="k-means++",
+            init_params=init_params,
             covariance_type="spherical",
             n_init=N_GM_INIT,
             random_state=rng.integers(0, 4096).item(),
         ).fit(sample_rs)
 
         # noinspection PyUnresolvedReferences
         means_and_weights = np.append(g.means_.transpose(), g.weights_.reshape(1, -1), axis=0)
@@ -110,16 +117,16 @@
             mw_filter_2 = means_and_weights[1, :] > (1 / (gm_filter_factor * n_alleles))
         else:
             mw_filter_2 = means_and_weights[1, :] > np.finfo(np.float32).eps
 
         mw_filter = mw_filter_1 & mw_filter_2
         n_useless = np.size(mw_filter) - np.count_nonzero(mw_filter)
         if not n_useless:
-            # No useless components left to remove, so escape
-            break
+            # No useless components left to remove, so return the GMM
+            return g
         n_components -= n_useless
 
     return g
 
 
 class CallDict(TypedDict):
     call: Union[NDArray[np.int32], NDArray[np.float]]
@@ -163,22 +170,31 @@
     assert fwd_strand_reads.shape == fwd_strand_weights.shape
     assert rev_strand_reads.shape == rev_strand_weights.shape
 
     combined_reads = np.concatenate((fwd_strand_reads, rev_strand_reads), axis=None)
     combined_weights = np.concatenate((fwd_strand_weights, rev_strand_weights), axis=None)
     combined_len = combined_reads.shape[-1]
 
-    # If the locus/allele only has one value, don't bother bootstrapping
-    if np.unique(combined_reads).shape[0] == 1:
-        logger_.debug(f"{debug_str} - skipping bootstrap for allele(s) (single value)")
-        bootstrap_iterations = 1
-
     if combined_len < min_reads:
         return None
 
+    # If the locus/allele only has one value, don't bother bootstrapping
+    if np.unique(combined_reads).shape[0] == 1:
+        logger_.debug(f"{debug_str} - skipping bootstrap / GMM fitting for allele(s) (single value)")
+        cn = combined_reads[0]
+        return {
+            "call": np.array([cn] * n_alleles),
+            "call_95_cis": np.array([[cn, cn] * n_alleles]),
+            "call_99_cis": np.array([[cn, cn] * n_alleles]),
+            "peaks": np.array([cn] * n_alleles, dtype=np.float_),
+            "peak_weights": np.array([1.0] * n_alleles) / n_alleles,
+            "peak_stdevs": np.array([0.0] * n_alleles),
+            "modal_n_peaks": 1,  # 1 peak, since we have 1 value
+        }
+
     nal = na_length_list(n_alleles)
     allele_samples = np.array(nal, dtype=np.float32)
     allele_weight_samples = np.array(nal, dtype=np.float32)
     allele_stdev_samples = np.array(nal, dtype=np.float32)
     sample_peaks = np.array([], dtype=np.int32)
 
     rng: np.random.Generator = np.random.default_rng(seed=seed)
```

### Comparing `strkit-0.8.0a8/strkit/call/caller/align_matrix.py` & `strkit-0.8.0a9/strkit/call/caller/align_matrix.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/call/caller/call_locus.py` & `strkit-0.8.0a9/strkit/call/caller/call_locus.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from strkit.call.allele import CallDict, get_n_alleles, call_alleles
 from strkit.utils import apply_or_none
 
 from .align_matrix import match_score
 from .realign import realign_read
 from .repeats import get_repeat_count, get_ref_repeat_count
-from .snvs import SNV_OUT_OF_RANGE_CHAR, get_read_snvs, calculate_useful_snvs, call_useful_snvs
+from .snvs import SNV_OUT_OF_RANGE_CHAR, get_read_snvs, calculate_useful_snvs, call_and_filter_useful_snvs
 from .types import ReadDict
 from .utils import normalize_contig, round_to_base_pos
 
 
 __all__ = [
     "call_locus",
 ]
@@ -53,15 +53,15 @@
     left_flank_coord: int,
     left_coord: int,
     right_coord: int,
     right_flank_coord: int,
     motif: str,
     motif_size: int,
     query_seq: str,
-    matched_pairs
+    matched_pairs: list[tuple[int, int]],
 ) -> tuple[int, int, int, int]:
     left_flank_end = -1
     right_flank_start = -1
     right_flank_end = -1
 
     last_idx = -1
 
@@ -166,43 +166,52 @@
     return overlapping_segments, read_lengths, chimeric_read_status
 
 
 def calculate_read_distance(
     n_reads: int,
     read_dict_items: Sequence[tuple[str, ReadDict]],
     pure_snv_peak_assignment: bool,
-    relative_cn_distance_weight_scaling: float = 0.5,  # TODO: CLI specifyable param
+    relative_cn_distance_weight_scaling_few: float = 0.5,
+    relative_cn_distance_weight_scaling_many: float = 0.1,
+    many_snvs_quantity: int = 3,
 ) -> NDArray[np.float_, np.float_]:
     """
     Calculate pairwise distance for all reads using either SNVs ONLY or a mixture of SNVs and copy number.
     :param n_reads: Number of reads.
     :param read_dict_items: Itemized read dictionary entries: (read name, read data)
     :param pure_snv_peak_assignment: Whether to use just SNVs for peak assignment
-    :param relative_cn_distance_weight_scaling: How much to weight 1-difference in CN vs SNVs
-            (indels are more erroneous in CCS)
+    :param relative_cn_distance_weight_scaling_few: How much to weight 1-difference in CN vs SNVs with few SNVs
+            available (indels are more erroneous in CCS)
+    :param relative_cn_distance_weight_scaling_many: How much to weight 1-difference in CN vs SNVs with many SNVs
+            available (indels are more erroneous in CCS)
+    :param many_snvs_quantity: How many SNVs constitutes "many" for the different weights.
     :return: The distance matrix.
     """
 
     # Initialize a distance matrix for all reads
-    distance_matrix = np.zeros((n_reads, n_reads))
+    distance_matrix = np.zeros((n_reads, n_reads), dtype=np.float_)
 
     # Loop through and compare all vs. all reads. We can skip a few indices since the distance will be symmetrical.
     for i in range(n_reads - 1):
         for j in range(i + 1, n_reads):
             r1 = read_dict_items[i][1]
             r2 = read_dict_items[j][1]
             r1_snv_u = r1["snvu"]
             r2_snv_u = r2["snvu"]
 
-            d = 0 if pure_snv_peak_assignment else abs(r1["cn"] - r2["cn"]) * relative_cn_distance_weight_scaling
-            for b1, b2 in zip(r1_snv_u, r2_snv_u):
-                if b1 == SNV_OUT_OF_RANGE_CHAR or b2 == SNV_OUT_OF_RANGE_CHAR:
-                    continue
-                if b1 != b2:
-                    d += 1
+            comparable_snvs = [
+                (b1, b2) for b1, b2 in zip(r1_snv_u, r2_snv_u)
+                if b1 != SNV_OUT_OF_RANGE_CHAR and b2 != SNV_OUT_OF_RANGE_CHAR
+            ]
+
+            d: float = float(sum(1 for b1, b2 in comparable_snvs if b1 != b2))
+            if not pure_snv_peak_assignment:  # Add in copy number distance
+                d += abs(r1["cn"] - r2["cn"]) * (
+                    relative_cn_distance_weight_scaling_many if len(comparable_snvs) >= many_snvs_quantity
+                    else relative_cn_distance_weight_scaling_few)
 
             distance_matrix[i, j] = d
             distance_matrix[j, i] = d
 
     return distance_matrix
 
 
@@ -226,44 +235,46 @@
     locus_log_str: str,
 ) -> tuple[Literal["dist", "snv", "snv+dist", "single"], Optional[dict, list[dict]]]:
     assign_method: Literal["dist", "snv", "snv+dist", "single"] = "dist"
 
     # TODO: parametrize min 'enough to do pure SNV haplotyping' thresholds
 
     read_dict_items_with_many_snvs: list[tuple[str, ReadDict]] = []
-    read_dict_items_with_some_snvs: list[tuple[str, ReadDict]] = []
-    read_dict_items_with_few_or_no_snvs: list[tuple[str, ReadDict]] = []
+    read_dict_items_with_at_least_one_snv: list[tuple[str, ReadDict]] = []
+    read_dict_items_with_no_snvs: list[tuple[str, ReadDict]] = []
 
     print_snvs = False
 
-    for rn, read in read_dict_items:
+    for read_item in read_dict_items:
+        rn, read = read_item
+
         read_useful_snv_bases = tuple(read_dict_extra[rn]["snv_bases"][bi] for bi, _pos in useful_snvs)
         non_blank_read_useful_snv_bases = [bb for bb in read_useful_snv_bases if bb != SNV_OUT_OF_RANGE_CHAR]
 
-        if (nbr := len(non_blank_read_useful_snv_bases)) >= 2:  # TODO: parametrize
-            read_dict_items_with_some_snvs.append((rn, read))
+        if nbr := len(non_blank_read_useful_snv_bases):  # TODO: parametrize
+            read_dict_items_with_at_least_one_snv.append(read_item)
             if nbr >= 3:  # TODO: parametrize
-                read_dict_items_with_many_snvs.append((rn, read))
+                read_dict_items_with_many_snvs.append(read_item)
         else:
-            read_dict_items_with_few_or_no_snvs.append((rn, read))
+            read_dict_items_with_no_snvs.append(read_item)
 
         read["snvu"] = read_useful_snv_bases  # Store read-level 'useful' SNVs
 
         if print_snvs:
-            print(rn, f"\t{read['cn']:.0f}", "\t", "".join(read_useful_snv_bases), len(non_blank_read_useful_snv_bases))
+            print(rn, f"\t{read['cn']:.0f}", "\t", "".join(read_useful_snv_bases), nbr)
 
     n_reads_with_many_snvs: int = len(read_dict_items_with_many_snvs)
     pure_snv_peak_assignment: bool = n_reads_with_many_snvs == n_reads_in_dict
 
     # TODO: parametrize: how many reads with SNV information
     min_snv_incorporation_read_portion = 0.5
     min_snv_incorporation_read_abs = 16
 
     can_incorporate_snvs: bool = pure_snv_peak_assignment or (
-        len(read_dict_items_with_some_snvs) >=
+        len(read_dict_items_with_at_least_one_snv) >=
         min(n_reads_in_dict * min_snv_incorporation_read_portion, min_snv_incorporation_read_abs)
     )
 
     if not can_incorporate_snvs:
         # TODO: How to use partial data?
         return assign_method, None
 
@@ -357,19 +368,22 @@
         # TODO: Readjust peak weights when combining or don't include
         "peak_weights": np.concatenate(tuple(cc["peak_weights"] for cc in cdd), axis=0)[peak_order],
 
         "peak_stdevs": np.concatenate(tuple(cc["peak_stdevs"] for cc in cdd), axis=0)[peak_order],
         "modal_n_peaks": n_alleles,  # # alleles = # peaks always -- if we phased using SNVs
     }
 
-    return assign_method, (
-        call_data,
-        # Called useful SNVs to add to the final return dictionary:
-        call_useful_snvs(n_alleles, read_dict, useful_snvs, peak_order, locus_log_str, logger_)
-    )
+    # Called useful SNVs to add to the final return dictionary:
+    called_useful_snvs: list[dict] = call_and_filter_useful_snvs(
+        n_alleles, read_dict, useful_snvs, peak_order, locus_log_str, logger_)
+
+    if not called_useful_snvs:  # No useful SNVs left, so revert to "dist" assignment method
+        return "dist", None
+
+    return assign_method, (call_data, called_useful_snvs)
 
 
 def call_locus(
     t_idx: int,
     t: tuple,
     bfs: tuple[AlignmentFile, ...],
     ref: FastaFile,
@@ -560,26 +574,23 @@
             if pairs_new is not None:
                 pairs = pairs_new
                 realigned = True
 
         if pairs is None:
             pairs = segment.get_aligned_pairs(matches_only=True)
 
-        # Cache aligned pairs, since it takes a lot of time to extract, and we use it for calculate_useful_snvs
-        read_pairs[rn] = pairs
-
         left_flank_start, left_flank_end, right_flank_start, right_flank_end = get_read_coords_from_matched_pairs(
             left_flank_coord,
             left_coord_adj,
             right_coord_adj,
             right_flank_coord,
             motif,
             motif_size,
             query_seq=qs,
-            matched_pairs=pairs
+            matched_pairs=pairs,
         )
 
         if any(v == -1 for v in (left_flank_start, left_flank_end, right_flank_start, right_flank_end)):
             logger_.debug(
                 f"{locus_log_str} - skipping read {rn}: could not get sufficient flanking sequence"
                 f"{' (post-realignment)' if realigned else ''}")
             continue
@@ -588,29 +599,27 @@
         if qqs.shape[0] and (m_qqs := np.mean(qqs)) < min_avg_phred:  # TODO: check flank?
             logger_.debug(
                 f"{locus_log_str} - skipping read {rn} due to low average base quality ({m_qqs:.2f} < {min_avg_phred})")
             continue
 
         # -----
 
-        tr_read_seq = qs[left_flank_end:right_flank_start]
-
         # Truncate to flank_size (plus some leeway for small indels in flanking region) to stop any expansion sequences
         # from accidentally being included in the flanking region; e.g. if the insert gets mapped onto bases outside
         # the definition coordinates.
         # The +10 here won't include any real TR region if the mapping is solid, since the flank coordinates will
         # contain a correctly-sized sequence.
 
         # TODO: wildcards in flanking region too?
-        flank_left_seq = qs[left_flank_start:left_flank_end][:flank_size+10]
-        flank_right_seq = qs[right_flank_start:right_flank_end][-(flank_size+10):]
+        flank_left_seq: str = qs[left_flank_start:left_flank_end][:flank_size+10]
+        flank_right_seq: str = qs[right_flank_start:right_flank_end][-(flank_size+10):]
 
-        tr_len = len(tr_read_seq)
-        flank_len = len(flank_left_seq) + len(flank_right_seq)
-        tr_len_w_flank = tr_len + flank_len
+        tr_len: int = right_flank_start - left_flank_end  # i.e., len(tr_read_seq)
+        flank_len: int = len(flank_left_seq) + len(flank_right_seq)
+        tr_len_w_flank: int = tr_len + flank_len
 
         tr_read_seq_wc = calculate_seq_with_wildcards(qs[left_flank_end:right_flank_start], qqs)
 
         if count_kmers != "none":
             read_kmers.clear()
             for i in range(0, tr_len - motif_size + 1):
                 read_kmers.update((tr_read_seq_wc[i:i+motif_size],))
@@ -662,14 +671,17 @@
         # Reads can show up more than once - TODO - cache this information across loci
 
         if should_incorporate_snvs:
             # Store the segment sequence in the read dict for the next go-around if we've enabled SNV incorporation,
             # in order to pass the query sequence to the get_read_snvs function with the cached ref string.
             read_dict_extra[rn]["_qs"] = qs
 
+            # Cache aligned pairs, since it takes a lot of time to extract, and we use it for calculate_useful_snvs
+            read_pairs[rn] = pairs
+
     # End of first read loop -------------------------------------------------------------------------------------------
 
     n_reads_in_dict: int = len(read_dict)
 
     call_dict_base = {
         "locus_index": t_idx,
         "contig": contig,
@@ -701,18 +713,18 @@
     call_data = {}
     # noinspection PyTypeChecker
     read_dict_items: tuple[tuple[str, ReadDict], ...] = tuple(read_dict.items())
 
     assign_method: Literal["dist", "snv", "snv+dist", "single"] = "dist"
     if n_alleles < 2:
         assign_method = "single"
-    min_snv_read_coverage: int = 10  # TODO: parametrize
+    min_snv_read_coverage: int = 8  # TODO: parametrize
 
     # LIMITATION: Currently can only use SNVs for haplotyping with haploid/diploid
-    if should_incorporate_snvs:
+    if should_incorporate_snvs and n_reads_in_dict >= min_snv_read_coverage:
         # Loop through a second time if we are using SNVs. We do a second loop rather than just using the first loop
         # in order to have collected the edges of the reference sequence we can cache for faster SNV calculation.
 
         ref_cache = ref.fetch(contig, left_most_coord, right_most_coord + 1).upper()
 
         for rn, read in read_dict_items:
             snvs = get_read_snvs(
@@ -720,17 +732,15 @@
                 right_coord_adj)
             locus_snvs.update(snvs.keys())
             read_dict_extra[rn]["snv"] = snvs
 
         # End of second read loop --------------------------------------------------------------------------------------
 
         useful_snvs: list[tuple[int, int]] = (
-            calculate_useful_snvs(n_reads_in_dict, read_dict_items, read_dict_extra, read_pairs, locus_snvs)
-            if n_reads_in_dict >= min_snv_read_coverage else []
-        )
+            calculate_useful_snvs(n_reads_in_dict, read_dict_items, read_dict_extra, read_pairs, locus_snvs))
         n_useful_snvs: int = len(useful_snvs)
 
         if not n_useful_snvs:
             logger_.debug(f"{locus_log_str} - no useful SNVs")
         else:
             am, call_res = call_alleles_with_incorporated_snvs(
                 n_alleles=n_alleles,
@@ -767,14 +777,19 @@
         #    - if we have LOTS of SNV data for the majority of reads, do assignment just using SNV data and assign
         #      reads to peaks after (random assignment if equal chance of both groups)
         #    - if we have COMPLETE SNV data (4+ for every read) we can do phasing + peak assignment just with SNVs
         #      and just call the Gaussians from the separated reads (even just calculate stdev + mean for each bootstrap
         #      iteration, which might save us some time...).
         #    - keep track of which option as 'peak_calling_method' (pcm) or something
 
+    elif n_reads_in_dict < min_snv_read_coverage:
+        logger_.debug(
+            f"{locus_log_str} - not enough coverage for SNV incorporation "
+            f"({n_reads_in_dict} < {min_snv_read_coverage})")
+
     single_or_dist_assign: bool = assign_method in ("single", "dist")
 
     if single_or_dist_assign:  # Didn't use SNVs, so call the 'old-fashioned' way - using only copy number
         # Dicts are ordered in Python; very nice :)
         rdvs = tuple(read_dict.values())
         rcns = tuple(r["cn"] for r in rdvs)
         read_cns = np.fromiter(rcns, dtype=np.float_ if fractional else np.int_)
@@ -791,15 +806,15 @@
             separate_strands=False,
             read_bias_corr_min=0,  # TODO: parametrize
             gm_filter_factor=3,  # TODO: parametrize
             hq=hq,
             force_int=not fractional,
             seed=_get_new_seed(rng),
             logger_=logger_,
-            debug_str=f"{contig}:{left_coord}-{right_coord}",
+            debug_str=locus_log_str,
         ) or {}  # Still false-y
 
     # Extract data from call_data --------------------------------------------------------------------------------------
 
     call = call_data.get("call")
 
     call_95_cis = call_data.get("call_95_cis")
@@ -810,15 +825,15 @@
     call_stdevs = call_data.get("peak_stdevs")
     call_modal_n = call_data.get("modal_n_peaks")
 
     # Assign reads to peaks and compute peak k-mers --------------------------------------------------------------------
 
     # We cannot call read-level cluster labels with >2 peaks using distance alone;
     # don't know how re-sampling has occurred.
-    call_peak_n_reads = []
+    call_peak_n_reads: list[int] = []
     peak_kmers: list[Counter] = [Counter() for _ in range(call_modal_n or 0)]
     if read_peaks_called := call_modal_n and call_modal_n <= 2:
         peaks: NDArray = call_peaks[:call_modal_n]
         stdevs: NDArray[np.float_] = call_stdevs[:call_modal_n]
         weights: NDArray[np.float_] = call_weights[:call_modal_n]
 
         allele_reads: list[list[str]] = []
```

### Comparing `strkit-0.8.0a8/strkit/call/caller/call_sample.py` & `strkit-0.8.0a9/strkit/call/caller/call_sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from datetime import datetime
 from pysam import AlignmentFile
 
 from typing import Optional, Union
 
 from strkit import __version__
 
-from strkit.exceptions import ParamError
 from strkit.json import dumps_indented, json
 from strkit.logger import logger
 
 from .call_locus import call_locus
 
 __all__ = [
     "call_sample",
@@ -183,19 +182,14 @@
     log_level: int = logging.WARNING,
     json_path: Optional[str] = None,
     indent_json: bool = False,
     output_tsv: bool = True,
     processes: int = 1,
     seed: Optional[int] = None,
 ) -> None:
-    # Check parameter validity
-
-    if incorporate_snvs and not hq:
-        raise ParamError("Cannot use --incorporate-snvs without --hq.")
-
     # Start the call timer
     start_time = datetime.now()
 
     # Get sample ID from read file(s)
 
     bfs = tuple(AlignmentFile(rf, reference_filename=reference_file) for rf in read_files)
```

### Comparing `strkit-0.8.0a8/strkit/call/caller/cigar.py` & `strkit-0.8.0a9/strkit/call/caller/cigar.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/call/caller/realign.py` & `strkit-0.8.0a9/strkit/call/caller/realign.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/call/caller/repeats.py` & `strkit-0.8.0a9/strkit/call/caller/repeats.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/call/caller/snvs.py` & `strkit-0.8.0a9/strkit/call/caller/snvs.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .types import ReadDict
 
 
 __all__ = [
     "SNV_OUT_OF_RANGE_CHAR",
     "get_read_snvs",
     "calculate_useful_snvs",
-    "call_useful_snvs",
+    "call_and_filter_useful_snvs",
 ]
 
 SNV_OUT_OF_RANGE_CHAR = "-"
 
 # TODO: annotate with rsID if file provided
 
 
@@ -93,23 +93,24 @@
 ) -> dict[int, str]:
     """
     Given a list of tuples of aligned (read pos, ref pos) pairs, this function finds non-reference SNVs which are
     surrounded by a stretch of aligned bases of a specified size on either side.
     :return: Dictionary of {position: base}
     """
 
-    snvs: dict[int, str] = {}
+    # Tried to vectorize this with numpy, and it ended up slower... oh well
 
+    snvs: dict[int, str] = {}
     for read_pos, ref_pos in pairs:
         if tr_start_pos <= ref_pos < tr_end_pos:  # base is in the tandem repeat itself; skip it
             continue
         if (read_base := query_sequence[read_pos]) != ref_seq[ref_pos - ref_coord_start]:
             snvs[ref_pos] = read_base
 
-    if len(snvs) >= too_many_snvs_threshold:  # TOO MANY, some kind of mismapping going on
+    if len(snvs) >= too_many_snvs_threshold:  # TOO MANY, some kind of mismapping going on?
         return _get_read_snvs_meticulous(
             query_sequence,
             pairs,
             ref_seq,
             ref_coord_start,
             tr_start_pos,
             tr_end_pos,
@@ -193,15 +194,15 @@
                 n_alleles_meeting_threshold += 1
         if n_alleles_meeting_threshold >= 2:
             useful_snvs.append(si)
 
     return [(si, sorted_snvs[si]) for si in useful_snvs]  # Tuples of (index in STR list, ref position)
 
 
-def call_useful_snvs(
+def call_and_filter_useful_snvs(
     n_alleles: int,
     read_dict: dict[str, ReadDict],
     useful_snvs: list[tuple[int, int]],
     peak_order: NDArray[int],
     locus_log_str: str,
     logger,
 ) -> list[dict]:
@@ -225,38 +226,54 @@
 
     for _, u_ref in useful_snvs:
         peak_base_counts[u_ref] = {p: Counter() for p in allele_range}
 
     for rn, read in read_dict.items():
         p: Optional[int] = read.get("p")
         if p is None:
+            logger.debug(f"call_useful_snvs: no peak found for read {rn}")
             continue
         for u_idx, (_, u_ref) in enumerate(useful_snvs):
             peak_base_counts[u_ref][p].update((read["snvu"][u_idx],))
 
     called_snvs: list[dict] = []
+    skipped_snvs: set[int] = set()
 
-    for u_ref, peak_counts in peak_base_counts.items():
+    for u_idx, (u_ref, peak_counts) in enumerate(peak_base_counts.items()):
         call: list[str] = []
         rs: list[int] = []
 
+        skipped: bool = False
+
         for a in allele_range:
             mc = peak_counts[a].most_common(2)
             mcc = mc[0]
             try:
                 if mcc[0] == SNV_OUT_OF_RANGE_CHAR:  # Chose most common non-uncalled value
                     mcc = mc[1]
-            except IndexError:  # - is the only value, somehow
+            except IndexError:  # '-' is the only value, somehow
                 logger.warn(
                     f"{locus_log_str} - for SNV {u_ref}, found only '{SNV_OUT_OF_RANGE_CHAR}' with {mcc[1]} reads")
                 logger.debug(f"{locus_log_str} - for SNV {u_ref}: {mc=}, {peak_counts[a]=}")
-                pass  # TODO: should we set mcc[1] to 0 here?
+                skipped = True
+                break
+
             call.append(mcc[0])
             rs.append(mcc[1])
 
+        if skipped:
+            skipped_snvs.add(u_idx)  # Skip this useful SNV, since it isn't actually useful
+            continue
+
         called_snvs.append({
             "pos": u_ref,
             "call": np.array(call)[peak_order].tolist(),
             "rs": np.array(rs)[peak_order].tolist(),
         })
 
+    # If we've skipped any SNVs, filter them out of the read dict - MUTATION
+    if skipped_snvs:
+        for read in read_dict.values():
+            read["snvu"] = tuple(b for i, b in enumerate(read["snvu"]) if i not in skipped_snvs)
+        logger.debug(f"{locus_log_str} - filtered out {len(skipped_snvs)} not-actually-useful SNVs")
+
     return called_snvs
```

### Comparing `strkit-0.8.0a8/strkit/call/caller/types.py` & `strkit-0.8.0a9/strkit/call/caller/types.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/call/re_caller.py` & `strkit-0.8.0a9/strkit/call/re_caller.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/call/repeathmm.py` & `strkit-0.8.0a9/strkit/call/repeathmm.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/call/straglr.py` & `strkit-0.8.0a9/strkit/call/straglr.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/call/tandem_genotypes.py` & `strkit-0.8.0a9/strkit/call/tandem_genotypes.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/catalog/combine.py` & `strkit-0.8.0a9/strkit/catalog/combine.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/constants.py` & `strkit-0.8.0a9/strkit/constants.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/convert/converter.py` & `strkit-0.8.0a9/strkit/convert/converter.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/entry.py` & `strkit-0.8.0a9/strkit/entry.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/logger.py` & `strkit-0.8.0a9/strkit/logger.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/mi/base.py` & `strkit-0.8.0a9/strkit/mi/base.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/mi/expansionhunter.py` & `strkit-0.8.0a9/strkit/mi/expansionhunter.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/mi/gangstr.py` & `strkit-0.8.0a9/strkit/mi/gangstr.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/mi/repeathmm.py` & `strkit-0.8.0a9/strkit/mi/repeathmm.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/mi/result.py` & `strkit-0.8.0a9/strkit/mi/result.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/mi/straglr.py` & `strkit-0.8.0a9/strkit/mi/straglr.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/mi/strkit.py` & `strkit-0.8.0a9/strkit/mi/strkit.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/mi/tandem_genotypes.py` & `strkit-0.8.0a9/strkit/mi/tandem_genotypes.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/mi/vcf_utils.py` & `strkit-0.8.0a9/strkit/mi/vcf_utils.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/utils.py` & `strkit-0.8.0a9/strkit/utils.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/viz/server.py` & `strkit-0.8.0a9/strkit/viz/server.py`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/viz/static/logo.png` & `strkit-0.8.0a9/strkit/viz/static/logo.png`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit/viz/templates/browser.html` & `strkit-0.8.0a9/strkit/viz/templates/browser.html`

 * *Files identical despite different names*

### Comparing `strkit-0.8.0a8/strkit.egg-info/PKG-INFO` & `strkit-0.8.0a9/strkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strkit
-Version: 0.8.0a8
+Version: 0.8.0a9
 Summary: A toolkit for analyzing variation in short(ish) tandem repeats.
 Home-page: https://github.com/davidlougheed/strkit
 Author: David Lougheed
 Author-email: david.lougheed@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `strkit-0.8.0a8/strkit.egg-info/SOURCES.txt` & `strkit-0.8.0a9/strkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

